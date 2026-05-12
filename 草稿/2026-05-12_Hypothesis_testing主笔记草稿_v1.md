---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-05-12
type: 专题笔记草稿
status: 雏形 v1 / 仅 Null hypothesis 章节 / 待逐步补充 Type I-II / Power / p / CI
---

# USMLE Hypothesis Testing 主笔记（草稿 v1）

> [!info] 这张笔记的定位
> 这是 **2026-05-12 Biostats 错题 Q3941 (Null hypothesis)** 触发生成的雏形，将作为未来 [[完整笔记/专题笔记/_衍生_USMLE_统计推断]] 主笔记的核心骨架。
> 
> **整合时机**：等积累 3+ 道 Hypothesis testing 题（含 Type I/II / Power / p-value / CI）后，让 Claude Code 读错题本 + 这份草稿 → 生成最终主笔记。
> 
> **当前进度**：
> - ✅ 第 1 章：Null hypothesis（H0 vs H1 + Study design 决定术语）
> - 🚧 第 2 章：Type I vs Type II error（待积累错题后填充）
> - 🚧 第 3 章：Power（统计效能）
> - 🚧 第 4 章：p-value 解读
> - 🚧 第 5 章：Confidence Interval（CI）
> - 🚧 第 6 章：统计检验选择（t / χ² / ANOVA / 回归）
> 
> **当前素材来源**：Q3941 + 对话扩展讲解

---

## 1. Null Hypothesis（零假设）⭐ 已填充

### 1.1 核心概念

> [!success] 一句话本质
> **Null hypothesis (H0)** = 研究中假定的"**无差异 / 无关联 / 无效应**"状态 — 研究者**想推翻**的假设。

### 1.2 H0 vs H1 对照

| 概念 | 缩写 | 内容 | 角色 |
|---|---|---|---|
| **Null hypothesis** | H0 | 无差异 / 无关联 / 无效应 | 研究者想**推翻** |
| **Alternative hypothesis** | H1 (Ha) | 有差异 / 有关联 / 有效应 | 研究者想**支持** |

**逻辑根基**：科学不能直接证明"有"，只能通过**推翻"没有"**来间接支持"有"。

### 1.3 统计推断核心逻辑

```
        H0：CRP 和结肠癌之间无关联
        H1：CRP 和结肠癌之间有关联
                       |
                       ▼
                  统计分析
                       |
              +--------+--------+
              |                 |
          p < 0.05          p ≥ 0.05
       Reject H0         Fail to reject H0
              |                 |
              ▼                 ▼
       "证据强，支持H1"    "证据不够说有关联"
                          ⚠️ 不等于"证明 H0 为真"！
```

### 1.4 法庭类比

> [!tip] 用法庭审判理解 H0
> - **H0（被告无罪）**：默认假设，必须"超出合理怀疑"才能推翻
> - **H1（被告有罪）**：检察官想证明的
> - **p < 0.05** = 证据足够强 → reject H0 → 接受 H1
> - **p ≥ 0.05** = 证据不够 → fail to reject H0 → 注意：**不是"证明无罪"，是"没法证明有罪"**

### 1.5 Study Design 决定 H0 的术语 ⭐⭐ 核心考点

> [!danger] USMLE 高频陷阱
> Null hypothesis 不仅要"方向对"（陈述"无"），**还要措辞和 study design 匹配**！

| Study Design | 可用测量术语 | 标准 H0 措辞 |
|---|---|---|
| **RCT / Cohort** | RR, Risk, Incidence | "The **risk** of X is the same..." 或 "**No difference in incidence**" |
| **Case-control** | OR | "**OR = 1**" 或 "No association"（OR 是 case-control 唯一可算的关联指标） |
| **Cross-sectional** | Prevalence, POR | "**No association**" 或 "Equal prevalence"（❌ 不能用 risk / incidence） |
| **任何设计** | Association | **"No association between X and Y"** ⭐ 万能、最安全 |

### 1.6 术语速查：Risk / Prevalence / Odds / Association

| 术语 | 含义 | 适用 design |
|---|---|---|
| **Risk** | 新发病例 / 起始人群（前瞻性概念） | Cohort, RCT |
| **Incidence** | 某时段内新发率（前瞻性概念） | Cohort, RCT |
| **Prevalence** | 某时点患病比例 | Cross-sectional |
| **Odds** | 病例组 vs 对照组的暴露 odds 之比 | Case-control |
| **Association** | 中性万能词，不暗示时序/因果 | ⭐ 任何 design |

> [!success] 一刀切原则
> **不确定 H0 措辞时，选用 "no association" 的选项永远安全。**

### 1.7 USMLE Null Hypothesis 题三大错误类型

| 错误类型 | 表现 | 例子 |
|---|---|---|
| **方向错** | 写成 H1（陈述"有关联"） | "Colon cancer is more prevalent in CRP+" |
| **设计错** ⭐ | 方向对但术语和 design 不匹配 | Cross-sectional 用 "risk" / "incidence" |
| **时序错** | 暗示因果方向（cross-sectional 无法判定） | "Cancer does not affect CRP" |

**正确选项 = 同时通过这三道关**：表达"无" + 措辞中性 + 不暗示时序。

### 1.8 做题 SOP（3 步定位 H0）

```
拿到 Null hypothesis 题
        |
        ▼
[Step 1] 识别 study design
        |
   找线索：prevalence? incidence? cases vs controls? randomized?
        |
        ▼
[Step 2] 排除所有 H1 选项
        |
   任何陈述"有关联/有差异/更易/更多/更少"的都是 H1
        |
        ▼
[Step 3] 在剩余选项里选 design 匹配的措辞
        |
   Cross-sectional → 用 "association" / "prevalence"
   Cohort/RCT      → 用 "risk" / "incidence"
   Case-control    → 用 "OR = 1"
   不确定          → 选 "no association"（永远安全）
```

