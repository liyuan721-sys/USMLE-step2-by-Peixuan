---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-06-24
type: 做题前复习总结
---

# Biostatistics 做题前复习总结

关联：

- [[完整笔记/Biostats_Master]]
- [[完整笔记/_衍生_高频评分_公式]]

> [!info] 使用方式
> 做题前先扫 15-20 分钟。目标不是学完整统计学，而是建立 Step 2 CK 的反射：**题目问什么指标 → 用哪张 2x2 表 / 哪个研究设计 / 哪种 bias / 哪个检验。**

## 一、2x2 表核心

先把表画出来：

| | Disease + | Disease - |
|---|---:|---:|
| Test + | TP | FP |
| Test - | FN | TN |

```
Sensitivity = TP / (TP + FN)
Specificity = TN / (TN + FP)
PPV = TP / (TP + FP)
NPV = TN / (TN + FN)

Prevalence = (TP + FN) / total
Accuracy = (TP + TN) / total
```

> [!tip] 秒记
> - **Sensitivity** 看病人里面测出来多少：Disease+ 这一列。
> - **Specificity** 看没病人里面排除多少：Disease- 这一列。
> - **PPV** 看阳性结果有多少真病：Test+ 这一行。
> - **NPV** 看阴性结果有多少真没病：Test- 这一行。

## 二、SNOUT / SPIN

> [!danger] Screening vs confirmation
> **High sensitivity** test 适合 rule out：**SNOUT**。  
> **High specificity** test 适合 rule in：**SPIN**。

| 指标高 | 用途 | 例子 |
|---|---|---|
| Sensitivity high | Negative result rules out disease | HIV screening, D-dimer in low-risk PE |
| Specificity high | Positive result rules in disease | Confirmatory test |

> [!warning] 常见陷阱
> 敏感度高不等于阳性就确诊；特异度高不等于阴性就排除。  
> 记住方向：**Sensitive test 的 negative 最有用；Specific test 的 positive 最有用。**

## 三、Prevalence 对 PPV/NPV 的影响

Sensitivity 和 specificity 是测试本身性质，**不随 prevalence 变**。

| Prevalence | PPV | NPV |
|---|---|---|
| 增加 | 增加 | 下降 |
| 下降 | 下降 | 增加 |

> [!tip] 口算逻辑
> 病越常见，阳性越可信：PPV ↑。  
> 病越罕见，阴性越可信：NPV ↑。

## 四、Likelihood Ratio

```
LR+ = sensitivity / (1 - specificity)
LR- = (1 - sensitivity) / specificity
```

| LR | 意义 |
|---|---|
| LR+ >10 | positive result strongly rules in |
| LR- <0.1 | negative result strongly rules out |
| LR around 1 | useless test |

> [!info] 考法
> Likelihood ratio 连接的是 **pretest probability → posttest probability**。  
> 如果题目问“哪个 test 最能改变诊断概率”，选 LR+ 最大或 LR- 最小。

## 五、Risk / Odds / Rate

```
Risk = events / total at risk
Odds = events / non-events
Rate = events / person-time
```

| 概念 | 分母 | 关键词 |
|---|---|---|
| Risk | 人数 | over a period |
| Odds | 没发生的人 | case-control 常用 |
| Rate | person-time | incidence rate |

## 六、RR / OR / AR / NNT

2x2 暴露表：

| | Disease + | Disease - |
|---|---:|---:|
| Exposed | a | b |
| Unexposed | c | d |

```
Risk in exposed = a / (a + b)
Risk in unexposed = c / (c + d)

Relative risk (RR) = [a/(a+b)] / [c/(c+d)]
Odds ratio (OR) = (a/b) / (c/d) = ad/bc
Attributable risk (AR) = risk exposed - risk unexposed
Absolute risk reduction (ARR) = control risk - treatment risk
Number needed to treat (NNT) = 1 / ARR
Number needed to harm (NNH) = 1 / absolute risk increase
```

> [!danger] 研究设计对应
> - **Cohort / RCT**：可以算 incidence、risk、RR、ARR、NNT。
> - **Case-control**：不能直接算 incidence/risk/RR，通常算 **OR**。

> [!tip] RR/OR 解读
> - RR/OR = 1：无关联
> - >1：暴露增加风险
> - <1：暴露保护

## 七、NNT 快速算法

题目常给百分比：

```
ARR = control event rate - treatment event rate
NNT = 1 / ARR
```

例：

```
Placebo event rate = 10%
Drug event rate = 5%
ARR = 5% = 0.05
NNT = 1 / 0.05 = 20
```

> [!warning] NNT/NNH 单位
> 百分比必须转小数。  
> 2% = 0.02 → NNT = 50。

## 八、研究设计

