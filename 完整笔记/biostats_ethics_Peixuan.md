**BIOSTATISTICS and Ethics**

考点总结

1\. 诊断试验：解读你的报告单

| 核心考点 | 关键口诀 / 判定准则 | 患病率的影响 |
|----|----|----|
| 灵敏度 & 特异度 | 试验的“出厂配置”，描述抓病人和放好人的能力。 | 不变 |
| PPV (阳性预测值) | 拿阳性报告问：“我真有病吗？” | 同向 (患病率 PPV ) |
| NPV (阴性预测值) | 拿阴性报告问：“我真没病吗？” | 反向 (患病率 NPV ) |
| 似然比 (LR+/LR-) | 定海神针。将检前概率转化为检后概率的倍数。 | 不变 |
| 准确度 (Accuracy) | 所有人里测对的总比例。 | 加权变化 |

------------------------------------------------------------------------

2\. 推断统计： 值与置信区间的博弈

- 中心法则：置信区间（CI）必须以样本观察值为中心（对称分布）。

- 拉伸法则：置信水平越高（），区间越宽，结论越可靠，但精确度越低。

- 显著性判定：

  - 均值差 (Difference)：不包含 0 显著 ()。

  - 比率 (OR/RR)：不包含 1 显著 ()。

- 统计学 vs. 临床： 只代表“差异是真的”；临床意义看“差异够不够大”。

------------------------------------------------------------------------

3\. 统计方法选择：看准变量的“脸”

- 检验：比较 2 组人的数值（均值）（如：男 vs 女的血压）。

- ANOVA (方差分析)：比较 组人的数值（均值）。

- 卡方检验 (Chi-square)：比较两组人的比例 / 分类结局（如：有效 vs 无效）。

- 相关分析 (r)：研究两个数值之间的线性关系强度（ 到 ）。

------------------------------------------------------------------------

4\. 研究设计与因果评价

- 样本量 (Sample Size)：人多眼尖。样本量 检验效能 (Power) II 型错误 () 。

- Hill 因果标准：

  - 剂量-反应：剂量越大，风险越高（阶梯上升）。

  - 可逆性：撤除暴露，风险下降（最强实验证据）。

  - 强度： 离 1 越远，关联越强。

------------------------------------------------------------------------

5\. 易错红线（绝对禁忌）

1.  相关 因果：哪怕 ，也不能说谁引起了谁。

2.  值 错误率：它是在 为真时观察到现状的概率。

3.  ROC 曲线坐标：纵轴是灵敏度，横轴是 （不是特异度本人！）。

**MEASURES OF CENTRAL TENDENCY**

**Mean**

- The mean is the average.

- You calculate it by adding all values and dividing by the total number of values.

- It is highly affected by outliers.

**Median**

- The median is the middle number after arranging values in order.

- It is the most reliable measure in skewed distributions.

**Mode**

- The mode is the number that appears most frequently.

**Bimodal distribution**

- A bimodal distribution has two peaks.

- This suggests two different populations (example: young and elderly patients).

**SKEWED DISTRIBUTIONS**

- In any skewed distribution, the median is always in the middle.

**Positive skew (right-tailed distribution)**

- Order from lowest to highest: mode, median, mean

- The mean is pulled toward the higher values.

**Negative skew (left-tailed distribution)**

- Order from lowest to highest: mean, median, mode

- The mean is pulled toward the lower values.

**SENSITIVITY AND SPECIFICITY**

**Sensitivity**

- Sensitivity is the proportion of people with disease who test positive.

- It is used for screening tests.

- A highly sensitive test has very few false negatives but more false positives.

- Think of sensitivity like a fishing net: it catches everything, including false positives.

**Specificity**

- Specificity is the proportion of people without disease who test negative.

- It is used for confirmatory testing.

- A highly specific test has very few false positives but more false negatives.

**CORE TEST-TAKING RULE (MOST IMPORTANT)**

- Do not focus on whether a threshold is raised or lowered.

- Always determine what happens to the size of the positive group.

→ If the group gets bigger → sensitivity increases

→ If the group gets smaller → specificity increases

**CHANGING DIAGNOSTIC THRESHOLDS**

**Raising a threshold (example: diabetes 126 → 130)**

- Fewer people meet criteria

- The group becomes smaller

- Sensitivity decreases

- Specificity increases

**Lowering a threshold (example: 126 → 100)**

- More people meet criteria

- The group becomes bigger

- Sensitivity increases

- Specificity decreases

**INCIDENCE AND PREVALENCE**

**Incidence**

- Number of new cases

- Used in prospective studies

**Prevalence**

- Total number of cases (new + existing)

- Used in cross-sectional and retrospective studies

| **指标** | **定义** | **适用场景** |
|:---|:---|:---|
| **患病率 (Prevalence)** | **某时间点现存病例数 / 总人口** | **描述疾病负担（横断面研究）** |
| **发病率 (Incidence)** | **某期间新发病例数 / 风险人口** | **描述风险（队列研究）** |
| **患病率比 (PR)** | **暴露组患病率 / 非暴露组患病率** | **比较不同人群的疾病分布** |

**PREDICTIVE VALUES**

**Positive Predictive Value (PPV)**

- Probability that a person has disease given a positive test

- PPV increases when prevalence increases

- PPV decreases when false positives increase

**Negative Predictive Value (NPV)**

- Probability that a person does not have disease given a negative test

- NPV increases when sensitivity is high (few false negatives)

- NPV decreases when prevalence increases

<img src="images/media/image2.jpeg" style="width:2.74841in;height:1.99493in" /><img src="images/media/image3.jpeg" style="width:2.98462in;height:2.16785in" /><img src="images/media/image4.png" style="width:6.4739in;height:1.92752in" />

**B🡪A, sensitivity↑**

**B🡪C, specificity↑**

**HIGH-YIELD RULE**

If prevalence increases

→ PPV increases

→ NPV decreases

If a test is overly sensitive

→ False positives increase → PPV decreases

→ False negatives decrease → NPV increases

<img src="images/media/image5.png" style="width:2.12153in;height:1.07569in" />

**RELATIVE RISK AND ODDS RATIO**

