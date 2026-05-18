---
nbme: 12
type: 学习Dashboard
tags:
  - USMLE-Step2
  - NBME模拟题
  - 学习Dashboard
---

# NBME 12 学习 Dashboard

> [!info] 这是什么
> 单套题的**学习导航中心**。读取 [[_做题结果_NBME12]] 表格数据，
> 按"学科 × 4 种状态"任意组合筛选题目，点击跳转到 breakdown 学习。
> 
> 📂 配套文件（v6.2）：
> - 做题结果（输入）：[[_做题结果_NBME12]]
> - 题目详解（4 Section）：[[NBME12_S1_breakdown]] · [[NBME12_S2_breakdown]] · [[NBME12_S3_breakdown]] · [[NBME12_S4_breakdown]]
> - 套题入口：[[NBME12_套题索引]]
> - 全局视图：[[NBME_全局学习Dashboard]]

---

## 📊 总体进度

```dataviewjs
// 读取做题结果文件的纯文本，解析 4 个 Section 表格
const resultFile = "_做题结果_NBME" + dv.current().nbme;
const path = dv.pages('"' + resultFile + '"').first()?.file?.path 
  || dv.pages().where(p => p.file.name === resultFile).first()?.file?.path;

if (!path) {
  dv.paragraph(`⚠️ 找不到做题结果文件：${resultFile}.md`);
} else {
  const content = await dv.io.load(path);
  const lines = content.split("\n");
  const records = [];
  let currentSection = null;
  
  for (const line of lines) {
    // 兼容 ## 或 ### Section 标题（容错）
    const sectionMatch = line.match(/^#{2,3}\s+Section\s*(\d+)/);
    if (sectionMatch) {
      currentSection = parseInt(sectionMatch[1]);
      continue;
    }
    
    if (line.match(/^\|\s*\d+\s*\|/)) {
      const cells = line.split("|").map(c => c.trim()).filter((c, i, arr) => i > 0 && i < arr.length - 1);
      // v6.2 表格 8 列：Q# | 学科 | 主题 | HY | r/w | mk | 选 | 备注
      if (cells.length >= 6) {
        const qid = cells[0];
        const subject = cells[1];
        const topic = cells[2];
        const hy = cells[3];
        const rw = cells[4].toLowerCase();
        const mk = cells[5].toLowerCase();
        const choice = cells[6] || "";
        const note = cells[7] || "";
        
        records.push({
          qid: qid.padStart(3, "0"),
          qidRaw: qid,
          section: currentSection,
          subject,
          topic,
          hy: parseInt(hy) || 0,
          result: rw === "r" ? "right" : (rw === "w" ? "wrong" : "blank"),
          mark: mk === "m",
          my_choice: choice,
          my_note: note,
        });
      }
    }
  }
  
  // 储存到全局供后续查询用
  window._learnDashRecords = records;
  window._learnDashNbme = dv.current().nbme;
  
  // v6.2 拆 Section：helper 函数，根据 qid 决定指向哪个 Section 文件
  window._qLinkSection = (r) => {
    const nbme = window._learnDashNbme;
    const qn = parseInt(r.qidRaw);
    const sec = qn <= 50 ? "S1" : qn <= 100 ? "S2" : qn <= 150 ? "S3" : "S4";
    return `[[NBME${nbme}_${sec}_breakdown#^Q${r.qid}|Q${r.qid}]]`;
  };
  
  // 统计
  const right = records.filter(r => r.result === "right");
  const wrong = records.filter(r => r.result === "wrong");
  const blank = records.filter(r => r.result === "blank");
  const answered = right.length + wrong.length;
  
  const cleanRight = records.filter(r => r.result === "right" && !r.mark);
  const pseudo = records.filter(r => r.result === "right" && r.mark);
  const markedWrong = records.filter(r => r.result === "wrong" && r.mark);
  const cleanWrong = records.filter(r => r.result === "wrong" && !r.mark);
  
  dv.table(["指标", "数值", "说明"],
    [
      ["📝 已答", answered + "/" + records.length, ""],
      ["综合正确率", answered > 0 ? ((right.length/answered)*100).toFixed(1) + "%" : "—", ""],
      ["—", "—", "—"],
      ["🟢 干净对", cleanRight.length, "确认掌握"],
      ["⚠️ 伪掌握", pseudo.length, "🔴 真考高危区"],
      ["🟡 标记错", markedWrong.length, "自知盲区"],
      ["🔴 干净错", cleanWrong.length, "完全盲区"],
    ]
  );
}
```

---

## 📊 学科 × 状态矩阵

```dataviewjs
const records = window._learnDashRecords || [];

