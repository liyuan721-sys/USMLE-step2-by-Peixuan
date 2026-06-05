---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-05-12
updated: 2026-05-12
type: 专题笔记草稿
status: 雏形 v3 / Null hypothesis + CI + OR 表判读 + Confounder vs Independent Risk Factor 已填充 / 待补 Type I-II / Power / p / 统计检验
---

# USMLE Hypothesis Testing 主笔记（草稿 v3）

> [!info] 这张笔记的定位
> 这是 **2026-05-12 Biostats 错题** 触发生成的雏形，将作为未来 [[完整笔记/专题笔记/_衍生_USMLE_统计推断]] 主笔记的核心骨架。
> 
> **整合时机**：等积累 3+ 道 Type I/II / Power / p-value 等题后，让 Claude Code 读错题本 + 这份草稿 → 生成最终主笔记。
> 
> **当前进度（v3）**：
> - ✅ 第 1 章：Null hypothesis（H0 vs H1 + Study design 决定术语）
> - 🚧 第 2 章：Type I vs Type II error（待积累错题后填充）
> - 🚧 第 3 章：Power（统计效能）
> - 🚧 第 4 章：p-value 解读
> - ✅ 第 5 章：Confidence Interval（CI）
> - ✅ 第 6 章：OR 表 / Forest plot 判读
> - ✅ 第 7 章：Confounder vs Independent Risk Factor — **v3 新增核心概念区分**
> - ✅ 第 8 章：USMLE OR 表 5 种题型问法对照 — **v3 新增**
> - ✅ 第 9 章：Confounding（实战）
> - 🚧 第 10 章：统计检验选择（t / χ² / ANOVA / 回归）
> 
> **v3 素材来源**：Q3941（Null hypothesis）+ Q21248（OR/CI 判读 + Confounding）+ 对话深度澄清

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
| **Case-control** | OR | "**OR = 1**" 或 "No association" |
| **Cross-sectional** | Prevalence, POR | "**No association**" 或 "Equal prevalence"（❌ 不能用 risk / incidence）|
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

## 5. Confidence Interval（置信区间）⭐ 已填充

### 5.1 CI 的正确定义

> [!success] 一句话本质
> **95% CI** = "如果重复抽样 100 次、每次都算 CI，约 95 次的 CI 会包含真实参数"
> 
> 不是"真实参数在 CI 内的概率是 95%"（这是常见误解）。

### 5.2 CI 与统计显著性的关系 ⭐⭐ 核心考点

| 测量指标 | Null value | CI 跨 null → | CI 完全偏离 null → |
|---|---|---|---|
| **RR (Relative Risk)** | **1.0** | 不显著 | 显著 |
| **OR (Odds Ratio)** | **1.0** | 不显著 | 显著 |
| **HR (Hazard Ratio)** | **1.0** | 不显著 | 显著 |
| **Mean difference** | **0** | 不显著 | 显著 |
| **Risk difference (RD)** | **0** | 不显著 | 显著 |

> [!danger] 一刀切口诀
> - **比值类指标（RR / OR / HR）→ 看 CI 是否跨 1.0**
> - **差值类指标（mean difference / RD）→ 看 CI 是否跨 0**

### 5.3 CI 宽度反映什么

| CI 宽度 | 含义 | 影响因素 |
|---|---|---|
| **窄 CI** | 估计精确 | 样本量大 / 数据变异小 |
| **宽 CI** | 估计不精确 | 样本量小 / 数据变异大 |

### 5.4 OR 11.84 但 CI 跨 1.0：怎么理解？

> [!warning] 经典陷阱解读
> 
> 一个 OR 的**点估计**（如 11.84）只是"在这次研究里观察到的值"。CI 反映"这个估计有多准"。
> 
> **CI 跨 1.0 意味着：基于现有数据，我们不能排除"真实 OR = 1（无关联）"的可能性**。
> 
> 所以即使点估计看起来很惊人，**只要 CI 跨 1.0，统计上就不能说"有显著关联"**。
> 
> 类比：你测一个人身高，第一次量得 180cm，但量尺误差很大（±50cm）→ 真实身高可能 130-230cm → 不能下结论说"他很高"。

### 5.5 CI 章节自测

> [!question]- 自测题 1
> 一项 RCT 比较新药和安慰剂对死亡率的影响：
> - 新药组死亡率 5%
> - 安慰剂组死亡率 10%
> - RR = 0.5, 95% CI (0.3, 0.85)
> 
> 以下结论**正确**的是：
> 
> A. 新药把死亡风险降低了 50%，且结果统计显著
> B. 新药把死亡风险降低了 50%，但结果不显著
> C. 真实 RR 一定在 0.3 到 0.85 之间
> D. 新药对死亡率无影响
> E. 需要更大样本量才能下结论