**Relative Risk**

- Measures risk of developing disease given exposure

- Used in prospective cohort studies

- <img src="images/media/image6.png" style="width:1.00833in;height:0.41458in" />Uses incidence

**Odds Ratio**

- Measures likelihood that diseased individuals had prior exposure

- <img src="images/media/image7.png" style="width:1.01736in;height:0.375in" />Used in retrospective case-control studies

- Uses prevalence

**Key concept**

- Relative risk looks forward

- Odds ratio looks backward

**This is for informational purposes only. For medical advice or diagnosis, consult a professional.**

比值比 (Odds Ratio, OR) 和 相对危险度 (Relative Risk/Risk Ratio, RR)都用于衡量“暴露”与“结局”之间的关联强度；当发病率极低时，两者可视为等价。

1\. 原理分析：概率 vs. 比值, 理解它们的前提是分清“风险”和“比值”：

- 风险 (Risk/Probability)：**事件发生人数/总人数**（如：10人吸烟，2人得病，风险 = 2/10=20%）

- 比值 (Odds)：**事件发生人数/未发生人数**（如：10人吸烟，2人得病，8人没病，Odds=2/8=0.25）

核心公式：

- RR (相对危险度) = 暴露组风险 / 非暴露组风险。

- OR (比值比) = 暴露组 Odds / 非暴露组 Odds 。

2\. 临床应用：研究设计决定指标

**<span class="mark">RR</span>**（风险倍数），**<span class="mark">：多用于队列研究 (Cohort Study)</span>**

- 应用场景：**从现在追踪到未来。由于我们知道总人数（分母），可以计算出真实的发病率（风险）**

- 临床意义：直接告诉医生“暴露于某因素后，患病风险增加了几倍”。这是最直观、最符合临床直觉的指标 。

**<span class="mark">OR</span>**（比值倍数）**<span class="mark">：多用于病例对照研究 (Case-Control Study)</span>** <span class="mark">you take the case to the OR</span>

- 应用场景：回顾过去。**研究开始时，病例数和对照数是由研究者预设的**（比如找100个病人和100个正常人），我们无法得知人群中真实的发病率，因此不能计算 RR 。

- 临床意义：通过比值的比例来**估算关联强度** 。此外，**Logistic Regression的直接产出结果就是 OR 值** 。

在**回顾性研究**中，即便我们算出的是 OR，但**<span class="mark">如果该疾病在人群中非常罕见</span>**（发病率很低，通常 \<10%），那么分母中的 (1-P) 就趋近于 1，此时 **<span class="mark">OR= RR</span>** 。

3\. 记忆方法：两板斧

- 看设计：**<span class="mark">Cohort (队列) 🡪Count risk (计算风险) 🡪RR</span>**；**<span class="mark">Case-control (病例对照)🡪 OR</span>**。

- 看分母：RR 的分母是“全家桶”（总人数），OR 的分母是“对立面”（没病的人数） 。

**ATTRIBUTABLE RISK AND ABSOLUTE RISK REDUCTION**

**Attributable risk**归因风险

- 两组发病率的“差值”；它衡量的是如果消除这一暴露因素，暴露组能减少多少发病人数

- Number of cases caused by a risk factor

- Represents how much incidence would drop if the risk factor is removed

**Absolute risk reduction**

- Difference in risk between exposed and unexposed groups

**NNT AND NNH**

**Number Needed to Treat (NNT)**

- Number of people treated to benefit one patient

- You want this number to be small

Formula

NNT = 1 / absolute risk reduction

**NNT 是绝对风险降低率 (ARR) 的倒数，解读时必须带上“<span class="mark">对照组</span>”和“<span class="mark">观察期限</span>”。**

**描述时，人数、对照、结局、时间，缺一不可**

<img src="images/media/image8.png" style="width:4.12257in;height:2.12084in" />

在临床决策中，NNT 比相对风险降低率 (RRR) 更具参考价值：

- **NNT 越小**：治疗效果越显著（只需治几个人就能救一个，效率高）。

> 如果算出来是小数（如 10.2），考试或实际应用中要**向上取整**（变成 11）

- **成本效益分析**：如果一个药很贵但 NNT 很大（比如 1000），临床上可能就不划算。

- **与 NNH 对比**：临床医生常对比 NNT（获益）和 **NNH (Number Needed to Harm，需致残/毒数)** 来评估治疗的净获益。

**Number Needed to Harm (NNH)**

- Number of people treated to harm one patient

- You want this number to be large

Formula

<img src="images/media/image9.png" style="width:1.32986in;height:2.9625in" />NNH = 1 / attributable risk

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 39%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr>
<th colspan="3" style="text-align: left;">Common measures of therapeutic efficacy</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: left;">Term</td>
<td style="text-align: left;">Definition</td>
<td style="text-align: left;">Calculation</td>
</tr>
<tr>
<td style="text-align: left;">Absolute risk reduction (ARR)</td>
<td style="text-align: left;">Percentage indicating the actual difference in event rate between control &amp; treatment groups</td>
<td style="text-align: left;">ARR = control rate – treatment rate</td>
</tr>
<tr>
<td style="text-align: left;">Relative risk reduction (RRR)</td>
<td style="text-align: left;">Percentage indicating relative reduction in the treatment event rate compared to the control group</td>
<td style="text-align: left;"><p>RRR = ARR / control rate</p>
<p>=1-RR</p></td>
</tr>
<tr>
<td style="text-align: left;">Relative risk (RR)</td>
<td style="text-align: left;">Ratio of the probability of an event occurring in the treatment group compared to the control group</td>
<td style="text-align: left;">RR = treatment rate / control rate</td>
</tr>
<tr>
<td style="text-align: left;">Number needed to treat (NNT)</td>
<td style="text-align: left;">Number of individuals who need to be treated to prevent a negative outcome in 1 patient</td>
<td style="text-align: left;">NNT = 1 / ARR</td>
</tr>
</tbody>
</table>

