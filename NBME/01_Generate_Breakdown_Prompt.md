# NBME 批量 Breakdown 生成 Prompt（v6.2 — 4 Section 拆分 + 编辑友好版）

> **v6.2 关键变化**（基于 v6.1 试跑反馈）：
> - 🆕 **拆 200 题为 4 个 Section 文件**：单文件 1.3MB→320KB，避免 Obsidian 编辑卡顿
> - 🆕 **每 Section 独立 frontmatter**：`section: 1/2/3/4` + `section_range: Q001-Q050`
> - 🆕 **跨 Section wiki-link**：`[[NBME10A_S2_breakdown#^Q078]]` 跳转
> - 🆕 **统一文件夹**：`NBME/nbme-records/NBME{NN}{A/B}/` 内放全部 ~9 个文件
> 
> **v6.1 继承**（已并入正式格式）：
> - ✅ 单题内部新顺序：💡→🔑→✅→🧠→📊→🎣→❌（移到末尾）→✏️ Peixuan 补充 →🔗→元数据沉底
> - ✅ 每题预留 `✏️ Peixuan 补充笔记` 区（提问/讨论/UW同类题三栏；**不嵌套 callout**，直接用 `> -` 列表 — 编辑时只需 `>` 单层引用）
> - ✅ 元数据全部沉底到单题 callout 末尾（v5 在顶 → v6.1 沉底）
> - ✅ frontmatter 启用 `cssclasses: full-width`（配 `.obsidian/snippets/full-width.css`）
> 
> **v6 继承**：
> - ❌ 删除 `related_vault` 元数据字段
> - ❌ 「🔗 关联 vault」段落不写主学科链接（跳大文件顶部无意义）
> - ✅ 只保留精准跳转链接（11 个专题白名单 + TODO + 同类题）
> 
> **v5 继承**：
> - ✅ 做题结果模板（4 Section 表格，预填 Q#/学科/主题/HY）
> - ✅ 支持二刷架构（round 字段）

---

## 📋 给 AI 的指令（直接复制以下内容喂给 Claude Code）

