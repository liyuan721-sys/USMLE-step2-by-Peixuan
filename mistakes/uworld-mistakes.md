# UWorld 错题整理

## 2026-05-10

### Hill's criteria:看到剂量分层 + RR 单调递增 = 选 dose-response

#biostats #causality #dose-response 🟡

- **来源**:UW Q20787
- **题干要点**:RCT 比较运动 vs 标准护理对糖尿病停药率影响,运动组按剂量分 T1/T2/T3 三组,RR 随剂量从 12.1→25.2→38.9 单调递增
- **正确答案**:B — 更大运动量与更高停药率显著相关(= biological gradient / dose-response)
- **我选了**:B(做对但 Mark)— 纠结点:B vs D
- **关键 buzzword / 识别公式**:
  - "**剂量分层 + 结果单调** → dose-response" 
  - "**additional support**" → 排除已在题干主结果里的信息(D 是 RCT 主结果,不算 additional)
  - **Hill's 三大金刚**:dose-response / temporality / strength of association
- **关联笔记**:[[Biostats_Master#Causality / Hill's criteria]]
- **重做次数**:☐ 1st
- **状态**:🟡 不熟(Mark)

**干扰项分析**:
- A. "Bias completely eliminated" — 错。"completely" 是 USMLE 经典绝对化陷阱,RCT 也不可能完全消除 bias
- C. 12 个月随访时长 — 错。follow-up 时长是研究设计要素,但**不是 Hill's criteria**
- D. RCT 主结果(intensive vs standard 有显著关联)— 错。这是题干已给的信息,不是 "additional" 支持

### OR 方向陷阱 + case-control 不能算 risk

#biostats #odds-ratio #case-control #方向陷阱 🔴

- **来源**: UW Q20227
- **题干要点**: Case-control 研究,Black vs Non-Hispanic White 女性的 pregnancy-related death,未调整 OR = 3.07 (95% CI 2.78-4.20),调整后 OR = 2.65 (95% CI 2.12-3.45) 仍显著
- **正确答案**: B — 调整后关联仍显著,提示有**未被研究纳入的外部因素**(如结构性歧视)在起作用
- **我选了**: D — 错因:**方向陷阱 + risk/odds 混淆**(双重陷阱)
- **关键 buzzword / 识别公式**:
  - **OR > 1 → 暴露组 odds 高于 reference 组**(谁是暴露谁是 reference,看题干"X compared to Y" — X 是暴露)
  - **Case-control 只能算 OR,不能算 risk/RR**(因为不是从暴露追到结局,是从结局倒推暴露)
  - "**adjusted OR 仍显著**" → 残留关联 → 暗示有**未测量的混杂**(unmeasured confounders / external factors)
- **关联笔记**: [[Biostats_Master#Odds Ratio]] / [[Biostats_Master#Study Design - Case-Control]]
- **重做次数**: ☐ 1st
- **状态**: 🔴 反复错

**干扰项分析**:
- A. "primarily due to poverty / low prenatal care" — 错。这些因素已经在 adjusted model 里 controlled 了,关联仍显著说明这些**不是主因** 
- C. "case-control design 不能得出 statistically significant conclusions" — 错。case-control **可以**做 OR + CI,这是其核心用途(尤其对罕见结局)
- **D. "NHW 是 Black 的 3 倍"** — 错。**方向反了**。题干 "Black compared to NHW" 意思是 Black 是暴露组,OR 3.07 = Black 的 odds 是 NHW 的 3 倍。USMLE 经典反向陷阱
- E. "调整 contraception use → advanced maternal age contributes" — 错。研究**没有**调整 contraception use,而且 maternal age >35 的 p = 0.12 不显著

**⚠️ CK 高频陷阱**:
1. **OR 方向永远看"X compared to Y" — X 是暴露,Y 是 reference**
2. **Case-control 永远算 OR,不算 RR/risk**(选项里说 "risk" 还涉及 case-control → 警惕)
3. **Adjusted OR 仍显著 → 有 unmeasured confounders**(经典考点,常考"种族健康差异"vignette)

## 2026-05-11

### ARP vs RR/ARI/NNH:"attributed to" + 两组 risk = (Re−Ru)/Re,分母是暴露组

#biostats #ARP #relative-risk 🔴

- **来源**:UW Q20430
- **题干要点**:HIV(+) 产妇 RCT 母乳 vs 配方奶,24mo 母亲死亡率 11.2% vs 3.5% (p=0.02),问母乳组中**归因于母乳**的死亡占百分之几
- **正确答案**:E — 68.8% (ARP = (0.112−0.035)/0.112 × 100 ≈ 68.75%)
- **我选了**:B — 3.5%(把 unexposed risk 当成"non-attributable %",分母搞反)
- **关键 buzzword / 识别公式**:
  - **"attributed to (exposure)" + 给了两组 risk → ARP**
  - **ARP = (Re−Ru)/Re = (RR−1)/RR**,分母永远是 **exposed 组**
  - "母乳组里多少死亡是母乳害的"→ 自然除以**母乳组**总死亡
- **一家人速查**(Re=0.112, Ru=0.035):
  - RR = Re/Ru = **3.2 倍**(单位:倍数)
  - ARI = Re−Ru = **7.7%**(单位:比例差)
  - ARP = (Re−Ru)/Re = **68.75%**(单位:百分比)← 本题答案
  - NNH = 1/ARI ≈ **13 人**(单位:人数,不是%)
- **关联笔记**:[[完整笔记/Biostats_Master#RR / RRR / ARR 互补关系深度推导]] / [[notes/Biostats_Epi]]
- **重做次数**:☐ 1st
- **状态**:🔴 概念混淆(分母方向)

**干扰项分析**:
- A. **3.2** — RR(倍数,不是百分比)。陷阱:题问 "percentage",3.2 连百分号都没有
- B. **3.5**(选的)— Risk_unexposed。**核心思路错位**:想成"3.5% 是本来就会死的(不归因)"→ 但题问的是"归因%",不是"不归因%";且 Risk_unexposed 的分母是配方奶组**总人数**,而 "non-attributable %" 的分母应该是母乳组**死亡人数**,两者分母不同
- C. **11.2** — Risk_exposed。是 ARP 公式的**分母**,不是答案
- D. **13.0** — NNH(人数,不是%)。看到带小数的两位数 → 警惕单位陷阱

**⚠️ CK 高频陷阱**:
1. **"attributed to" + 两组 risk → 9 成是 ARP**;分母是 exposed 组
2. **NNH/NNT 单位是人数**,不是 %;选项给你 "13" 不带%号就要警惕
3. **题外**:HIV(+) 产妇喂养——**资源充足国家 → 配方奶**,**资源匮乏国家 → 母乳**(水源污染/感染风险 > 母乳传播风险)

> [!example]- Biostats / ARR 反推样本量 (Q20057)
> 
> ## 一句话识别
> 给 ARR + 给一组发病人数 + 问样本量 n → **必须先算 Rt，再 n = 病例数 / Rt**
> 
> ## 核心思路（2 步）
> Step 1: 用 ARR 反推 Rt
>    Rt = Rc − ARR = 0.16 − 0.10 = **0.06**
> Step 2: 用 Rt 反推 n
>    n = 病例数 / Rt = 12 / 0.06 = **200** ✅
> 
> ## 反推公式速查
> 
> | 已知 | 求 | 公式 |
> |------|-----|------|
> | ARR + Rc | Rt | Rt = Rc − ARR |
> | Rt + 发病数 | n | n = 发病数 / Rt |
> | NNT | ARR | ARR = 1/NNT |
> | RR + Rc | Rt | Rt = RR × Rc |
> 
> ## 我为什么错
> 选了 C. 160 = **跳过"先算 Rt"这关键一步**，用了错误的比例当分母
> **核心陷阱**：反推 n 必须用**那一组自己的 Risk**（不是 ARR，不是另一组的 Rc）
> 
> ## 记忆挂钩
> **"桶装水"**：水 ÷ 水位 = 桶大小
> - 桶 = n（要求的样本量）
> - 水 = 发病数（题目给的 12）
> - 水位 = 那一组的 Risk（必须先算出 Rt，不是直接给的）
> 
> ## Stem 模式速诊
> 
> | 关键词组合 | 考点 |
> |-----------|------|
> | "given ARR" + "数 of patients with X" + 问 n in [某组] | 反推 n |
> | "given NNT" → 问 ARR | NNT 反推 |
> | "given RR" + "Rc" → 问 Rt | RR 反推 |
> | "given OR + odds" → 反推 prevalence | OR 反推 |
> 
> ## 关联
> - [[完整笔记/Biostats_Master#反推公式]]
> - [[完整笔记/_衍生_高频评分_公式#流行病学反推]]
> - [[mistakes/uworld-mistakes]] 搜 Q20430（上一道 ARP）
> 
> ## 跨科考点（OB / 手术）
> - 剖宫产术后切口感染预防 = **Cephalexin** 口服
> - 加 metronidazole = 覆盖厌氧菌
> - 适应症：**肥胖产妇**（感染高风险）
> 
> ## 复盘
> - [ ] 1 周后重做这题
> - [ ] 默写"桶装水"反推思路
> - [ ] 加 #薄弱点 到 [[完整笔记/Biostats_Master]]
> - [ ] 找 3 道反推题练习
> - [ ] 加 #考前必看

> [!example]- [2026-05-11] Biostats / LR+ 阳性似然比 (Q107214)
> 
> ## 一句话识别
> 给 2×2 表 + 问 LR+ → **LR+ = 有病阳性率 / 无病阳性率 = Sens / (1−Spec)**
> 
> ## 核心公式（按意义算）
> - LR+ = (有病阳性) / (无病阳性) = Sens / (1−Spec)
> - LR− = (有病阴性) / (无病阴性) = (1−Sens) / Spec
> 
> 本题：
> - Sens = 375/500 = 0.75
> - Spec = 680/800 = 0.85; 1−Spec = 0.15
> - LR+ = 0.75/0.15 = **5** ✅
> - LR− = 0.25/0.85 = 0.29
> 
> ## 🤔 我的提问 / 卡点（学习路径）⭐
> 
> 1. **"LR 跟敏感性特异性我联系不上，但我能算 LR"**
>    → 顿悟：LR 公式和直观语言是"翻译"关系
>    → "Sens = 有病阳性" 这 2 句话是地基
> 
> 2. **"我知道了，Sens = 有病阳性，Spec = 无病阴性"**
>    → 这就是我的**核心记忆挂钩** ⭐
>    → 剩下 4 个格子全靠"1 减"推出
> 
> ## 核心 2 句话（我的顿悟）⭐
> **Sens = 有病阳性**
> **Spec = 无病阴性**
> 剩下全靠"1 减"：1−Sens = 有病阴性；1−Spec = 无病阳性
> 
> ## 4 大分母法则
> 
> | 分母 | 指标 |
> |------|------|
> | 有病组 | Sens |
> | 无病组 | Spec |
> | 阳性组 | PPV |
> | 阴性组 | NPV |
> 
> ## 我为什么错
> 选了 C. 15 = 瞎凑数字
> **核心陷阱**：把 LR− (0.29) 和 LR+ (5) 配对当干扰项；不熟悉 LR+ 公式
> 
> ## 记忆挂钩
> "LR+ 看阳性那行，两组比值相除"
> "LR− 看阴性那行，两组比值相除"
> 
> ## 受 prevalence 影响吗？
> - Sens, Spec, LR+, LR− → ❌ 不受
> - PPV, NPV → ✅ 受
> 
> ## 同类题验证（自己做对了 ✅）
> 同样数据问 LR− → 0.25/0.85 = 0.29 ✅
> 
> ## 关联
> - [[完整笔记/Biostats_Master#诊断试验]]
> - [[完整笔记/Biostats_Master#LR]]
> - [[notes/Biostats_Epi]]
> 
> ## 复盘
> - [ ] 1 周后重做
> - [ ] 默写"Sens = 有病阳性；Spec = 无病阴性"
> - [ ] 加 #薄弱点 #考前必看 到 [[Biostats_Master#诊断试验]]

> [!example]- [2026-05-11] Biostats / ROC 曲线 + Cutoff 跷跷板 (Q7711)
> 
> ## 一句话识别
> **问 1**：ROC 上移 + sens 数据 46%→70% → **aspirin 增加 sensitivity**
> **问 2**：Cutoff 1→4 μg/g（升高）→ **假阳性 ↓**（跷跷板规则）
> 
> ## 🤔 我的提问 / 卡点（学习路径）⭐
> 
> 1. **"我不明白这题的意思，两问全选错了"**
>    → 顿悟：题目信息量大时要**先简化故事**
>    → aspirin 让 ROC 上移 = sens ↑（46→70%）
> 
> 2. **"哪里看到的 46%, 70%, 82%, 79% 这些数字"**
>    → 重要追问 ⭐ — 数字不在 ROC 图本身，而在右侧解释文字
>    → 学到：**主动验证数据来源**比被动接受重要
> 
> 3. **"ROC 曲线下面积 = accuracy?"**
>    → 精确区分：AUC ≈ accuracy 但不完全等同
>    → AUC = 检测**整体能力**（不依赖 cutoff）
>    → Accuracy = 特定 cutoff 下的表现（依赖 cutoff + prevalence）
> 
> ## 核心规则：Cutoff "跷跷板"⭐
> 
> | 指标 | Cutoff ↑（严）| Cutoff ↓（宽）|
> |------|--------------|--------------|
> | 真阳性 TP | ↓ | ↑ |
> | 假阴性 FN | ↑ | ↓ |
> | 真阴性 TN | ↑ | ↓ |
> | **假阳性 FP** | **↓** ⭐ | ↑ |
> | Sensitivity | ↓ | ↑ |
> | Specificity | ↑ | ↓ |
> | AUC | **不变** ⭐ | **不变** |
> 
> ## ROC 曲线移动方向
> - 上移 → Sens ↑
> - 左移 → Spec ↑
> - 左上角 = 完美检测
> - 整体上移 → AUC ↑ → accuracy ↑
> 
> ## AUC vs Accuracy（我的提问引出）
> - **AUC**：检测整体能力（跨所有 cutoff，不依赖 cutoff，不受 prevalence 影响）
> - **Accuracy**：特定 cutoff 下"测对的比例"（依赖 cutoff，受 prevalence 影响）
> - Cutoff 改变 → Accuracy 变 + **AUC 不变** ⭐
> - 检测本身改进（如加 aspirin）→ ROC 曲线移 + AUC 变 + Accuracy 变
> 
> ## 本题数据（来自 stem 文字 + 子图标注）
> 
> | 状态 | Sens | Spec |
> |------|------|------|
> | 不用 aspirin (cutoff=1) | 46% | 82% |
> | 用 aspirin (cutoff=1) | **70%** | **79%** |
> | 用 aspirin (cutoff=4) | **60%** | **90%** |
> 
> 数字来源：第一张图右侧文字 + 第二张图子图标注 + 第三张图解释
> 
> ## 本题机制（aspirin 为何 sens↑）
> Aspirin → 抑制血小板 → 肠道病灶更易出血 → iFOBT 更易测阳 → **Sens ↑**
> 
> ## 我为什么错
> - 问 1 选 B（降低 sens）= 把 "aspirin 副作用" 误解为"干扰检测"
> - 问 2 选 C（真阳性 ↑）= 混淆"真阳性人数 (TP)" vs "真阳性率 (PPV)"
> **核心陷阱**：cutoff ↑ → 阳性数全面 ↓（TP 和 FP 都 ↓，不是质量 ↑）
> 
> ## 记忆挂钩
> **"老师改考卷"**：及格线提高 → 及格人数减少 + 及格者质量更高
> - cutoff ↑ = 标准变严 = 阳性数 ↓
> - Sens ↓（漏诊 ↑）+ Spec ↑（误诊 ↓）
> 
> ## 应用场景
> - **筛查**（怕漏诊）→ 低 cutoff → Sens↑
> - **确诊**（怕误诊）→ 高 cutoff → Spec↑
> 
> ## 关联
> - [[完整笔记/Biostats_Master#ROC]]
> - [[完整笔记/Biostats_Master#Cutoff]]
> - [[完整笔记/Biostats_Master#AUC]]
> - [[完整笔记/_衍生_高频陷阱#ROC]]
> 
> ## 复盘
> - [ ] 1 周后重做
> - [ ] 默写"跷跷板"完整表（含 AUC 不变 ⭐）
> - [ ] 画 ROC 曲线 + 标关键点（左上角/对角线/AUC）
> - [ ] 默写 AUC vs Accuracy 区别
> - [ ] 加 #薄弱点 #难记 #考前必看 到 [[Biostats_Master#ROC]]

> [!example]- [2026-05-11] Biostats / Matching 控制 Confounding (Q4182)
> 
> ## 一句话识别
> Case-control + 邻居匹配 + 控制 age/race → **匹配是为了控制 Confounding** ✅
> 
> ## 🤔 我的提问 / 卡点（学习路径）⭐
> 
> 1. 选了 **B. Recall bias**
>    → 看到 "case-control + interviewed" 条件反射想 recall bias
>    → 没看清题目问"匹配能解决什么"，而不是"这种 study 有什么 bias"
> 
> 2. **顿悟**：题目问的"角度"比 bias 类型本身更关键
>    → 匹配是"专药"，只治 confounding
> 
> ## 核心规则
> **Matching（匹配）= 控制 Confounding 的专药**
> - 让 case 和 control 在某变量上一致（如 age, race）
> - 消除该变量作为 confounder 的可能
> - 不能解决其他类型的 bias
> 
> ## 8 大偏倚速查 ⭐
> 
> | 偏倚 | 控制方法 |
> |------|----------|
> | Selection bias | Random sampling |
> | **Recall bias** | Medical records（不靠 interview）|
> | Observer bias | **Blinding**（盲法）|
> | Ascertainment bias | Standardized criteria |
> | **Confounding** | **Matching/Stratification/Regression/Randomization/Restriction** ⭐ |
> | Lead-time bias | Compare mortality（不比生存期）|
> | Length bias | Compare mortality |
> | Hawthorne effect | Blinding |
> 
> ## 控制 Confounding 5 大方法
> | 方法 | 阶段 |
> |------|------|
> | Randomization | 设计阶段（金标准）|
> | Restriction | 设计阶段 |
> | **Matching** ⭐ | 设计阶段 |
> | Stratification | 分析阶段 |
> | Multivariate regression | 分析阶段 |
> 
> ## 我为什么错
> 选了 B. Recall bias = 看到 "case-control + interviewed" 条件反射想 recall bias
> **核心陷阱**：混淆"case-control **的固有问题**（recall bias）"和"**匹配能解决什么**（confounding）"
> 题目问的是"匹配能控制什么"，不是"这种 study 有什么问题"
> 
> ## 记忆挂钩
> **"约会配对"**：matching = 强制配同龄同种族
> → 消除"基础特征差异"（confounding）
> → 但不能消除"双方回忆问题"（recall bias）或"选样本偏差"（selection bias）
> 
> **看到 stem 关键词反应**：
> - "matched on age/race" → 立刻想"控制 confounding"
> - "interviewed patients" → 想"可能 recall bias"
> - "researcher knew group" → 想"observer bias / 需要盲法"
> 
> ## Confounding vs Effect Modification（高频区分）
> | | Confounding | Effect Modification |
> |---|-------------|---------------------|
> | 是什么 | 假关联 | 真的不同效应 |
> | 处理 | **消除**（控制）| **报告**（分层）|
> 
> ## 关联
> - [[完整笔记/Biostats_Master#Bias]]
> - [[完整笔记/Biostats_Master#Confounding]]
> - [[完整笔记/Biostats_Master#Study Design]]
> - [[完整笔记/_衍生_高频陷阱#Biostats偏倚]]
> 
> ## 复盘
> - [ ] 1 周后重做
> - [ ] 默写 8 大偏倚 + 控制方法
> - [ ] 默写"5 大控制 Confounding 方法"
> - [ ] 区分 Confounding vs Effect Modification
> - [ ] 加 #薄弱点 #难记 #考前必看 到 [[Biostats_Master#Bias]]