| **指标 (Measure)** | **计算公式** | **在本题中的含义** |
|----|----|----|
| **相对风险 (RR)** | **Rexposed/Rcontrol** | **暴露组发病概率是由于对照组的多少倍 (0.4)** |
| **绝对风险降低 (ARR)** | **Rcontrol−Rexposed** | **预防措施让发病率绝对下降了多少个百分点 (0.3 或 30%)** |
| **相对风险降低 (RRR)** | **1−RR** | **干预措施减少了多少比例的风险 (60%)** |
| **需治疗人数 (NNT)** | **1/ARR** | **需让多少人饮用氟化水才能预防 1 例龋齿 (≈3.3 人)** |

**RRR+RR=1 (相对风险降低+相对风险=100%)**

**在干预措施下，剩下的风险（相对风险）和被消除掉的风险（相对风险降低）加起来，刚好等于原本 100% 的风险。**

<img src="images/media/image10.png" style="width:2.23819in;height:0.82067in" /> <img src="images/media/image11.png" style="width:2.23595in;height:0.81178in" />

**绝对风险降低率 (ARR)**：衡量的是**治疗前后，患病率或事件发生率数值上直接减少了多少，<span class="mark">用于计算 NNT</span>**

计算公式：**<span class="mark">ARR = 对照组发生率 - 实验组发生率</span> (Absolute（绝对），直接相减)**

ARR 的特点：它与基线风险密切相关，能反映真实的临床获益 。

- 应用：它是计算 需治数 (NNT) 的基础 (**<span class="mark">NNT = 1 / ARR</span>**) 。<span class="mark">医生</span>更看重 ARR，因为它能直接告诉我们要治多少人才能省下一笔医疗开支或救下一条命 。

相对风险降低率 (RRR)：衡量的是**治疗组相对于对照组，风险下降的比例（百分比），<span class="mark">常因基线风险低而显得数值更大</span>。**

计算公式：**<span class="mark">RRR = ARR/对照组发生率</span>（Relative（相对），ARR 除以对照组，算出百分比）**

RRR数值通常看起来非常“惊艳” 。

- *例子*：如果一种病的发病率从 2% 降到 1%，ARR 只有 1%，但 RRR 却是 50%。

- 应用：<span class="mark">药企</span>往往喜欢宣传 RRR，因为它能突出药物的效力

**RR (Relative Risk, 相对危险度)**

- 定义：治疗组发生事件的概率与对照组发生事件概率的比值 。

- 公式：RR=治疗组发生率/对照组发生率

- 物理意义：治疗后，患病风险变成了原来的几倍 。

RR 与 RRR 的互补关系：**<span class="mark">RRR=1-RR，</span>两者之和恒等于 1**

- **RR 是风险的余数（剩多少），就像“折扣率”：RR=0.7相当于商品打7折**

- **RRR 是风险的降幅（少多少），** **就像“优惠额度”：打7折意味着你少花了30%的钱**

- 如果治疗后的风险变成了原来的 0.8 倍（RR=0.8），那么风险就相对下降了1-0.8=0.2 ，即20% (RRR=20%) 。

RR 与 ARR 的关系

- 公式：ARR=对照组发生率X(1-RR)

- 解释：ARR 取决于两个因素：风险下降的程度（1-RR）以及疾病原本的严重程度（对照组发生率） 。

2\. 临床应用

- RR 的直观性：医生在看研究结果时，如果看到RR\<1 ，立刻就知道治疗有效 ；如果 RR=0.6，说明治疗能把风险降到原来的60%。

- 风险评估：在队列研究中，RR 是最核心的指标，用于衡量暴露因素与结局的因果强度 。

  - <span class="mark">RR=1🡪治疗无效</span> (如果 RR的95% 置信区间（CI）包含了 1.0，说明结果没有统计学意义)

  - <span class="mark">RR\<1🡪治疗有效</span>（风险降低），**<span class="mark">RR 离 1 越远（越小），RRR 就越大，疗效越好</span>**

  - <span class="mark">RR\>1🡪治疗有害</span>（风险增加，比如吸烟导致肺癌的 RR 通常\>1 ） 。

<span class="mark">RR 是风险的倍数，1 减去 RR 便是风险降低的比例 (RRR)</span>。

**<span class="mark">高 RR 值代表强关联，而风险随暴露剂量增加而上升则确证了剂量-反应关系。</span>**

**<span class="mark">撤除暴露因素后效应随之减弱或消失（可逆性），是判定因果关系最强有力的实验性证据。</span>**

**核心判定逻辑：**

- <span class="mark">**关联强度 (Strength of Association)**：看 RR偏离 **1.0** 的程度</span>。

1.  **剂量-反应关系 (Dose-Response Relationship)**：

    - **判定标准**：**随着暴露剂量（吸烟量）的增加，效应（患癌风险）是否也相应地、单调地增加**？

    - **分析**：吸烟量增加（1🡪2🡪3 PPD），风险值也随之阶梯式上升（2.4🡪3.0🡪4.1）

    - **结论**：具有明显的**剂量-反应关系**。

**2. 临床与科研价值**

- **生物学合理性**：**<span class="mark">剂量-反应关系是支持“因果关系”</span>**最强有力的证据之一。它暗示了某种生物学机制（如烟草毒素积累）在起作用，而不仅仅是偶然的关联。

- **公共卫生意义**：这告诉我们，哪怕不能戒烟，减少吸烟量（从 3 PPD 降到 1 PPD）也能显著降低患癌风险。

**3. 考试陷阱**

- **陷阱 1：只看到关联而忽略趋势**。有些题目RR很大，但不同剂量下的RR差不多（比如都是 3.0），那时候就没有剂量-反应关系。

- **陷阱 2：统计学意义 vs 关联强度**。 **<span class="mark">P\<0.05只代表关联是真实的</span>**，不代表关联是强的。**<span class="mark">关联强度只看RR的绝对数值</span>**。

**4. 记忆方法：台阶效应**

- **强关联：离地标（RR=1）很远。**

- **剂量-反应：像爬台阶，剂量上一层，风险也高一层。**

**2x2 TABLE INTERPRETATION**

**Cells**

- A = disease positive and exposure/test positive

- B = disease negative and exposure/test positive

- C = disease positive and exposure/test negative

- D = disease negative and exposure/test negative

→ Always check the axes before calculating.