if (records.length > 0) {
  const subjectMap = {};
  for (const r of records) {
    const subj = r.subject || "未分类";
    if (!subjectMap[subj]) {
      subjectMap[subj] = { cleanRight: [], pseudo: [], markedWrong: [], cleanWrong: [], blank: [] };
    }
    if (r.result === "blank") subjectMap[subj].blank.push(r);
    else if (r.result === "right" && !r.mark) subjectMap[subj].cleanRight.push(r);
    else if (r.result === "right" && r.mark) subjectMap[subj].pseudo.push(r);
    else if (r.result === "wrong" && r.mark) subjectMap[subj].markedWrong.push(r);
    else if (r.result === "wrong" && !r.mark) subjectMap[subj].cleanWrong.push(r);
  }
  
  const sorted = Object.entries(subjectMap).sort((a, b) => {
    const probA = a[1].pseudo.length + a[1].cleanWrong.length + a[1].markedWrong.length;
    const probB = b[1].pseudo.length + b[1].cleanWrong.length + b[1].markedWrong.length;
    return probB - probA;
  });
  
  const rows = sorted.map(([subj, stat]) => {
    const total = stat.cleanRight.length + stat.pseudo.length + stat.markedWrong.length + stat.cleanWrong.length + stat.blank.length;
    return [
      subj,
      total,
      stat.cleanRight.length || "—",
      stat.pseudo.length || "—",
      stat.markedWrong.length || "—",
      stat.cleanWrong.length || "—",
    ];
  });
  
  dv.table(
    ["学科", "总数", "🟢 干净对", "⚠️ 伪掌握", "🟡 标记错", "🔴 干净错"],
    rows
  );
}
```

---

## ⚠️ 全部伪掌握题（按学科）

```dataviewjs
const records = window._learnDashRecords || [];
const qLink = window._qLinkSection;
const pseudo = records.filter(r => r.result === "right" && r.mark);

if (pseudo.length === 0) {
  dv.paragraph("✨ 没有伪掌握题。");
} else {
  const grouped = {};
  for (const r of pseudo) {
    const subj = r.subject || "未分类";
    if (!grouped[subj]) grouped[subj] = [];
    grouped[subj].push(r);
  }
  
  for (const [subj, items] of Object.entries(grouped).sort()) {
    dv.header(4, `${subj} (${items.length} 道)`);
    dv.list(items.map(r => 
      `${qLink(r)} **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
    ));
  }
}
```

---

## 🔴 全部干净错题（按学科）

```dataviewjs
const records = window._learnDashRecords || [];
const qLink = window._qLinkSection;
const cleanWrong = records.filter(r => r.result === "wrong" && !r.mark);

if (cleanWrong.length === 0) {
  dv.paragraph("✨ 没有干净错题。");
} else {
  const grouped = {};
  for (const r of cleanWrong) {
    const subj = r.subject || "未分类";
    if (!grouped[subj]) grouped[subj] = [];
    grouped[subj].push(r);
  }
  
  for (const [subj, items] of Object.entries(grouped).sort()) {
    dv.header(4, `${subj} (${items.length} 道)`);
    dv.list(items.map(r => 
      `${qLink(r)} **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
    ));
  }
}
```

---

## 🟡 全部标记错题（按学科）

```dataviewjs
const records = window._learnDashRecords || [];
const qLink = window._qLinkSection;
const markedWrong = records.filter(r => r.result === "wrong" && r.mark);