> [!question]- 自测题 2
> 一项 case-control 研究"咖啡 - 心律失常"，OR = 1.6, 95% CI (0.8, 3.2)。结论应该是：
> 
> A. 咖啡显著增加心律失常风险
> B. 咖啡可能与心律失常无关联
> C. 咖啡是保护因子
> D. 需要 cohort study 验证
> E. 真实 OR 在 0.8-3.2 之间，所以无意义

---

## 6. OR 表 / Forest Plot 判读 ⭐ 已填充

### 6.1 核心规则：三步法

> [!success] OR 表判读三步
> 1. **只看 Multivariate (adjusted) 那栏** — Bivariate 未控制 confounder，不可信
> 2. **看 95% CI 是否跨 null value (1.0)** — 跨 1.0 = 不显著
> 3. **看患者真的暴露了吗** — 显著 + 暴露 = 答案

### 6.2 Bivariate vs Multivariate

| 维度 | Bivariate (Unadjusted) | Multivariate (Adjusted) ⭐ |
|---|---|---|
| **控制 confounder?** | ❌ 不控制 | ✅ 控制 |
| **哪个更可信?** | ❌ 容易被 confounding 扭曲 | ✅ **真实关联** |
| **看哪个?** | ❌ 不看（除非问"未调整"）| ✅ 永远以此为准 |
| **关注差异时机** | bivariate ≠ multivariate 差很大 → 提示**有强 confounding** |

### 6.3 表脚注释的重要性

> [!warning] "(adjusted for age, sex, X)" 这行小字必须读
> 
> 表脚告诉你**哪些变量被当作 confounder 来调整**。
> 
> ⭐ **关键认知**：被列入 adjusted for 的变量，**在 multivariate 里失去显著性是设计使然，不是 bug**。详见第 7 章。

### 6.4 USMLE OR 表判读三大陷阱

| 陷阱 | 表现 | 修复 |
|---|---|---|
| **只看点估计 OR** | 被 OR 11.84 震住直接选 | 永远先看 CI |
| **看错栏** | 只看 bivariate 忽略 multivariate | "Adjusted 才算数" |
| **忽略表脚** | 没读 "(adjusted for X, Y, Z)" | 表脚揭示哪些变量被当作 confounder |

### 6.5 Forest Plot（森林图）判读

> [!tip] Forest plot = OR 表的图形化版本
> 
> ```
>           OR 点估计 + 95% CI
>           ──────────────────
>           
>   Factor 1   |    *━━━━━           ← 横线 = CI 范围
>              |
>   Factor 2  ━*━━━━━━              ← 跨 1.0 = 不显著
>              |
>   Factor 3   |          *━━━       ← 完全 > 1.0 = 显著危险因素
>              |
>   ───────────|─────────────────
>             1.0 (null line)
> ```
> 
> 判读规则同 OR 表：横线（CI）跨过 1.0 那条竖线 → 不显著。

### 6.6 OR 表判读章节自测

> [!question]- 自测题
> 一项 case-control study 研究"阿司匹林使用与胃溃疡风险"，结果如下：
> 
> | 因子 | Unadjusted OR (95% CI) | Adjusted OR (95% CI) |
> |---|---|---|
> | NSAID 使用 | 3.5 (2.1-5.8) | 3.2 (1.9-5.4) |
> | 阿司匹林使用 | 2.8 (1.6-4.9) | 1.4 (0.7-2.8) |
> | 吸烟 | 1.8 (1.3-2.5) | 1.6 (1.1-2.3) |
> 
> 调整变量：年龄、性别、NSAID 使用、酒精。
> 
> 以下说法**正确**的是：
> 
> A. 阿司匹林是胃溃疡的独立危险因素
> B. NSAID 和吸烟都是独立显著的危险因素
> C. 吸烟的关联可能完全由 NSAID 使用解释
> D. 阿司匹林的真实关联被低估了
> E. 这个研究的样本量不够大

---

## 7. Confounder vs Independent Risk Factor ⭐⭐ v3 新增核心概念

### 7.1 两个完全不同的概念

> [!danger] USMLE 高频混淆点
> 
> "Confounder" 和 "Independent Risk Factor" 是**两个完全不同的角色**，处理方式相反。

| 概念 | 角色 | 处理方式 | 例子 |
|---|---|---|---|
| **Confounder（混杂变量）** | 干扰真实关联的第三方变量 | **要 adjust 掉**（消除影响）| 研究"咖啡→肺癌"时的吸烟 |
| **Independent Risk Factor（独立危险因素）** | 真正独立致病的变量 | **不调整**，让它显示真实效应 | 研究"咖啡→肺癌"时的咖啡本身 |

### 7.2 "Adjusted for" 的真实含义