### 1.9 双 vs 单尾假设

| 类型 | H1 表达 | 用法 |
|---|---|---|
| **Two-tailed (双尾)** | A ≠ B | 默认，"新药和安慰剂**有差异**" |
| **One-tailed (单尾)** | A > B 或 A < B | 少用，需事先 justify"新药**优于**安慰剂" |

USMLE 默认双尾，除非 stem 明说单向假设。

### 1.10 Null hypothesis 章节自测

> [!question]- 自测题 1
> 研究者做 **case-control study** 研究"吸烟与膀胱癌"的关系。Cases = 100 个膀胱癌患者；Controls = 100 个无膀胱癌者；问吸烟史。
> 
> 以下哪个是**正确的 null hypothesis**？
> 
> A. The risk of bladder cancer is the same in smokers and non-smokers
> B. The odds ratio of bladder cancer for smokers vs non-smokers is 1
> C. Smoking causes bladder cancer
> D. The incidence of bladder cancer is the same in smokers and non-smokers
> E. Bladder cancer is more prevalent in smokers

> [!question]- 自测题 2
> RCT 研究新降压药 vs 安慰剂，主要 outcome 是 6 个月后血压差异。以下哪个是**正确的 null hypothesis**？
> 
> A. The new drug is better than placebo
> B. The new drug and placebo have the same effect on blood pressure
> C. The prevalence of hypertension is the same in both groups
> D. The new drug causes a greater decrease in blood pressure
> E. There is no association between drug type and patient age

*答完发我，对照后给反馈。*

---

## 2. Type I vs Type II Error 🚧 待填充

> [!info] 占位章节
> 等积累相关错题后填充。预览结构：

| 错误类型 | 含义 | 控制方法 | 概率符号 |
|---|---|---|---|
| Type I error | 错误地 reject H0（H0 真但说假）= 假阳性 | α 水平（一般 0.05） | α |
| Type II error | 错误地 fail to reject H0（H0 假但说真）= 假阴性 | 增大样本量 | β |

> [!tip] 类比记忆（先存着）
> - **Type I (α) = 冤枉好人**（H0 真但被推翻）
> - **Type II (β) = 放过坏人**（H1 真但没识别）

---

## 3. Power（统计效能）🚧 待填充

> [!info] 占位章节
> 预览：
> - **Power = 1 - β** = "H1 为真时，正确 reject H0 的概率"
> - **影响 Power 的 4 个因素**：样本量 ↑ / 效应大小 ↑ / α ↑ / 数据精度 ↑
> - USMLE 高频考点：**怎样增加 Power？** → 增大 sample size（首选答案）

---

## 4. p-value 解读 🚧 待填充

> [!info] 占位章节
> 预览：
> - p-value 的**正确定义**：假设 H0 为真，得到当前观察结果或更极端结果的概率
> - 常见误解：
>   - ❌ "p < 0.05 = H0 错误的概率 < 5%"（错！）
>   - ❌ "p 值越小，效应越大"（错！p 受样本量影响）
> - 临床意义 vs 统计学意义的区别

---

## 5. Confidence Interval（置信区间）🚧 待填充

> [!info] 占位章节
> 预览：
> - 95% CI 的正确解读：重复抽样 100 次，约 95 次的 CI 包含真实参数
> - CI 与统计显著性的关系：
>   - **均值差异 CI 包含 0** → 不显著
>   - **RR / OR 的 CI 包含 1** → 不显著
> - CI 宽度反映精度（样本量 ↑ → CI 越窄）

---

## 6. 统计检验选择 🚧 待填充

> [!info] 占位章节
> 预览决策树：

```
                    要比较什么？
                          |
        +-----------------+-----------------+
        |                                   |
   比较均值（连续变量）              比较比例（分类变量）
        |                                   |
        ▼                                   ▼
   2 组 → t-test                       2 组 → χ² 或 Fisher exact
   ≥3 组 → ANOVA                       ≥3 组 → χ²
   配对 → paired t-test
        |
   相关 / 预测 → 回归分析
   生存数据 → Kaplan-Meier / Cox
```

---

## 7. 关联

- 🔁 **相关错题**：
  - [[mistakes/uworld-mistakes#Q3941]] Null hypothesis（本笔记 1.x 章节主素材）
  - 待补充：Type I/II / Power / p / CI 系列题
- 📚 **主笔记**：
  - [[完整笔记/Peixuan分科笔记/Biostats_Master]]
  - [[完整笔记/专题笔记/Biostats_6指标决策树_纯净版]]（RR/OR/Prevalence 基础）
- 🌱 **TODO**：
  - 等 Hypothesis testing 错题积累 3+ → 让 Claude Code 整合本草稿 + 错题本 → 生成正式 [[完整笔记/专题笔记/_衍生_USMLE_统计推断]]
  - 同期可生成 [[完整笔记/专题笔记/_衍生_USMLE_Bias_5大鉴别]]（今日另一份草稿） + [[完整笔记/专题笔记/USMLE_Study_Design决策树]] —— Biostats 三件套

---

## 8. 一句话章节速查（持续更新）

| 章节 | 一句话精华 |
|---|---|
| **Null hypothesis** | Null = "无关联" + 措辞必须配 study design；"no association" 永远安全 |
| Type I error | 🚧 待填 |
| Type II error | 🚧 待填 |
| Power | 🚧 待填 |
| p-value | 🚧 待填 |
| CI | 🚧 待填 |
| 统计检验 | 🚧 待填 |