**Formulas**

- **<span class="mark">Relative risk = \[A/(A+B)\] divided by \[C/(C+D)\]</span>**

- **<span class="mark">Odds ratio = (A × D) divided by (B × C)</span>**

- **<span class="mark">Attributable risk = A/(A+B) minus C/(C+D)</span>**

- **<span class="mark">Absolute risk reduction = C/(C+D) minus A/(A+B)</span>**

**STUDY DESIGNS**

**Cohort study**

- Prospective

- Measures incidence

- Uses relative risk

**Case-control study**

- Retrospective

- Measures prevalence

- Uses odds ratio

**Cross-sectional study**

- Snapshot in time

- Measures prevalence

**Case report**

- Single unusual patient

**Case series**

- Multiple unusual patients

**TWIN AND ADOPTION STUDIES**

**Twin studies**

- Genetics are the same

- Used to study environmental factors

**Adoption studies**

- Environment is shared

- Used to study genetic factors

**CLINICAL TRIAL PHASES**

**Phase 0**

- Very early human exposure

- Determines whether to proceed

**Phase 1**

- Safety and toxicity

**Phase 2**

- Efficacy and side effects

**Phase 3**

- Comparison to current standard

**Phase 4**

- Post-marketing

- Focus on real-world use, compliance, and adverse effects

**STATISTICAL TESTS**

**T-test**

- Compares **two means**

**ANOVA**

- Compares **three or more means**

**Chi-square**

- Compares **proportions or categorical variables**

**POWER**

- Power is the ability to detect a true effect.

- The best way to **increase power** is to **increase sample size**.

<img src="images/media/image12.png" style="width:5.29394in;height:2.35187in" />

| 自变量 (组别) | 因变量 (结局) | 推荐检验 |
|----|----|----|
| 分类 (2 组) | 定量 (**均值**) | **t test** （比较两个独立组别的**数值均值**）**<span class="mark">均值被视为连续变量</span>** |
| 分类 (\>2 组) | 定量 (**均值**) | **ANOVA (analysis of variance)** |
| 分类 (2 组) | 分类 (**频率**) | **Chi-square** （比较两个**分类变量**之间的关联） |
| 定量 (**连续**) | 定量 (**连续**) | **Correlation/linear regression** （描述两个**定量变量**之间的线性关系） |

自变量 (Independent Variable), 因变量 (Dependent Variable)

双定量选回归，双定性选卡方，自定性因定量选 t/ANOVA。

**卡方检验**（**Chi-square**）是看**两组分类变量**之间“**有没有关系**”

- **因变量类型**：定性/**<span class="mark">分类变量</span>** 。

- **自变量类型**：只能是**定性/<span class="mark">分类变量</span>** 。

- **核心目的**：检验两个分类变量之间是否**相互独立**（有没有关联） 。它给出的主要是一个<span class="mark">p值</span>，告诉你“吸烟和肺癌之间是否有统计学关联”

常用于基础的**组间比较**。比如：比较 A 组（用药）和 B 组（安慰剂）的有效率是否有差异。

**<span class="mark">即便原始数据是连续的，只要研究者按门槛将其划分为“是/否”两类，统计分析就必须使用卡方检验。</span>**

**逻辑回归**（**Logistic Regression**）是看“**关系有多大**”，并且能同时考虑**多个影响因素**。

- **因变量类型**：定性/**<span class="mark">分类变量（通常是二分类）</span>** 。

- **自变量类型**：非常灵活，<span class="mark">可以是**分类变量**，也可以是**连续数值（定量变量）**</span> 。

- **核心目的**：量化关联的**强度**。它不仅给你 **<span class="mark">p值</span>**，还会给你 **<span class="mark">OR 值</span>** ，告诉你“吸烟者患肺癌的风险是不吸烟者的几倍”。

常用于**多因素分析/预测**。比如：同时考虑年龄（连续数值）、性别（分类）、是否吸烟（分类）对“是否患肺癌”的影响。它可以排除年龄和性别的干扰，得出吸烟的独立风险。

**<span class="mark">双分类变量看关联选卡方</span>；<span class="mark">自变量包含连续数值或需要计算 OR 值/校正因素选逻辑回归</span>。**

如果题目只问“**两者是否有关联**”，**<u>卡方</u>**通常是最简便的选择；

如果要求“**计算 OR 值**”或“**控制混杂因素**”，则必须选**<u>逻辑回归</u>** 。

| **特性**            | **卡方检验 (Chi-square)** | **逻辑回归 (Logistic)** |
|---------------------|---------------------------|-------------------------|
| **自变量 (X) 要求** | **必须是分类**            | 分类、定量皆可          |
| **主要功能**        | 比较比例/检验独立性       | 风险预测/计算 OR        |
| **处理变量数**      | 通常 2 个（单因素）       | 可以多个（多因素）      |

| **特性** | **线性回归 (Linear regression)** | **逻辑回归 (Logistic regression)** |
|----|----|----|
| **因变量 (Y)** | **连续数值/定量 (如：身高、血压)** | **二分类结局**/**定性(如：生/死)** |
| **主要产出** | **系数 (β)** | **比值比 (OR)** |
| **图形形状** | **直线** | **S 型曲线 (Sigmoid curve)** |

<img src="images/media/image13.jpeg" style="width:2.34167in;height:2.50903in" />

**ACCURACY AND PRECISION**

**Accuracy (validity)**

- Measures how close results are to the true value

**Precision (reliability)**

- Measures consistency of results

→ **<span class="mark">Accuracy = correct</span>**

→ **<span class="mark">Precision = consistent</span>**

**<span class="mark">Accuracy = (TP + TN) / (TP + FP + TN + FN)</span>**

**BIAS (HIGH-YIELD)**

**Selection / Sampling**

- Selection bias

  - Sample is not representative

  - Fix with randomization

- Berkson bias

  - Selection of hospitalized patients

**Data Collection**

- Recall bias

  - Faulty memory

  - Fix by shortening recall time and asking multiple questions

- Measurement bias

  - Inconsistent tools

  - Fix by using the same tool for all subjects

**Study Execution**

- Attrition bias

  - Loss of participants

