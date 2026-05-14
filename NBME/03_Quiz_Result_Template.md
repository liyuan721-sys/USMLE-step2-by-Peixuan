---
nbme: 12
date: 
round: 1                # 第几刷（1 = 一刷，2 = 二刷）
status: not_started     # not_started / phase1_done / phase2_done / reviewed
total_score: 
target: 250
duration_minutes: 
tags:
  - USMLE-Step2
  - NBME模拟题
  - 做题结果
---

# NBME 12 做题结果（第 1 刷）

> [!info] 套题信息
> - **套题入口**：[[NBME12_套题索引]]（含 4 Section 文件链接）
> - **题目详解**：[[NBME12_S1_breakdown]] · [[NBME12_S2_breakdown]] · [[NBME12_S3_breakdown]] · [[NBME12_S4_breakdown]]
> - **学习视图**：[[NBME12_学习Dashboard]]
> - **全局视图**：[[NBME_全局学习Dashboard]]
> - **二刷文件**（如有）：[[_做题结果_NBME12_R2]]

---

## 🗒️ 两阶段工作流速查

> [!tip]- 📌 输入说明（首次使用必读）
> 
> ### 阶段 1：做完题当天填（10-15 分钟）
> 
> 用 NBME Fighter 截图喂给 Claude Code（**推荐**），或在下方表格的 `r/w` 和 `mk` 列填字符：
> 
> | 字段 | 输入值 | 说明 |
> |---|---|---|
> | `r/w` | `r` | 答对 |
> | `r/w` | `w` | 答错 |
> | `r/w` | 留空 | 未答 |
> | `mk` | `m` | NBME Fighter 标记过 |
> | `mk` | 留空 | 没标记 |
> 
> 4 种组合 → 4 种状态：
> 
> | r/w | mk | 状态 | 优先级 |
> |---|---|---|---|
> | r | （空） | 🟢 干净对 | 低 |
> | r | m | ⚠️ 伪掌握 | 🔴 最高 |
> | w | m | 🟡 标记错 | 🟡 中 |
> | w | （空） | 🔴 干净错 | 🔴 高 |
> 
> ### 阶段 2：复盘时补充（20-30 分钟，仅关键题）
> 
> 打开 [[NBME12_学习Dashboard]] → 看伪掌握/错题清单 → 点击跳到 breakdown 看解析 → 回到本文件补：
> - `选` 列：你当时选的字母（A/B/C/D/E）
> - `备注` 列：一句话错因
> 
> ⚠️ 干净对的题不用补任何东西。

> [!info]- 🔄 二刷使用说明
> 
> 想二刷错题和标记题？做法：
> 1. **不要**修改本文件（保留一刷数据）
> 2. 复制本文件 → 改名 `_做题结果_NBME12_R2.md`
> 3. 改 frontmatter：`round: 2`
> 4. 清空 `r/w`、`mk`、`选`、`备注` 4 列（学科和主题保留）
> 5. 只填你计划二刷的那些题（一般是一刷的错题 + 标记题）
> 6. 全局 Dashboard 会自动识别两次刷的数据，做横向对比

---

## 📊 实时统计

```dataviewjs
const page = dv.current();
const fileContent = await dv.io.load(dv.current().file.path);
const lines = fileContent.split("\n");

const records = [];
let currentSection = null;

for (const line of lines) {
  // 兼容 ## 或 ### Section 标题
  const sectionMatch = line.match(/^#{2,3}\s+Section\s*(\d+)/);
  if (sectionMatch) {
    currentSection = parseInt(sectionMatch[1]);
    continue;
  }
  
  // 表格行：| Q# | 学科 | 主题 | HY | r/w | mk | 选 | 备注 |
  if (line.match(/^\|\s*\d+\s*\|/)) {
    const cells = line.split("|").map(c => c.trim()).filter((c, i, arr) => i > 0 && i < arr.length - 1);
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

window._nbmeRecords = records;
window._nbmeNumber = page.nbme;
window._nbmeRound = page.round || 1;

const right = records.filter(r => r.result === "right");
const wrong = records.filter(r => r.result === "wrong");
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
```