> [!success] 关键认知（修正常见误解）
> 
> 表脚 "Adjusted for X, Y, Z" 的**真实含义**：
> 
> > **"研究者怀疑 X、Y、Z 可能是 confounder（干扰其他因子和结局的真实关联），所以分析时把它们的影响扣除，看剩下因子的真实独立效应。"**
> 
> **不是**："X、Y、Z 是独立危险因素，所以我们把它们平衡掉"
> 
> **而是**："X、Y、Z 可能是干扰，我们想消除它们，看真相"

### 7.3 类比理解：调音师消除噪音

> [!example] 录音棚类比
> - 你的声音 = **想研究的因子**
> - 环境噪音（空调声、键盘声）= **confounder**
> - 调音师 = **研究者**
> 
> 调音师做的事："我用算法把空调声、键盘声**滤掉**（adjust for），这样听众听到的就是**纯净的人声**。"
> 
> 调音师**不是说**"空调声很重要，我们要给它平衡的露出"。**恰恰相反**：他认为空调声是干扰，所以**消除**它，让人声真实呈现。
> 
> 同样地，研究者把变量列入 adjusted —— 不是因为它们重要值得"展示"，而是因为它们是干扰，需要**滤掉**。

### 7.4 为什么被 adjusted 的变量自己 multivariate 会"失去显著性"？

> [!info] 数学上的"信号被用尽"
> 
> 当一个变量**同时**出现在因子列和表脚 adjusted 列表里（如 Q21248 的 CPB duration）：
> 
> 1. Bivariate 时它独自分析 → OR 包含"直接影响" + "通过其他变量的间接影响"
> 2. Multivariate 时模型先扣除它的影响（作为 confounder），再回头估它的"独立效应" → 已经被"用尽"的信号自然变小
> 3. 加上它和其他因子（如乳酸）可能高度相关 → **多重共线性**让信号被分走

```
真相可能是：
    CPB duration ──► 乳酸升高 ──► ARF
              ↑                  ↑
         "原因之原因"         "直接原因"
         （间接危险）         （独立危险）
```

→ multivariate 失去显著性是**设计使然**，不代表它"没用" — 它的影响主要通过其他途径（乳酸升高）传递。

### 7.5 三种 Multivariate 结果的含义

| Bivariate | Multivariate | 真相 |
|---|---|---|
| 显著 | **显著** | ✅ **真独立危险因素** |
| 显著 | **不显著** | ❌ **伪危险因素**（表观关联来自 confounder）/ 或被相关变量"吃掉"信号 |
| 不显著 | 显著（罕见）| 抑制效应（suppressor effect，偶见）|

### 7.6 Memory Hook

> [!success] 关键口诀
> 
> - **"Adjusted for X" = 想消除 X，不是平衡 X**
> - **被列入 adjusted = 借给隔壁部门用了** — 它自己原本工作的时间就不够了，不是它没用，是工时分出去了
> - **独立危险因素 = multivariate CI 不跨 1.0**（不是"不显著"！）

---

## 8. USMLE OR 表 5 种题型问法对照 ⭐⭐ v3 新增

> [!danger] 不同问法 → 不同答法

| 题目问法 | 怎么答 |
|---|---|
| "**Which is an independent risk factor**?" | 选 multivariate **CI 不跨 1.0** 的（显著）|
| "Most **significant** risk factor for **this patient**" | multivariate 显著 **+ 该患者真的暴露** |
| "Which factor's association is **explained by confounding**?" | 选 bivariate **显著** + multivariate **不显著** 的 |
| "Which factor **lost significance** after adjustment?" | 选 bivariate 显著、multivariate 不显著的 |
| "Which factor needs to be **controlled** in the analysis?" | 选**潜在 confounder**（表脚 adjusted 列表里的，或临床上知道是 confounder 的变量）|

> [!tip] 做题时务必精读题干
> 
> "独立危险因素" ≠ "被 confounding 解释的因素" ≠ "需要控制的变量" — 三种问法考察的是同一张表的不同侧面，答案完全不同。
> 
> **关键习惯**：先问自己"题目要的是哪种角色？"

---

## 9. Confounding 实战应用 ⭐ 已填充

### 9.1 核心概念回顾

> [!info] Confounding ≠ Bias
> Confounding 不是研究"方法错误"，而是**第三变量同时影响暴露和结局** → 即使方法完美也存在。
> 
> 详见 [[完整笔记/专题笔记/_衍生_USMLE_Bias_5大鉴别_草稿]] 第 4 章。

### 9.2 Residual Confounding（残余混杂）

> [!success] 一句话本质
> 看到"调整了 A, B, C"→ 立刻想"D, E, F 没调整呢？"

