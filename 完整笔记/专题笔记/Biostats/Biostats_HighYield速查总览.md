---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-06-12
type: 专题笔记
---

# Biostatistics & Epidemiology（生物统计与流行病学）High-Yield 速查总览（决策导向 / 总索引）

> [!info] 用途
> 整科 Biostats / Epi（生物统计与流行病学）"**下一步 next step / 怎么判读**"决策速查，派生自 [[完整笔记/Peixuan分科笔记/Biostats_Master]]（分科主笔记，只读）全 1114 行提炼。
> 本卡 = **决策骨架 + 钥匙 + 公式 + 判读规则**；各深挖主题已有独立专题笔记 → 🧩 指向，本卡不重复展开。
> 公式 / 阈值 / 数字均按 Biostats_Master 原文，未自行补充。

---

> [!note]- 目录（点击跳转）
> - [[#〇、一题流总决策树（看到 Biostats 题先分类）|〇 一题流总决策树]]
> - [[#一、2×2 表 — 所有公式的根|一 2×2 表]]
> - [[#二、诊断检验四指标 — Sn / Sp / PPV / NPV / LR / ROC|二 诊断检验四指标]]
> - [[#三、风险与效应指标 — RR / OR / ARR / RRR / NNT|三 风险与效应指标]]
> - [[#四、研究设计 — 一句话秒认 + 可算指标|四 研究设计]]
> - [[#五、偏倚 Bias — 记情境不记定义|五 偏倚 Bias]]
> - [[#六、假设检验 — α / β / Power / p / CI|六 假设检验]]
> - [[#七、统计检验选择（给场景选检验）|七 统计检验选择]]
> - [[#八、Hill 因果判定 + 流行病学指标关系|八 Hill 因果判定]]
> - [[#九、其余高频小点|九 其余高频小点]]
> - [[#🔗 关联|关联]] · [[#✅ 复盘行动|复盘行动]]

## 〇、一题流总决策树（看到 Biostats 题先分类）

```
Biostats 题
   │
   ├─ 给 2×2 表 / 给数字 → 算指标？
   │     ├─ 已知"患病状态"求检测概率 → Sn / Sp（不受患病率影响）
   │     ├─ 已知"检测结果"求真实患病 → PPV / NPV（受患病率影响）
   │     └─ 给暴露/治疗 → RR / OR / ARR / RRR / NNT（见 §三）
   │
   ├─ 描述研究方法 → 识别研究设计？（见 §四）
   │     "随机分组"=RCT / "前瞻追踪暴露"=cohort / "回顾找暴露"=case-control
   │     "某时点同时测"=cross-sectional
   │
   ├─ 描述一个"系统性偏差"情境 → 认 bias？（见 §五）
   │
   ├─ 给 p 值 / CI / α / β → 判读显著性？（见 §六）
   │
   ├─ 给场景选统计检验？（见 §七）
   │
   └─ 谈"早发现是否真获益 / 关联是否因果" → 筛查偏倚 / Hill（见 §五、§八）
```

> [!tip] 90% 的 Biostats 题不需要硬算
> 多数题考**判读 / 识别 / 选择**，不是计算。先分类到上面某一支，再调对应钥匙。

---

## 一、2×2 表 — 所有公式的根

> [!warning] 做任何题前先确认行/列方向
> 口诀**"行是测试，列是疾病"**；UW 常把方向反过来骗你。

```
                Disease (+)     Disease (−)
  Test (+)          a               b
  Test (−)          c               d
```

a = 真阳性 true positive, TP（有病测阳）/ b = 假阳性 false positive, FP（无病测阳）/ c = 假阴性 false negative, FN（有病测阴）/ d = 真阴性 true negative, TN（无病测阴）

核心公式（照原文）：

| 指标 | 公式 |
|---|---|
| Sensitivity 灵敏度 | `a / (a + c)` |
| Specificity 特异度 | `d / (b + d)` |
| PPV 阳性预测值 | `a / (a + b)` |
| NPV 阴性预测值 | `d / (c + d)` |
| Prevalence 患病率 | `(a + c) / total` |
| Accuracy 准确度 | `(a + d) / total` |
| Relative Risk (RR) | `[a/(a+b)] / [c/(c+d)]` |
| Odds Ratio (OR) | `(a × d) / (b × c)` |
| Attributable Risk (AR) | `a/(a+b) − c/(c+d)` |
| Absolute Risk Reduction (ARR) | `c/(c+d) − a/(a+b)`（对照组率 − 治疗组率）|

---

## 二、诊断检验四指标 — Sn / Sp / PPV / NPV / LR / ROC

### 2.1 核心 2 句话（必背）

> **Sensitivity = 有病阳性**（在确实有病的人里测阳的比例）
> **Specificity = 无病阴性**（在确实无病的人里测阴的比例）

### 2.2 决策口诀 + 受不受患病率影响

| 口诀 | 含义 | 用途 |
|---|---|---|
| **SnNout** | Sn 高 → **阴性**结果可**排除**疾病 | 筛查（怕漏诊 rule OUT）|
| **SpPin** | Sp 高 → **阳性**结果可**确诊** | 确诊（怕误诊 rule IN）|

| 指标 | 受 prevalence 影响？ |
|---|---|
| Sn, Sp, LR+, LR− | ❌ **不受**（检测固有属性）|
| PPV, NPV | ✅ **受**（跟患病率摇摆）|

> [!tip] 记忆
> **S 和 L 不受影响，P 和 N 受影响**。Prevalence ↑ → PPV ↑（同向）、NPV ↓（反向）。

> [!warning] 因果方向陷阱（高频）
> ❌ "因为 NPV 高所以选 Sn 高"（倒置）
> ✅ "因为怕漏诊所以选 Sn 高；恰好 NPV 也高（副产品）"

### 2.3 调阈值（cutoff）—— 别纠结升降，看阳性组变大变小

| 动作 | 阳性组 | Sn | Sp |
|---|---|---|---|
| Cutoff 调低（126→100）| 变大 | ↑ | ↓ |
| Cutoff 调高（126→130）| 变小 | ↓ | ↑ |

### 2.4 似然比 LR（不受患病率影响）

```
LR+ = Sn / (1 − Sp)   = 真阳性率 / 假阳性率   → 越大越能确诊
LR− = (1 − Sn) / Sp                          → 越小越能排除
```

| 数值 | 解读 |
|---|---|
| LR+ > 10 | 强诊断价值 → 可确诊 |
| LR+ = 1 / LR− = 1 | 检测毫无价值（做了白做）|
| LR− < 0.1 | 强阴性价值 → 可排除 |

> [!tip] 经典数字气质（看选项猜指标）
> 0.1–0.9 小数字 = LR−；5–100 = LR+；~75% / ~85% = Sn / Sp / PPV / NPV。

### 2.5 ROC 曲线 + AUC

- ROC（receiver operating characteristic，受试者工作特征曲线）：**纵轴 = Sensitivity（真阳性率 true positive rate, TPR）**，**横轴 = 1 − Specificity（假阳性率 false positive rate, FPR）**（不是 Sp 本人！）
- **最佳 cutoff = 距左上角 (0,1) 最近的点**（"瞄左上角，最近的就是答案"）
- **AUC（area under the curve，曲线下面积）** = 曲线下面积，范围 0.5–1.0，**不依赖任何 cutoff、不受患病率影响**；= 0.5 瞎猜，> 0.9 极高

> [!warning] AUC vs Accuracy 别混
> Accuracy 依赖 cutoff + 受 prevalence 影响；AUC 不依赖 cutoff + 不受 prevalence。
> **改 cutoff → Sn/Sp 跷跷板 + Accuracy 变 + AUC 不变**；**改检测本身 → ROC 曲线移动 + AUC 变**。

🧩 诊断 4 指标动态 + PPV 患病率陷阱深挖 → [[完整笔记/专题笔记/Biostats/Biostats_诊断4指标动态_PPV陷阱]]

---

## 三、风险与效应指标 — RR / OR / ARR / RRR / NNT

### 3.1 RR vs OR — 设计决定指标

| 指标 | 公式 | 适用设计 | 含义 |
|---|---|---|---|
| **RR 相对危险度** | 暴露组风险 / 非暴露组风险 | **Cohort、RCT** | 患病风险变原来几倍 |
| **OR 比值比** | `(a×d)/(b×c)` | **Case-control**、logistic 回归 | 估算关联强度 |

> [!tip] 口诀 + 罕见病例外
> **Cohort → Count risk → RR**；**Case-control → OR**（"you take the **case** to the **OR**"）。
> 疾病罕见（发病率 <10%）时，case-control 的 **OR ≈ RR**。

### 3.2 救人 vs 害人 — 6 指标镜像（治疗 vs 暴露）

| 问什么 | 救人（治疗降险）| 害人（暴露增险）|
|---|---|---|
| 绝对差（百分点）| **ARR** = Rc − Rt | **ARI / AR** = Re − Ru |
| 相对比（%）| **RRR** = ARR/Rc = 1 − RR | **RRI / ARP** = (Re−Ru)/Re |
| 需治/暴露人数 | **NNT** = 1/ARR | **NNH** = 1/ARI |

（Re=暴露组、Ru=非暴露、Rt=治疗组、Rc=对照组风险）

> [!warning] 判读硬规则
> - **NNT 算出小数 → 向上取整**（10.2 → 11）。
> - **关联强度只看 RR/OR 偏离 1.0 的程度**；P 值只代表"差异是真的"，不代表"强"。
> - **RRR 看着惊艳要查 ARR**：2%→1% 时 RRR=50% 但 ARR 仅 1%（药企爱报 RRR，医生爱报 ARR/NNT）。
> - **Case-control 不能算 RR / incidence**，只能算 OR。

### 3.3 CI 包含的"无效值"（判显著性）

| 指标类型 | 无效点 | CI 跨过它 = |
|---|---|---|
| 差值 / ARR / 均值差 mean difference, MD | **0** | 不显著 |
| RR / OR / HR（hazard ratio，风险比；比率）| **1** | 不显著 |

> 记忆：**差值看 0（拔河力气一样 → 位移 0），比率看 1（分蛋糕一样 → 比例 1:1）**。

🧩 6 指标决策树深挖 → [[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]]
🧩 OR / CI / 因果三连陷阱 → [[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]

---

## 四、研究设计 — 一句话秒认 + 可算指标

| 设计 | 一句话识别 | 报告指标 | 关键优缺点 |
|---|---|---|---|
| **Cross-sectional 横断面** | 某时点同时测暴露+疾病（"快照"）| Prevalence | 快便宜；无因果 |
| **Case-control 病例对照** | 已有病 vs 没病，**回头查暴露** | **OR** | 适合罕见病/长潜伏期；Recall bias 高 |
| **Cohort 队列（前瞻）** | 暴露 vs 不暴露，**往前追踪** | **RR、Incidence** | 可推因果、适合罕见暴露；慢贵 |
| **RCT** | 随机分组干预 | RR、ARR、NNT | 最高证据；贵、伦理限制 |
| **Crossover** | 同一人先 A 后 B，自做对照 | 同 RCT | 控个体差异；残留效应 carry-over |
| **Meta-analysis** | 汇总多个研究 | 综合 RR/OR | **↑power、缩窄 CI**；异质性、发表偏倚 |
| **Case series/report** | 几例/1 例描述 | 无 | 发现新病；无对照不能推因果 |
| **Ecological 生态学** | 单位是**人群**（群体率 vs 群体暴露，如各国糖摄入 vs 糖尿病率）| 群体层面相关 | ❌ 不能算个体 incidence；有 **ecological fallacy 生态学谬误**（群体关联 ≠ 个体）|

> [!tip] 证据等级
> Meta > RCT > Cohort > Case-control > Cross-sectional > Case series > Case report。

> [!warning] Study Design 决定术语（高频反复错点）
> - **RCT / Cohort** → 可算 RR / Risk / Incidence。
> - **Case-control** → 只能 OR，❌ 不能算 RR / Incidence。
> - **Cross-sectional** → Prevalence / POR（prevalence odds ratio，患病率比值比），❌ 不能算 RR / Incidence / "Risk"。
> - **写零假设 / 描述结果时，用 "association" 永远安全**（任何 design 都适用）。
> - 看到 **"risk / incidence"** → 必 cohort/RCT；**"OR"** → 多半 case-control；**"prevalence"** → cross-sectional。

> [!info] Case-control vs Cohort 谁更适合（不是谁更好）
> - **病罕见 / 长潜伏期 / 多 risk factor** → Case-control（去医院找病人最快）。
> - **暴露罕见 / 多个 outcome** → Cohort（找暴露人群最快）。

补充：Twin study 控基因看环境；Adoption study 控环境看遗传。Clinical Trial Phase：1=安全性(健康志愿者)、2=有效性、3=对比现行标准(关键 RCT)、4=上市后监测。Factorial RCT = ≥2 变量同时随机。

> [!warning] PP vs ITT 分析人群（处理脱落者方向相反）
> 
> | | Per-protocol（PP，符合方案）| Intention-to-treat（ITT，意向性分析）|
> |---|---|---|
> | 谁进分析 | 只留**依从+完成**者，**排除全部脱落/不依从** | **全部按随机分组保留**，不管脱落/转组 |
> | 效应估计 | 理想条件"真实效应"，但**高估**疗效 | 更**保守**，贴近真实临床"预期效应" |
> | 偏倚 | 破坏随机化 → 可能 selection bias | 保护随机化 |
> 
> 口诀：**PP = 只留乖学生（排脱落、高估）；ITT = 进门就算（全保留、保守）**。源 [[mistakes/uworld-mistakes_2026-06#^Q20458]]
> 
> ![[{7E1FFA88-108A-4246-9299-66D181F7F6C0}.png]]
> 
> 图示（每组 n=10）：PP 剔除 noncompliance/dropout（不依从/脱落）→ 分母缩小（A 3/8、B 4/7）；ITT 全保留 → A 3/10、B 4/10。

> [!tip] "比较两个地点/人群" ≠ ecological（高频陷阱）
> Ecological 关键是**只有群体汇总率、无个体数据**；若能**随访两地个体**得发病率 → 那是 **cohort**（要 incidence / RR 一律 cohort）。源 [[mistakes/uworld-mistakes_2026-06#^Q4686]]

---

## 五、偏倚 Bias — 记情境不记定义

### 5.1 选择偏倚（谁进入研究有问题）

> [!info] UWorld 把系统误差分两大类
> **选择偏倚 Selection（5 个：谁进入/留存研究有问题）** = Ascertainment / Nonresponse / Berkson / Neyman(Prevalence) / Attrition；**测量观察偏倚 Observational（4 个：怎么测出来有问题）** = Recall / Observer / Reporting / Surveillance（见 §5.2）。先判"挑人 vs 测人"再 5/4 选 1。

| Bias | Stem 钥匙 | 防范 |
|---|---|---|
| **Ascertainment（sampling 抽样偏倚）** | "convenience sample" / 单一诊所招募 / **样本 ≠ 目标人群**（撒网地方不对）| 随机抽样、确保样本代表总体 |
| **Nonresponse / Selection** | "response rate 30%" + 不应答者不同 | 随机抽样、提高应答率 |
| **Berkson** | "controls from **hospitalized** patients" | 用人群对照 |
| **Neyman (Prevalence)** | 致死病 + "long before disease assessment"（早死/早愈被漏）| 用 incidence |
| **Attrition 失访** | "X% lost to follow-up" + 失访者不同 | 高随访率 + 如实报告失访；分析用 **ITT** |

> [!success] Berkson 一句话锁定
> **B**erkson = **B**ed（住院床）—— 看到 "hospital / hospitalized controls" 闭眼选。

> [!warning] Attrition bias 深一层（失访 = selection bias 亚型）
> - **只有失访原因与结局相关时才成偏倚**（完全随机的失访不致偏）。
> - **方向双向**：哪一组选择性丢掉高危个体，关联就被**高估或低估**。
>   - 例（UWorld 高脂 vs 低脂饮食-结直肠癌题）：低脂组因**不依从严格饮食**退出、高脂组因**健康问题（肥胖 obesity / 糖尿病 diabetes / 心血管病 cardiovascular disease, CVD）**退出 → 高危的高脂个体被选择性丢失 → 脂肪-结直肠癌关联被**低估**。
> - **防范**：力争**高随访率** + **如实报告失访人数**（让读者知晓潜在 selection bias）；分析端用 **ITT（intention-to-treat 意向性分析）** 保留全部随机对象（PP 排脱落会高估，见 §四 PP vs ITT 表）。

### 5.2 测量/观察偏倚（怎么测出来有问题）

> [!tip] 一刀切口诀
> **问问题谁说谎 = Reporting；测东西谁手抖 = Observer；想不起来 = Recall；查得多 = Surveillance。**

| Bias | Stem 钥匙 | 谁有问题 |
|---|---|---|
| **Recall** | "asked to recall" + retrospective | 受访者记忆 |
| **Reporting** | "anonymous vs in-person" / 污名话题 → 故意改答案 | 受访者主动 |
| **Observer (Interviewer)** | "researcher knew group assignment" | 研究者 |
| **Surveillance (Detection)** | 暴露组 "monitored more closely" → 多检出 | 研究者监测频率 |

### 5.3 筛查特有偏倚（评估筛查项目 4 大）

1. **Selection** — 愿被筛查者本身更健康
2. **Lead-time** — 早发现 ≠ 真活更久（只是知道得早）
3. **Length-time** — 筛查抓到的多是惰性慢病
4. **Overdiagnosis** — 发现不会进展的病变 → 过度治疗

> [!warning] 高频陷阱
> "筛查后平均生存期 3 年→5 年" → **别急说筛查有效，先排 lead-time bias**；只有**疾病特异死亡率**才能判真实获益。

### 5.4 Confounding vs Effect Modification（终极对比）

| 特性 | **混杂 Confounding** | **效应修饰 Effect Modification** |
|---|---|---|
| 本质 | 第三变量产生虚假关联 | 不同亚组关联**大小不同** |
| 统计表现 | **校正前后效应显著改变** | **分层后各层效应彼此不等** |
| 处理 | **消除/控制**（随机化/匹配/分层/多元回归/限制）| **分析/描述**（分层报告，❌不要校正掉）|
| 口诀 | **总分不等，层间相等** | **层间不等，各显神通** |
| 例 | 总 RR=4.0，分层后两层都 2.0 | 总 RR=2.0，男 4.0 / 女 1.0 |

🧩 OR / CI / 因果三连陷阱（含 confounding 判读）→ [[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]

---

## 六、假设检验 — α / β / Power / p / CI

### 6.1 错误类型矩阵

```
                  实际无差异          实际有差异
检验"无差异"      ✅ 正确            ❌ Type II (β) 假阴性，漏掉真差异
检验"有差异"      ❌ Type I (α)      ✅ Power = 1 − β
                  假阳性，误认有差异
```

### 6.2 关键公式 + 判读

```
CI = (1 − α)%        → 95% CI 对应 α = 0.05
Power = 1 − β        → 通常希望 ≥ 80%（即 β ≤ 0.20）
样本量 N ↑ → 标准误 ↓ → CI 变窄 → 精度 ↑ → Power ↑（β ↓）
```

提高 Power 的办法：**①↑样本量（最有效，Meta 也走这条）** ②↑效应大小 ③↑α（代价是更易假阳性）④↓变异度。

> [!info] p 值硬核定义（别背错）
> **在 H₀ 为真的前提下，观察到当前结果或更极端结果的概率。**
> ❌ p 值 ≠ "研究犯错的概率"。

> [!warning] CI 判读硬规则
> - CI 包含无效点（差值含 0 / 比率含 1）= **无统计学意义**；CI 是否含无效值必须与 p 值显著性**绝对一致**。
> - **样本量太小** → 问缺点选 "low power / high Type II"；问改进选 "增样本量 / 做 meta-analysis"。
> - **置信水平越高（95%>90%）CI 越宽；样本量越大 CI 越窄**；Power 越大越好 vs CI 越窄越好（方向不一致）。
> - 统计显著是非黑即白；**临床显著看效应大小**（P=0.04 vs 0.06 别过度解读）。

🧩 α / β / Power 深挖 → [[完整笔记/专题笔记/Biostats/Biostats_α_β_Power]]
🧩 统计显著 vs 临床显著 → [[完整笔记/专题笔记/Biostats/Biostats_统计显著vs临床显著]]

---

## 七、统计检验选择（给场景选检验）

> [!tip] 总口诀
> **双定量选回归，双定性选卡方，自定性因定量选 t / ANOVA。**

| 自变量（组别）| 因变量（结局）| 检验 |
|---|---|---|
| 分类 2 组 | 定量（均值）| **t-test** |
| 分类 >2 组 | 定量（均值）| **ANOVA** |
| 分类 2 组 | 分类（频率）| **Chi-square 卡方** |
| 定量连续 | 定量连续 | **Correlation / 线性回归** |

特殊情况补充：

| 情况 | 检验 |
|---|---|
| 小样本分类（单元格 < 5）| **Fisher's exact** |
| 配对数据（同人前后）| **Paired t-test** |
| 等级 / 非正态相关 | **Spearman** |
| 正态连续双向相关 | **Pearson** |

> [!warning] 卡方 vs 逻辑回归
> 只问"两者是否有关联" → **卡方**（最简便，只出 p 值）；要"算 OR"或"控制混杂" → **必须逻辑回归**（出 p 值 + OR，可多变量）。
> 逻辑回归因变量 = 二分类结局，产出 OR，S 型曲线；线性回归因变量 = 连续，产出系数 β，直线。

---

## 八、Hill 因果判定 + 流行病学指标关系

### 8.1 Hill's Criteria 三大核心（CK 最常考）

1. **Temporality 时序** — 唯一"必须满足"的硬条件（因在果前）；但只有时序**不充分**证因果（"because A preceded B, A causes B" 是绝对化陷阱）。
2. **Strength 关联强度** — RR/OR 偏离 1.0 越远越强。
3. **Dose-Response 剂量-反应** — 暴露↑ → 风险**单调阶梯式**↑（不同剂量 RR 都一样 = 无剂量-反应）。

> [!warning] 因果陷阱
> **P<0.05 ≠ 因果**（只代表关联真实）；**相关 ≠ 因果**（r=0.99 也不能说谁致谁）；**cross-sectional / case-control 不能直接推因果**（只有 cohort 和 RCT 能）。

### 8.2 流行病学指标关系（必背）

```
Prevalence ≈ Incidence × Duration
  慢性病(糖尿病) → duration 长 → prevalence 高
  急性致死(狂犬病) → duration 极短 → prevalence 低
  治愈率↑ → duration 短 → prevalence ↓（≠ incidence 下降！）
```

横断面测 Prevalence；队列测 Incidence；Case-fatality rate = 病死数/病例数（疾病致死性）。

### 8.3 Crude rate vs Age-standardized rate（粗率 vs 标化率）⭐

| 概念 | 定义 | 受年龄构成影响？ | 用途 |
|---|---|---|---|
| **Crude rate（粗率，如 CMR crude mortality rate）** | 总事件 / 总人口 | ✅ **受**（年龄等人群构成混杂）| 单人群描述 |
| **Age-standardized / adjusted rate（年龄标化率，ASMR age-standardized mortality rate）** | 用**标准人口**加权各年龄别率 | ❌ **去除**年龄构成差异 | **跨人群比较** |

> [!warning] CMR 差但 ASMR 同 = 差异全由年龄结构解释（confounding by age）
> - 两地**粗率（CMR）不同**但**标化率（ASMR）相同** → 真实死亡风险无差异，差异 = **年龄构成不同**。
> - 心脏病等死亡随年龄↑ → **CMR 低的一方人群更年轻**（年轻人群粗率自然低）。
> - 类比：标化 = 把两人群"拉到同一年龄结构"再比，等同于 confounding 的**控制**（见 §5.4 / Matching）。源 [[mistakes/uworld-mistakes_2026-06#^Q108007]]

---

## 九、其余高频小点

- **集中趋势/偏态**："Median 永远在中间"；**右偏（收入）Mode<Median<Mean**；左偏反之。Mean 对 outlier 敏感，偏态优选 Median。Bimodal 双峰 = 两个不同人群。
- **正态 68/95/99.7 + percentile 换算**：±1SD=68%、±2SD(1.96)=95%、±3SD=99.7%。**percentile = 左侧累计面积**：−2 / −1 / 0 / +1 / +2 / +3 SD → **2.5 / 16 / 50 / 84 / 97.5 / 99.85**th。⚠️ "区间内%"（68/95）≠ percentile（源 [[mistakes/uworld-mistakes_2026-06#^Q20538]]：+2SD = 97.5th）。

> [!info]- 📊 68-95-99.7 正态分布图（各带 % + 双尾，对照 percentile 换算）
> ![[{D2F4BD49-76A2-4587-8563-72E4610506CE} 1.png]]
> 
> 各带由内向外：34% / 13.5% / 2.35% / 0.15%；双尾累计 ±1SD 外 16%、±2SD 外 2.5%、±3SD 外 0.15%。**percentile = 该点左侧累计**（如 +2SD：右侧 2.5% → 左侧 97.5th）。

- **相关系数 r（correlation coefficient）**：散点图（scatter plot）先判**关联类型**（线性/非线性）；线性可算 **r ∈ [−1, +1]**——**符号 = 斜率方向**（升=正 / 降=负）、**绝对值 = 线性贴合度**（越贴线 |r|→1，越散→0）。⚠️ 相关 = **粗分析**：**不控混杂、不证因果**（源 [[mistakes/uworld-mistakes_2026-06#^Q4315]]）。
- **Prevention 4 级**：Primary 防发病（疫苗/戒烟）→ Secondary 早期发现（筛查）→ Tertiary 治已病防并发症 → Quaternary 避免过度医疗。
- **Patient Safety 患者安全**：Active error（前线正发生）查 **RCA（root cause analysis 根因分析，反应性/事后）**；Latent error（系统潜伏缺陷）用 **FMEA（failure mode and effects analysis 失效模式与效应分析，主动性/事前预防）**；Near miss（未遂事件）上报（无惩罚文化）。
- **Aging 衰老生理**：脉压↑（收缩压 systolic BP, SBP↑ / 舒张压 diastolic BP, DBP↓）、快速眼动睡眠（rapid eye movement, REM）↓、残气量（residual volume, RV）↑而总肺活量（total lung capacity, TLC）不变、智商保持稳定（别轻易诊断痴呆 dementia）。

---

## 🔗 关联

- 🔁 同主题错题：
  - [[NBME11_错题本#^Q114]] 一级预防 = 改建成环境(步道)；筛查 = 二级、已病管理/手术 = 三级（误选减肥比赛）
  - [[mistakes/uworld-mistakes_2026-06#^Q21797]] PPV·NPV 行指标 vs 列指标判读
  - [[mistakes/uworld-mistakes_2026-06#^Q20561]] RRR vs ARR 半步陷阱
  - [[mistakes/uworld-mistakes_2026-06#^Q20376]] Study Design — 比较"发病风险"用 cohort（🔴 反复错）
  - [[mistakes/uworld-mistakes_2026-06#^Q4686]] Study Design — incidence 用 cohort（误选 ecological；🔴 反复错）
  - [[mistakes/uworld-mistakes_2026-06#^Q3922]] Study Design — 单样本单时点同时测 = cross-sectional（误选 case-control）
  - [[mistakes/uworld-mistakes_2026-06#^Q108443]] Case-control 对照组 = 无病 + 与暴露无关
  - [[mistakes/uworld-mistakes_2026-06#^Q108007]] Crude vs Age-standardized rate（§8.3；CMR 低 = 人群更年轻）
  - [[mistakes/uworld-mistakes_2026-06#^Q20420]] 显著性不可排名 + 只读 adjusted 列
  - [[mistakes/uworld-mistakes_2026-06#^Q20458]] PP vs ITT — per-protocol 排除全部脱落者
  - [[mistakes/uworld-mistakes_2026-06#^Q20538]] 68-95-99.7 → percentile 换算（+2SD = 97.5th）
  - [[mistakes/uworld-mistakes_2026-06#^Q3909]] p 值 ↔ CI 互译（不含 null ⟺ p<0.05）
  - [[mistakes/uworld-mistakes_2026-06#^Q106495]] 统计显著 vs 临床显著
  - [[mistakes/uworld-mistakes_2026-05#^Q20227]] OR 方向陷阱 + Case-control 不能算 risk
  - [[mistakes/uworld-mistakes_2026-05#^Q7711]] ROC 曲线 + Cutoff 跷跷板
  - [[mistakes/uworld-mistakes_2026-05#^Q12685]] Reporting bias
  - [[mistakes/uworld-mistakes_2026-05#^Q4182]] Matching 控制 Confounding
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]（分科主笔记，只读）
- 🧩 专题深挖：[[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]] / [[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]] / [[完整笔记/专题笔记/Biostats/Biostats_α_β_Power]] / [[完整笔记/专题笔记/Biostats/Biostats_统计显著vs临床显著]] / [[完整笔记/专题笔记/Biostats/Biostats_诊断4指标动态_PPV陷阱]]
- 🏥 跨学科：
  - [[完整笔记/Peixuan分科笔记/Ethics_Master]]（研究伦理 / 知情同意 / 机构审查委员会 institutional review board, IRB —— 任何 Clinical Trial Phase 前都需 IRB 批准）
  - [[完整笔记/Peixuan分科笔记/newborn care and screening]]（筛查原则：Sn 高优先、lead/length-time bias 评估）
  - 各临床科筛查指南（乳腺/宫颈/结直肠癌筛查 = Secondary prevention，套用敏感度优先 + 偏倚校正）
- 🌱 TODO（待生成衍生）：
  - 攒够"统计检验选择"错题后 → 拆 `Biostats_统计检验选择决策树`（t/ANOVA/卡方/Fisher/回归）
  - 攒够"研究设计识别"错题后 → 拆 `Biostats_研究设计秒认与可算指标`
  - 攒够"5 大 bias 鉴别"错题后 → 拆 `Biostats_偏倚情境鉴别速查`

## ✅ 复盘行动

- [ ] 默写 2×2 四指标公式（Sn/Sp/PPV/NPV）+ "S/L 不受患病率、P/N 受影响"
- [ ] 默写 6 效应指标镜像表（救人 ARR/RRR/NNT vs 害人 ARI/RRI/NNH）+ NNT=1/ARR 向上取整
- [ ] 默写"研究设计 → 可算指标"（RCT/cohort=RR；case-control=OR；cross-sec=prevalence）
- [ ] 默写 5 大 bias 钥匙（Berkson 住院对照 / Recall 记不起 / Reporting 故意改 / lead-time 早发现 / Neyman 早死漏）
- [ ] 默写 Confounding（总分不等层间相等，要控制）vs Effect modification（层间不等，要分层报告）
- [ ] 默写 α/β/Power/CI 关系 + "CI 含无效点（差值 0/比率 1）= 不显著"
- [ ] 默写统计检验选择口诀（双定量回归 / 双定性卡方 / 自定性因定量 t-ANOVA；<5 用 Fisher、配对用 paired）

---

## 版本记录

- **v1**（2026-06-12）：通读分科笔记 [[完整笔记/Peixuan分科笔记/Biostats_Master]] 全 1114 行提炼建卡。覆盖 一题流总决策树、2×2 表与公式、诊断 4 指标（Sn/Sp/PPV/NPV/LR/ROC/AUC + 患病率关系 + cutoff）、风险效应指标（RR/OR/ARR/RRR/NNT/NNH + CI 无效值）、研究设计（7 类秒认 + 可算指标 + 决定术语）、偏倚（选择/测量/筛查 5 大鉴别 + Confounding vs Effect modification）、假设检验（α/β/Power/p/CI 判读）、统计检验选择、Hill 因果 + 流行病学指标关系、统计描述/Prevention/Patient Safety/Aging 小点。深挖主题 🧩 双链至 5 个已有 Biostats 专题笔记，本卡作总索引/决策骨架不重复展开。