if (markedWrong.length === 0) {
  dv.paragraph("✨ 没有标记错题。");
} else {
  const grouped = {};
  for (const r of markedWrong) {
    const subj = r.subject || "未分类";
    if (!grouped[subj]) grouped[subj] = [];
    grouped[subj].push(r);
  }
  
  for (const [subj, items] of Object.entries(grouped).sort()) {
    dv.header(4, `${subj} (${items.length} 道)`);
    dv.list(items.map(r => 
      `${qLink(r)} **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
    ));
  }
}
```

---

## 🟢 干净答对题（折叠，便于检索）

> [!example]- 点击展开干净答对清单

```dataviewjs
const records = window._learnDashRecords || [];
const qLink = window._qLinkSection;
const cleanRight = records.filter(r => r.result === "right" && !r.mark);

if (cleanRight.length === 0) {
  dv.paragraph("还没有干净答对的题。");
} else {
  const grouped = {};
  for (const r of cleanRight) {
    const subj = r.subject || "未分类";
    if (!grouped[subj]) grouped[subj] = [];
    grouped[subj].push(r);
  }
  
  for (const [subj, items] of Object.entries(grouped).sort()) {
    dv.header(4, `${subj} (${items.length} 道)`);
    dv.list(items.map(r => 
      `${qLink(r)} ${r.topic || ""}`
    ));
  }
}
```

---

## 🎯 按单个学科深度检索

> 💡 改下面 `TARGET_SUBJECT` 来查任何学科。学科名必须**精确**匹配做题结果表格里的 `学科` 列。

```dataviewjs
// ⚙️ 改这里
const TARGET_SUBJECT = "心内";

const records = window._learnDashRecords || [];
const qLink = window._qLinkSection;
const filtered = records.filter(r => r.subject === TARGET_SUBJECT);

if (filtered.length === 0) {
  dv.paragraph(`没有学科 = "${TARGET_SUBJECT}" 的题。请检查学科名拼写。`);
} else {
  dv.header(3, `📚 ${TARGET_SUBJECT} - 全部 ${filtered.length} 道题`);
  dv.paragraph(`主笔记：[[完整笔记/Peixuan分科笔记/${TARGET_SUBJECT}]]`);
  
  const stats = {
    "🟢 干净对": filtered.filter(r => r.result === "right" && !r.mark),
    "⚠️ 伪掌握": filtered.filter(r => r.result === "right" && r.mark),
    "🟡 标记错": filtered.filter(r => r.result === "wrong" && r.mark),
    "🔴 干净错": filtered.filter(r => r.result === "wrong" && !r.mark),
  };
  
  for (const [label, items] of Object.entries(stats)) {
    if (items.length > 0) {
      dv.header(4, `${label} (${items.length} 道)`);
      dv.list(items.map(r => 
        `${qLink(r)} **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
      ));
    }
  }
  
  const answered = stats["🟢 干净对"].length + stats["⚠️ 伪掌握"].length + stats["🟡 标记错"].length + stats["🔴 干净错"].length;
  const correct = stats["🟢 干净对"].length + stats["⚠️ 伪掌握"].length;
  if (answered > 0) {
    dv.paragraph(`**${TARGET_SUBJECT} 综合正确率**：${correct}/${answered} = ${((correct/answered)*100).toFixed(1)}%`);
  }
}
```

---

## 📚 本套复盘 Prompt

```
请基于以下文件生成 NBME12 个性化复盘报告：

【输入】
- 做题结果：[[_做题结果_NBME12]]
- 题目详解（4 Section）：
  - [[NBME12_S1_breakdown]] Q001-Q050
  - [[NBME12_S2_breakdown]] Q051-Q100
  - [[NBME12_S3_breakdown]] Q101-Q150
  - [[NBME12_S4_breakdown]] Q151-Q200

【复盘优先级】
1. 伪掌握（r/w=r + mk=m）— 最高优先级
2. 干净错题（r/w=w + mk=空）— 完全盲区
3. 标记错题（r/w=w + mk=m）— 自知盲区

【输出 NBME12_复盘报告.md】

1. 总体表现：估分、正确率、学科正确率排行
2. 三类问题题深度分析（引用题号用 `[[NBME12_S{N}_breakdown#^Q###]]` 格式）
3. 陷阱模式归类：trap_type / thinking_error_type / stem_pattern
4. 关联到 vault：哪些主笔记加「薄弱点」
5. 考前必看清单：基于本套 + [[薄弱点]] 的 15-25 个考点
```
