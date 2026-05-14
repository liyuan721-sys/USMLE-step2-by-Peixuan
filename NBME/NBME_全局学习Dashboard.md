---
type: dashboard
tags:
  - USMLE-Step2
  - NBME汇总
---

# NBME 9-16 全局学习 Dashboard

> [!info] 这是什么
> 跨 8 套 NBME 题的**全局学习入口**。自动读取所有 `_做题结果_NBME*.md` 表格数据，
> 按"学科 × 4 种状态"任意组合，跨套题检索题目。

---

## 📊 总体进度

```dataviewjs
// 找到所有做题结果文件
const pages = dv.pages('#做题结果').sort(p => p.nbme);

if (pages.length === 0) {
  dv.paragraph("⚠️ 还没有任何做题记录文件。");
} else {
  const allRecords = [];
  
  for (const page of pages) {
    const content = await dv.io.load(page.file.path);
    const lines = content.split("\n");
    let currentSection = null;
    
    for (const line of lines) {
      // 兼容 ## 或 ### Section 标题
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
          
          allRecords.push({
            qid: qid.padStart(3, "0"),
            qidRaw: qid,
            nbme: page.nbme,
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
  }
  
  // 储存全局
  window._allNbmeRecords = allRecords;
  
  // v6.2 拆 Section：helper 函数，根据 qid 决定指向哪个 Section 文件
  window._qLinkGlobal = (r) => {
    const qn = parseInt(r.qidRaw);
    const sec = qn <= 50 ? "S1" : qn <= 100 ? "S2" : qn <= 150 ? "S3" : "S4";
    return `[[NBME${r.nbme}_${sec}_breakdown#^Q${r.qid}|NBME${r.nbme} Q${r.qid}]]`;
  };
  
  const right = allRecords.filter(r => r.result === "right");
  const wrong = allRecords.filter(r => r.result === "wrong");
  const answered = right.length + wrong.length;
  
  const cleanRight = allRecords.filter(r => r.result === "right" && !r.mark);
  const pseudo = allRecords.filter(r => r.result === "right" && r.mark);
  const markedWrong = allRecords.filter(r => r.result === "wrong" && r.mark);
  const cleanWrong = allRecords.filter(r => r.result === "wrong" && !r.mark);
  
  dv.table(["指标", "数值", "说明"],
    [
      ["📚 已完成套数", pages.length + "/8", ""],
      ["📝 已答题总数", answered, ""],
      ["综合正确率", answered > 0 ? ((right.length/answered)*100).toFixed(1) + "%" : "—", ""],
      ["—", "—", "—"],
      ["🟢 干净答对", cleanRight.length, "确认掌握"],
      ["⚠️ 伪掌握", pseudo.length, "🔴 真考高危区"],
      ["🟡 标记答错", markedWrong.length, "自知盲区"],
      ["🔴 干净答错", cleanWrong.length, "完全盲区"],
    ]
  );
}
```

---

## 📈 各套题表现

```dataviewjs
const pages = dv.pages('#做题结果').sort(p => p.nbme);
const allRecords = window._allNbmeRecords || [];

if (allRecords.length > 0) {
  const byNbme = {};
  for (const r of allRecords) {
    if (!byNbme[r.nbme]) byNbme[r.nbme] = [];
    byNbme[r.nbme].push(r);
  }
  
  const rows = pages.map(page => {
    const records = byNbme[page.nbme] || [];
    const right = records.filter(r => r.result === "right").length;
    const wrong = records.filter(r => r.result === "wrong").length;
    const pseudo = records.filter(r => r.result === "right" && r.mark).length;
    const cleanWrong = records.filter(r => r.result === "wrong" && !r.mark).length;
    const answered = right + wrong;
    const accuracy = answered > 0 ? ((right/answered)*100).toFixed(1) + "%" : "—";
    
    return [
      page.file.link,
      page.date || "—",
      page.total_score || "—",
      right + "/" + answered,
      accuracy,
      pseudo,
      cleanWrong,
    ];
  });
  
  dv.table(
    ["套题", "日期", "估分", "对/答", "正确率", "⚠️伪掌握", "🔴干净错"],
    rows
  );
}
```

---

## 🌍 跨套题学科 × 状态矩阵

```dataviewjs
const allRecords = window._allNbmeRecords || [];

if (allRecords.length > 0) {
  const subjectMap = {};
  for (const r of allRecords) {
    const subj = r.subject || "未分类";
    if (!subjectMap[subj]) {
      subjectMap[subj] = { cleanRight: 0, pseudo: 0, markedWrong: 0, cleanWrong: 0 };
    }
    if (r.result === "right" && !r.mark) subjectMap[subj].cleanRight++;
    else if (r.result === "right" && r.mark) subjectMap[subj].pseudo++;
    else if (r.result === "wrong" && r.mark) subjectMap[subj].markedWrong++;
    else if (r.result === "wrong" && !r.mark) subjectMap[subj].cleanWrong++;
  }
  
  const sorted = Object.entries(subjectMap).sort((a, b) => {
    const probA = a[1].pseudo + a[1].cleanWrong + a[1].markedWrong;
    const probB = b[1].pseudo + b[1].cleanWrong + b[1].markedWrong;
    return probB - probA;
  });
  
  const rows = sorted.map(([subj, stat]) => {
    const total = stat.cleanRight + stat.pseudo + stat.markedWrong + stat.cleanWrong;
    const correct = stat.cleanRight + stat.pseudo;
    const accuracy = total > 0 ? ((correct / total) * 100).toFixed(0) + "%" : "—";
    return [
      subj,
      total,
      accuracy,
      stat.cleanRight || "—",
      stat.pseudo || "—",
      stat.markedWrong || "—",
      stat.cleanWrong || "—",
    ];
  });
  
  dv.paragraph("📌 按"问题题数"倒序（伪掌握 + 标记错 + 干净错），暴露最需复盘的学科。");
  
  dv.table(
    ["学科", "总数", "正确率", "🟢 干净对", "⚠️ 伪掌握", "🟡 标记错", "🔴 干净错"],
    rows
  );
}
```

---

## ⚠️ 跨套题所有伪掌握题（按学科）

```dataviewjs
const allRecords = window._allNbmeRecords || [];
const pseudo = allRecords.filter(r => r.result === "right" && r.mark);