---

## 🎯 错题与伪掌握快速跳转（按优先级）

```dataviewjs
const records = window._nbmeRecords || [];
const nbme = window._nbmeNumber;

// v6.2 拆 Section：根据 qid 自动指向对应 Section 文件
const qLink = (r) => {
  const qn = parseInt(r.qidRaw);
  const sec = qn <= 50 ? "S1" : qn <= 100 ? "S2" : qn <= 150 ? "S3" : "S4";
  return `[[NBME${nbme}_${sec}_breakdown#^Q${r.qid}|Q${r.qid}]]`;
};

const pseudo = records.filter(r => r.result === "right" && r.mark);
const cleanWrong = records.filter(r => r.result === "wrong" && !r.mark);
const markedWrong = records.filter(r => r.result === "wrong" && r.mark);

if (pseudo.length > 0) {
  dv.header(3, `⚠️ 伪掌握（${pseudo.length} 道）— 最高优先级`);
  dv.paragraph("**🔴 真考翻车高危区**：标记了但答对，意味着你不踏实。");
  dv.list(pseudo.map(r => 
    `${qLink(r)} [${r.subject || "?"}] **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
  ));
}

if (cleanWrong.length > 0) {
  dv.header(3, `🔴 干净错（${cleanWrong.length} 道）— 完全盲区`);
  dv.paragraph("没标记直接错 = 完全不知道这是个考点。");
  dv.list(cleanWrong.map(r => 
    `${qLink(r)} [${r.subject || "?"}] **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
  ));
}

if (markedWrong.length > 0) {
  dv.header(3, `🟡 标记错（${markedWrong.length} 道）— 自知盲区`);
  dv.paragraph("知道自己不会，针对性补即可。");
  dv.list(markedWrong.map(r => 
    `${qLink(r)} [${r.subject || "?"}] **${r.topic || ""}** [HY:${r.hy}]${r.my_choice ? " — 选了 " + r.my_choice : ""}${r.my_note ? " | " + r.my_note : ""}`
  ));
}

if (pseudo.length === 0 && cleanWrong.length === 0 && markedWrong.length === 0) {
  dv.paragraph("✨ 还没有错题/伪掌握数据。先填下方表格的 r/w 和 mk 列。");
}
```

---

## 📚 按学科 × 状态聚合

```dataviewjs
const records = window._nbmeRecords || [];

if (records.length > 0) {
  const subjectMap = {};
  for (const r of records) {
    const subj = r.subject || "未分类";
    if (!subjectMap[subj]) {
      subjectMap[subj] = { cleanRight: 0, pseudo: 0, markedWrong: 0, cleanWrong: 0, blank: 0 };
    }
    if (r.result === "blank") subjectMap[subj].blank++;
    else if (r.result === "right" && !r.mark) subjectMap[subj].cleanRight++;
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
    const total = stat.cleanRight + stat.pseudo + stat.markedWrong + stat.cleanWrong + stat.blank;
    const answered = stat.cleanRight + stat.pseudo + stat.markedWrong + stat.cleanWrong;
    const correct = stat.cleanRight + stat.pseudo;
    const accuracy = answered > 0 ? ((correct / answered) * 100).toFixed(0) + "%" : "—";
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
  
  dv.table(
    ["学科", "总数", "正确率", "🟢 干净对", "⚠️ 伪掌握", "🟡 标记错", "🔴 干净错"],
    rows
  );
}
```

---

# 📝 做题数据输入区

> ⚠️ **下面 4 个 Section 表格是你的主要输入区**。
> 
> 📌 **Q#、学科、主题、HY 4 列已由 v4 prompt 自动填好，不要修改**。
> 📌 **只编辑 `r/w`、`mk`、`选`、`备注` 4 列**。

---

## Section 1（Item 1-50）

| Q# | 学科 | 主题 | HY | r/w | mk | 选 | 备注 |
|----|------|------|----|-----|----|----|------|
| 1  | （由 v4 prompt 自动填入）| | | | | | |
| 2  | | | | | | | |
| 3  | | | | | | | |
| 4  | | | | | | | |
| 5  | | | | | | | |
| 6  | | | | | | | |
| 7  | | | | | | | |
| 8  | | | | | | | |
| 9  | | | | | | | |
| 10 | | | | | | | |
| 11 | | | | | | | |
| 12 | | | | | | | |
| 13 | | | | | | | |
| 14 | | | | | | | |
| 15 | | | | | | | |
| 16 | | | | | | | |
| 17 | | | | | | | |
| 18 | | | | | | | |
| 19 | | | | | | | |
| 20 | | | | | | | |
| 21 | | | | | | | |
| 22 | | | | | | | |
| 23 | | | | | | | |
| 24 | | | | | | | |
| 25 | | | | | | | |
| 26 | | | | | | | |
| 27 | | | | | | | |
| 28 | | | | | | | |
| 29 | | | | | | | |
| 30 | | | | | | | |
| 31 | | | | | | | |
| 32 | | | | | | | |
| 33 | | | | | | | |
| 34 | | | | | | | |
| 35 | | | | | | | |
| 36 | | | | | | | |
| 37 | | | | | | | |
| 38 | | | | | | | |
| 39 | | | | | | | |
| 40 | | | | | | | |
| 41 | | | | | | | |
| 42 | | | | | | | |
| 43 | | | | | | | |
| 44 | | | | | | | |
| 45 | | | | | | | |
| 46 | | | | | | | |
| 47 | | | | | | | |
| 48 | | | | | | | |
| 49 | | | | | | | |
| 50 | | | | | | | |

---

## Section 2（Item 51-100）

| Q# | 学科 | 主题 | HY | r/w | mk | 选 | 备注 |
|----|------|------|----|-----|----|----|------|
| 51 | | | | | | | |
| 52 | | | | | | | |
| 53 | | | | | | | |
| 54 | | | | | | | |
| 55 | | | | | | | |
| 56 | | | | | | | |
| 57 | | | | | | | |
| 58 | | | | | | | |
| 59 | | | | | | | |
| 60 | | | | | | | |
| 61 | | | | | | | |
| 62 | | | | | | | |
| 63 | | | | | | | |
| 64 | | | | | | | |
| 65 | | | | | | | |
| 66 | | | | | | | |
| 67 | | | | | | | |
| 68 | | | | | | | |
| 69 | | | | | | | |
| 70 | | | | | | | |
| 71 | | | | | | | |
| 72 | | | | | | | |
| 73 | | | | | | | |
| 74 | | | | | | | |
| 75 | | | | | | | |
| 76 | | | | | | | |
| 77 | | | | | | | |
| 78 | | | | | | | |
| 79 | | | | | | | |
| 80 | | | | | | | |
| 81 | | | | | | | |
| 82 | | | | | | | |
| 83 | | | | | | | |
| 84 | | | | | | | |
| 85 | | | | | | | |
| 86 | | | | | | | |
| 87 | | | | | | | |
| 88 | | | | | | | |
| 89 | | | | | | | |
| 90 | | | | | | | |
| 91 | | | | | | | |
| 92 | | | | | | | |
| 93 | | | | | | | |
| 94 | | | | | | | |
| 95 | | | | | | | |
| 96 | | | | | | | |
| 97 | | | | | | | |
| 98 | | | | | | | |
| 99 | | | | | | | |
| 100 | | | | | | | |

---

## Section 3（Item 101-150）

| Q# | 学科 | 主题 | HY | r/w | mk | 选 | 备注 |
|----|------|------|----|-----|----|----|------|
| 101 | | | | | | | |
| 102 | | | | | | | |
| 103 | | | | | | | |
| 104 | | | | | | | |
| 105 | | | | | | | |
| 106 | | | | | | | |
| 107 | | | | | | | |
| 108 | | | | | | | |
| 109 | | | | | | | |
| 110 | | | | | | | |
| 111 | | | | | | | |
| 112 | | | | | | | |
| 113 | | | | | | | |
| 114 | | | | | | | |
| 115 | | | | | | | |
| 116 | | | | | | | |
| 117 | | | | | | | |
| 118 | | | | | | | |
| 119 | | | | | | | |
| 120 | | | | | | | |
| 121 | | | | | | | |
| 122 | | | | | | | |
| 123 | | | | | | | |
| 124 | | | | | | | |
| 125 | | | | | | | |
| 126 | | | | | | | |
| 127 | | | | | | | |
| 128 | | | | | | | |
| 129 | | | | | | | |
| 130 | | | | | | | |
| 131 | | | | | | | |
| 132 | | | | | | | |
| 133 | | | | | | | |
| 134 | | | | | | | |
| 135 | | | | | | | |
| 136 | | | | | | | |
| 137 | | | | | | | |
| 138 | | | | | | | |
| 139 | | | | | | | |
| 140 | | | | | | | |
| 141 | | | | | | | |
| 142 | | | | | | | |
| 143 | | | | | | | |
| 144 | | | | | | | |
| 145 | | | | | | | |
| 146 | | | | | | | |
| 147 | | | | | | | |
| 148 | | | | | | | |
| 149 | | | | | | | |
| 150 | | | | | | | |

---

## Section 4（Item 151-200）

| Q# | 学科 | 主题 | HY | r/w | mk | 选 | 备注 |
|----|------|------|----|-----|----|----|------|
| 151 | | | | | | | |
| 152 | | | | | | | |
| 153 | | | | | | | |
| 154 | | | | | | | |
| 155 | | | | | | | |
| 156 | | | | | | | |
| 157 | | | | | | | |
| 158 | | | | | | | |
| 159 | | | | | | | |
| 160 | | | | | | | |
| 161 | | | | | | | |
| 162 | | | | | | | |
| 163 | | | | | | | |
| 164 | | | | | | | |
| 165 | | | | | | | |
| 166 | | | | | | | |
| 167 | | | | | | | |
| 168 | | | | | | | |
| 169 | | | | | | | |
| 170 | | | | | | | |
| 171 | | | | | | | |
| 172 | | | | | | | |
| 173 | | | | | | | |
| 174 | | | | | | | |
| 175 | | | | | | | |
| 176 | | | | | | | |
| 177 | | | | | | | |
| 178 | | | | | | | |
| 179 | | | | | | | |
| 180 | | | | | | | |
| 181 | | | | | | | |
| 182 | | | | | | | |
| 183 | | | | | | | |
| 184 | | | | | | | |
| 185 | | | | | | | |
| 186 | | | | | | | |
| 187 | | | | | | | |
| 188 | | | | | | | |
| 189 | | | | | | | |
| 190 | | | | | | | |
| 191 | | | | | | | |
| 192 | | | | | | | |
| 193 | | | | | | | |
| 194 | | | | | | | |
| 195 | | | | | | | |
| 196 | | | | | | | |
| 197 | | | | | | | |
| 198 | | | | | | | |
| 199 | | | | | | | |
| 200 | | | | | | | |

---

## ✏️ 复盘行动清单

- [ ] **阶段 1**：做完题当天填完 4 个 Section 的 r/w 和 mk 列
- [ ] 查看顶部统计 + 错题/伪掌握快速跳转
- [ ] **阶段 2**：打开 [[NBME12_学习Dashboard]] 看深度分类
- [ ] 点击关键题跳到 breakdown 看详解
- [ ] 回到本文件补关键题的 `选` 和 `备注` 列
- [ ] 在 breakdown 对应 callout 末尾追加 [🤯 我的复盘]
- [ ] 让 Claude Code 跑复盘 prompt
- [ ] 1-2 周后：复制本文件 → `_做题结果_NBME12_R2.md` → 二刷错题和标记题
