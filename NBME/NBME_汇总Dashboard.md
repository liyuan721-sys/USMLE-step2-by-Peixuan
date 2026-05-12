---
type: dashboard
tags:
  - USMLE-Step2
  - NBME汇总
---

# NBME 9-16 汇总 Dashboard

> [!info] 使用说明
> 这个 Dashboard 自动聚合所有 `_做题结果_NBME*.md` 文件的数据。
> 跑完一套就会自动更新一行。**不需要手动维护**。
> 
> ⚠️ 前提：每个套题结果文件的 frontmatter 必须包含 `nbme` 和 `tags: [做题结果]`

---

## 📊 总体进度

```dataviewjs
const pages = dv.pages('#做题结果').sort(p => p.nbme);

if (pages.length === 0) {
  dv.paragraph("⚠️ 还没有任何做题记录文件。请先完成至少一套 NBME。");
} else {
  let totalAnswered = 0;
  let totalCorrect = 0;
  let totalWrong = 0;
  let totalMarked = 0;
  let totalLowConfRight = 0;
  
  for (const p of pages) {
    const qs = p.qs || [];
    totalAnswered += qs.filter(q => q.result).length;
    totalCorrect += qs.filter(q => q.result === "right").length;
    totalWrong += qs.filter(q => q.result === "wrong").length;
    totalMarked += qs.filter(q => q.result === "marked").length;
    totalLowConfRight += qs.filter(q => q.result === "right" && q.conf === "low").length;
  }
  
  dv.table(["指标", "数值"],
    [
      ["📚 已完成套数", pages.length + "/8"],
      ["📝 已答题总数", totalAnswered],
      ["✅ 总答对", totalCorrect + (totalAnswered > 0 ? " (" + ((totalCorrect/totalAnswered)*100).toFixed(1) + "%)" : "")],
      ["❌ 总答错", totalWrong],
      ["🏷️ 总标记", totalMarked],
      ["⚠️ 伪掌握累积", totalLowConfRight + " 道（真考高危）"],
    ]
  );
}
```

---

## 📈 各套题表现

```dataviewjs
const pages = dv.pages('#做题结果').sort(p => p.nbme);

if (pages.length > 0) {
  const rows = pages.map(p => {
    const qs = p.qs || [];
    const answered = qs.filter(q => q.result).length;
    const correct = qs.filter(q => q.result === "right").length;
    const wrong = qs.filter(q => q.result === "wrong").length;
    const marked = qs.filter(q => q.result === "marked").length;
    const accuracy = answered > 0 ? ((correct/answered)*100).toFixed(1) + "%" : "—";
    
    return [
      p.file.link,
      p.date || "—",
      p.total_score || "—",
      correct + "/" + answered,
      accuracy,
      wrong,
      marked,
    ];
  });
  
  dv.table(
    ["套题", "日期", "估分", "对/答", "正确率", "错题", "标记"],
    rows
  );
}
```

---

## ⚠️ 跨套题伪掌握警报

```dataviewjs
const pages = dv.pages('#做题结果').sort(p => p.nbme);
const allPseudoMastery = [];

for (const p of pages) {
  const qs = p.qs || [];
  const pseudoQs = qs.filter(q => q.result === "right" && q.conf === "low");
  for (const q of pseudoQs) {
    allPseudoMastery.push({
      nbme: p.nbme,
      qid: q.qid,
      choice: q.my_choice,
      note: q.my_note || "—",
      link: dv.fileLink("NBME" + p.nbme + "_breakdown") + "#Q" + q.qid,
    });
  }
}

if (allPseudoMastery.length === 0) {
  dv.paragraph("✨ 目前没有标记为「低置信度答对」的题。继续保持。");
} else {
  dv.paragraph(`⚠️ 累积 **${allPseudoMastery.length}** 道伪掌握题。这些题答对了但你不确定 → 真考试翻车高危区。`);
  dv.table(
    ["套题", "题号", "我选", "备注", "跳转"],
    allPseudoMastery.map(p => [p.nbme, p.qid, p.choice || "?", p.note, p.link])
  );
}
```

---

## 🚨 跨套题错题清单

```dataviewjs
const pages = dv.pages('#做题结果').sort(p => p.nbme);
const allWrong = [];

for (const p of pages) {
  const qs = p.qs || [];
  const wrongQs = qs.filter(q => q.result === "wrong");
  for (const q of wrongQs) {
    allWrong.push({
      nbme: p.nbme,
      qid: q.qid,
      choice: q.my_choice,
      note: q.my_note || "—",
      link: dv.fileLink("NBME" + p.nbme + "_breakdown") + "#Q" + q.qid,
    });
  }
}

if (allWrong.length === 0) {
  dv.paragraph("✨ 目前还没有错题记录。");
} else {
  dv.paragraph(`📊 累积 **${allWrong.length}** 道错题`);
  dv.table(
    ["套题", "题号", "我选", "备注", "跳转"],
    allWrong.map(p => [p.nbme, p.qid, p.choice || "?", p.note, p.link])
  );
}
```

---

## ✏️ 综合复盘 Prompt（做完 4+ 套后用）

```
请读取所有 NBME 做题记录 + breakdown 文件，生成跨套题综合复盘报告：

【输入】
- 所有 _做题结果_NBME*.md（按 nbme frontmatter 找）
- 所有 NBME*_breakdown.md
- 所有 NBME*_学科索引.md

【输出 NBME_综合复盘报告.md】

1. **【学科错误率排行】**
   - 跨套题统计每个学科的正确率
   - 标注哪些学科持续表现差 vs 偶尔翻车
   - 对照 [[薄弱点]] 验证

2. **【反复中招的考点】**
   - 跨套题出现 ≥2 次且我错过/犹豫过的 high_yield_concept
   - 每个考点列出涉及的 NBME## Q###

3. **【陷阱模式归类】**
   - 统计 trap_type 累积出现次数
   - 找出最容易掉的陷阱 TOP 5
   - 给每类陷阱写 3-5 句"反陷阱口诀"

4. **【思维错误归类】**
   - 统计 thinking_error_type 累积出现次数
   - 识别核心认知盲区

5. **【伪掌握警报】**
   - 跨套题累积的低置信度答对题
   - 涉及哪些考点？这些是真考试高危区

6. **【考前 7 天必看清单】**
   - 基于以上分析，列出 30-50 个最关键考点
   - 每个考点链接到 vault 笔记 + 涉及的 NBME 题号

7. **【vault 笔记建议】**
   - 哪些主笔记该加 #薄弱点 / #考前必看
   - 哪些应该生成 _衍生_xxx 专题（用 🌱 TODO 标记）
   - 哪些 mistakes/uworld-mistakes 错题该回顾
```

---

## 🔗 快速跳转

- 📋 [[复习入口_Dashboard]]
- 🎯 [[薄弱点]]
- 📊 [[诊断报告]]
- 📚 [[错题本]]
- 🗂️ [[NBME/nbme-records|NBME 记录目录]]
