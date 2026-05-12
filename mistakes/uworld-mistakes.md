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

> [!example]- [2026-05-11] Biostats / ARP 阳性归因比 (Q20430)
> 
> ## 一句话识别
> ARP vs RR/ARI/NNH:"attributed to" + 两组 risk = (Re−Ru)/Re,分母是暴露组
> 
> #biostats #ARP #relative-risk 🔴
> 
> - **来源**:UW Q20430
> - **题干要点**:HIV(+) 产妇 RCT 母乳 vs 配方奶,24mo 母亲死亡率 11.2% vs 3.5% (p=0.02),问母乳组中**归因于母乳**的死亡占百分之几
> - **正确答案**:E — 68.8% (ARP = (0.112−0.035)/0.112 × 100 ≈ 68.75%)
> - **我选了**:B — 3.5%(把 unexposed risk 当成"non-attributable %",分母搞反)
> - **关键 buzzword / 识别公式**:
>   - **"attributed to (exposure)" + 给了两组 risk → ARP**
>   - **ARP = (Re−Ru)/Re = (RR−1)/RR**,分母永远是 **exposed 组**
>   - "母乳组里多少死亡是母乳害的"→ 自然除以**母乳组**总死亡
> - **一家人速查**(Re=0.112, Ru=0.035):
>   - RR = Re/Ru = **3.2 倍**(单位:倍数)
>   - ARI = Re−Ru = **7.7%**(单位:比例差)
>   - ARP = (Re−Ru)/Re = **68.75%**(单位:百分比)← 本题答案
>   - NNH = 1/ARI ≈ **13 人**(单位:人数,不是%)
> - **关联笔记**:[[完整笔记/Peixuan分科笔记/Biostats_Master#RR / RRR / ARR 互补关系深度推导]] / [[notes/Biostats_Epi]]
> - **重做次数**:☐ 1st
> - **状态**:🔴 概念混淆(分母方向)
> 
> **干扰项分析**:
> - A. **3.2** — RR(倍数,不是百分比)。陷阱:题问 "percentage",3.2 连百分号都没有
> - B. **3.5**(选的)— Risk_unexposed。**核心思路错位**:想成"3.5% 是本来就会死的(不归因)"→ 但题问的是"归因%",不是"不归因%";且 Risk_unexposed 的分母是配方奶组**总人数**,而 "non-attributable %" 的分母应该是母乳组**死亡人数**,两者分母不同
> - C. **11.2** — Risk_exposed。是 ARP 公式的**分母**,不是答案
> - D. **13.0** — NNH(人数,不是%)。看到带小数的两位数 → 警惕单位陷阱
> 
> **⚠️ CK 高频陷阱**:
> 1. **"attributed to" + 两组 risk → 9 成是 ARP**;分母是 exposed 组
> 2. **NNH/NNT 单位是人数**,不是 %;选项给你 "13" 不带%号就要警惕
> 3. **题外**:HIV(+) 产妇喂养——**资源充足国家 → 配方奶**,**资源匮乏国家 → 母乳**(水源污染/感染风险 > 母乳传播风险)

> [!example]- [2026-05-11] Biostats / ARR 反推样本量 (Q20057)
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
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#反推公式]]
> - [[完整笔记/专题笔记/_衍生_高频评分_公式#流行病学反推]]
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
> - [ ] 加 #薄弱点 到 [[完整笔记/Peixuan分科笔记/Biostats_Master]]
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
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#诊断试验]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#LR]]
> - [[notes/Biostats_Epi]]
> 
> ## 复盘
> - [ ] 1 周后重做
> - [ ] 默写"Sens = 有病阳性；Spec = 无病阴性"
> - [ ] 加 #薄弱点 #考前必看 到 [[完整笔记/Peixuan分科笔记/Biostats_Master#诊断试验]]

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
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#ROC]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Cutoff]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#AUC]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#ROC]]
> 
> ## 复盘
> - [ ] 1 周后重做
> - [ ] 默写"跷跷板"完整表（含 AUC 不变 ⭐）
> - [ ] 画 ROC 曲线 + 标关键点（左上角/对角线/AUC）
> - [ ] 默写 AUC vs Accuracy 区别
> - [ ] 加 #薄弱点 #难记 #考前必看 到 [[完整笔记/Peixuan分科笔记/Biostats_Master#ROC]]

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
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Bias]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Confounding]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Study Design]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#Biostats偏倚]]
> 
> ## 复盘
> - [ ] 1 周后重做
> - [ ] 默写 8 大偏倚 + 控制方法
> - [ ] 默写"5 大控制 Confounding 方法"
> - [ ] 区分 Confounding vs Effect Modification
> - [ ] 加 #薄弱点 #难记 #考前必看 到 [[完整笔记/Peixuan分科笔记/Biostats_Master#Bias]]

> [!example]- [2026-05-11] Biostats / PPV NPV vs Prevalence (Q21656)
> 
> ## 一句话识别
> 同一检测两组 NPV 不同 → **必定是 prevalence 不同**
> NPV ↑ → Prevalence ↓ → 无病人比例 ↑
> 
> ## 核心规则
> **PP 同向，NP 反向**
> - Prevalence ↑ → PPV ↑（正相关）
> - Prevalence ↑ → NPV ↓（负相关）
> 
> ## Prevalence 影响表
> 
> | 指标 | 受 prevalence 影响 |
> |------|------------------|
> | Sens, Spec, LR+, LR− | ❌ 不受 |
> | **PPV, NPV** | **✅ 受** |
> | Accuracy | ✅ 受 |
> 
> 口诀：**S 和 L 不受，P 和 N 受**
> 
> ## 我为什么错
> 选了"prevalence A > B" = **方向搞反**
> NPV 高在 A → A 组无病人多 → prevalence **低**（不是高）
> **核心陷阱**：NPV 与 prevalence **负相关**，不是正相关
> 
> ## 语言陷阱
> "Prevalence 低" ≡ "无病人比例高"（同一件事，包装不同）
> 
> ## 记忆挂钩
> **"海里捞鱼"**：
> - 鱼少（低 prevalence）→ 说没鱼基本真没鱼 → NPV ↑
> - 鱼多（高 prevalence）→ 捞到多半是鱼 → PPV ↑
> 
> ## 筛查 vs 确诊（USMLE 核心）⭐
> 
> **正确因果链**（注意方向不要倒置）：
> 
> | 阶段 | 筛查 | 确诊 |
> |------|------|------|
> | 临床目的 | 怕漏诊 (rule OUT) | 怕误诊 (rule IN) |
> | **设计选择** | **Sens 高** | **Spec 高** |
> | 应用人群 | 普通人群 | 有症状人群 |
> | 人群 Prevalence | 低 | 高 |
> | 应用结果 | NPV 高 | PPV 高 |
> 
> **必背口诀**：
> - **SnNout**: Sens 高 → 阴性 rules **N**egatives **out**
> - **SpPin**: Spec 高 → 阳性 rules **P**ositives **in**
> 
> **关键认知**：
> - ❌ 错误：选 sens 高是因为 NPV 高
> - ✅ 正确：选 sens 高是因为**怕漏诊**，NPV 高是副产品
> 
> ## Stem 模式速诊
> 
> | 关键词 | 反应 |
> |--------|------|
> | 同一检测 + 两组 PPV/NPV 不同 | Prevalence 不同 |
> | NPV 高 | 该组 prevalence 低 |
> | PPV 高 | 该组 prevalence 高 |
> | "screening" | Sens 高 + NPV 高 |
> | "diagnosis/confirm" | Spec 高 + PPV 高 |
> 
> ## 关联
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#PPV NPV]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#筛查 vs 确诊]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#PPV NPV 方向]]
> 
> ## 复盘
> - [ ] 1 周后重做
> - [ ] 默写"PP 同向，NP 反向"
> - [ ] 默写"SnNout / SpPin"
> - [ ] 区分"选 sens/spec 高的原因 ≠ 因为 NPV/PPV 高"
> - [ ] 加 #薄弱点 #难记 #考前必看 到 [[完整笔记/Peixuan分科笔记/Biostats_Master#PPV NPV]]

> [!example]- [2026-05-11] Biostats / HR 解读 (Q7688)
>
> ## 🎯 Stem 模式
> "Which factor **most significantly increases risk**" + **HR 表格** → 找**最大的 HR（>1 且 CI 不跨 1）**
>
> ## 🔑 核心概念
> **Hazard Ratio (HR, 风险比)** = 含**时间维度**的事件率比值
> - 分母 = **person-years**（不是人数）→ "**per 100 patient-years**" 是 HR 的语言
> - 来自 **Cox proportional hazards model**，配套 **Kaplan-Meier 曲线** + **Log-rank test**
> - **= 1 无效 / > 1 危险 / < 1 保护 / CI 跨 1 不显著（一票否决）**
>
> ## 📊 通用 HR/RR/OR 表格题 SOP（必背）
> ```
> Step 1: 这是什么指标？(HR/RR/OR → 决定 =1/>1/<1 含义)
> Step 2: 题目问 max 还是 min？("increase"→最大>1; "protective"→最小<1)
> Step 3: 看 CI 是否跨 1（跨 1 = 不显著 = 一票否决，无论点估计多大）
> Step 4: 把选项映射到表的对应行
> ```
>
> ## 🆚 HR vs RR vs OR
> | 指标 | 分母 | 含时间？ | 适用研究 | 配套 |
> |---|---|---|---|---|
> | **HR** | person-years | ✅ 是 | RCT/Cohort + 随访不等长 / 关心 time-to-event | Cox + KM 曲线 |
> | **RR** | persons | ❌ 否 | RCT / Cohort | 2×2 表 |
> | **OR** | odds | ❌ 否 | Case-control | 2×2 表 |
>
> ## 💊 利尿剂对 K+ 影响（本题关键医学知识）
> | 类别 | 对 K+ | 机制 |
> |---|---|---|
> | **Thiazide / Loop** | ⬇️ **降钾** | 远端 Na+ 增加 → K+ 排泄↑ |
> | **K+-sparing**（spironolactone, amiloride）| ⬆️ 升钾 | 拮抗醛固酮 / 阻 ENaC |
> | **ACE-I / ARB** | ⬆️ 升钾 | ↓ 醛固酮 |
>
> → ACE-I 患者**加 thiazide = 保护性对冲**（HR < 1）
>
> ## ❌ 我为什么错
> - **选了 B（加 thiazide）**
> - **错因**：① 不知道 HR 概念 → 不会读表 ② 以为"加药=危险"，没看 HR 方向 ③ 不知道 thiazide 是**降钾药**
> - **核心陷阱**：**HR 方向陷阱** — 看到"add a drug"凭直觉选"危险"，没去查 HR 数值方向；同时混淆 thiazide 电解质效应
>
> ## ⚠️ 表格题三大坑（普适）
> 1. **方向坑**：HR<1 是保护，不是危险
> 2. **CI 坑**：HR 看似>1 但 CI 跨 1 = 不显著
> 3. **直觉坑**：凭印象（"加药=危险"）而不是看数据
>
> ## 🎴 Memory Hook
> - **"HR 找最大，跨 1 不算数"**
> - **"Thi-azide 把 K 踢出去"** → thiazide 降钾
> - HR 几何想象：=1 地平线 / >1 山峰 / <1 山谷 / CI 跨 1 = 桥跨过地平线（不显著）
>
> ## 🤔 我的提问 / 卡点
> - **Q：HR 的时间维度怎么体现？**
>   → 学到：HR 分母是 **person-years**（不是人数）；来自 Cox 模型；图里 "per 100 patient-years" 就是时间体现；适合**随访不等长**或**关心 time-to-event** 的研究
> - **元层面诊断**：两题都是"不知道概念 + 不会看表" → 需要建立**看表 SOP**（4 步法）
>
> ## 🔗 关联
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Hazard Ratio]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#RR vs OR vs HR]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Confidence Interval 跨 1]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#HR 方向陷阱]]
> - [[完整笔记/Peixuan分科笔记/肾脏#Hyperkalemia 鉴别]]
> - [[完整笔记/专题笔记/_衍生_高频评分_公式#利尿剂电解质效应对比]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 + 默写 HR/RR/OR 对比表
> - [ ] 默写**4 类利尿剂对 K+ 的影响**
> - [ ] 默写**Thiazide 五大副作用**（"3 Hypo + 3 Hyper"）
> - [ ] 给 [[完整笔记/Peixuan分科笔记/Biostats_Master]] 加 #薄弱点（HR 部分）
> - [ ] 整理"看表 SOP（4 步法）"到 [[完整笔记/专题笔记/_衍生_高频评分_公式]]
> - [ ] 找 3 道 HR 题练习（重点：CI 跨 1 判断）

> [!example]- [2026-05-11] Biostats / Study Design Factorial 识别 (Q7688-Item2)
>
> ## 🎯 Stem 模式
> Stem 出现 **"randomized to ... AND TO ..."** 句式 → **≥2 个独立变量同时随机化** → **Factorial design**
>
> "AND TO" 是 Factorial 的**金标准指纹**
>
> ## 🔑 核心概念
> **Factorial design (析因设计)** = 同一 RCT 中**同时随机化 ≥2 个独立干预变量**，一次试验回答多个问题（主效应 + 交互效应）
> - 2 变量 × 各 N 水平 → N×N 网格（如 3 药 × 2 BP 目标 = 6 组）
> - 优势：一次测多个干预；劣势：复杂、可能交互
>
> ## 📐 Study Design 识别 SOP（必背）
> ```
> Step 1: 有 "randomized" 吗？
>   ✅ 有 → RCT 家族（4 选 1）
>   ❌ 没 → 观察性（cohort/case-ctrl/cross-sec）
>
> Step 2 (RCT)：数有几个独立变量同时随机化？
>   1 个 → Parallel 或 Cross-over
>   ≥2 个 → Factorial ⭐
>
> Step 3 (1 变量)：每人接受几种治疗？
>   1 种（同期对比）→ Parallel
>   2 种（前后换 + washout）→ Cross-over
>
> 特殊：按"群体"随机？→ Cluster
> ```
>
> ## 🆚 RCT 4 类对比
> | 设计 | 核心特征 | Stem 指纹 |
> |---|---|---|
> | **Parallel** | 1 变量，各组只 1 种治疗，同期 | "Group A gets X, Group B gets Y" |
> | **Cross-over** | 同一人先后 2 种治疗 + washout | "Patients received A, then washout, then B" |
> | **Factorial** | **≥2 独立变量同时随机化** | "randomized to A/B/C **AND TO** X/Y" ⭐ |
> | **Cluster** | 按**群体**（学校/医院/社区）随机 | "Hospitals/schools **were randomized**" |
>
> ## ⚠️ 高频陷阱
> 1. **多中心 ≠ Cluster** — "21 medical centers" 只是多中心，**按医院随机**才是 cluster
> 2. **第二个变量盲点** — 只看到第一个 randomized 就停止思考，漏掉 stem 里的第二个变量
> 3. **Cross-over 治疗时长长 = 不合理** — Cross-over 通常短期可逆病
>
> ## ❌ 我为什么错
> - **选了 D（Parallel-group）**
> - **错因**：① 不知道 Factorial 的"指纹"概念 ② 漏读 stem 里第二个独立变量（BP 目标） ③ 看到"3 个药分组"就默认 Parallel
> - **核心陷阱**：**"第二个变量盲点"** — Factorial 题的 USMLE 出题模板就是**把第二个变量藏在 stem 里**
>
> ## 🎴 Memory Hook
> - **"两个变量同时随机 = Factorial"**
> - **几何想象**：
>   - Factorial = **格子表格** (2×2, 2×3 矩阵)
>   - Parallel = **两条平行线** (永不相交)
>   - Cross-over = **X 字形** (先 A 后 B 交叉)
>   - Cluster = **一锅端** (整个群体同组)
> - **指纹句式**：`"randomized to ... AND TO ..."` 是 Factorial DNA
>
> ## 🤔 我的提问 / 卡点
> - **元层面诊断**：两题都是"不知道概念 + 不会看 stem" → 需要建立**Study Design 识别 SOP**（3 步法）
> - **关键认知升级**：下次读 stem 时**主动数 "randomized" 出现次数**或**数有几个独立变量**
>
> ## 🔗 关联
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Study Design 4 类对比]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#RCT]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#Factorial vs Parallel]]
> - [[完整笔记/专题笔记/_衍生_高频评分_公式#Study Design 决策树]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 + 默写 RCT 4 类指纹
> - [ ] 默写 **Study Design 决策树**（RCT 4 类 + 观察性 3 类）
> - [ ] 整理"**Factorial 的 stem 指纹**"到 [[完整笔记/专题笔记/_衍生_高频陷阱]]
> - [ ] 给 [[完整笔记/Peixuan分科笔记/Biostats_Master]] 加 #薄弱点（Study Design 部分）
> - [ ] 找 3 道 study design 题（Factorial vs Parallel 辨析）
> - [ ] **刷题时主动数 "randomized" 次数**（养成习惯）

> [!example]- [2026-05-11] Biostats / Case Series 局限性 + 证据等级 (Q20090)
>
> ## 🎯 Stem 模式
> "Single report + 小样本 + 全员接受治疗 + 与历史/published outcomes 比较（**no control group**）" → **Case Series** → 证据等级低 → **不足以推荐治疗**
>
> ## 🔑 核心概念
> **Case Series（病例系列）** = 描述性观察研究，**无对照组**
> - 只能描述（describe），**不能证明因果（causation）**
> - **无论样本量多大**，case series 都不足以推荐新疗法
> - **只有 RCT 才能确立因果关系**
>
> ## 🌲 Study Design 决策树（必背）
> ```
>                 Study Design 研究设计
>                         │
>         ┌───────────────┴───────────────┐
>    Observational 观察性            Experimental 实验性
>    (无随机化)                      (有随机化)
>         │                               │
>         ├── 描述性 Descriptive          ├── Parallel
>         │   ├── Case report (n=1)      ├── Cross-over
>         │   └── Case series (无对照)   ├── Factorial
>         │                              └── Cluster
>         ├── 分析性 Analytic
>         │   ├── Cohort (前瞻/回顾)
>         │   └── Case-control (回顾)
>         │
>         └── Cross-sectional (横断面)
> ```
>
> ## 📊 证据等级金字塔
> ```
> Meta-analysis / Systematic review  ⭐⭐⭐⭐⭐
> RCT                                ⭐⭐⭐⭐
> Cohort (前瞻 > 回顾)               ⭐⭐⭐
> Case-control                       ⭐⭐
> Cross-sectional                    ⭐⭐
> Case series                        ⭐  ← 本题
> Case report (n=1)                  ⭐
> Expert opinion                     ★
> ```
>
> ## 🆚 观察性研究 4 类对比
> | 类型 | 分组依据 | 时间方向 | 有对照？ |
> |---|---|---|---|
> | **Case series** | — | 描述性 | ❌ 无 |
> | **Cohort** | 按**暴露**分组 | 前瞻/回顾 | ✅ |
> | **Case-control** | 按**结局**分组 | 回顾 | ✅ |
> | **Cross-sectional** | 同时测暴露+结局 | "快照" | ✅ |
>
> ## ⚠️ Case Series 证据不足的根本原因
> 1. **没有同期对照组** — 不知道"不治疗"或"标准治疗"会怎样
> 2. **没有随机化** — 无法控制 confounding
> 3. **使用历史对照** — 不公平比较（时代、医疗水平、人群差异）
> 4. **选择方法未知** — selection bias **状态未知**
>
> → 这些是**设计层面**的根本缺陷，**不需要假设任何具体情况**（如病情轻重）
>
> ## ❌ 我为什么错
> - **选了 E（No evidence of selection bias）**
> - **错因**：① 不知道 case series 缺 control group 是设计层面的根本缺陷 ② 把"stem 没提 selection bias"误读为"已排除 selection bias"
> - **核心陷阱**：**"信息缺失陷阱"** — 把"未知"当成"不存在"
>
> ## 🚨 "三不"原则（评价研究质量时）⭐ 今日核心 take-away
> 1. **不脑补 stem 没说的信息**（不替 stem 编解释）
> 2. **不混淆"未知"和"无"**（stem 没提 ≠ 已排除）
> 3. **不用"可能性"代替"证据"**（脑补的可能性不是证据）
>
> → 真正能说的：**只看 design 本身有没有缺陷**
>
> ## 🔓 USMLE "Bias 状态判断"原则
> | Stem 情况 | 正确解读 |
> |---|---|
> | Stem 没提到某 bias | **未知**，不能说"已排除"或"已存在" |
> | "Randomly assigned" | **已排除** confounding |
> | "Double-blind" | **已排除** observer bias |
> | "High compliance + low attrition" | **已排除** attrition/selection bias |
>
> **规则**：只能排除**stem 明确说"已控制"的 bias**
>
> ## 🎴 Memory Hook
> - **"看到 case series（无对照），永远选'证据不足'"** — 不管结果多好、样本多大
> - **Case Series = "故事会"** 📖 → 没说"另外没吃药的怎么样" → **没对照**
> - **RCT = "公平擂台"** 🥊 → 掷硬币分组 → **只有擂台能定胜负**
> - **口诀**："实验最强，对照次之，描述最弱"
>
> ## ⚠️ 干扰项三大陷阱（普适）
> 1. **"样本量万能论"**：以为放大样本就能解决一切 — 但观察性研究的局限是**设计层面**的（A 的陷阱）
> 2. **"层级倒置"**：把观察性研究排在 RCT 之上 — **RCT > Cohort > Case-control > Cross-sec > Case series**（B 的陷阱）
> 3. **"预设结论"**：把"应该做 RCT"和"RCT 一定显示有效"混为一谈 — RCT 是**验证工具**，不是预言机（C 的陷阱）
>
> ## 🤔 我的提问 / 卡点
> - **Q：题目哪里说是轻症了？**
>   → 学到：**Stem 完全没说**病情轻重 — 我之前脑补了。**Stem 没说 = 状态未知**，不能用"可能是轻症"作为证据。这正好印证 E 选项的陷阱（"未提及 ≠ 不存在"），强化了"三不原则"
> - **元层面顿悟**：评价研究质量时，**只看 design 本身**，不脑补 stem 没说的信息
>
> ## 🔗 关联
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Study Design 决策树]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#证据等级金字塔]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Case Series vs Cohort vs RCT]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#观察性 vs 实验性研究]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#未提及不等于不存在]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#样本量万能论]]
> - [[完整笔记/Peixuan分科笔记/儿科#Pompe 病]]
> - [[专题笔记#Lysosomal storage disease]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 + 默写 Study Design 决策树
> - [ ] 默写 **证据等级金字塔**
> - [ ] 默写 **观察性研究 4 类对比表**（分组依据 / 时间方向 / 有无对照）
> - [ ] 整理"**三不原则**"到 [[完整笔记/专题笔记/_衍生_高频陷阱]]
> - [ ] 整理"**Bias 状态判断原则**"到 [[完整笔记/专题笔记/_衍生_高频陷阱]]
> - [ ] 给 [[完整笔记/Peixuan分科笔记/Biostats_Master]] 加 #薄弱点（Study Design 部分）
> - [ ] 在 [[完整笔记/Peixuan分科笔记/儿科]] 补 Pompe disease 笔记（婴儿型 GAA 缺陷、酶替代治疗）
> - [ ] 找 3 道 study design 题（observational vs experimental 辨析）
> - [ ] **下次刷题习惯：读 stem 先定位 study type**

> [!example]- [2026-05-11] Biostats / Case-Control vs Cohort 场景适配 (Q20283)
>
> ## 🎯 Stem 模式
> "**Rare disease** + **Long latent period** + **Find risk factors**" → **Case-Control 金三角** → 秒选 case-control
>
> ## 🔑 核心概念
> **"Most appropriate" study design = 场景适配**，不是抽象证据等级
> - **Case-Control** = "侦探破案" — 从已确诊病例倒查暴露
> - **Cohort** = "盯职业人群" — 找到已暴露的人前瞻跟踪
> - **两者不是谁更好，是谁更适合**
>
> ## 🌟 "最佳" vs "最合适" 原则 ⭐ 今日核心 take-away
> | 概念 | 含义 | 决策方式 |
> |---|---|---|
> | **Best evidence level** | 抽象层级：RCT > Cohort > Case-control | 选金字塔最上层 |
> | **Most appropriate** ⭐ | **场景适配**：哪个能回答这个问题 | 看疾病特点 + 研究问题 |
>
> → 看到 "**most appropriate**" 不要默认选最高等级！要看**场景**
>
> ## 📊 "罕见性" 决定 design（核心决策法则）
> ```
> 病罕见 (rare disease)   → Case-Control（去医院找病人最快）
> 暴露罕见 (rare exposure) → Cohort（找暴露人群最快，跟踪他们）
> 都罕见                   → 难做（nested case-control / registry）
> 都常见                   → 都能做（看成本/速度）
> ```
>
> ## 🆚 Case-Control vs Cohort 终极对比
> | 维度 | Case-Control | Cohort（前瞻）|
> |---|---|---|
> | **方向** | 结局 → 暴露（反向）| 暴露 → 结局（正向）|
> | **分组依据** | 按**疾病状态** | 按**暴露状态** |
> | **指标** | **OR** | **RR / HR** |
> | **能算 incidence？** | ❌ 不能 | ✅ 能 |
> | **罕见病** | ✅ **最佳** | ❌ 招不到病人 |
> | **罕见暴露** | ❌ 招不到暴露者 | ✅ **最佳** |
> | **长潜伏期** | ✅ **最佳** | ❌ 等不起 |
> | **多个 risk factors** | ✅ 一次研究多个 | ✅ 可 |
> | **多个 outcomes** | ❌ 一次研究一个 | ✅ 一次研究多个 |
> | **Recall bias** | ⚠️ 高 | ✅ 低 |
> | **时间成本** | 短（数月）| 长（数年-数十年）|
> | **证据等级** | ⭐⭐ | ⭐⭐⭐ |
>
> ## 🏭 Cohort 罕见暴露的来源（重要：cohort 不是"主动暴露"）
> Cohort 是**观察性研究** — 暴露**已经存在**，研究者**只找到这些人 + 跟踪**：
> 1. **职业人群**：石棉→船厂工人 / 放射→核电站员工 / 化学品→化工厂
> 2. **特殊事件**：原爆幸存者 / 灾区居民 / 越战退伍军人（Agent Orange）
> 3. **登记数据库**：罕见药物使用者 / 罕见手术患者 / 遗传病登记
>
> → 如果研究者**主动**给一组人暴露 → 那是 **RCT**，不是 cohort
>
> ## ❌ 我为什么错
> - **选了 D（Cohort study）**
> - **错因**：① 不知道 Case-Control 在"罕见病/长潜伏期"的独家优势 ② "证据等级最高 = 最合适"的误解（层级 vs 适配混淆）③ 没识别 stem 的双重指纹："rare" + "long latent period"
> - **核心陷阱**：**"层级 vs 适配"陷阱** — 按抽象证据等级选 Cohort，但 USMLE 问的是 "most appropriate"（场景适配），而罕见病 + 长潜伏期是 **Case-Control 的独家场景**
>
> ## 🎴 Memory Hook
> - **"Rare + Latent + Risk factors = Case-Control 金三角"**
> - **场景 → 设计映射**：
>   ```
>   罕见病 / 长潜伏期 / 多 risk factors → Case-Control 🔍 "侦探破案"
>   罕见暴露 / 多 outcomes / 算 incidence → Cohort 🏭 "盯职业人群"
>   ```
> - **方向口诀**：**"病-暴 vs 暴-病"**
>   - Case-control：先有**病**，倒查**暴**露
>   - Cohort：先有**暴**露，等出**病**
>
> ## 🔑 USMLE Study Design 题 3 层问法
> 1. **"What IS the design?"** → 识别（用 stem 指纹）
> 2. **"Limitation/strength?"** → 评价（从设计本质推）
> 3. **"MOST APPROPRIATE design?"** ⭐ → 选择（场景适配，不是抽象层级）
>
> → 第 3 类题型不能用证据金字塔做！要看场景
>
> ## 🤔 我的提问 / 卡点
> - **Q：为啥 cohort 适合罕见暴露？故意去暴露吗？**
>   → 学到：**Cohort 是观察性研究，研究者不主动暴露**。罕见暴露的人**已经存在**（如石棉工人、核电站员工），研究者只是**找到他们 + 跟踪**。如果是主动分配暴露 → 那是 **RCT**。修正了"cohort = 主动暴露"的概念混淆
> - **元层面顿悟**：判断 design 适配性的 2 个问题：① **怎么找到研究对象？**（从暴露端 vs 疾病端）② **需要等多久？**（前瞻 vs 回顾）
>
> ## 🔗 关联
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Case-Control vs Cohort 终极对比]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#Study Design 决策树]]
> - [[完整笔记/Peixuan分科笔记/Biostats_Master#最佳 vs 最合适原则]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#层级 vs 适配陷阱]]
> - [[完整笔记/专题笔记/_衍生_高频陷阱#cohort 不等于主动暴露]]
> - [[完整笔记/专题笔记/_衍生_高频评分_公式#Study Design 场景适配]]
> - [[完整笔记/Peixuan分科笔记/外科#头颈部肿瘤]]（Adenoid cystic carcinoma）
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 + 默写 Case-Control vs Cohort 终极对比表
> - [ ] 默写 **"Rare + Latent + Risk factors = Case-Control 金三角"**
> - [ ] 默写 **"罕见性决定 design" 决策法则**
> - [ ] 整理 **"最佳 vs 最合适"原则** 到 [[完整笔记/专题笔记/_衍生_高频陷阱]]
> - [ ] 整理 **"USMLE Study Design 3 层问法"** 到 [[完整笔记/专题笔记/_衍生_高频评分_公式]]
> - [ ] 在 [[完整笔记/Peixuan分科笔记/Biostats_Master]] 加 #薄弱点（Case-Control 部分）
> - [ ] 找 3 道场景适配题练习（rare disease vs rare exposure 辨析）
> - [ ] **下次刷题主动识别 stem 关键词**：rare / latent / common / multiple outcomes

> [!example]- [2026-05-11] Biostats / 广告题双题：复合终点 + NNT (Q7708 + Q7709, Efrenzia)
>
> ## 🎯 Stem 模式
> **Q7708（Item 1）**："Based on drug ad, ... decrease which event?" → **找驱动复合终点差异的 outcome**（其他 outcomes 通常无显著差异）
> **Q7709（Item 2）**："Need to treat ... to prevent 1 ..." + **亚组限定** → **NNT = 1 / ARR**（用对应亚组的 ARR）
>
> ## 🔑 核心概念
>
> ### 概念 1：Composite Endpoint（复合终点）拆解
> - **复合终点** = 多个 outcome 打包（如 CV death + MI + stroke）
> - **总差异常由单个 outcome 驱动**，其他 outcomes 可能无显著差异
> - **必须拆开看 individual components**，特别是 mortality 和 safety
>
> ### 概念 2：NNT 计算
> - **NNT = 1 / ARR**（不是 1/RRR！）
> - **必须用 stem 限定亚组的 ARR**
> - NNT 越小药越有效
>
> ## 📋 广告题 5 步 SOP（见 [[完整笔记/专题笔记/USMLE广告题解题策略]]）
> ```
> Step 1: 识别 composite endpoint
> Step 2: 看 RRR vs ARR 差异（戏剧化陷阱）
> Step 3: 找哪个 outcome 真正驱动差异
> Step 4: 查 safety data（藏在小字 / 末页）
> Step 5: 区分广告说的 vs 题目问的
> ```
>
> ## ⚠️ 广告题 5 大陷阱
> 1. **RRR 夸大效益**（大字 RRR vs 小字 ARR）
> 2. **Composite endpoint 掩盖真相**（单一驱动 / 反方向信号）
> 3. **Safety 藏在小字**（bleeding 等副作用）
> 4. **"Treatment of choice" 是营销语**
> 5. **Subgroup analysis 过度解读**
>
> ## 📊 复合终点 3 种情况
> | 情况 | 特征 | 解读 |
> |---|---|---|
> | **A 均匀贡献** | 各 outcome 都显著降低 | 真正全面效益（最强证据）|
> | **B 单一驱动** ⬅ Efrenzia | 只 1 个 outcome 显著，其他无差 | 警惕：药只防 X，不防 Y |
> | **C 相反信号** | 1 个降低、1 个增加，复合"无差" | 危险：药害被掩盖 |
>
> ## 🆚 Hard vs Soft Outcomes
> - **Hard**：Death, MI, Stroke（客观、临床重要）
> - **Soft**：Hospitalization, Revascularization, Symptom relief（主观、临床意义低）
> - **All-cause mortality 是最硬的硬终点** — 若无差异，药效需打折扣
>
> ## 🧮 NNT 速查 + 临床解读
> | NNT | 临床意义 |
> |---|---|
> | 1-10 | 极有效 |
> | 10-25 | 不错（Efrenzia UA/NSTEMI+DM 在这）|
> | 25-50 | 一般 |
> | 50-100 | 边际效益 |
> | >100 | 临床意义低 |
>
> ## 🚫 NNT 计算两大陷阱
> 1. **NNT = 1/RRR 错记**（应为 1/ARR）— 易导致严重低估治疗成本
> 2. **亚组错位**：忽略 stem 双重限定（如"with diabetes" + "UA/NSTEMI"）
>
> ## 🎴 Memory Hook
> - **"打包数字看着大，拆开才知真相在哪一只"** 📦
> - **"RRR 大字骗眼睛，ARR 小字才真心"**
> - **"NNT 必用 ARR，亚组限定双 check"**
> - **NNT 救人 KPI**：数字越小，"救人效率"越高
>
> ## 📍 6 个问题 framework（看 composite endpoint RCT 必问）
> 1. 复合包含哪些 outcomes？
> 2. Hard outcomes 还是 soft outcomes 为主？
> 3. 总效果显著吗？
> 4. 各 component 单独看谁显著？⭐
> 5. Mortality 有无差异？
> 6. 有反方向信号吗？
>
> ## ❌ Q7708 / Q7709 我都做对了 ✅
> **关键验证**：
> - Q7708：确认是看了广告第 3 页 "primarily due to MI" 这句吗？还是凭感觉选的？
> - Q7709：第一反应是 NNT = 1/ARR 还是 1/RRR？（如果是 1/RRR → 危险信号）
>
> **未来可能踩坑**：
> - 复合终点的"反方向信号"题（情况 C）
> - Forest plot 识别哪个 component 显著
> - "What is misleading about this ad?" 批判性问法
>
> ## 🤔 我的提问 / 卡点
> - **Q：复合终点的差异只能归因于某个 outcome 是什么意思？**
>   → 学到：总差异 = 各 component 差异之和；如果其他 components 不显著，总差异就**完全来自**那个显著的 component（如 Efrenzia 只防 MI，不防 stroke / death）
> - **元层面顿悟**：广告永远用"打包数字"，临床医生要会"拆包"看真相；这是 Critical Appraisal 的核心
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#Q107183]] RRR 计算（亚组限定 + 分母法则）
>   - [[mistakes/uworld-mistakes#Q20057]] ARR 反推样本量（早上）
>   - [[mistakes/uworld-mistakes#Q20430]] ARP 阳性归因比（早上）
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]] / [[完整笔记/专题笔记/USMLE广告题解题策略]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/心内]]（ACS / NSTEMI / 抗血小板药 — Efrenzia 类似 ticagrelor，新型 P2Y12 抑制剂）
> - 🌱 TODO（待生成衍生）：Biostats 章节复习完后，请 Claude Code 整合所有"广告/摘要解读"类错题 → 扩充 [[完整笔记/专题笔记/USMLE广告题解题策略]]
> - 🌱 TODO（待生成衍生）：整合"亚组限定 + 数据筛选"类错题（Q7709 + Q107183 + Q7688 + 未来）→ 生成 [[完整笔记/专题笔记/_衍生_高频陷阱/Biostats 读题 SOP — 亚组限定与数据定位]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 + 默写广告题 5 步 SOP + 5 大陷阱
> - [ ] 默写 **复合终点 3 种情况**（均匀 / 单一驱动 / 相反信号）
> - [ ] 默写 **NNT = 1/ARR**（强化区分 RRR）
> - [ ] 默写 **6 个问题 framework**
> - [ ] 找 3 道 NBME 广告题练习
> - [ ] 在 [[完整笔记/Peixuan分科笔记/心内]] 补 ACS 抗血小板药对比（clopidogrel / ticagrelor / prasugrel）
> - [ ] **下次广告题主动按 SOP 走，不被大字数字忽悠**

> [!example]- [2026-05-11] Biostats / Clinical Trial Phase III 识别 (Q20058)
>
> ## 🎯 Stem 模式
> "**Large multicenter** + **affected patients** + **randomized + placebo-controlled** + **efficacy**" → **Phase III**
>
> 这 5 个指纹同时满足 → 秒选 Phase III
>
> ## 🔑 核心概念
> **Phase III** = **大样本 RCT 对比 placebo/standard treatment**，在 **affected patients** 中评估 **efficacy + safety**，**FDA 批准前的关键证据**
>
> ## 📊 5 阶段指纹速记（详见 [[完整笔记/专题笔记/USMLE临床试验分期]]）
> | Phase | 受试者 | 样本量 | 核心问题 |
> |---|---|---|---|
> | Preclinical | 动物 | — | 能不能用于人？|
> | **I** | **健康志愿者** | 小 20-100 | **Is it safe?** + MTD + PK |
> | **II** | 少病人 | 中 100-300 | **Does it work?** + optimal dose |
> | **III** ⭐ | **大量病人** | 大 数百-数千 | **Better than current?** + FDA 批准 |
> | **IV** | 上市后病人 | 极大 | **Long-term / rare AE?** |
>
> ## 🎴 Memory Hook
> - **5 阶段口诀**：**S**afe(I) → **W**ork(II) → **B**etter(III) → **L**ong-term(IV)
> - **Phase III 五大指纹**：Large + Multicenter + Affected patients + Randomized + Placebo/Standard 对照
> - **核心判别**：看到 placebo-controlled + large + randomized → **Phase III**
>
> ## ⚠️ 4 大易错陷阱
> 1. **受试者类型**：Phase I = 健康志愿者；II/III/IV = 病人（**例外**：肿瘤药 Phase I 也在病人做）
> 2. **样本量误判**：small + efficacy → Phase II；large + efficacy + randomized → Phase III
> 3. **忽略对照**：没对照的"efficacy"研究 → Phase II；有对照 + 随机化 → Phase III
> 4. **Phase IV ≠ "safety phase"**：所有 Phase 都监测 safety，IV 特指**上市后** long-term / rare AE
>
> ## 🆚 Phase II vs Phase III（高频辨析）
> | 维度 | Phase II | Phase III |
> |---|---|---|
> | 样本量 | 100-300 | 数百-数千 |
> | 目的 | **初步** efficacy + 找剂量 | **确证** efficacy + safety |
> | 随机化 | 可选 | **必须** |
> | 对照 | 不一定 | **必须** |
> | 关键问题 | "Does it work?" | "Better than current?" |
>
> ## 📋 5 步识别 Phase（SOP）
> 1. 在人身上做吗？No → Preclinical
> 2. 健康志愿者 vs 病人？Healthy → 多半 Phase I
> 3. 样本量大不大？Small (<300) → 多半 Phase II
> 4. 上市了没？Yes → Phase IV；No → Phase III
> 5. 有 randomized + 对照吗？Yes → 强化 Phase III 判断
>
> ## ✅ Q20058 我做对了
> **关键验证**：是不是真的会用 5 个指纹排除其他选项？
> - A Preclinical：人身上做了 → 排
> - B Phase I：1000 人 + 病人 → 排
> - C Phase II：1000 人 + multicenter + placebo → 排
> - E Phase IV：还没上市评估 → 排
> - **D Phase III ✅**
>
> ## 🤔 我的提问 / 卡点
> - **元层面顿悟**：本题确认了 5 阶段框架的稳健性 — 5 个指纹中只要满足 3-4 个就基本能定 Phase III
> - **下次练习重点**：Phase II vs Phase III 的边界题（样本量 200-500 那种）
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#Q7688]] HR 解读（同为大型 multicenter RCT = Phase III）
>   - [[mistakes/uworld-mistakes#Q7708]] Efrenzia 广告题（Phase III 后的真实广告）
>   - [[mistakes/uworld-mistakes#Q20283]] Case-Control vs Cohort（观察性 vs 实验性 study design）
> - 📚 主笔记：
> - [[完整笔记/专题笔记/USMLE临床试验分期]] ⭐ 今日新建
> - 🌱 TODO（待生成衍生）：Biostats 章节复习完后，请 Claude Code 整合所有 Phase 相关错题 → 扩充 [[完整笔记/专题笔记/USMLE临床试验分期]]
> - 🌱 TODO（待生成衍生）：整合"药物开发流程"相关错题（Phase + FDA 审批 + 撤市经典案例如 Vioxx）→ 生成 [[完整笔记/专题笔记/_衍生_核心疾病专题/药物开发与上市流程]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 + 默写 5 阶段速查表
> - [ ] 默写 **Phase III 五大指纹**（Large + Multicenter + Affected + Randomized + Controlled）
> - [ ] 默写 **5 步识别 SOP**
> - [ ] 默写 **Phase II vs Phase III 边界**
> - [ ] 在 [[完整笔记/Peixuan分科笔记/hematology oncology]] 补 pegfilgrastim / G-CSF 相关笔记
> - [ ] 找 3 道 Phase 识别题（特别是 Phase II vs III 辨析）

> [!example]- [2026-05-11] Biostats / Internal Validity + Blinding (Q22363)
> 题目主旨：Blinded raters 对主观量表评估的作用 → 减少 measurement bias → 提升 Internal validity
> 详见主笔记：[[完整笔记/专题笔记/USMLE临床试验分期#Part 2：临床试验质量评价]]

## 2026-05-12

> [!example]- [2026-05-12] Biostats / ROC 最佳 cutoff (Q107800)
> 
> ## Stem 模式
> 给 ROC 曲线图 + 标注几个 cut point（A-E）+ 每个点的 (TPR, FPR) 坐标 → 问 "best diagnostic accuracy" 是哪个。
> 通常会**故意放两个极端陷阱**：
> - 一个点 FPR = 0% 但 TPR 很低（看起来"零误伤"）
> - 一个点 TPR = 100% 但 FPR 极高（看起来"全抓住"）
> 
> ## 核心概念
> 
> **ROC = Receiver Operating Characteristic curve**
> - y 轴 = **Sensitivity (TPR)** = 真阳性率
> - x 轴 = **1 - Specificity (FPR)** = 假阳性率
> 
> **最佳 cutoff = 距离左上角 (0, 1) 最近的点** = TPR 高 + FPR 低 的最优平衡。
> 
> ## 普适规则
> 
> ### ROC 几何示意
> 
> ```
>        y = Sensitivity (TPR)
>        
>    1.0 |  *(0,1) 完美点                    
>        |   <-- 最佳目标
>    0.9 |          *⭐ BEST 点      
>        |          (左上角附近)
>    0.7 |     
>        |
>    0.5 |                  . . .  
>        |              . . .
>    0.3 |                              <-- 太保守区
>        |          . . .
>    0.0 +-----.-.-.------------------------- x = 1-Specificity (FPR)
>        0.0   0.2   0.4   0.6   0.8   1.0
> 
>    . . . 对角线 = 随机猜测 (AUC = 0.5，无诊断价值)
>    完美点 (0, 1) = 100% 敏感 + 0% 误伤（现实不存在）
> ```
> 
> ### 4 个关键位置
> 
> | 位置 | 含义 | 临床解读 |
> |---|---|---|
> | **(0, 1) 左上角** | TPR=100%, FPR=0% | 完美试验目标 |
> | **(0, 0) 左下角** | 全判阴性 | cutoff 极高，谁都不诊断 |
> | **(1, 1) 右上角** | 全判阳性 | cutoff 极低，全民确诊 |
> | **对角线** | 随机猜测 | AUC = 0.5，无价值 |
> 
> ### Cutoff 移动的影响
> 
> - **Cutoff ↑**（更严）→ TPR ↓ + FPR ↓ → 点向左下移
> - **Cutoff ↓**（更松）→ TPR ↑ + FPR ↑ → 点向右上移
> - 不可能同时让 TPR ↑ 又 FPR ↓（除非换更好的试验）
> 
> ### 做题 SOP（4 步）
> 
> 1. **认轴**：y = Sensitivity (TPR)；x = 1 - Specificity (FPR)
> 2. **找左上**：哪个点最靠近 (0, 1)？
> 3. **比邻近点**：
>    - TPR 相同时，选 FPR 更低的
>    - FPR 相同时，选 TPR 更高的
> 4. **排极端**：FPR = 0% 的点（漏诊多）和 TPR = 100% 的点（误诊多）通常都不是答案
> 
> ### AUC（曲线下面积）解读
> 
> | AUC | 评价 |
> |---|---|
> | 0.5 | 等于扔硬币（对角线） |
> | 0.7 - 0.8 | 中等 |
> | 0.8 - 0.9 | 良好 |
> | 0.9+ | 优秀 |
> | 1.0 | 完美（曲线完全贴左上） |
> 
> ## 易混陷阱（普适）
> 
> ### 两端极端陷阱
> 
> | 陷阱类型 | 表面诱惑 | 真实问题 |
> |---|---|---|
> | **A 型**（FPR = 0%, TPR 低）| "零误伤" | 漏诊大量真病人，临床灾难 |
> | **E 型**（TPR = 100%, FPR 高）| "全抓住" | 误诊大量健康人，全民假阳性 |
> 
> USMLE **永远在测试你能否拒绝极端，选择平衡点**。
> 
> ### 临床偏好调整（不同情境选不同 cutoff）
> 
> | 临床情境 | 偏好 | 选 ROC 上的位置 |
> |---|---|---|
> | 致死可治、需早抓（HIV / 败血症 / MI）| 高 Sensitivity | 偏右上（多抓不漏） |
> | 侵入性确诊、误诊代价大（活检 / 化疗 / 手术）| 高 Specificity | 偏左下（宁可错过） |
> | 筛查 → 确诊 两阶段 | 先 Sens 后 Spec | 筛查右上，确诊左下 |
> | "best diagnostic accuracy" 题 ⭐ | 平衡 | 左上角附近 |
> 
> ## 我为什么错
> 
> 选了 **A (77 ng/mL, TPR=30%, FPR=0%)**。
> 
> - **概念混淆**：把"最佳 cutoff"等同于"最低 FPR"。最佳 ≠ 单一指标极致，而是两个指标的最优平衡
> - **没建立几何直觉**：没意识到"最佳 = 最靠近左上角"。建立这个直觉后看图秒选
> - **临床思维缺失**：TPR = 30% 在肾上腺功能不全诊断里是灾难（漏掉 70% 真病人 → adrenal crisis 死亡风险）。FPR = 0% 对应"我只敢确诊百分百肯定的"——临床上毫无用处
> 
> **核心陷阱**：A 选项的设计就是用"看起来完美的 0% FPR"诱骗考生忽略 TPR。
> 
> ## Memory Hook
> 
> **ROC 选最佳 = "瞄左上角 (0, 1)，最近的就是答案"**
> 
> 类比：ROC 像爬山，**左上角是山顶**（完美），所有点都在通往山顶的不同路径上。最佳 cutoff = **离山顶直线距离最近的营地**。
> 
> 口诀：**"敏特相搏，左上为王"**（Sensitivity 和 Specificity 互相博弈，最佳点在左上角）
> 
> 极端两端都是坑：FPR=0% 漏诊多，TPR=100% 误诊多 — 都不是答案。
> 
> ## 🤔 我的提问 / 卡点
> 
> - **Q: ROC 图怎么找最佳点？**
>   → 不是算公式，是**几何直觉**——找距离 (0,1) 最近的点。本题 C(0.2, 0.9) 显然比 B(0.2, 0.7) 高、比 D(0.4, 0.9) 左、比 E(0.9, 1.0) 左很多。
> 
> - **Q: 笔记格式怎么处理 ASCII 图？**
>   → 只用半角字符（`|` `-` `*` `+`），避免全角（`┤` `●` `┘`）混排错位；必须包在 ` ``` ` 代码块里；Obsidian 友好替代方案 = 坐标表 + 文字描述。
> 
> ## 🔗 关联
> 
> - 🔁 同主题错题：
>   - 首题，等后续 ROC / AUC 题积累
>   - 广义"敏感性/特异性"族：如有 Q5589 等 6 指标题
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/Biostats_Master]]
>   - [[完整笔记/专题笔记/Biostats_6指标决策树_纯净版]]（ROC 是 Sens/Spec 的图形扩展）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/endocrine]]（临床背景：肾上腺功能不全 ITT vs GST 诊断切点 —— 内分泌可能直接考 ITT/GST 流程，但本题考的是 Biostats）
> - 🌱 TODO（待生成衍生）：
>   - 等积累 2-3 道 ROC 题后，请 Claude Code 整合 → 生成 [[完整笔记/专题笔记/_衍生_ROC曲线判读]] 或并入 [[完整笔记/专题笔记/Biostats_6指标决策树_纯净版]] 作为图形章节
>   - 同时可作为未来 [[完整笔记/专题笔记/USMLE_Study_Design决策树]]（诊断试验评估章节）的素材
> 
> ## ✅ 复盘行动
> 
> - [ ] 1 周后重做 Q107800
> - [ ] 默写 ROC 两轴定义（y = TPR = Sens；x = FPR = 1 - Spec）
> - [ ] 默写"最佳 cutoff = 最靠近左上角"规则
> - [ ] 找 2-3 道类似 ROC 题练习（UWorld 搜 "ROC" / "receiver operating"）
> - [ ] 关键习惯：看到诊断试验题，先问"这是 2x2 表问题（PPV/NPV）还是 ROC 问题（cutoff）"
> - [ ] 进阶：学习 AUC（曲线下面积）的解读，也是高频考点

> [!example]- [2026-05-12] Biostats / Reporting bias (Q12685)
> 
> ## Stem 模式
> 同人群、当面 vs 匿名两次调查 → 结果不同。话题自带社会污名（含糖饮料、肥胖、酒精、毒品、性、家暴、体重）。Stem 主动写明"response rate and demographics comparable"——出题人在喊话："Ascertainment / Nonresponse 不是答案。"
> 
> ## 核心概念
> **Reporting bias** = 受访者因社会压力 **故意** 改答案（少报/多报暴露）。
> 属于 **Measurement bias（测量层面）**，不是 selection bias。
> 
> ## 普适规则
> 
> ### 5 大 selection bias（"挑人有问题"）
> 
> | Bias | Stem 关键词 | 一刀切口诀 |
> |---|---|---|
> | **Ascertainment** | convenience sample / 非随机抽样 | 撒网地方不对 |
> | **Nonresponse** | response rate 30% | 不上钩 |
> | **Berkson** | hospital-based controls | 在医院找对照 |
> | **Neyman** | rapidly fatal / 暴露长期前 | 早死早愈漏网 |
> | **Attrition** | X% lost to follow-up | 上钩又跑了 |
> 
> ### 4 大 measurement bias（"测人有问题"）
> 
> | Bias | Stem 关键词 | 一刀切口诀 |
> |---|---|---|
> | **Recall** | "asked to recall" + 暴露很久前 | 想不起来（脑子） |
> | **Reporting** ⭐ | anonymous vs in-person / 污名话题 | 不想说（嘴） |
> | **Observer** | not blinded / 主观评分 | 研究者手抖 |
> | **Surveillance** | monitored more closely | 查得多就发现得多 |
> 
> ### 做题 SOP（3 步定位）
> 
> 1. 看 stem **主动排除**了什么？（"response rate comparable" → 直接划掉 selection bias）
> 2. 问题出在"挑人"还是"测人"？
>    - 挑人 → Selection 5 选 1
>    - 测人 → Measurement 4 选 1
> 3. 找最具体的"暗号词" → 90% 题里都有一个明确指向
> 
> ## 易混陷阱（普适）
> 
> ### Recall vs Reporting ⭐ 最高频混淆
> 
> | 维度 | Recall | Reporting |
> |---|---|---|
> | 本质 | 想不起来（记忆问题） | 不想说（社会压力） |
> | 是否故意 | ❌ 不故意 | ✅ 故意 |
> | 触发词 | "asked to recall" + 暴露很久前 | anonymous vs in-person / 污名话题 |
> | 典型场景 | 畸形婴儿妈妈回忆孕期用药 | 含糖饮料/酒精/毒品/体重自报 |
> | 典型 design | Case-control (retrospective) | 任何设计都可能 |
> 
> **口诀**：想不起来 = Recall（脑子）；不想说 = Reporting（嘴）
> 
> ### Berkson vs Neyman
> 
> | 维度 | Berkson | Neyman |
> |---|---|---|
> | 出问题的组 | **对照组**（住院对照不健康） | **病例组**（致死病的病例漏掉） |
> | 触发词 | "controls from hospitalized" | "rapidly fatal" / "long latency" |
> | 经典例子 | 咖啡-胰腺癌（消化溃疡当对照） | 雪铲-MI（猝死者不进医院） |
> 
> **口诀**：住院对照 = Berkson；病例没机会进研究 = Neyman
> 
> ### RCT ≠ 万能
> 
> | 偏倚 | RCT 能消除吗 |
> |---|---|
> | Confounding | ✅ 能（随机化核心作用） |
> | Selection（招募阶段） | ⚠️ 部分能 |
> | Recall / Reporting | ❌ 不能（测量层面） |
> | Observer | ⚠️ 要靠 blinding |
> | Surveillance | ⚠️ 要靠协议规定相同监测频率 |
> 
> Randomization 只解决"分组前"差异，测量过程 bias 要靠 blinding + 标准化操作。
> 
> ## 我为什么错
> 
> 选了 **A. Ascertainment bias**。
> 
> - **没看清 stem 暗号**："response rate and demographics comparable" 这句话就是出题人主动给你排除 Ascertainment / Nonresponse 的提示，看到这句话 A 和 D 必须立刻划掉
> - **概念混淆**：把"两次结果不同 → 偏倚"等同于"选择偏倚"。其实 bias 大类分两支 —— Selection（谁进入）vs Measurement（怎么测出来）。本题是测量层面
> - **忽略社会污名信号**：含糖饮料 + 肥胖 = USMLE 在喊"Reporting bias"
> 
> ## Memory Hook
> 
> **"当面不敢说，匿名才说真" = Reporting bias**
> 
> 类比：**警察问酒驾** vs **匿名问酒驾** — 两次答案不同就是 Reporting。
> 
> USMLE 偏爱的"reporting 触发组合"：含糖饮料 / 酒精 / 毒品 / 性行为 / 家暴 / 体重 / BMI。
> 
> ## 🤔 我的提问 / 卡点
> 
> - **Q: 不明白 ascertainment 什么意思？**
>   → Ascertainment = "确认/查明"研究对象时的偏倚 = 抽样偏倚（sampling bias）。本质：撒网的地方不对，捞上来的鱼不能代表整个海。Stem 触发词：convenience sample / 单一诊所招募 / sample ≠ target population。
>   → **本题选 A 错的根本原因**：没读到 stem 那句"sample comparable"的暗号。
> 
> - **Q: Berkson 是找的对照太重是吗？**
>   → 直觉对，但要精确：Berkson 是用"住院病人"做对照 → 对照组本身就不健康/已有暴露 → 病例-对照差异被稀释/扭曲。
>   → 是 ascertainment 的一种特殊形式（父子关系），但 USMLE 当并列选项考。看到 "hospital-based controls" 闭眼选 Berkson。
> 
> - **Q: Neyman 怎么理解？**
>   → "暴露太早，研究太晚 — 早死的和早愈的都不在了"。研究池里只剩"中等病程"患者，不代表所有发病者。
>   → 经典：雪铲-MI（猝死者直接死在自家院子里，没机会被研究）/ 重度饮酒-食管癌（重度饮酒者先死于其他原因）。
>   → 触发词：rapidly fatal / long latency / exposure long before assessment。
> 
> ## 🔗 关联
> 
> - 🔁 同主题错题：
>   - Q12684 (Item 1 同 vignette) — Observational study identification（做对了，但同一 stem 两个考点 = 高频考法）
>   - [[mistakes/uworld-mistakes#Q3941]] Bias 鉴别题（如已建）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/Biostats_Master]]
>   - [[完整笔记/专题笔记/_衍生_高频陷阱]]
> - 🏥 跨学科：无（纯 Biostats）
> - 🌱 TODO（待生成衍生）：
>   - 等 Biostats 章节复习完，请 Claude Code 整合 Bias 系列错题（Q12685 + Q3941 + Q20090 + 后续）→ 生成 [[完整笔记/专题笔记/_衍生_USMLE_Bias_5大鉴别]]，骨架：Selection (5) vs Measurement (4) 两大类对比 + Stem 触发词速查 + 经典错题引用
>   - 已有草稿（见今日产出 `2026-05-12_Bias主笔记草稿_v1.md`）可直接作为雏形
> 
> ## ✅ 复盘行动
> 
> - [ ] 1 周后重做 Q12684 + Q12685 整套 vignette
> - [ ] 默写 5 大 selection bias + 4 大 measurement bias 触发词（不看答案）
> - [ ] 默写 "Recall vs Reporting" 一刀切区分
> - [ ] 找 3 道类似 Reporting bias 题（UWorld 搜 "anonymous" / "self-reported"）
> - [ ] 关键习惯：以后做 bias 题先看 stem 有没有"主动排除某些 bias 的暗号"
