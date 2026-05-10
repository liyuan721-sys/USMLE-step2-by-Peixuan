# Biostatistics & Epidemiology — Step 2 CK 速查笔记

> 核心思想:CK 的 Biostats 不是数学考试,是**模式识别**。
> 全部内容 ≈ 8 个公式 + 6 种研究设计 + 10 种 bias + 几个假设检验概念。

---

## 一、2×2 表 — 所有公式的根

```
                Disease (+)     Disease (−)
  Test (+)          a               b
  Test (−)          c               d
```

记忆口诀:**"行是测试,列是疾病"**

---

## 二、诊断指标(必背)

| 指标 | 公式 | 含义 | 备注 |
|---|---|---|---|
| **Sensitivity (Sn)** | a / (a+c) | 病人里测出阳的比例 | **SnNout**:Sn 高,阴性可排除 |
| **Specificity (Sp)** | d / (b+d) | 没病的里测出阴的比例 | **SpPin**:Sp 高,阳性可确诊 |
| **PPV** | a / (a+b) | 测阳里真有病的比例 | **随 prevalence 升高而升高** |
| **NPV** | d / (c+d) | 测阴里真没病的比例 | **随 prevalence 升高而降低** |
| **Prevalence** | (a+c) / total | 患病率 | 影响 PPV/NPV,不影响 Sn/Sp |
| **Accuracy** | (a+d) / total | 总体正确率 | 较少考 |

### 关键概念:Sn/Sp 是检测的"固有属性",PPV/NPV 受人群影响

- 罕见病(低 prevalence)→ PPV 低,即使 test 很准也容易假阳
- 常见病(高 prevalence)→ PPV 高
- **CK 高频题**:同一个 test 用在筛查 vs 确诊场景,PPV/NPV 会变

### Likelihood Ratio(进阶,但 CK 偶尔考)

- **LR+ = Sn / (1 − Sp)** — 阳性结果的诊断价值,>10 强阳性
- **LR− = (1 − Sn) / Sp** — 阴性结果的诊断价值,<0.1 强阴性

---

## 三、风险与效应指标

| 指标 | 公式 | 用于哪种研究 |
|---|---|---|
| **Relative Risk (RR)** | [a/(a+b)] / [c/(c+d)] | Cohort、RCT |
| **Odds Ratio (OR)** | (a×d) / (b×c) | Case-control |
| **Absolute Risk Reduction (ARR)** | 对照组发病率 − 治疗组发病率 | RCT |
| **Relative Risk Reduction (RRR)** | ARR / 对照组发病率 = 1 − RR | RCT |
| **Number Needed to Treat (NNT)** | 1 / ARR | RCT,越小越有效 |
| **Number Needed to Harm (NNH)** | 1 / 副作用绝对增加率 | 越大越安全 |
| **Attributable Risk (AR)** | 暴露组发病率 − 非暴露组发病率 | Cohort |

### 解读规则

- **RR/OR = 1**:无关联
- **RR/OR > 1**:暴露增加风险
- **RR/OR < 1**:暴露是保护性因素
- **CI 跨过 1**:统计不显著(对 RR/OR 而言)
- **CI 跨过 0**:统计不显著(对差值/ARR 而言)

---

## 四、研究设计(6 种,必须秒认)

| 设计 | 一句话识别 | 报告指标 | 优点 | 缺点 |
|---|---|---|---|---|
| **Cross-sectional** | "在某时点同时测暴露和疾病" | Prevalence | 快、便宜 | 无因果 |
| **Case-control** | "已有病的 vs 没病的,回头查暴露" | OR | 适合罕见病 | Recall bias |
| **Cohort(prospective)** | "暴露 vs 不暴露,往前追踪" | RR、Incidence | 可推因果 | 慢、贵 |
| **Cohort(retrospective)** | "用既往记录追踪" | RR | 较快 | 数据质量差 |
| **RCT** | "随机分组干预" | RR、ARR、NNT | 最高证据 | 贵、伦理限制 |
| **Crossover trial** | "受试者先 A 后 B" | 同 RCT | 控制个体差异 | 残留效应 |
| **Meta-analysis** | "汇总多个研究" | 综合 RR/OR | 增加 power | 各研究异质性 |
| **Case series / report** | "几例描述" | 无 | 发现新病 | 无对照 |

---

## 五、Bias(高频前 10)

> 关键:**记情境,不是记定义**

| Bias | 典型情境 | 防范 |
|---|---|---|
| **Selection bias** | 研究对象不能代表总体(如 non-response) | 随机抽样 |
| **Recall bias** | Case-control 中,病人比对照记得更清楚 | 用客观记录 |
| **Lead-time bias** | 筛查"延长生存期",其实只是早发现 | 用疾病特异死亡率 |
| **Length-time bias** | 筛查发现的多是惰性病变,生存假性更长 | RCT 校正 |
| **Confounding** | 第三变量同时影响暴露和结局(经典:咖啡-肺癌-吸烟) | 分层、回归、随机化 |
| **Effect modification** | 不同亚组效应不同(不是 bias,但常考) | 分层报告,不要校正掉 |
| **Hawthorne effect** | 被观察者改变行为 | 盲法 |
| **Observer / Pygmalion bias** | 研究者预期影响测量 | 双盲 |
| **Berkson bias** | 用住院患者作样本造成偏倚 | 用人群对照 |
| **Attrition bias** | 失访造成不均 | Intent-to-treat 分析 |
| **Publication bias** | 阳性结果更易发表 | Funnel plot |
| **Lead-time vs Length-time** | 都和筛查相关,前者"早发现"假象,后者"惰性病变多" | 区分点:lead-time 是时间提前,length-time 是疾病性质 |

