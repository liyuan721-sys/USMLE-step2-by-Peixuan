---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-06-22
type: 专题笔记
---

# Biostats 统计检验选择决策树（Statistical Test Selection）

> 派生自 [[NBME/nbme-records/NBME 11/NBME11_错题本#^Q105]]（2 组连续比均值 = 非配对 t 检验 unpaired t-test）。
> 这是 USMLE 高频"给场景选检验"题的**单一真相源**：把题干翻译成数据结构（几组？什么变量类型？是否配对？）→ 套决策树落检验。

> [!tip] 一句话解题口诀（先问结局变量类型，再问组数 / 是否配对）
> **双定量选回归，双定性选卡方，自定性因定量选 t / ANOVA。**
> （自变量是分类、因变量是定量 → 2 组用 t，≥3 组用 ANOVA；两个都定量 → 相关 / 回归；两个都定性 → 卡方。）

---

## 一、为什么 USMLE 爱考这个（薄弱科背景说明）

这类题**不需要算**，只考"识别数据结构 → 套表"。题干会埋三类钥匙信息：

1. **结局变量（因变量 dependent variable）是什么类型？**
   - **连续 continuous / 定量**：血压、胆固醇浓度、体重、住院天数（能取小数、能算均值 mean）
   - **分类 categorical / 定性**：治愈 vs 未治愈、生 vs 死、有病 vs 无病（只能数频数 / 算比例）
   - **序数 ordinal / 非正态 non-normal**：疼痛评分 1–10、肿瘤分期、明显偏态的数据
2. **比较几组？**（数自变量有几个水平：2 组？≥3 组？）
3. **组与组是否独立 independent，还是同一批人配对 paired / 前后对照？**

> [!warning] 解题铁律：先定"结局变量类型"再做任何事
> 很多人（包括我 Q105）一看到"比较几组均值"就反射 ANOVA，**漏数组数**。正确顺序：
> ① 结局变量类型（连续 / 分类 / 序数）→ 砍掉一半选项；
> ② 几组 + 是否配对 → 在剩下的里定具体检验。

---

## 二、主决策树（ASCII，先看结局变量类型）

**图 A — 自变量 × 因变量 2×2 矩阵**（自变量 independent variable, IV / 因变量 dependent variable, DV）：IV 连续 + DV 二分类 → logistic regression（逻辑回归）这格补全了 §五

![[Pasted image 20260622170819.png]]

**图 B — 数据结构速查表**（对应 §一口诀）

![[{BF810AAF-E81F-4F81-B646-975FC07AE65D}.png]]

```
                  题干 → 先问：结局变量（因变量 Y）是什么类型？
                                  │
        ┌─────────────────────────┼─────────────────────────┐
        │                         │                          │
   连续 / 定量               分类 / 定性               序数 / 非正态 / 明显偏态
   (continuous)             (categorical)            (ordinal / non-normal)
        │                         │                          │
   再问：几组？               比较的是              （连续型本应用参数检验，
   是否配对？                 比例 / 频率              但偏态/序数 → 改用非参数
        │                         │                   non-parametric 对应版本）
        │                         │                          │
   ┌────┼─────────┐         ┌─────┴─────┐            ┌───────┼────────┐
   │    │         │         │           │            │       │        │
 2组   2组       ≥3组    一般样本    小样本        2组独立  2组配对   ≥3组
 独立  配对/前后  比均值  期望频数≥5  期望频数<5      │       │        │
   │    │         │         │           │       Mann-     Wilcoxon  Kruskal-
unpaired paired  ANOVA   Chi-square  Fisher    Whitney U  signed    Wallis
 t-test  t-test  方差分析  卡方检验    精确检验   (=Wilcoxon  -rank    (非参数
(非配对  (配对                                  rank-sum)  (配对版)   ANOVA)
 t检验)  t检验)
```

> [!info] 第三类（连续↔连续 关系）单独看
> 当**自变量和因变量都是连续变量**（没有"分组"，而是问"两个连续量之间的关系 / 趋势 / 预测"）→ 走相关 / 回归分支（见 §五）。

---

## 三、结局连续 + 自变量分类（最高频，Q105 在这里）

自变量是分组（分类），因变量是连续数值、比较的是**均值 mean** → 看组数 + 是否配对。

| 数据结构 | 推荐检验 | 中文 | 经典 stem 钩子 |
|---|---|---|---|
| **2 组独立 + 连续 + 比均值** ✅ | **unpaired (Student's) t-test** | 非配对 t 检验 | "随机分到 X 组 vs Y 组，比较平均血压"（不同人） |
| 2 组配对 / 同人前后 + 连续 | **paired t-test** | 配对 t 检验 | "同一批人用药前 vs 用药后血压差" |
| **≥3 组 + 连续 + 比均值** | **ANOVA** (analysis of variance) | 方差分析 | "比较 A / B / C 三种药的平均胆固醇" |

> [!danger] Q105 的核心陷阱：2 组 ≠ ANOVA
> ANOVA 是 **≥3 组**才用的（一次比较 3 组以上均值，避免多次 t 检验膨胀 α）。
> 只有 **2 组**时用 **t-test**；我当时反射成 ANOVA = 漏数组数。
> 记忆：**"两组、连续、比均值"三连 = t 检验；三组以上才 ANOVA。**

> [!info] 为什么 ≥3 组不能反复做 t-test？（USMLE 常追问）
> 3 组两两比要做 3 次 t 检验，每次 α = 0.05，多次比较会让**总 I 型错误率（假阳性）膨胀**（≈ 1 − 0.95³ ≈ 14%）。ANOVA 一次性检验"至少有一组均值不同"，控制总体 α。ANOVA 显著后再做 **post-hoc（事后两两比较）**（如 Tukey 检验）找出是哪几组不同。

### 独立 vs 配对怎么分（中文解释）

- **独立 independent**：两组是**不同的人**（随机分配到两组、男 vs 女、用药 vs 安慰剂）→ unpaired。
- **配对 paired**：**同一个人测两次**（治疗前 vs 后）、或刻意一一配对（双胞胎、左眼 vs 右眼、年龄性别 1:1 matched）→ paired。
- 钥匙词：题干出现 **"before and after / pre-post / same patients / matched pairs / each subject"** → paired。

---

## 四、结局分类 + 自变量分类 → 卡方 / Fisher

因变量是**分类**（比的是**比例 / 频率 / 频数**，不是均值）→ 卡方家族。

| 数据结构 | 推荐检验 | 中文 | 触发条件 |
|---|---|---|---|
| 分类 vs 分类，**期望频数（expected count）每格 ≥ 5** | **Chi-square test** | 卡方检验 | 一般样本量 |
| 分类 vs 分类，**期望频数 < 5**（或样本很小） | **Fisher's exact test** | Fisher 精确检验 | 小样本 / 稀疏格子 |

> [!warning] 卡方 vs t 检验最爱混的点
> **卡方比"比例 / 频率"，不是均值。** 看到结局是"治愈率 / 死亡率 / 阳性率 / 有无并发症的人数"= 分类 → 卡方；看到"平均值 / mean / 浓度 / 天数" = 连续 → t / ANOVA。
> 即便原始数据是连续的（如血压），只要研究者**按门槛切成"高 / 正常"两类**再比人数 → 也必须用**卡方**。

> [!info] 为什么小样本要用 Fisher（中文解释）
> 卡方是**近似检验**，依赖每格期望频数足够大（经验阈值 ≥ 5）才能让卡方统计量近似卡方分布。格子里期望人数太少时近似失效 → 改用 **Fisher 精确检验**，它直接用超几何分布算精确 p 值，不依赖大样本近似。
> 钥匙词：**"small sample / 2×2 table with few patients / expected count < 5"** → Fisher。

---

## 五、连续 ↔ 连续：相关与回归

当两个变量**都是连续**、问"关系 / 趋势 / 预测"而**不是分组比均值**时：

| 目的 | 检验 / 方法 | 中文 | 说明 |
|---|---|---|---|
| 两连续量是否**同向变化**（正态）| **Pearson correlation** | 皮尔逊相关 | 给相关系数 r（−1~+1），只说**强度 + 方向**，不说因果 |
| 两量**非正态 / 序数**的相关 | **Spearman correlation** | 斯皮尔曼（秩）相关 | 用秩次算，偏态 / 等级数据用它 |
| 用 X **预测 / 解释** 连续 Y | **linear regression** | 线性回归 | 产出回归系数 β（直线），Y 必须连续 |
| 用 X 预测**二分类**结局 Y（生/死、有病/无病）| **logistic regression** | 逻辑（二元）回归 | 产出 **OR（odds ratio 比值比）**，S 型曲线；能多变量校正混杂 |

> [!tip] 卡方 vs 逻辑回归（高频追问）
> - 只问"两分类变量**是否有关联**" → **卡方**（最简便，只出 p 值，单变量）。
> - 要"**算 OR**"或"**控制 / 校正混杂 adjust for confounders**"（多个自变量同时放进去）→ 必须**逻辑回归**（出 p 值 + 校正 OR）。
> - 区分线性 vs 逻辑：**看因变量 Y** —— Y 连续 = 线性回归（β）；Y 二分类 = 逻辑回归（OR）。

> [!warning] 相关 ≠ 因果
> 即使 r = 0.99，相关也不能证明谁导致谁（可能有混杂或反向因果）。因果只能由 RCT / cohort + Hill 标准支撑。

---

## 六、序数 / 非正态 → 非参数检验（参数检验的"平行宇宙"）

当数据是**序数（ordinal，如疼痛 1–10 分、肿瘤分期）或明显偏态 / 非正态、小样本不能假设正态**时，把参数检验换成对应的**非参数 non-parametric** 版本（用秩次 rank 而非原始均值）：

| 参数检验（正态/连续）| → 非参数对应版 | 中文 | 用途 |
|---|---|---|---|
| unpaired t-test（2 组独立）| **Mann-Whitney U test**（= Wilcoxon rank-sum） | 曼-惠特尼 U 检验 | 2 组独立、序数 / 非正态 |
| paired t-test（2 组配对）| **Wilcoxon signed-rank test** | 威尔科克森符号秩检验 | 同人前后、序数 / 非正态 |
| ANOVA（≥3 组）| **Kruskal-Wallis test** | 克鲁斯卡尔-沃利斯检验 | ≥3 组、序数 / 非正态 |
| Pearson correlation | **Spearman correlation** | 斯皮尔曼相关 | 序数 / 非正态相关 |

> [!info] 何时切到非参数（中文解释）
> 钥匙词：**"non-normally distributed / skewed / ordinal / ranked / Likert scale / small sample, distribution unknown"** → 非参数。
> 反之 Q105 那种 **300 vs 200 例大样本（趋正态）+ 连续浓度** → 用参数 t 检验，**不要**跳到 Mann-Whitney。"非正态"必须题干明说或强烈暗示才选非参数。

---

## 七、生存数据（time-to-event）

结局是"**到事件发生的时间**"（死亡、复发、移植失败），且常有**删失 censoring**（随访结束还没发病）：

| 目的 | 方法 | 中文 | 说明 |
|---|---|---|---|
| 画生存曲线、估中位生存 | **Kaplan-Meier (KM) curve** | Kaplan-Meier（KM）生存曲线 | 阶梯状曲线，处理删失 |
| **比较两条生存曲线**是否不同 | **log-rank test** | 对数秩检验 | 比 KM 曲线组间差异 |
| 多变量校正下的生存风险 | **Cox proportional hazards regression** | Cox 比例风险回归（Cox PH 回归）| 产出 **HR（hazard ratio 风险比）**，可多变量校正 |

> [!tip] 生存题钥匙词
> "survival / time to death / time to recurrence / followed until event or end of study / censored" → 想到 **KM + log-rank**；要 HR + 校正混杂 → **Cox 回归**。

---

## 八、总速查表（考前一张图）

| 因变量（结局）| 自变量 / 情境 | 检验 |
|---|---|---|
| 连续，比均值 | 分类 2 组独立 | **unpaired t-test** |
| 连续，比均值 | 分类 2 组配对 / 前后 | **paired t-test** |
| 连续，比均值 | 分类 ≥3 组 | **ANOVA** |
| 分类（比例/频率）| 分类，期望频数 ≥5 | **Chi-square 卡方** |
| 分类（比例/频率）| 分类，期望频数 <5 / 小样本 | **Fisher's exact** |
| 连续 | 连续（关系/趋势，正态）| **Pearson correlation** |
| 连续 | 连续（关系，非正态/序数）| **Spearman correlation** |
| 连续 | 连续（预测/解释）| **linear regression** |
| 二分类（生/死、病/不病）| 一个或多个自变量 | **logistic regression（出 OR）** |
| 序数 / 非正态，2 组独立 | — | **Mann-Whitney U** |
| 序数 / 非正态，2 组配对 | — | **Wilcoxon signed-rank** |
| 序数 / 非正态，≥3 组 | — | **Kruskal-Wallis** |
| 生存时间（含删失）| 画曲线 / 比两组 / 多变量 | **KM / log-rank / Cox（HR）** |

---

## 九、自测题（盲做，先不看答案）

> [!question]- Q1. 一项 RCT（randomized controlled trial 随机对照试验）把 500 名高胆固醇患者随机分到药 X（300 例）和药 Y（200 例），6 个月后测**血清胆固醇浓度（mg/dL）**，问比较两组**均值**最合适的检验？（派生自 Q105）
> **unpaired (Student's) t-test 非配对 t 检验。**
> 钥匙：2 组（排 ANOVA）+ 独立不同人（排 paired）+ 连续浓度比均值（排卡方）+ 大样本趋正态（排 Mann-Whitney）。

> [!question]- Q2. 比较**三种**降压药对平均收缩压的影响，每组不同患者，数据近似正态。用什么检验？
> **ANOVA 方差分析**（≥3 组 + 连续 + 比均值）。显著后做 post-hoc（如 Tukey）。

> [!question]- Q3. 同一批 40 名患者，记录**戒烟前 vs 戒烟后**的平均体重，比较前后差异。用什么？
> **paired t-test 配对 t 检验**（同人前后 = 配对 + 连续）。

> [!question]- Q4. 比较两种疗法的**治愈率（治愈 vs 未治愈的人数比例）**，每组 200 人。用什么？
> **Chi-square 卡方检验**（结局是分类/比例，期望频数充足）。

> [!question]- Q5. 一个 2×2 表，某格只有 2 个患者（期望频数 <5），比较两组并发症发生率。用什么？
> **Fisher's exact test 精确检验**（小样本 / 期望频数 <5 的分类数据）。

> [!question]- Q6. 研究者想知道**血清维生素 D 浓度**与**骨密度**（都是连续、近似正态）之间的关系强度。用什么？
> **Pearson correlation 皮尔逊相关**（两连续变量、正态、看关系，不是分组）。

> [!question]- Q7. 用年龄、BMI（body mass index 体质指数）、吸烟（多个自变量）预测**是否发生心梗（myocardial infarction, MI；是/否）**，并校正混杂。用什么？
> **logistic regression 逻辑回归**（二分类结局 + 多变量校正，出 OR）。

> [!question]- Q8. 比较两种化疗方案的**生存时间**，随访至死亡或研究结束（有删失），问比较两条生存曲线的检验？
> **log-rank test**（比较 Kaplan-Meier 曲线）；要 HR + 校正混杂则 **Cox 回归**。

> [!question]- Q9. 疼痛评分（0–10 序数、明显偏态）在两组**不同患者**间比较。用什么？
> **Mann-Whitney U test**（= Wilcoxon rank-sum；2 组独立 + 序数/非正态 → 非参数）。

---

## 🔗 关联

- 🔁 同主题错题：
  - [[NBME/nbme-records/NBME 11/NBME11_错题本#^Q105]] 2 组连续比均值 = 非配对 t 检验（本笔记种子）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]（§八 统计检验选择）/ [[完整笔记/专题笔记/Biostats/Biostats_HighYield速查总览]]（§七 统计检验选择，速查版；本笔记是其拆出的深度版）
- 🏥 跨学科：[[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]（逻辑回归出 OR / 相关≠因果）
- 🌱 TODO：攒够"研究设计识别"题 → 建 [[完整笔记/专题笔记/Biostats/Biostats_研究设计秒认与可算指标]]（cohort/case-control/cross-sectional → 可算 RR/OR）

## ✅ 复盘行动

- [ ] 默写主决策树（先结局变量类型 → 再组数 / 配对）
- [ ] 默写非参数对应表（t→Mann-Whitney、paired t→Wilcoxon signed-rank、ANOVA→Kruskal-Wallis）
- [ ] 见"比较几组均值"先确认**不是 ≥3 组才落 t**（Q105 错点）
- [ ] 找 3 道类似检验选型题验证反射