| 设计 | 方向 | 关键词 | 能算 |
|---|---|---|---|
| Cross-sectional | 同一时间看 exposure + disease | prevalence | prevalence |
| Case-control | 先按 disease 分组，再回看 exposure | rare disease | OR |
| Cohort | 先按 exposure 分组，随访 disease | rare exposure | RR, incidence |
| RCT | 随机分治疗/对照 | best for causality | RR, ARR, NNT |
| Crossover trial | 同一人先后接受 A/B | chronic stable disease | each patient own control |
| Meta-analysis | 合并多个研究 | forest plot | higher power |

> [!tip] 秒杀
> - Rare disease → case-control。
> - Rare exposure → cohort。
> - Randomization → RCT。
> - Same patients get both treatments → crossover。
> - One-time survey → cross-sectional。

## 九、Bias 高频表

| Bias | 中文 | 题干线索 | 解决 |
|---|---|---|---|
| Selection bias | 选择偏倚 | sample not representative | random sampling |
| Sampling bias | 抽样偏倚 | volunteers / clinic-only sample | random sample |
| Recall bias | 回忆偏倚 | patients with disease remember exposure more | objective records |
| Observer bias | 观察者偏倚 | researcher expectation affects measurement | blinding |
| Interviewer bias | 访谈者偏倚 | leading questions | standardized interview/blinding |
| Measurement bias | 测量偏倚 | faulty instrument / inconsistent measurement | calibrate, standardize |
| Confounding | 混杂 | third variable associated with exposure and outcome | randomization, restriction, matching, stratification, multivariable analysis |
| Lead-time bias | 领先时间偏倚 | earlier diagnosis seems longer survival, no mortality change | compare mortality, not survival time |
| Length-time bias | 病程长度偏倚 | screening detects slow-growing less aggressive disease | mortality endpoint |
| Healthy worker bias | 健康工人偏倚 | workers healthier than general population | use comparable control |
| Attrition bias | 失访偏倚 | differential loss to follow-up | intention-to-treat, reduce dropout |
| Publication bias | 发表偏倚 | positive studies more likely published | funnel plot |

> [!danger] Screening bias 三兄弟
> - **Lead-time**：提前发现，survival time 看起来变长，但死亡时间没变。
> - **Length-time**：screening 更容易抓到慢性、温和、病程长的病。
> - **Overdiagnosis**：发现本来不会造成症状/死亡的病。

## 十、Confounding vs Effect Modification

Confounding：

- 第三个变量同时关联 exposure 和 outcome
- 会扭曲真实关系
- 需要控制

Effect modification：

- 暴露效应在不同 subgroup 真实不同
- 不是 bias，不应该消除
- 应该分层报告

> [!tip] 题干判断
> 如果题目问“stratified analysis 后两个 strata 结果相似，但和 crude result 不同” → confounding。  
> 如果“不同 strata 的 effect size 本来就不同” → effect modification。

## 十一、Randomization / Blinding / Intention-to-Treat

| 方法 | 主要解决 |
|---|---|
| Randomization | confounding |
| Allocation concealment | selection bias before assignment |
| Blinding | observer/performance bias |
| Placebo | placebo effect |
| Intention-to-treat analysis | attrition/nonadherence bias; preserves randomization |

> [!warning] Intention-to-treat
> 按最初随机分组分析，不管病人是否 adherence / crossover / dropout。  
> 优点：更接近真实世界，保留 randomization。

## 十二、Hypothesis Testing

```
Null hypothesis (H0): no difference / no association
Alternative hypothesis (H1): difference exists
P value: assuming H0 true, probability of observing this result or more extreme
```

| 概念 | 意义 |
|---|---|
| alpha | Type I error threshold, usually 0.05 |
| p < alpha | reject H0 |
| p > alpha | fail to reject H0 |
| confidence interval crossing null | not statistically significant |

Null value：

| Measure | Null |
|---|---|
| Difference | 0 |
| RR / OR / HR | 1 |

> [!danger] P value 不代表
> P value 不是“结果是假的概率”，也不是“临床重要性”。大样本可以让很小差异 statistically significant，但不一定 clinically significant。

## 十三、Type I / Type II Error

| | Reality: H0 true | Reality: H0 false |
|---|---|---|
| Reject H0 | Type I error alpha | Correct |
| Fail to reject H0 | Correct | Type II error beta |

```
Power = 1 - beta
```

| Error | 中文 | 含义 |
|---|---|---|
| Type I / alpha | 假阳性 | 说有差异，其实没有 |
| Type II / beta | 假阴性 | 说没差异，其实有 |

> [!tip] Power 增加方法
> 增加 sample size、增加 effect size、降低 variability、提高 alpha。  
> 最常考：**increase sample size → increase power → decrease type II error**。

