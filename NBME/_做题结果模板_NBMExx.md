---
nbme: 12
date: 
status: not_started      # not_started / in_progress / completed / reviewed
total_score: 
target: 250
duration_minutes: 
review_pass: 0           # 已复盘轮次（0 = 还没复盘）
tags:
  - USMLE-Step2
  - NBME模拟题
  - 做题结果
---

# NBME 12 做题结果

> [!info] 套题信息
> - **主文件**：[[NBME12_breakdown]]
> - **套题索引**：[[NBME12_套题索引]]
> - **学科索引**：[[NBME12_学科索引]]
> - **考点索引**：[[NBME12_考点索引]]

---

## 📊 实时统计（Dataview 自动生成）

```dataview
TABLE WITHOUT ID
  "已答题数" as "字段",
  length(filter(this.qs, (q) => q.result != null)) as "数值"
WHERE file.name = this.file.name
```

> [!tip]- 📈 详细统计（点击展开）
> 
> ```dataviewjs
> // 自动统计当前文件的做题数据
> const page = dv.current();
> const qs = page.qs || [];
> 
> const answered = qs.filter(q => q.result);
> const correct = qs.filter(q => q.result === "right");
> const wrong = qs.filter(q => q.result === "wrong");
> const marked = qs.filter(q => q.result === "marked");
> const unanswered = qs.filter(q => !q.result || q.result === "blank");
> 
> // 置信度
> const lowConf = qs.filter(q => q.conf === "low");
> const highConfRight = qs.filter(q => q.result === "right" && q.conf === "high");
> const lowConfRight = qs.filter(q => q.result === "right" && q.conf === "low");
> 
> dv.table(["指标", "数值", "占比"],
>   [
>     ["✅ 答对", correct.length, ((correct.length / 200) * 100).toFixed(1) + "%"],
>     ["❌ 答错", wrong.length, ((wrong.length / 200) * 100).toFixed(1) + "%"],
>     ["🏷️ 标记/犹豫", marked.length, ((marked.length / 200) * 100).toFixed(1) + "%"],
>     ["⬜ 未答", unanswered.length, ((unanswered.length / 200) * 100).toFixed(1) + "%"],
>     ["---", "---", "---"],
>     ["🟢 高置信度答对（真会）", highConfRight.length, "确认掌握"],
>     ["🔴 低置信度答对（蒙对/伪掌握）", lowConfRight.length, "⚠️ 高危区"],
>     ["📊 正确率（已答）", correct.length + "/" + answered.length, 
>      answered.length > 0 ? ((correct.length / answered.length) * 100).toFixed(1) + "%" : "—"],
>   ]
> );
> ```

---

## 📝 题目状态表

> [!example]- 📌 状态说明（首次使用展开）
> 
> **result 字段**（4 选 1）：
> - `right` ✅ 答对
> - `wrong` ❌ 答错
> - `marked` 🏷️ 标记（不确定/犹豫，留待复查）
> - `blank` ⬜ 未答（默认）
> 
> **conf 字段（置信度）**（3 选 1）：
> - `high` 🟢 秒选、有把握
> - `medium` 🟡 想了想
> - `low` 🔴 蒙的、纠结的
> 
> ⚠️ **关键**：答对但 `conf: low` = **伪掌握**（真考试翻车高危区）
> 
> ---
> 
> **三种填写策略**（任选其一）：
> 
> 🅰️ **手动全填**（推荐二刷/复盘时用）
> - 一次性把 200 行填完
> - 最准确，置信度信息最完整
> 
> 🅱️ **双轨制**（推荐一刷模拟考用）
> - 第 1 步：用 NBME 软件做完整套
> - 第 2 步：截图喂 Claude Code，让它只填 `result` 列（对/错）
> - 第 3 步：你手动只补 `conf` + `my_note`，且**只补 wrong + marked + 不确定的题**
> - 答对且没犹豫的题留 `conf: ` 空着即可
> 
> 🅲️ **极简模式**（时间紧急）
> - 只填 result 列
> - 跳过 conf 和 my_note
> - 复盘价值降低 60%，但比不填强

### 题目列表（200 行）

```dataview
TABLE WITHOUT ID
  qid as "Q#",
  result as "结果",
  conf as "置信度",
  my_choice as "我选",
  my_note as "备注"
FROM ""
WHERE file.name = this.file.name
FLATTEN qs as q
WHERE q.qid
SORT q.qid ASC
```

<!-- ↓↓↓ 数据存储区（不要删除这部分）↓↓↓ -->

> [!example]- 📋 完整 200 题数据（点击展开/折叠编辑）