---

## 六、假设检验(简化版)

### 错误类型

| | 实际无差异 | 实际有差异 |
|---|---|---|
| **检验"无差异"** | ✅ | ❌ Type II (β) |
| **检验"有差异"** | ❌ Type I (α) | ✅ Power (1−β) |

- **Type I error (α)**:假阳性,通常设 0.05
- **Type II error (β)**:假阴性,通常 0.20
- **Power = 1 − β**:真有差异时检测出的能力
- **如何提高 power**:↑样本量、↑效应大小、↑α(让标准变松)、↓变异度

### p 值与置信区间

- **p < 0.05**:统计显著(传统标准)
- **95% CI**:重复实验 95% 的区间会包含真实值
- **CI 与显著性的关系**:
  - 比较两组均值差异 → CI 不跨 0 = 显著
  - 比较 RR/OR → CI 不跨 1 = 显著

### 统计检验选择(题目给场景,选检验)

| 数据类型 | 检验 |
|---|---|
| 两组均值(连续变量) | t-test |
| 三组及以上均值 | ANOVA |
| 两组比例(分类变量) | Chi-square |
| 小样本分类 | Fisher's exact |
| 配对数据 | Paired t-test |
| 相关性 | Pearson(连续)/ Spearman(等级) |

---

## 七、统计描述

### 集中趋势

- **Mean**:对极端值敏感
- **Median**:不受极端值影响,**偏态分布优选**
- **Mode**:出现最多的值

### 偏态分布

- **正偏(右偏)**:尾巴在右,Mean > Median > Mode(如收入)
- **负偏(左偏)**:尾巴在左,Mean < Median < Mode

### 正态分布

- 68% 在 ±1 SD 内
- 95% 在 ±2 SD 内(精确 1.96)
- 99.7% 在 ±3 SD 内

---

## 八、Screening Test 概念

- 好的筛查 test 要求 **Sn 高**(漏诊代价大)
- 好的确诊 test 要求 **Sp 高**(误诊代价大)
- **Cutoff 调低** → Sn↑, Sp↓
- **Cutoff 调高** → Sn↓, Sp↑

### 评估筛查项目的 4 个偏倚(必考)

1. **Selection bias**:愿意被筛查的人本身更健康
2. **Lead-time bias**:早发现 ≠ 真的活更久
3. **Length-time bias**:筛查抓到的多是慢病
4. **Overdiagnosis bias**:发现了不会进展的病变

---

## 九、流行病学高频概念

- **Incidence**:新发病例 / 风险人群 / 时间 — 反映"风险"
- **Prevalence ≈ Incidence × Duration** — 慢性病 prevalence 高
- **Mortality rate**:死亡数 / 人群
- **Case-fatality rate**:病死数 / 病例数
- **Standardized rate**:校正人口结构差异后的率

---

## 十、考试套路总结

### 题型 1:给 2×2 表算指标
- 看清问的是 Sn / Sp / PPV / NPV / 哪个
- **小心**:它常给你 prevalence 让你算 PPV(贝叶斯)

### 题型 2:识别研究设计
- "回顾性看暴露" → case-control → OR
- "前瞻追踪" → cohort → RR
- "随机分组" → RCT
- 看到"在某时点测量了..."→ cross-sectional

### 题型 3:识别 bias
- 给一个研究场景,问哪种 bias
- 关键词识别:"病人记得更清楚" → recall;"住院患者样本" → Berkson;"早发现等于活更久?" → lead-time

### 题型 4:统计检验选择
- 看变量类型(连续 vs 分类)+ 组数 → 套表

### 题型 5:p 值/CI 解读
- "CI 跨过 1" → 不显著(RR/OR)
- "p = 0.08" → 不显著
- 90% 的题不需要算,只需要解读

---

## 十一、复习计划(3–5 天搞定)

- **Day 1**:背公式表 + 研究设计表(本笔记 1 小时过一遍)
- **Day 2**:UW 刷 30–40 题 → 错题对照本笔记
- **Day 3**:UW 刷剩下的 → 二刷错题
- **Day 4**:错题三刷 + 整理薄弱点
- **Day 5**:做一次 NBME 风格小测,目标 85%+

---

## 十二、给 Claude Code 的提示词模板

```
我刚学完 Biostats,按 USMLE Step 2 CK 难度出 10 道题,涵盖:
- Sn/Sp/PPV/NPV
- RR/OR/NNT
- Bias 识别
- Study design 识别
- 统计检验选择
每题 5 个选项,我答完你公布答案 + 解析,
重点解释干扰项为什么错。
```