- Procedure bias

  - Different groups treated differently

  - Fix by applying the same protocol and blinding

**Observer Effects**

- Hawthorne effect

  - Subjects change behavior because they are being observed

  - Fix with blinding and placebo

- Observer expectancy bias (Pygmalion effect)

  - Researcher expectations influence results

  - Fix with double or triple blinding

**Variables**

- **Confounding bias**

  - **<span class="mark">Unwanted variable</span>** affecting both exposure and outcome

  - **Fix with** **<span class="mark">matching</span>** or **<span class="mark">crossover studies</span>**

- **Effect modification**

  - **<span class="mark">Variable that changes the outcome and should be studied</span>**, not removed

<table style="width:93%;">
<colgroup>
<col style="width: 23%" />
<col style="width: 34%" />
<col style="width: 34%" />
</colgroup>
<thead>
<tr>
<th>特性</th>
<th>混杂因素 (Confounding)</th>
<th>效应修饰 (Effect Modification)</th>
</tr>
</thead>
<tbody>
<tr>
<td>与暴露/结局关系</td>
<td><p>均有关联，非中间环节</p>
<p>产生一种虚假的相关性</p>
<p><strong>需要被校正的“干扰项”</strong></p></td>
<td><p>改变暴露与结局关联的大小</p>
<p><strong>需要被分层展示的“交互作用”</strong></p></td>
</tr>
<tr>
<td>统计学表现</td>
<td>校正前后效应值显著改变</td>
<td>分层后的效应值彼此不等</td>
</tr>
<tr>
<td>处理目标</td>
<td>消除/控制 (Control)</td>
<td>分析/描述 (Analyze)</td>
</tr>
</tbody>
</table>

**<u>控制混杂因素</u>**

**设计阶段**：

- **随机化 (Randomization)**：通过随机分配，平衡组间已知和未知的混杂因素 。

- **配对 (Matching)**：确保对照组和病例组在混杂因素（如年龄、性别）上是一致的。

- **交叉设计 (Crossover studies)**：受试者先后接受不同处理，自己做自己的对照，消除个体间的混杂。

**分析阶段**：

- **分层分析 (Stratified analysis)**：按照混杂因素的不同水平分别分析（如按是否抽烟分层） 。

- **多元回归 (Multiple regression)**：在模型中纳入混杂因素作为**协变量**进行校正，从而看清主要研究因素的“净效应” 。

效应修饰：用于**<span class="mark">亚组分析 (Subgroup analysis)</span>**。通过发现效应修饰，医生可以实现**“精准医疗”**，确定**哪类特定人群最能从治疗中获益**。

**混杂因素** (Confounding) **<span class="mark">总分不等，层间相等</span>**（大家都被同一个因素忽悠了） 。

- 特征：**分层后，各层的结果趋于一致（不管有没有意义，大家都差不多），但这个一致的结果和分层前的总结果不一样** 。

- 例子：原本总 RR=4.0，分层后两层都变成了 RR=2.0 。虽然 2.0 依然“有意义”（大于1），但因为它和 4.0 不一样，所以它是混杂 。

- 临床意义：说明总体的那个结果是被“污染”的假象，必须通过校正来消除 。

**效应修饰** (Effect Modification) **<span class="mark">层间不等，各显神通</span>**（不同人有不同反应）

- 特征：**分层后，各层的结果各长各的**（有的有意义，有的没意义；或者一个大，一个小） 。

- 例子：原本总 RR=2.0，分层后发现男性的 RR=4.0（非常有意义），女性的 RR=1.0（完全没意义）

- 临床意义：这说明暴露因素对不同人群的影响本来就不同，这叫“交互作用”，需要分别报告 。

**LEAD TIME AND LENGTH TIME BIAS**

**Lead time bias**

- Earlier diagnosis makes survival appear longer

- Does not actually improve survival

**Length time bias**

- Slower diseases are more likely to be detected

- Also overestimates survival

**PREVENTION**

**Primary prevention**

- Prevent disease before it occurs

- Example: vaccination

**Secondary prevention**

- Detect disease early

- Example: screening tests

**Tertiary prevention**

- Treat disease to prevent complications

- Example: diabetes management

**Quaternary prevention**

- Avoid unnecessary testing and overmedicalization

**ERRORS AND SAFETY**

**Active error**

- Error occurring now

- Use root cause analysis

**Latent error**

- Error waiting to happen

- Use failure mode and effects analysis

**Near miss**

- Error almost occurred but was prevented

**AGING (HIGH-YIELD)**

- Pulse pressure increases with age

- Systolic pressure increases

- Diastolic pressure decreases

- Immune response slows

- REM sleep decreases

- Muscle decreases, fat increases

- Residual lung volume increases

- Total lung capacity stays the same

- Intelligence remains stable

**ETHICS **

**CORE PRINCIPLES**

**Autonomy**

- Patient has full control over their body

**Beneficence**

- Act in patient’s best interest

**Nonmaleficence**

- Do no harm

**Justice**

- Fair distribution of resources

**AUTONOMY (MOST IMPORTANT)**

**Schloendorff v. Society of New York Hospital (1914)**

- Established patient autonomy

- Treating without consent = assault and battery

**CAPACITY VS COMPETENCY**

**Capacity**

- Determined by physician

**Competency**

- Determined by court

- Capacity is based on understanding, reasoning, memory, and judgment

- Suicidal patients lack capacity

**MINORS**

- Parents or guardians make decisions

**Exceptions (partial emancipation)**

- STDs

- Contraception

- Pregnancy

- Substance abuse

- Emancipated minors can make all decisions

- Parents cannot refuse life-saving treatment

**INFORMED CONSENT**

- Must include risks, benefits, and alternatives

- Must be understandable

- Consent is implied in emergencies

- Physician must disclose experience if asked

**CONFIDENTIALITY**

- Cannot disclose without consent

**Exceptions**

- **Danger to self or others**

- **Abuse**

- **Reportable disease**

- **Court order**

**Tarasoff case**

- Duty to warn potential victims

**ADVANCE DIRECTIVES**

**Living will**

**Health-care proxy**

- Proxy speaks patient’s wishes