**Q21248 Item 2 经典例子**：
- 研究调整了 age, sex, CPB duration
- 但临床上还有**其他重要 confounder 没调整**：
  - 术前 creatinine（baseline 肾功能）
  - Proteinuria / albuminuria（已存在肾损伤）
  - ACE inhibitor 使用（影响肾灌注）
  - 其他药物 / 合并症

→ 残余 confounding → 研究结论可能仍受未测变量扭曲。

### 9.3 Confounding 题干扰项排除模板

| 选项类型 | 适用场景 | 在 case-control 里是否成立 |
|---|---|---|
| **Differential mortality** | RCT / Cohort（有 follow-up）| ❌ Case-control 没时间维度 |
| **Lack of power** | 无显著结果时才考虑 | ❌ 已有多个显著结果 → power 够 |
| **Limited adjustment for confounders** | adjusted 变量少 + 临床上还有其他 | ✅ 高频答案 |
| **Misclassification** | 诊断标准模糊 / 主观 | ❌ 标准化分级（如 pRIFLE）不易误分类 |

### 9.4 Confounding 处理方法（设计 vs 分析阶段）

| 阶段 | 方法 | 说明 |
|---|---|---|
| **设计** | Randomization ⭐ | RCT 把潜在 confounder 平均分到两组 |
| **设计** | Matching | Case-control 中按 confounder 配对 |
| **设计** | Restriction | 限制研究人群（如只研究非吸烟者）|
| **分析** | Stratification | 分层分析 |
| **分析** | Multivariate regression ⭐ | 多元回归调整 |

---

## 10. 统计检验选择 🚧 待填充

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

## 11. 关联

- 🔁 **相关错题**：
  - [[mistakes/uworld-mistakes_2026-05#^Q3941]] Null hypothesis（第 1 章主素材）
  - [[mistakes/uworld-mistakes_2026-05#^Q21248]] OR/CI 表判读 + Confounding（第 5, 6, 7, 8, 9 章主素材）
  - 待补充：Type I/II / Power / p / 统计检验 系列题
- 📚 **主笔记**：
  - [[完整笔记/Peixuan分科笔记/Biostats_Master]]
  - [[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]]（RR/OR/Prevalence 基础）
  - 同期草稿：[[完整笔记/专题笔记/_衍生_USMLE_Bias_5大鉴别_草稿]]（v1）
- 🌱 **TODO**：
  - 等 Hypothesis testing 错题积累 3+（Type I/II / Power / p / 统计检验）→ 让 Claude Code 整合本草稿 + 错题本 → 生成正式 [[完整笔记/专题笔记/_衍生_USMLE_统计推断]]
  - 第 6-8 章 OR 表判读 + Confounder vs Independent Risk Factor + 题型对照 可能值得拆出独立笔记 [[完整笔记/专题笔记/_衍生_USMLE_OR_CI判读]]，等积累更多类似题再决定

---

## 12. 一句话章节速查（持续更新）

| 章节 | 一句话精华 |
|---|---|
| **1. Null hypothesis** ✅ | Null = "无关联" + 措辞必须配 study design；"no association" 永远安全 |
| 2. Type I error | 🚧 待填 |
| 3. Type II error | 🚧 待填 |
| 4. Power | 🚧 待填 |
| 5. p-value | 🚧 待填 |
| **6. CI** ✅ | 比值类盯 1，差值类盯 0；CI 跨 null = 不显著（无论点估计多大）|
| **7. OR 表判读** ✅ | 三步：① 看 multivariate ② CI 不跨 1.0 ③ 患者真的暴露 |
| **8. Confounder vs Independent Risk Factor** ✅ | "Adjusted for X" = 想消除 X（confounder），不是平衡 X（risk factor）；两者角色相反 |
| **9. USMLE OR 表 5 种问法对照** ✅ | 不同问法 → 不同答法：独立危险 vs 最显著 vs 被解释 vs lost significance vs needs control |
| **10. Confounding 实战** ✅ | "调整了 A,B,C → 想 D,E,F 没调整呢？"= residual confounding |
| 11. 统计检验 | 🚧 待填 |

---

## 13. 版本更新记录

| 版本 | 日期 | 更新内容 | 触发错题 |
|---|---|---|---|
| v1 | 2026-05-12 | 初版，仅 Null hypothesis 章节 | Q3941 |
| v2 | 2026-05-12 | 填充 CI（第 5 章）+ 新增 OR 表判读（第 6 章）+ Confounding 实战（第 7 章） | Q21248 |
| **v3** | 2026-05-12 | **新增 Confounder vs Independent Risk Factor 核心区分（第 7 章）+ USMLE OR 表 5 种题型问法精确对照（第 8 章）+ 解释 "adjusted for" 真实含义（消除噪音，非平衡 risk factor）+ 修正"独立危险因素 = multivariate CI 不跨 1.0"判读规则** | Q21248 + 对话深度澄清 |