```
你是一位 USMLE Step 2 CK 备考助手。我会给你一份 NBME 模拟题的题目+官方解析 PDF（共 ~200 题）。

请生成 **8 个 Markdown 文件**，全部放进 `NBME/nbme-records/NBME{NN}{A/B}/` 文件夹（如 `NBME10A/`）：

1. **`NBME10A_S1_breakdown.md`** — Section 1 题目详解（Q001-Q050，折叠 callout）
2. **`NBME10A_S2_breakdown.md`** — Section 2 题目详解（Q051-Q100）
3. **`NBME10A_S3_breakdown.md`** — Section 3 题目详解（Q101-Q150）
4. **`NBME10A_S4_breakdown.md`** — Section 4 题目详解（Q151-Q200）
5. `NBME10A_套题索引.md` — 4 Section 入口 + 全局导航
6. `NBME10A_学科索引.md` — 按学科分组（跨 Section）
7. `NBME10A_考点索引.md` — 按考点/HY 分组（跨 Section）
8. `_做题结果_NBME10A.md` — 4 Section 表格模板（预填 Q# / 学科 / 主题 / HY）

> ⚠️ **v6.2 关键**：题目详解从单文件改成 **4 个 Section 文件**，避免单文件 ~1.3MB 时 Obsidian 卡顿。每文件 ~320KB 流畅。

═══════════════════════════════════════════
🚨 立场声明（首要原则）
═══════════════════════════════════════════

**你不知道用户的做题结果。**

PDF 中的"错题标记"等都来自 PDF 准备者，不代表用户本人对错。

- ❌ 不要写"这是错题"等带预判的措辞
- ❌ 不要根据"对错"调整详略——所有题用**统一详细模板**
- ✅ 用中立语言："USMLE 考生常见思维误区"代替"你容易错"

═══════════════════════════════════════════
🚨 用户 vault 真实结构（必须严格对齐）
═══════════════════════════════════════════

✅ 学科主笔记：`[[完整笔记/Peixuan分科笔记/{学科名}]]`
✅ 专题笔记：`[[完整笔记/专题笔记/{笔记名}]]`
❌ 禁止：`[[完整笔记/{学科}]]`（缺少 Peixuan分科笔记 层）
❌ 禁止：`[[完整笔记/Peixuan分科笔记/心内#PPCM]]`（不要 #章节锚点）

═══════════════════════════════════════════
🚨 学科白名单（必须严格使用）
═══════════════════════════════════════════

22 个真实学科：
```
Biostats_Master / derm / endocrine / ethics / Ethics_Master / GI / GYN /
hematology oncology / neuro / newborn care and screening / OB / psych /
pulmonary / 儿科 / 免疫疫苗 / 外科 / 心内 / 感染 / 消化腺 / 消化补充内容 /
眼科 / 肾脏 / 骨科
```

**强制重定向映射**：

| AI 想用的 | 必须重定向到 |
|---|---|
| 血管外科 / PAD / Leriche | `心内` |
| 心血管 / 心脏病 / 冠心病 | `心内` |
| 预防医学 / Prevention / 死因排序 | `Biostats_Master` |
| 急诊（按系统归） | 气胸→pulmonary / ACS→心内 |
| 胸外科 | `pulmonary` + 副 `外科` |
| 血液 / 血小板病 / 凝血 | `hematology oncology` |
| 肿瘤 / 癌症 | `hematology oncology` 或 副归相关系统 |
| 消化 / 胃肠 | `GI` |
| 胰腺/胆道外科 | `GI` + 副 `外科` |
| 妇科 / 月经 | `GYN` |
| 产科 / 围产期 | `OB` |
| 精神 / 抑郁 | `psych` |
| 神经 / 脑卒中 | `neuro` |
| 神经外科 | `neuro` + 副 `外科` |
| 内分泌 / 糖尿病 | `endocrine` |
| 肾内 | `肾脏` |
| 泌尿外科 | `外科` + 副 `肾脏` |
| 皮肤 | `derm` |
| 风湿 / 免疫 / 疫苗 | `免疫疫苗` |
| 感染 / 传染病 / 微生物 | `感染` |
| 儿科（除新生儿） | `儿科` |
| 新生儿 | `newborn care and screening` |
| 眼科 | `眼科` |
| 骨科 / 创伤 | `骨科` |
| 伦理 / 法律 / 沟通 | `ethics` 或 `Ethics_Master` |
| 公共卫生 / 卫生系统 | `Biostats_Master` |
| 普外 | `外科` |

**双归属**：跨学科题用 subject_primary + subject_secondary。

═══════════════════════════════════════════
🚨 已建专题笔记白名单
═══════════════════════════════════════════

仅以下 11 个可在 related_vault 链接：
- [[完整笔记/专题笔记/USMLE广告题解题策略]]
- [[完整笔记/专题笔记/USMLE临床试验分期]]
- [[完整笔记/专题笔记/Biostats_6指标决策树_纯净版]]
- [[完整笔记/专题笔记/TORCH]]
- [[完整笔记/专题笔记/Turner_综合征]]
- [[完整笔记/专题笔记/产科新生儿感染抗生素对照表]]
- [[完整笔记/专题笔记/孕期致畸药]]
- [[完整笔记/专题笔记/避孕]]
- [[完整笔记/专题笔记/_衍生_鉴别诊断速查]]
- [[完整笔记/专题笔记/_衍生_高频评分_公式]]
- [[完整笔记/专题笔记/_衍生_高频陷阱]]

其他高频主题 → 用 🌱 TODO 标注："等积累足够，请 Claude Code 生成 [[完整笔记/专题笔记/_衍生_xxx]]"

═══════════════════════════════════════════
一、输出文件清单（共 8 个 — v6.2）
═══════════════════════════════════════════

对一套 NBME（假设第 10A 套），全部生成到 `NBME/nbme-records/NBME10A/` 文件夹：

1. `NBME10A_S1_breakdown.md` — Section 1 详解（Q001-Q050）
2. `NBME10A_S2_breakdown.md` — Section 2 详解（Q051-Q100）
3. `NBME10A_S3_breakdown.md` — Section 3 详解（Q101-Q150）
4. `NBME10A_S4_breakdown.md` — Section 4 详解（Q151-Q200）
5. `NBME10A_套题索引.md`
6. `NBME10A_学科索引.md`
7. `NBME10A_考点索引.md`
8. `_做题结果_NBME10A.md`

═══════════════════════════════════════════
二、文件 1-4：Section breakdown 文件结构（v6.2 拆分版）
═══════════════════════════════════════════

【每个 Section 文件顶部 frontmatter】

```yaml
---
nbme: 10A
section: 1                          # ⭐ v6.2 新增：1/2/3/4
section_range: Q001-Q050            # ⭐ v6.2 新增
total_questions_in_section: 50
generated_date: 2026-05-13
cssclasses:
  - full-width                      # ⭐ v6.1：宽屏（配 .obsidian/snippets/full-width.css）
tags:
  - USMLE-Step2
  - NBME模拟题
---
```

【每个 Section 文件头部】

```markdown
# NBME 10A — Section 1 Breakdown（Q001-Q050）

> [!info] Section 1 信息
> - 套题：NBME 10A
> - Section：1（题号范围 Q001-Q050）
> - 总题数：50

> [!info]- 🔀 跨 Section 跳转
> - **套题入口**：[[NBME10A_套题索引]]
> - **其他 Section**：
>   - [[NBME10A_S2_breakdown]] — Q051-Q100
>   - [[NBME10A_S3_breakdown]] — Q101-Q150
>   - [[NBME10A_S4_breakdown]] — Q151-Q200
> - **做题结果**：[[_做题结果_NBME10A]]

## 📑 本 Section 题目列表（点击题号跳转）

| Q# | 学科 | 主题 | HY |
|----|------|------|----|
| [Q001](#q001) | 心内 | Leriche 综合征 | 4 |
| [Q002](#q002) | Biostats_Master | 女性首位死因 | 3 |
| ...（本 section 50 题）

---

## 📝 题目详解（Section 1）

###### Q001
> [!example]- NBME10A Q001 心内 / Leriche 综合征（主髂动脉闭塞）
> ^Q001
> 
> ### 💡 一句话锁定
> ... (单题 9 部分内容，详见下方"三")
```

⭐ **v6.2 关键：题号锚点保持全局**

每题用 `^Q001` ~ `^Q200` 锚点（**不重置编号**），这样跨 Section 跳转：
- `[[NBME10A_S1_breakdown#^Q012]]` 跳到 S1 文件的 Q012
- `[[NBME10A_S3_breakdown#^Q127]]` 跳到 S3 文件的 Q127

⭐ **v6 已删除字段**：`related_vault`（不要再生成）

⭐ **v5 必备字段**：`topic_short`
- 长度：**10 个中文字符或 15 个英文字符以内**
- 内容：看一眼就能想起这道题
- 示例：`Leriche 综合征`、`PPCM 诊断`、`NNT 计算`、`ITP vs TTP`

═══════════════════════════════════════════
三、单题 10 部分内容（v6.1 调整后顺序 — 严格遵守）
═══════════════════════════════════════════

每题 callout 内部按以下顺序写（先讲题、再击破干扰项、再留补充位、元数据沉底）：

1. **^Q### 锚点**（紧跟 `[!example]-` 行）
2. **💡 一句话锁定**（> [!tip] callout）
3. **🔑 Stem 关键词识别**（表格：Key Clue / Why It Matters / 中文解析）
4. **✅ 答案 + Core Concept**（英中双语 + 为什么选这个）
5. **🧠 机制理解**（> [!info] + ASCII 图）
6. **📊 High-Yield 速查对比表**（视情况，常需）
7. **🎣 Memory Hook**（**不嵌套 callout**，用粗体 + 列表）
8. **❌ 干扰项击破**（移到这 — 含**最强干扰项**单一总结）
9. **✏️ Peixuan 补充笔记**（预留区，**不嵌套 callout**；详见下方 § 三-A）
10. **🔗 关联 vault**（v6 规则，详见下方 § 三-B）
11. **`---` 分隔**
12. **元数据**（沉底；详见下方 § 六）

⚠️ **关键禁忌**：
- 不要把 `[!note]` 等嵌套 callout 写进 `✏️ Peixuan 补充笔记`（编辑时需 `> >` 双层引用，用户编辑容易破坏 callout 结构）
- 用 `>` 单层 + 普通粗体/列表即可
- 顺序不能颠倒（NBME 招牌的"先讲透再批判"哲学，元数据放底部 = 阅读时不挡眼）

═══════════════════════════════════════════
三-A：✏️ Peixuan 补充笔记区模板（v6.1 新增）
═══════════════════════════════════════════

每题在「干扰项击破」之后、「关联 vault」之前，固定插入：

```markdown
> ### ✏️ Peixuan 补充笔记
> 
> *提示：直接告诉 Claude Code 你要加的内容（提问/卡点/老师讲解/UW题号），我会帮你格式化插入这里，你不用手敲 `>` 标记。*
> 
> **我的提问 / 卡点**：
> - 
> 
> **新发现 / 老师讲解**：
> - 
> 
> **UWorld / 其他套题同类题**：
> - UW Q
```

⚠️ **必须用单层 `>` 引用** — 不要嵌套 `[!note]` callout（导致 `> >` 双层引用 + 用户编辑易出错）

═══════════════════════════════════════════
三-B：🔗 关联 vault 段落规则（v6 不变）
═══════════════════════════════════════════

⚠️ **核心原则：只保留能精准跳转的链接，删除所有跳到大文件顶部的链接**。

❌ **不要写以下内容**：
- 主学科链接：`[[完整笔记/Peixuan分科笔记/心内]]`（跳到大文件顶部无意义）
- 其他学科的主笔记链接：`[[完整笔记/Peixuan分科笔记/neuro]]`（同上）
- 任何 `#章节` 锚点（章节不存在）

✅ **可以写以下内容**：

1. **专题笔记链接**（仅限 11 个已建专题白名单内）
   - `[[完整笔记/专题笔记/USMLE临床试验分期]]`
   - `[[完整笔记/专题笔记/_衍生_高频陷阱]]`
   - 等等

2. **🌱 TODO 标注**（给 Claude Code 未来用）
   - "等血管疾病错题积累后，请 Claude Code 整合生成 [[完整笔记/专题笔记/_衍生_血管性跛行鉴别]]"

3. **同类题占位**（初始留空，Claude Code 跨套题分析后填）
   - "同类题：（初始留空，由 Claude Code 跨套题分析后补充）"

【新版「🔗 关联 vault」模板】：

```markdown
> ### 🔗 关联 vault
> 
> **相关专题笔记**（仅在确实有相关已建专题时写）：
> - [[完整笔记/专题笔记/USMLE临床试验分期]]
> 
> **🌱 TODO（待生成衍生笔记）**：
> - 等血管性疾病类错题积累后，请 Claude Code 整合生成 [[完整笔记/专题笔记/_衍生_血管性跛行鉴别]]
> 
> **同类题**：（初始留空，由 Claude Code 跨套题分析后补充）
> -
```

⚠️ **如果题目和 11 个已建专题完全无关 + 没有合适的衍生 TODO**：
- "相关专题笔记"那一节**整个省略**
- 只保留"🌱 TODO"和"同类题"两节
- 宁可简短，不要硬塞无效链接

═══════════════════════════════════════════
四、文件 5：做题结果模板（⭐ v5 新增）
═══════════════════════════════════════════

生成 `_做题结果_NBME09.md`，结构如下：

```markdown
---
nbme: 09
date: 
round: 1
status: not_started
total_score: 
target: 250
duration_minutes: 
tags:
  - USMLE-Step2
  - NBME模拟题
  - 做题结果
---

# NBME 09 做题结果（第 1 刷）

> [!info] 套题信息
> - **套题入口**：[[NBME10A_套题索引]]
> - **题目详解**（v6.2 4 Section）：[[NBME10A_S1_breakdown]] · [[NBME10A_S2_breakdown]] · [[NBME10A_S3_breakdown]] · [[NBME10A_S4_breakdown]]
> - **学习视图**：[[NBME10A_学习Dashboard]]
> - **全局视图**：[[NBME_全局学习Dashboard]]

---

[Dataview 统计代码块 - 见 v5 模板]

[Dataview 错题快速跳转代码块 - 见 v5 模板]

[Dataview 按学科聚合代码块 - 见 v5 模板]

---

# 📝 做题数据输入区

## Section 1（Item 1-50）

| Q# | 学科 | 主题 | HY | r/w | mk | 选 | 备注 |
|----|------|------|----|-----|----|----|------|
| 1  | 心内 | Leriche 综合征 | 4 |    |    |    |      |
| 2  | Biostats_Master | 女性首位死因 | 3 |    |    |    |      |
| 3  | pulmonary | 气胸处理 | 5 |    |    |    |      |
...（继续到 50）

## Section 2（Item 51-100）
...（同上结构，Q51-Q100）

## Section 3（Item 101-150）
...

## Section 4（Item 151-200）
...

---

## ✏️ 复盘行动清单
... (固定模板内容)
```

⭐ **关键要求**：

1. **Q#、学科、主题、HY 4 列必须预填**：
   - `Q#` = 题号（1-200，纯数字）
   - `学科` = 该题的 `subject_primary`
   - `主题` = 该题的 `topic_short`（v5 新增字段）
   - `HY` = 该题的 `high_yield_score`（数字）

2. **`r/w`、`mk`、`选`、`备注` 4 列保持空**

3. **严格 200 行**：4 个 Section 共 200 题，不能少不能多

4. **Section 划分**：
   - Section 1: Q1-Q50
   - Section 2: Q51-Q100
   - Section 3: Q101-Q150
   - Section 4: Q151-Q200

5. **Section 标题格式必须是**：`## Section 1（Item 1-50）`
   - 半角圆括号
   - 「Item 起-止」格式
   - 这个格式是 Dataview 脚本识别 Section 边界用的

6. **跨学科题如何写学科列**：
   - 如果 `subject_secondary` 非空：填 `主学科/副学科`（如 `GI/外科`）
   - 否则只填 `subject_primary`

═══════════════════════════════════════════
五、文件 5-7：三个索引文件（v6.2 调整 — 链接指向 Section 文件）
═══════════════════════════════════════════

⭐ **v6.2 调整**：索引文件的 wiki-link 必须指向**对应 Section breakdown 文件**的题目锚点，不再指向单文件。

### 5. `NBME10A_套题索引.md`（4 Section 入口 + 全局导航）

```markdown
---
nbme: 10A
type: 套题索引
tags: [USMLE-Step2, NBME模拟题, 索引]
---

# NBME 10A 套题索引

## 📁 文件清单
- [[NBME10A_S1_breakdown]] — Section 1（Q001-Q050）
- [[NBME10A_S2_breakdown]] — Section 2（Q051-Q100）
- [[NBME10A_S3_breakdown]] — Section 3（Q101-Q150）
- [[NBME10A_S4_breakdown]] — Section 4（Q151-Q200）
- [[NBME10A_学科索引]]
- [[NBME10A_考点索引]]
- [[_做题结果_NBME10A]]
- [[NBME10A_学习Dashboard]]（从模板复制）

## 📊 全套统计（自动汇总，待填）
- 总题数：200
- HY 分布：5⭐ ≈10题 / 4⭐ ≈50题 / 3⭐ ≈80题 / 2⭐ ≈50题 / 1⭐ ≈10题
- 学科分布：见 [[NBME10A_学科索引]]
```

### 6. `NBME10A_学科索引.md`（跨 4 Section 聚合）

按学科分组列出所有 200 题。每题 link 用：
`[[NBME10A_S{1/2/3/4}_breakdown#^Q###]]`

示例：
```markdown
## 心内（约 25 题）
- [[NBME10A_S1_breakdown#^Q001]] Leriche 综合征 (HY 4)
- [[NBME10A_S1_breakdown#^Q017]] AFib 抗凝 (HY 5)
- [[NBME10A_S2_breakdown#^Q063]] PPCM 诊断 (HY 4)
- ...
```

### 7. `NBME10A_考点索引.md`（按 HY 分层）

```markdown
## ⭐⭐⭐⭐⭐ HY 5（约 10 题）
- [[NBME10A_S2_breakdown#^Q067]] anti-TNF 前 TB 筛查 — GI/感染
- ...

## ⭐⭐⭐⭐ HY 4（约 50 题）
- ...
```

═══════════════════════════════════════════
六、Frontmatter 字段定义（完整版）
═══════════════════════════════════════════

每题元数据：

```
> **元数据**
> - subject_primary: 心内              # 从白名单选
> - subject_secondary:                 # 跨科时填
> - subject_en: Cardiology
> - subtopic: PPCM, 心力衰竭
> - system: Cardiovascular
> - question_type: diagnosis           # 见枚举
> - correct_answer: B
> - topic_short: PPCM 诊断              # ⭐ v5 新增（10字以内）
> - high_yield_concept: PPCM 诊断三要素 · 围产期心衰时间窗
> - trap_type: 时间窗陷阱                # 见枚举
> - thinking_error_type: 锚定偏差        # 见枚举
> - stem_pattern: age_sex_主诉锁定        # 见枚举
> - high_yield_score: 4/5
```

⚠️ **v6 移除了 related_vault 字段**：之前用于链接学科主笔记，但跳转无法精准定位（大文件顶部），无效。学科信息已在 subject_primary 中。

枚举值（与 v4 一致）：

`question_type`（13 类）：
diagnosis / management / next_best_step / most_likely / mechanism / 
risk_factor / prevention / screening / pharmacology / biostats_calculation /
biostats_interpretation / ethics_dilemma / communication

`trap_type`（9 类）：
时间窗陷阱 / 首选vs次选 / 概念混淆 / 干扰项相似 / 计算陷阱 / 
机制vs症状 / Screening_vs_Diagnostic / 排除性诊断 / 无陷阱

`thinking_error_type`（6 类）：
锚定偏差 / 模式过早闭合 / 知识盲区 / 选项识别错误 / 
计算操作失误 / 中英文术语混淆

`stem_pattern`（8 类）：
经典三联征 / age_sex_主诉锁定 / 实验室矛盾 / 隐藏时间线 / 
鉴别诊断密集 / 多步推理 / 长stem干扰项 / 简短直击

`high_yield_score` 分布（200 题预期）：
- HY 5: ~5%
- HY 4: ~25%
- HY 3: ~40%
- HY 2: ~25%
- HY 1: ~5%

═══════════════════════════════════════════
七、Callout 格式严格规则（与 v4 一致）
═══════════════════════════════════════════

🚨 每行 `>` 开头（包括空行、表格行、代码块）
🚨 题间用 `> ---` + 普通空行 + `###### Q###` 分隔

═══════════════════════════════════════════
八、版权与风格（与 v4 一致）
═══════════════════════════════════════════

⚠️ 不复制原文（重述）
⚠️ 引用 ≤ 15 个英文连续单词
✅ 中英双语术语
✅ ASCII 图代替 Mermaid

═══════════════════════════════════════════
九、最终自检清单（v6.2）
═══════════════════════════════════════════

**文件结构**：
□ **8 个文件**全部生成（4 Section breakdown + 3 索引 + 做题结果模板）
□ 全部放进 `NBME/nbme-records/NBME{NN}{A/B}/` 文件夹
□ Section 文件命名：`NBME{NN}{A/B}_S{1/2/3/4}_breakdown.md`
□ 每个 Section 文件 frontmatter 含 `section: 1/2/3/4` + `section_range: Q###-Q###` + `cssclasses: full-width`

**单题分配**：
□ S1 = Q001-Q050 / S2 = Q051-Q100 / S3 = Q101-Q150 / S4 = Q151-Q200
□ 每题在折叠 `[!example]-` callout 内
□ `^Q###` 锚点不重置编号（全局 Q001-Q200，便于跨 Section wiki-link）

**单题内部顺序**（v6.1 调整后，严格遵守）：
□ ① 💡 锁定 → ② 🔑 关键词 → ③ ✅ 答案 → ④ 🧠 机制 → ⑤ 📊 HY 速查 → ⑥ 🎣 Memory Hook → ⑦ ❌ 干扰项击破 → ⑧ ✏️ Peixuan 补充 → ⑨ 🔗 关联 → ⑩ 元数据沉底
□ **✏️ Peixuan 补充笔记**预留区（三栏：提问/讨论/UW同类，**不嵌套 callout**，用 `>` 单层 + 普通粗体/列表）
□ 元数据沉底到单题 callout 末尾（不在顶部）

**元数据字段**：
□ 每题元数据齐全（含 `topic_short` ≤ 10 中文字符）
□ **不含** `related_vault` 字段（v6 已移除）
□ `subject_primary` 100% 来自 22 学科白名单
□ 三维度枚举值都从清单选

**关联 vault**（v6 规则）：
□ 不含主学科链接 / 不含其他学科主笔记链接 / 无 #章节锚点
□ 专题链接只用 11 个白名单（题目确实相关时才写）

**索引文件**（v6.2 调整）：
□ 套题索引列出 4 Section 文件入口
□ 学科索引 / 考点索引的题目链接用 `[[NBME{NN}A_S{X}_breakdown#^Q###]]` 跨 Section 跳转

**HY 分布**：
□ HY 分布合理（5:25:40:25:5）
□ 干扰项后只写一次「最强干扰项」

**做题结果模板**：
□ 4 个 Section × 50 题 = 200 行
□ Q# / 学科 / 主题 / HY 4 列预填，其余 4 列空
□ Section 标题格式：`## Section X（Item Y-Z）`
□ frontmatter 含 `tags: [做题结果]` 和 `round: 1`

**其他**：
□ Memory Hook 不嵌套 callout
□ tags 无 #高频 #陷阱 等手动标签
□ 无"错题"等预判语言
```

---

## 🎯 用法 SOP

### Phase 1：生成 8 个文件

1. 复制上面方框内的 prompt
2. 附上 NBME PDF（或截图）
3. Claude Code 输出 8 个文件 → 全部入库到对应 NBME 子文件夹：

```
NBME\nbme-records\NBME10A\
├── NBME10A_S1_breakdown.md      ⭐ Q001-Q050
├── NBME10A_S2_breakdown.md      ⭐ Q051-Q100
├── NBME10A_S3_breakdown.md      ⭐ Q101-Q150
├── NBME10A_S4_breakdown.md      ⭐ Q151-Q200
├── NBME10A_套题索引.md          ← 4 Section 入口
├── NBME10A_学科索引.md
├── NBME10A_考点索引.md
├── _做题结果_NBME10A.md          ⭐ 已预填 Q#/学科/主题/HY
└── NBME10A_学习Dashboard.md      ← 从模板单独复制
```

⚠️ **v6.2 性能优势**：单文件 ~320KB（vs v6 的 ~1.3MB），Obsidian 编辑流畅

### Phase 2：复制学习 Dashboard

从模板 `NBME12_学习Dashboard_v2.md` 复制改名 `NBME09_学习Dashboard.md`，改 frontmatter `nbme: 09`。

### Phase 3：做题 + 阶段 1 截图识别填表

用 NBME Fighter 截图识别 prompt v2（分 section 录入版）填 r/w 和 mk 列。

### Phase 4：阶段 2 复盘补 my_choice 和 my_note

打开学习 Dashboard 看分类列表，点击跳转看解析，补关键题字段。

### Phase 5（可选）：二刷错题和标记题

```bash
copy _做题结果_NBME09.md _做题结果_NBME09_R2.md
```

打开新文件：
- 改 frontmatter `round: 2`
- 清空 `r/w` `mk` `选` `备注` 4 列（学科/主题/HY 保留）
- 只填你计划二刷的题（一般是一刷的 wrong + marked）

全局 Dashboard 会自动识别 round 字段，做横向对比（v6 升级会加这功能）。

---

## ⚠️ v6.2 关键变化总结

### v6.1 → v6.2（性能拆分）
| v6.1 | v6.2 |
|---|---|
| 单文件 200 题 (~1.3MB) | **4 Section 文件，每文件 ~320KB** |
| 单文件名 `NBME09_breakdown.md` | `NBME10A_S{1/2/3/4}_breakdown.md` |
| frontmatter 无 section 字段 | 新增 `section: 1/2/3/4` + `section_range: Q###-Q###` |
| 索引文件 link 跳单文件 | 索引文件 link 跨 Section 跳转 `[[NBME10A_S{X}_breakdown#^Q###]]` |
| 文件分散在 NBME/ 根目录 | 全部入 `NBME/nbme-records/NBME{NN}{A/B}/` 子文件夹 |

### v6.0 → v6.1（编辑友好性）
| v6.0 | v6.1 |
|---|---|
| 元数据在单题顶部 | **元数据沉底**（callout 末尾）|
| 干扰项击破在答案后立即 | **干扰项移到 Memory Hook 之后** |
| 无 Peixuan 补充笔记区 | ⭐ **新增 ✏️ Peixuan 补充笔记**（三栏预留位）|
| 视觉默认 readable line length | ⭐ **`cssclasses: full-width`** 满宽 |
| Peixuan 补充用嵌套 `[!note]` | ❌ 改用单层 `>` + 粗体（避免 `> >` 双层引用编辑陷阱）|

### v5 → v6.0（精简关联）
| v5 | v6 |
|---|---|
| 元数据有 `related_vault` 字段 | ❌ **删除** |
| 关联 vault 含主学科链接 | ❌ **删除**所有主学科链接 |
| 关联区强制写"核心笔记 + 延伸考点" | ✅ 只写"专题白名单 + TODO + 同类题" |

### v4 → v5
| v4 | v5 |
|---|---|
| 元数据无 topic_short | ⭐ 元数据新增 topic_short（≤10 字主题） |
| 生成 4 个文件 | 生成 5 个文件（多了做题结果模板） |
| 不支持二刷 | frontmatter 加 round 字段，原生支持二刷 |

---

**v6.2 核心哲学**：
1. **链接必须能精准跳转** — 跳大文件顶部的链接 = 无效
2. **物理结构对齐使用结构** — NBME 自己 4 Section → 文件也 4 Section
3. **编辑友好优先** — 单层 `>`、补充笔记预留、元数据沉底，让 Peixuan 自己加内容时零思考成本
4. **性能可持续** — 单文件 ~320KB 是 Obsidian 流畅区间，未来 200+ 题/套也扛得住