- DNR only limits resuscitation

- All other care continues

**END-OF-LIFE**

- Patients can refuse any treatment

- No ethical difference between withholding and withdrawing care

**Doctrine of double effect**

- Pain relief is allowed even if it shortens life

**Physician-assisted suicide**

- Physician provides means

**Euthanasia**

- Physician administers (illegal)

- Brain death = death

**MALPRACTICE**

- Requires all four

  - Duty

  - Breach

  - Damage

  - Causation

- No harm = no malpractice

**REPORTING**

- Must report

  - Child abuse

  - Elder abuse

  - Gunshot wounds

  - Reportable diseases

- Do NOT report spousal abuse without consent

**ORGAN DONATION**

- Voluntary

- Cannot be sold

- Family has final say

【补充】

**Meta-analysis通过Pooling小样本研究来增加总体样本量，其主要目的是提高统计效能（Power）并缩小置信区间以提升精确度。**

- **Power (效能)：** 是指当处理效应确实存在时，研究能够正确地检测出该效应并拒绝零假设的可能性。

- **样本量↑🡪standard error**标准误**↓🡪confidence interval 变窄🡪precision精度↑🡪power↑，beta↓**

| **特征** | **I 型错误 (alpha)** | **II 型错误 (beta)** |
|:---|:---|:---|
| **定义** | <span class="mark">**假阳性**：误认为有差异</span> | <span class="mark">**假阴性**：漏掉了真实差异</span> |
|  | **<span class="mark">CI = (1-alpha)%</span>** | **<span class="mark">Power = 1-beta</span>** |
| **如何降低** | **<span class="mark">设定更严格的值 (如 0.01)</span>** | **<span class="mark">增加样本量 (N)</span>** |
| **Meta-analysis的作用** | 通常不直接影响 | **显著降低 (即增加 Power)** |

**样本量增加会提高检验效能 (Power)，从而显著降低发生 II 型错误 (beta) 的风险**

<img src="images/media/image14.png" style="width:5.64375in;height:1.89583in" />

在考试中，看到关于“研究样本量太小”的问题：

1.  **如果问缺点：** 选 “Low statistical power” 或 “High risk of Type II error”。

2.  **如果问怎么改进：** 选 “Increase sample size” 或 “Perform a meta-analysis”。

3.  **关于 <span class="mark">CI：</span>** <span class="mark">**Narrower = Better (More precise)**</span>。

**避坑指南：**在统计学里，我们想要的是 **<span class="mark">Increase Power</span>**，但想要的是 **<span class="mark">Decrease/Narrow CI</span>**

<img src="images/media/image15.jpeg" style="width:2.55696in;height:2.12511in" />

置信区间宽度原理：

置信区间（CI）是由样本数据计算出的一个范围，旨在以一定的置信水平捕捉真实的总体值 。置信水平C（如 95%）指的是如果重复多次实验，计算出的区间包含真实总体值的频率 。C=1-alpha, CI=C%

- 宽度变化 ：为了获得更高的置信度（即更有把握捕捉到真值），必须覆盖样本分布中更大比例的部分 。因此，在相同数据下，**置信水平越高，CI 就会越宽** 。即 95% CI 总是比 90% CI 更宽 。

**<span class="mark">CI包含的值：均值差看 0，比率（OR/RR）看 1</span>**

**置信区间接近 0，**通常出现在**比较两个均值（Means）或比例（Proportions）的差值**时。

- **指标**：**<span class="mark">均值差（Mean Difference, MD）</span>**或 **<span class="mark">绝对风险降低率（ARR）</span>**。

- <span class="mark">**无效点**=**0**</span>。因为如果两组没有差异，减法的结果就是 0。

- **接近 0 的意义**：

  - **统计学上**：如果 CI 包含了 0（例如 -0.1到 +0.5），说明结果**不显著** (P \> 0.05)。

  - **临床上**：如果 CI 离 0 非常近（例如 0.01 到 0.02），说明虽然在统计学上这药“有效”（P \< 0.05），但减出来的差值太小了，患者可能根本感受不到疗效。

**置信区间接近 1，**通常出现在计算比率（Ratios）时。

- **指标**：**<span class="mark">相对危险度（RR）或 比值比（OR）</span>**。

- <span class="mark">**无效点**=**1**</span>。因为如果两组风险一样，除法的结果就是 1。

- **接近 1 的意义**：

  - **统计学上**：如果 CI 包含了 1（例如 0.95 到 1.05），说明结果**不显著** (P \> 0.05)。

  - **临床上**：如果 CI 虽然没过 1，但紧贴着 1（例如 0.98到0.99），说明风险只降低了区区 1%。结论是：这个因素虽然“相关”，但关联强度极弱，实际临床意义很小。

**4. 总结与记忆方法**

- **差值（Difference）看 0**：想像成“拔河”，两边力气一样大，位移就是 0。

- **比率（Ratio）看 1**：想像成“分蛋糕”，两边分得一样多，比例就是 1:1。

| **研究指标** | **计算方式** | **无效点 (Null)** | **接近该点的意义** |
|:---|:---|:---|:---|
| **<span class="mark">均值差 (MD) / ARR</span>** | <span class="mark">减法</span> | **<span class="mark">0</span>** | 差异极小，临床获益微弱 |
| **<span class="mark">OR / RR / HR</span>** | <span class="mark">除法</span> | **<span class="mark">1</span>** | 风险改变极小，关联强度极弱 |

**<span class="mark">置信区间包含无效点（0 或 1）代表无统计学意义；若紧贴无效点则代表临床意义可能不足。</span>**

2\. 临床应用

在临床科研中**，提高置信水平**虽然**增加了结论的可信度**，但代价是区间变宽，即**精确度下降**：

- 权衡：研究者通常在 95% 置信水平（对应alpha = 0.05）下报告结果，这是临床研究的通用“金标准”。

- 决策：如果一个药物疗效的 95% CI 非常宽且接近 0，即使结果显著，医生也可能认为其临床价值不稳定。

<span class="mark">置信水平越高，区间越宽；若 CI 因变宽而包含了无效值（如 0 或 1），则显著性消失。</span>