```yaml
qs:
  - qid: "001"
    result: 
    conf: 
    my_choice: 
    my_note: 
  - qid: "002"
    result: 
    conf: 
    my_choice: 
    my_note: 
  - qid: "003"
    result: 
    conf: 
    my_choice: 
    my_note: 
  - qid: "004"
    result: 
    conf: 
    my_choice: 
    my_note: 
  - qid: "005"
    result: 
    conf: 
    my_choice: 
    my_note: 
  # ... 继续到 Q200，模板生成时由 AI 一次性铺好
```

---

## 🎯 错题快速跳转（Dataview 自动筛选）

```dataviewjs
const page = dv.current();
const qs = page.qs || [];
const wrong = qs.filter(q => q.result === "wrong");
const marked = qs.filter(q => q.result === "marked");
const lowConfRight = qs.filter(q => q.result === "right" && q.conf === "low");
const nbme = page.nbme;

if (wrong.length > 0) {
  dv.header(3, "❌ 错题（" + wrong.length + " 道）");
  dv.list(wrong.map(q => 
    `[[NBME${nbme}_breakdown#Q${q.qid}|Q${q.qid}]] — 我选 ${q.my_choice || "?"} | ${q.my_note || ""}`
  ));
}

if (marked.length > 0) {
  dv.header(3, "🏷️ 标记题（" + marked.length + " 道）");
  dv.list(marked.map(q => 
    `[[NBME${nbme}_breakdown#Q${q.qid}|Q${q.qid}]] — ${q.my_note || "待复查"}`
  ));
}

if (lowConfRight.length > 0) {
  dv.header(3, "⚠️ 伪掌握警报：低置信度答对（" + lowConfRight.length + " 道）");
  dv.paragraph("> 这些题虽然答对，但你不确定。真考试可能翻车，**和错题同等优先级**！");
  dv.list(lowConfRight.map(q => 
    `[[NBME${nbme}_breakdown#Q${q.qid}|Q${q.qid}]] — 选了 ${q.my_choice} | ${q.my_note || ""}`
  ));
}
```

---

## 🔍 学科表现分析（Dataview 跨文件查询）

```dataviewjs
const page = dv.current();
const qs = page.qs || [];
const nbme = page.nbme;

// 关联学科数据需要 breakdown 文件已存在
// 这里展示模板，实际数据由 Claude Code 复盘时填充
dv.paragraph("📊 学科表现分析将在 Claude Code 复盘后生成。");
dv.paragraph("👉 准备好后运行复盘 prompt: `分析 NBME" + nbme + " 错题模式 + 薄弱学科`");
```

---

## ✏️ 复盘行动清单

- [ ] 完成做题，填写完结果表
- [ ] 检查"伪掌握警报"区，标记真正需要复盘的题
- [ ] 把错题 + 标记题 + 伪掌握题对应的 breakdown callout 打开看一遍
- [ ] 在错题对应的 callout 末尾补充【🤯 我为什么错】区块
- [ ] 让 Claude Code 跑复盘 prompt → 生成本套薄弱点报告
- [ ] 1 周后选 10-20 道关键题重做（错题 + 伪掌握）

---

## 📚 复盘 Prompt（做完后复制给 Claude Code）

```
请读取以下文件并生成 NBME{12} 个性化复盘报告：

【输入文件】
- 做题结果：[[NBME12_做题结果]]
- 题目详解：[[NBME12_breakdown]]
- 套题索引：[[NBME12_套题索引]]
- 学科索引：[[NBME12_学科索引]]

【输出要求】
生成 `NBME12_复盘报告.md`，包含：

1. **【总体表现】**
   - 分数估算、正确率
   - 学科正确率排行
   - 对比用户自报薄弱学科（见 [[薄弱点]]），验证是否一致

2. **【错题模式分析】**
   - 按 trap_type 聚合错题，找出我反复掉进的陷阱
   - 按 thinking_error_type 聚合，识别思维盲区
   - 按 stem_pattern 聚合，识别 stem 识别弱点

3. **【伪掌握警报】**
   - 低置信度答对的题，涉及哪些 high_yield_concept？
   - 这些是真考试高危区

4. **【关联到 vault】**
   - 哪些学科主笔记需要加 #薄弱点 标签
   - 哪些题应该 1 周内重做
   - 哪些考点该生成 _衍生_xxx 专题笔记（标 🌱 TODO）

5. **【考前必看清单】**
   - 基于本套表现 + 薄弱点交叉分析
   - 列出 15-25 个最该再看的考点
   - 每个考点链接到 vault 笔记或 breakdown 题号
```