if (pseudo.length === 0) {
  dv.paragraph("✨ 没有伪掌握题。");
} else {
  dv.paragraph(`🔴 累积 **${pseudo.length}** 道伪掌握题 — **复盘最优先**。`);
  
  const grouped = {};
  for (const r of pseudo) {
    const subj = r.subject || "未分类";
    if (!grouped[subj]) grouped[subj] = [];
    grouped[subj].push(r);
  }
  
  const sorted = Object.entries(grouped).sort((a, b) => b[1].length - a[1].length);
  
  for (const [subj, items] of sorted) {
    dv.header(4, `${subj} (${items.length} 道)`);
    dv.list(items.map(r => 
      `${window._qLinkGlobal(r)} **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
    ));
  }
}
```

---

## 🔴 跨套题所有干净错题（按学科）

```dataviewjs
const allRecords = window._allNbmeRecords || [];
const cleanWrong = allRecords.filter(r => r.result === "wrong" && !r.mark);

if (cleanWrong.length === 0) {
  dv.paragraph("✨ 没有干净错题。");
} else {
  dv.paragraph(`📊 累积 **${cleanWrong.length}** 道干净错题（完全盲区）`);
  
  const grouped = {};
  for (const r of cleanWrong) {
    const subj = r.subject || "未分类";
    if (!grouped[subj]) grouped[subj] = [];
    grouped[subj].push(r);
  }
  
  const sorted = Object.entries(grouped).sort((a, b) => b[1].length - a[1].length);
  
  for (const [subj, items] of sorted) {
    dv.header(4, `${subj} (${items.length} 道)`);
    dv.list(items.map(r => 
      `${window._qLinkGlobal(r)} **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
    ));
  }
}
```

---

## 🟡 跨套题所有标记错题（按学科）

```dataviewjs
const allRecords = window._allNbmeRecords || [];
const markedWrong = allRecords.filter(r => r.result === "wrong" && r.mark);

if (markedWrong.length === 0) {
  dv.paragraph("✨ 没有标记错题。");
} else {
  dv.paragraph(`📊 累积 **${markedWrong.length}** 道标记错题（自知盲区）`);
  
  const grouped = {};
  for (const r of markedWrong) {
    const subj = r.subject || "未分类";
    if (!grouped[subj]) grouped[subj] = [];
    grouped[subj].push(r);
  }
  
  const sorted = Object.entries(grouped).sort((a, b) => b[1].length - a[1].length);
  
  for (const [subj, items] of sorted) {
    dv.header(4, `${subj} (${items.length} 道)`);
    dv.list(items.map(r => 
      `${window._qLinkGlobal(r)} **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
    ));
  }
}
```

---

## 🎯 跨套题单学科深度检索

> 💡 修改 `TARGET_SUBJECT` 查任何学科。

```dataviewjs
// ⚙️ 改这里
const TARGET_SUBJECT = "心内";

const allRecords = window._allNbmeRecords || [];
const filtered = allRecords.filter(r => r.subject === TARGET_SUBJECT);

if (filtered.length === 0) {
  dv.paragraph(`没有学科 = "${TARGET_SUBJECT}" 的题。请检查学科名拼写。`);
} else {
  dv.header(3, `📚 ${TARGET_SUBJECT} — 跨所有套题共 ${filtered.length} 道`);
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
        `${window._qLinkGlobal(r)} **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
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

## ✏️ 综合复盘 Prompt（做完 4+ 套后用）

```
请读取所有 NBME 做题记录 + breakdown，生成跨套题综合复盘报告。

【复盘优先级】
1. 伪掌握累积 — 最高优先级
2. 干净错题累积 — 完全盲区
3. 标记错题累积 — 自知盲区

【输入】
- 所有 _做题结果_NBME*.md（按 tags=做题结果 找）
- 所有 NBME*_breakdown.md

【输出 NBME_综合复盘报告.md】
1. 跨套题学科错误率排行（对照 [[薄弱点]]）
2. 三类问题题归类（按学科聚合）
3. 反复中招的考点
4. 陷阱模式归类（trap_type / thinking_error_type / stem_pattern）
5. 考前 7 天必看清单（30-50 个考点）
6. vault 笔记建议（哪些主笔记加 #薄弱点 / 哪些生成 _衍生_xxx）
```

---

## 🔗 快速跳转

- 📋 [[复习入口_Dashboard]]
- 🎯 [[薄弱点]]
- 📊 [[诊断报告]]
- 📚 [[错题本]]