**<span class="mark">正确的置信区间必须以样本差异值为中心，且其是否包含无效值（0）必须与p值的显著性保持绝对一致</span>**

**<span class="mark">p值是在假设两组无差异时，仅凭运气得到当前（或更极端）观测结果的概率。</span>**

**p值的“三大要素”：**

1.  **前提：假设 H0 是真的（两组没区别）。**

2.  **内容：看到目前这个差异（或更牛的差异）。**

3.  **结果：发生的概率（小概率事件）。**

P值的硬核定义：在零假设 (H0) 为真的前提下（即假设两组药其实没区别），观察到当前样本结果或更极端结果出现的概率。

本题逻辑：

- 零假设 (H0)：新药和二甲双胍的降糖效果完全一样（真实差异为 0）。

- 观察结果：新药比二甲双胍多降了0.5% 的 HbA1c。

- P=0.02的意义：如果这两组药实际上并没有任何区别，那么仅仅因为“运气”或随机误差，导致新药比二甲双胍表现好出≥0.5% 的可能性只有2% 。

<!-- -->

- **森林图（Forest Plot）**

<img src="images/media/image16.png" style="width:3.16098in;height:2.52619in" />

| 指标/现象 | 代表含义 | 显著性判断标准 |
|:---|:---|:---|
| 相对风险 (RR) / 比值比 (OR) | \>1：风险增加；\<1：风险降低 | 如果 95% CI 包含/跨越 1，则不显著 |
| P 值 (P-value) | 观察到的差异由随机误差导致的概率 | P\<0.05 认为具有统计学显著性 |
| 森林图中的菱形 | Meta分析的汇总效应值 | 菱形不触碰无效线（1.0）则显著 |
| 小型研究 (Small studies) | 往往由于样本量不足导致 95% CI 极宽且跨越 1.0 | 汇总后可缩小 95% CI，提高显著性 |

| 图像元素         | 代表效应值 (Point Estimate) | 代表 95% 置信区间 (95% CI) |
|:-----------------|:----------------------------|:---------------------------|
| 单项研究 (Study) | 黑块或圆点的中心            | 水平横线的长度             |
| 汇总结果 (Total) | 菱形中心的最宽处            | 菱形左右两个尖角的跨度     |

<span class="mark">菱形的宽度 = 单项研究中横线的长度</span>。

**无效线 (Line of Null Effect)**：图中位于 **1.0** 处的垂直实线被称为无效线

当横线“触碰”或“跨越”这条 1.0 的垂直线时，代表 **1.0 被包含在了该研究的 95% CI 之内** 。

| 图像特征                     | 统计学解读       | 临床意义举例             |
|:-----------------------------|:-----------------|:-------------------------|
| 横线/菱形跨越 1.0            | P≥0.05（不显著） | 无法确定是否能降低风险   |
| 横线/菱形在 1.0 左侧且不触碰 | P\<0.05（显著）  | 风险显著降低（保护因素） |
| 横线/菱形在 1.0 右侧且不触碰 | P\<0.05（显著）  | 风险显著增加（危险因素） |

这张图结论：森林图菱形在 1.0 左侧代表风险降低，其不触碰 1.0 垂直线且 P \< 0.05 代表结果具有统计学显著性。

<img src="images/media/image17.png" style="width:3.68694in;height:2.19636in" />

**<span class="mark">Sensitivity, specificity只与test有关</span>**

**Specificity (特异度/真阴性率) ：** 在所有**确实无病**的人中，测试结果为**阴性**的比例。

**Sensitivity (灵敏度/真阳性率) ：** 在所有**确实有病**的人中，测试结果为**阳性**的比例。

**<span class="mark">Accuracy = (TP + TN) / (TP + FP + TN + FN)</span>**

**=** **<span class="mark">(True positives + True negatives) / Total number of individuals tested</span>**

<img src="images/media/image18.jpeg" style="width:4.27692in;height:3.60598in" />

**ROC** 曲线帮助我们做两件事：

- **评估试验质量**：曲线越靠近左上角，曲线下面积 (AUC) 越大，试验的诊断准确性就越高。

- **寻找最佳切点 (Optimal Cut-off)**：通常选取曲线左上角最“凸”出的那个点（约登指数最大点），在那里灵敏度和特异度的综合效能最好。

- **左上角 (0, 1)**：代表 100% 灵敏度和 100% 特异度，这是诊断界的“神”。 **<span class="mark">左上角是“神”</span>**

- <span class="mark">右下角是随机瞎猜。</span>

- 点 X 的处境：它为了追求极高的灵敏度（不漏诊），牺牲了大量的特异度（导致大量误诊）

**AUC (Area Under the Curve)** 就是衡量一个试验“智商”的总分。

**1. 原理分析：从“点”到“面”**

我们在 ROC 曲线上看到的每一个点，都代表一个特定切点（Cut-off）下的灵敏度和特异度。而 AUC 则是把所有可能的切点都考虑进去后的总评价。

- <span class="mark">**AUC = 0.5**：代表试验完全没用</span>，相当于抛硬币瞎猜。

- **0.5 \< AUC \< 0.7**：诊断价值较低。

- **0.7 \< AUC \< 0.9**：诊断价值中等。

- <span class="mark">**AUC \> 0.9**：诊断价值极高</span>

- **<span class="mark">AUC = 1.0：完美试验</span>**（现实中基本不存在）。

**3. 考试陷阱**

- **陷阱 1：认为 AUC 与患病率有关**。

  - **避坑**：<span class="mark">AUC 由灵敏度和特异度推导而来</span>，是试验的**固有属性**，不受人群患病率的影响。

- **陷阱 2：曲线交叉**。

  - 如果两条 ROC 曲线发生了交叉（一截你在上，一截我在上），此时即便 AUC 相等，临床选择也会不同。如果你需要极高的灵敏度（筛查），就选左侧更陡的那条；如果你需要高特异度（确诊），就选右侧更高的地方。

**4. 记忆方法：地毯式搜索**

你可以把 AUC 想象成\*\*“扫雷”的覆盖率\*\*：

- 曲线越往左上角“顶”，它下面覆盖的面积（地毯）就越大。