## 十四、Confidence Interval

CI 表示：

- 如果重复抽样很多次，95% CI 中有 95% 会包含真实参数
- CI 越窄，precision 越高

影响 CI 宽度：

| 情况 | CI |
|---|---|
| Sample size 增加 | 变窄 |
| Variability 减少 | 变窄 |
| Confidence level 99% vs 95% | 变宽 |

> [!warning] CI 与 significance
> RR/OR/HR 的 95% CI 如果跨 1 → not significant。  
> Mean difference 的 95% CI 如果跨 0 → not significant。

## 十五、Statistical Tests

先问变量类型：

| 场景 | 检验 |
|---|---|
| Two means, independent groups | t-test |
| Two means, same subjects before/after | paired t-test |
| More than two means | ANOVA |
| Two categorical variables | Chi-square |
| Categorical + small expected cell count | Fisher exact |
| Correlation between continuous variables | Pearson correlation |
| Nonparametric / ranks | Mann-Whitney U, Wilcoxon |
| Survival/time-to-event | Kaplan-Meier, log-rank, Cox proportional hazards |

> [!tip] 快速判断
> Mean → t-test/ANOVA。  
> Proportion/category → chi-square/Fisher。  
> Time-to-event → Kaplan-Meier/Cox。

## 十六、Distribution

Normal distribution：

- Mean = median = mode
- Symmetric
- 68% within 1 SD, 95% within 2 SD, 99.7% within 3 SD

Skewed distribution：

| Skew | Tail | Mean vs Median |
|---|---|---|
| Positive/right skew | tail to right | mean > median |
| Negative/left skew | tail to left | mean < median |

> [!tip] Skewed data
> 用 median / interquartile range 更稳，不要用 mean 代表中心。

## 十七、Validity / Reliability

| 概念 | 意义 |
|---|---|
| Validity | accuracy，测的是不是对的 |
| Reliability | precision/reproducibility，重复测是否一致 |

| 情况 | 描述 |
|---|---|
| High validity + high reliability | 准且稳 |
| Low validity + high reliability | 每次都偏同一个方向 |
| High validity + low reliability | 平均准，但波动大 |
| Low validity + low reliability | 又不准又不稳 |

## 十八、Survival Analysis

| 概念 | 用途 |
|---|---|
| Kaplan-Meier curve | survival probability over time |
| Log-rank test | compare survival curves |
| Cox proportional hazards | hazard ratio with covariate adjustment |
| Hazard ratio | instantaneous risk over time |

HR 解读：

- HR = 1：无差异
- HR <1：治疗组 hazard lower
- HR >1：治疗组 hazard higher

## 十九、USMLE 常见问法反射

> [!question]- 题目给 sensitivity/specificity，问换到低 prevalence 人群会怎样？
> Sensitivity/specificity 不变；PPV 下降，NPV 上升。

> [!question]- 筛查让 survival from diagnosis 变长，但 mortality 不变？
> Lead-time bias。

> [!question]- 研究只更容易发现进展慢、病程长的癌？
> Length-time bias。

> [!question]- Case-control study 能算什么？
> Odds ratio。不能直接算 incidence/RR。

> [!question]- RCT 中很多人不按方案服药，怎么分析？
> Intention-to-treat。

> [!question]- 想减少 observer expectation 对 outcome assessment 的影响？
> Blinding。

> [!question]- 想减少 confounding？
> Randomization 最强；也可 matching/stratification/multivariable regression。

> [!question]- P value 0.03 意味着什么？
> 假设 null hypothesis 为真，观察到当前或更极端结果的概率是 3%。

> [!question]- 95% CI for RR = 0.7-1.2，显著吗？
> 不显著，因为跨 1。

> [!question]- 增加 sample size 对 power / beta / CI 的影响？
> Power 增加，beta 降低，CI 变窄。

## 二十、做题前 5 分钟默写

```
Sensitivity = TP/(TP+FN)
Specificity = TN/(TN+FP)
PPV = TP/(TP+FP)
NPV = TN/(TN+FN)

RR = risk exposed / risk unexposed
OR = ad/bc
ARR = control risk - treatment risk
NNT = 1/ARR

Power = 1 - beta
Type I = false positive
Type II = false negative

Case-control → OR
Cohort/RCT → RR
Cross-sectional → prevalence

High sensitivity negative → rule out
High specificity positive → rule in

Prevalence ↑ → PPV ↑, NPV ↓
Prevalence ↓ → PPV ↓, NPV ↑
```

> [!success] 最后一口气
> Biostats 不是靠感觉做题。看到题先分类：**公式题 / 研究设计题 / bias 题 / hypothesis testing 题 / statistical test 题**。分类对了，答案会自己冒出来。