- **面积越大**，说明它在区分敌我（病人 vs. 健康人）时犯错的总概率越小。

**5. 一句话总结考点**

**<span class="mark">AUC 是衡量诊断试验整体效能的指标，数值越接近 1，区分病人的能力就越强，且不受患病率影响</span>。**

**<span class="mark">PPV, NPV与prevalence有关</span>**

| **指标** | **英文口诀** | **分母 (Who are we looking at?)** | **含义** |
|:---|:---|:---|:---|
| **Sensitivity** | **SNOUT** | **所有确定的病人** | 灵敏度高，**阴性**结果可用来**排除**诊断。**<span class="mark">筛查</span>** |
| **Specificity** | **SPIN** | **所有确定没病的人** | 特异度高，**阳性**结果可用来**<span class="mark">确诊</span>**。 |
| **PPV** | \- | **所有测试阳性的人** | 如果我测出阳性，我**真有病的概率**是多少？ |
| **NPV** | \- | **所有测试阴性的人** | 如果我测出阴性，我**真没病的概率**是多少？ |

 **已知患病状态**→求检测结果概率→看 **灵敏度/特异度**。

 **已知检测结果**→求真实患病概率→看 **PPV/NPV**。

**PPV 和 NPV 会随着患病率“随风摇摆”**<img src="images/media/image19.jpeg" style="width:1.52778in;height:1.6in" />

**患病率越高，检测阳性时“真得病”的概率就越大。即 <span class="mark">患病率↑🡪 PPV↑</span>**

**患病率越低，检测阴性时“真没病”的概率就越大。即 <span class="mark">患病率↓🡪 NPV↑</span>**

**检后概率 (Post-test Probability)**

**对于已知测试为阴性的个体，其患病概率等于 \$1\$ 减去该测试的阴性预测值 (NPV)。**

**<span class="mark">当一个人的患病风险（Prevalence/Pretest Probability）升高时，该测试的 NPV 会下降。</span>**

**检前概率越高，阴性预测值 (NPV) 越低；对于极高危患者，阴性结果不足以排除诊断，通常需要更精准的“金标准”检查。**

这意味着，虽然她的活检是阴性，但因为她本身属于高危人群，这个“阴性”的可信度（即真正没病的概率）要比普通人低一些。

<img src="images/media/image20.png" style="width:6.50464in;height:1.41589in" />

**似然比是评价诊断试验强度的固定指标，它通过将检前概率转化为检后概率，帮助医生量化检测结果的临床价值。**衡量的是：**“病人和健康人相比，谁更容易出现这种检测结果？”**

**阳性似然比 (Positive Likelihood Ratio, LR+)**

它回答的是：患病的人拿到阳性结果的概率，是健康人拿到阳性结果概率的多少倍？

- **物理意义**： <span class="mark">**越大（通常\>10 ）🡪highly specific test**，说明这个阳性结果越牛，越能确诊疾病</span>。

**阴性似然比 (Negative Likelihood Ratio, LR-)**

它回答的是：患病的人拿到阴性结果的概率，是健康人拿到阴性结果概率的多少倍？

- **物理意义**： <span class="mark">**越小（越接近 0）🡪highly sensitive test，**说明这个阴性结果越给力，越能排除诊断</span>。

**LR 比 PPV/NPV 更好用**

- **独立性**：**LR** 只由灵敏度和特异度决定，**<span class="mark">不受患病率影响</span>**。

- **可解释性**：

  - **LR+=10：意味着阳性结果让患病概率提升了约 45%。**

  - **LR-=0.1：意味着阴性结果让患病概率降低了约 45%。**

  - **LR=1：意味着这个测试完全没用，做了白做。**

<img src="images/media/image21.png" style="width:5.76806in;height:2.14236in" />

<img src="images/media/image22.png" style="width:3.97688in;height:1.82584in" />

**<u>Pearson correlation coefficient</u>**

**<span class="mark">相关系数 r 的正负代表变量波动的方向，其绝对值代表关联的强度，但无论数值多大都不能直接推导出因果关系（相关≠因果）</span>**

在临床实践中，家属代为行使知情同意是常态，但在**开展医学研究**的语境下，法律和伦理的先后顺序非常严格。

以下是为什么不能直接选“获取家属知情同意”的原因分析：

**1️⃣ 法律地位的先后顺序：行政审批 vs. 临床执行**

- **IRB（机构审查委员会）是“准入证”**：在任何研究涉及第一个受试者（哪怕是有家属同意的受试者）之前，研究方案本身必须先经过 IRB 审批。没有 IRB 批准，任何形式的知情同意在法律上都是无效的。

- **家属同意是“执行环节”**：只有在 IRB 批准了研究方案，并明确了在患者无法表达时可以由家属代签后，医生才能去执行这一步。

**2️⃣ 急诊研究的特殊性 (Exception from Informed Consent, EFIC)**

这道题描述的是急诊危重症研究。在这种特殊情况下，家属往往也不在现场，或者情况紧急到根本没有时间进行详尽的解释。

- **IRB 的裁量权**：对于这种无法获得即时同意的急诊研究，IRB 有权根据法规（如美国 FDA 的 21 CFR 50.24）决定是否允许“知情同意豁免”**或**“延迟知情同意”。

- **结论**：是由 IRB 来决定“家属同意是否足够”或者“是否可以先救人后补签”，而不是由医生个人决定。

在医学伦理题目中，如果选项中出现了 **"Apply to the IRB"** 或 **"Consult the Ethics Committee"**，且当前研究尚未启动，这通常是优先级最高的“标准答案”。

家属同意能解决“代理授权”问题，但解决不了“研究合法性”问题；只有 **IRB 批准** 才是开展任何临床试验的法定第一步。

 **如果是研究（Research）**：只要题目提到“研究”、“评估效果”、“新药试验”，哪怕患者快死了，答案的第一步永远是 **“IRB Approval”**。

 **如果是救命（Emergency Treatment）**：如果题目问“昏迷患者大出血，找不到家属，下一步怎么做？”，答案通常是 **“Proceed with emergency treatment”**（紧急手术或输血），不需要等法院命令，也不需要等 IRB。
