# UWorld 错题整理

## 2026-05-10

> [!example]- [2026-05-10] Biostats / Hill's criteria — Dose-Response 识别 (Q20787)
> ^Q20787
> 
> ## Stem 模式
> RCT 比较运动 vs 标准护理对糖尿病停药率，运动组按剂量分 T1/T2/T3 三组，RR 随剂量从 12.1→25.2→38.9 **单调递增** → 问 "additional support" 这是因果（非偶然）的哪条证据？
> 
> ## 核心概念
> **剂量分层 + 结果单调 = Hill's biological gradient (dose-response)**
> Hill's criteria 是因果推断的 9 条经典准则；USMLE 高频考其中 3 条（dose-response / temporality / strength of association）。
> 
> ## 普适规则
> 
> ### Hill's 三大金刚（USMLE 高频）
> | 准则 | Stem 触发词 | 例子 |
> |---|---|---|
> | **Dose-response (biological gradient)** ⭐ | "剂量分层 + 结果单调" / T1/T2/T3 + RR 递增 | 本题 RR 12.1→25.2→38.9 |
> | **Temporality** | 暴露**先于**结局 | RCT 天然满足 |
> | **Strength of association** | RR / OR 数值大 | RR > 3 等 |
> 
> ### "Additional support" 解题原则 ⭐
> - 题问 "**additional**" → 排除**已经在题干主结果里的信息**
> - 主结果 = "intensive vs standard 显著关联" → 这是 stem 已给的，**不算 additional**
> - Additional = stem 在主结果之外**额外提供的信息**（如本题的剂量分层 + 单调）
> 
> ## 易混陷阱（普适）
> 
> ### 干扰项分析
> | 选项 | 为什么错 |
> |---|---|
> | A. "Bias completely eliminated" | **"completely" = USMLE 经典绝对化陷阱**；RCT 也不可能完全消除 bias |
> | C. 12 个月随访时长 | follow-up 时长是研究设计要素，**不是 Hill's criteria** |
> | D. RCT 主结果（intensive vs standard 有显著关联）| 这是 stem 已给的信息，**不是 "additional" 支持** |
> 
> ## 我为什么错 / 纠结
> 
> 选了 **B（做对但 Mark）** — 纠结点：B vs D
> 
> - 不确定 "additional support" 到底排除什么
> - 没建立 "主结果 vs additional information" 的分辨原则
> - 知识层不熟：Hill's 9 条只能背出几条名字，不会快速应用
> 
> 错因 = **pattern**（识别 dose-response 的模式未自动化）。
> 
> ## Memory Hook
> 
> > **"剂量分层 + 结果单调 → dose-response"** — 0.5 秒锁定
> > 
> > **"Additional support" 题型** = 排除 stem 主结果，找额外信号
> > 
> > Hill's 三金刚：**Dose-response / Temporality / Strength**
> 
> ---
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q20227]] OR 方向陷阱（同日 Biostats）
>   - 待积累更多 Hill's / 因果推断题
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
> - 🏥 跨学科：无
> - 🌱 TODO：等积累 ≥ 3 道因果推断题 → 生成 [[完整笔记/专题笔记/_衍生_因果推断与Hills准则]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q20787（验证模式自动化）
> - [ ] 默写 Hill's 三金刚
> - [ ] 默写"additional support 排除主结果"规则
> - [ ] 关键习惯：看到 RR / 风险按剂量递增 → 立刻喊"dose-response"
> 
> ---
> 
> 学科:: Biostats
> 主题:: Hill's criteria — Dose-Response
> 状态:: 🟡
> 错因:: pattern

> [!example]- [2026-05-10] Biostats / OR 方向陷阱 + Case-Control 不能算 risk (Q20227)
> ^Q20227
> 
> ## Stem 模式
> Case-control 研究：**Black vs Non-Hispanic White** 女性 pregnancy-related death，未调整 OR = 3.07 (95% CI 2.78-4.20)，调整后 OR = 2.65 (95% CI 2.12-3.45) **仍显著** → 问最可能结论。
> 
> ## 核心概念
> **Adjusted OR 仍显著 → 有 unmeasured confounders（残留关联指向未测量的外部因素，如结构性歧视）**
> 
> ## 普适规则
> 
> ### OR 方向铁律 ⭐
> - **OR > 1 → 暴露组 odds 高于 reference 组**
> - 谁是暴露 / 谁是 reference 看 stem **"X compared to Y"** → **X 是暴露**，Y 是 reference
> - 本题："Black compared to NHW" → Black 是暴露，OR 3.07 = **Black 的 odds 是 NHW 的 3 倍**
> 
> ### Case-control 测量铁律
> - **Case-control 只能算 OR**（odds ratio）— **不能算 risk / RR**
> - 原因：不是从暴露追到结局（前瞻），而是从结局倒推暴露（回顾）→ 没有分母 = total exposed
> - **看到 case-control + 选项里说 "risk" → 立刻警惕**
> 
> ### Adjusted vs Unadjusted OR 解读
> | 情况 | 含义 |
> |---|---|
> | Adj OR ≈ Unadj OR | 这些 confounders 没解释关联 → 真实关联 / 或有 unmeasured |
> | Adj OR < Unadj OR 但仍显著 | 部分关联被解释 + **残留有 unmeasured confounders** ← 本题 |
> | Adj OR → 1（不显著）| 关联完全由调整的 confounders 解释 |
> 
> ## 易混陷阱（普适）
> 
> ### 干扰项分析
> | 选项 | 为什么错 |
> |---|---|
> | A. "primarily due to poverty / low prenatal care" | 这些已经在 adjusted model 里 controlled，**关联仍显著说明它们不是主因** |
> | C. "case-control 不能得出 statistically significant conclusions" | Case-control **可以**做 OR + CI，这是其核心用途（罕见结局首选）|
> | **D. "NHW 是 Black 的 3 倍"** ⭐ 我选的 | **方向反了** — Black 是暴露，OR 3.07 = Black 的 odds 是 NHW 的 3 倍。USMLE 经典反向陷阱 |
> | E. "调整 contraception use → maternal age contributes" | 研究**没有**调整 contraception use；且 maternal age > 35 的 p = 0.12 **不显著** |
> 
> ### ⚠️ CK 高频陷阱（普适）
> 1. **OR 方向永远看 "X compared to Y" — X 是暴露，Y 是 reference**
> 2. **Case-control 永远算 OR，不算 RR / risk**（选项里说 "risk" 涉及 case-control → 警惕）
> 3. **Adjusted OR 仍显著 → 有 unmeasured confounders**（经典考点，常考"种族健康差异" vignette）
> 
> ## 我为什么错
> 
> 选了 **D. "NHW 是 Black 的 3 倍"**。错因 = **干扰项**（双重陷阱：方向 + risk/odds 混淆）。
> 
> - **方向陷阱**：没识别 "X compared to Y" 中 X 是暴露组，把 OR 3.07 反向理解
> - **概念混淆**：把 odds 当成 risk，case-control 里没注意"不能算 risk"的铁律
> - **被 stem 顺序迷惑**：题干先说 NHW 再说 Black，惯性把 NHW 当作"主语"
> 
> 核心陷阱：**USMLE 把方向反向 + 术语混用同时埋一个选项**，钓不看"X compared to Y"语序的人。
> 
> ## Memory Hook
> 
> > **"X compared to Y" → X 是暴露**（X 在前）
> > 
> > **Case-control = OR 专属**（永远不能说 risk）
> > 
> > **Adjusted OR 仍显著 → 还有没调的 confounder**（"残留 = 未测量"）
> > 
> > 类比：**赛跑成绩 "A 比 B 快"** → A 是被比较对象（暴露），B 是基准（reference）
> 
> ---
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q20787]] Hill's criteria（同日 Biostats）
>   - [[mistakes/uworld-mistakes#^Q20283]] Case-Control vs Cohort 场景适配
>   - [[mistakes/uworld-mistakes#^Q21248]] OR-CI 表格判读 + Confounding
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/OB]]（pregnancy-related death 流行病学 / 种族差异）
> - 🌱 TODO：等积累 ≥ 3 道 OR 方向 / case-control 错题 → 整合到 [[完整笔记/专题笔记/Biostats_6指标决策树_纯净版]] 或生成 [[完整笔记/专题笔记/_衍生_OR_RR方向陷阱]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q20227（验证方向陷阱是否还会中招）
> - [ ] 默写 "X compared to Y → X 是暴露" 铁律
> - [ ] 默写 Case-control 不能算 risk 的原因（无分母 = total exposed）
> - [ ] 默写 Adjusted OR 仍显著 → unmeasured confounders 含义
> - [ ] 关键习惯：看到 OR 题 → 强制找 "X compared to Y"，圈出 X / Y
> - [ ] 关键习惯：看到 case-control + 选项有 "risk" → 红灯
> 
> ---
> 
> 学科:: Biostats
> 主题:: OR 方向陷阱 + Case-control 不能算 risk
> 状态:: 🔴
> 错因:: 干扰项

## 2026-05-11

> [!example]- [2026-05-11] Biostats / ARP 阳性归因比 (Q20430)
> ^Q20430
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: ARP 阳性归因比
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / ARR 反推样本量 (Q20057)
> ^Q20057
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: ARR 反推样本量
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / LR+ 阳性似然比 (Q107214)
> ^Q107214
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: LR+ 阳性似然比
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / ROC 曲线 + Cutoff 跷跷板 (Q7711)
> ^Q7711
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: ROC 曲线 + Cutoff 跷跷板
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / Matching 控制 Confounding (Q4182)
> ^Q4182
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: Matching 控制 Confounding
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / PPV NPV vs Prevalence (Q21656)
> ^Q21656
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: PPV NPV vs Prevalence
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / HR 解读 (Q7688)
> ^Q7688
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: HR 解读
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / Study Design Factorial 识别 (Q7688-Item2)
> ^Q7688-Item2
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: Study Design Factorial 识别
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / Case Series 局限性 + 证据等级 (Q20090)
> ^Q20090
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: Case Series 局限性 + 证据等级
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / Case-Control vs Cohort 场景适配 (Q20283)
> ^Q20283
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: Case-Control vs Cohort 场景适配
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / 广告题双题：复合终点 + NNT (Q7708 + Q7709, Efrenzia)
> ^Q7708-Q7709-Efrenzia
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
>   - [[mistakes/uworld-mistakes#^Q107183]] RRR 计算（亚组限定 + 分母法则）
>   - [[mistakes/uworld-mistakes#^Q20057]] ARR 反推样本量（早上）
>   - [[mistakes/uworld-mistakes#^Q20430]] ARP 阳性归因比（早上）
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: 广告题双题：复合终点 + NNT
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / Clinical Trial Phase III 识别 (Q20058)
> ^Q20058
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
>   - [[mistakes/uworld-mistakes#^Q7688]] HR 解读（同为大型 multicenter RCT = Phase III）
>   - [[mistakes/uworld-mistakes#^Q7708-Q7709-Efrenzia]] Efrenzia 广告题（Phase III 后的真实广告）
>   - [[mistakes/uworld-mistakes#^Q20283]] Case-Control vs Cohort（观察性 vs 实验性 study design）
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: Clinical Trial Phase III 识别
> 状态:: 
> 错因:: 

> [!example]- [2026-05-11] Biostats / Internal Validity + Blinding (Q22363)
> ^Q22363
> 题目主旨：Blinded raters 对主观量表评估的作用 → 减少 measurement bias → 提升 Internal validity
> 详见主笔记：[[完整笔记/专题笔记/USMLE临床试验分期#Part 2：临床试验质量评价]]
> 
> ---
> 
> 学科:: Biostats
> 主题:: Internal Validity + Blinding
> 状态:: 
> 错因:: 

## 2026-05-12

> [!example]- [2026-05-12] Biostats / ROC 最佳 cutoff (Q107800)
> ^Q107800
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: ROC 最佳 cutoff
> 状态:: 
> 错因:: 

> [!example]- [2026-05-12] Biostats / Reporting bias (Q12685)
> ^Q12685
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
>   - [[mistakes/uworld-mistakes#^Q3941]] Bias 鉴别题（如已建）
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
> 
> ---
> 
> 学科:: Biostats
> 主题:: Reporting bias
> 状态:: 
> 错因:: 

> [!example]- [2026-05-12] Biostats / Null Hypothesis (Q3941)
> ^Q3941
> 
> ## Stem 模式
> Cross-sectional study（用 **prevalence** + **某时点** 锁定）→ 问 **best statement of null hypothesis**。
> 干扰项里**至少有一个**"方向对（表达无差异）但用错术语（risk / cause / affect）"的陷阱选项 — 这是 USMLE 双重叠加陷阱模板。
> 
> ## 核心概念
> 
> **Null hypothesis (H0)** = "无差异 / 无关联 / 无效应"，是研究者**想推翻**的假设。
> 
> Cross-sectional 的 H0 必须用**最中性的"association"措辞**，不能用：
> - ❌ "risk"（cohort/RCT 语言）
> - ❌ "incidence"（前瞻性语言）
> - ❌ "causes / affects"（暗示因果方向）
> 
> ## 普适规则
> 
> ### Null vs Alternative
> 
> | 概念 | 缩写 | 内容 | 角色 |
> |---|---|---|---|
> | Null hypothesis | H0 | 无差异/无关联/无效应 | 研究者想**推翻** |
> | Alternative hypothesis | H1 (Ha) | 有差异/有关联/有效应 | 研究者想**支持** |
> 
> **统计推断核心逻辑**：
> - p < 0.05 → **reject H0** → 支持 H1
> - p ≥ 0.05 → **fail to reject H0** → ⚠️ 不等于"证明 H0 为真"，只是"证据不够"
> 
> ### Study Design 决定术语 ⭐⭐
> 
> | Study Design | 可用测量术语 | 不能用 |
> |---|---|---|
> | RCT / Cohort | **RR (Relative Risk), Risk, Incidence** | — |
> | Case-control | **OR (Odds Ratio)** | ❌ 不能算 RR / Incidence |
> | Cross-sectional | **Prevalence, POR** | ❌ 不能算 Risk / Incidence |
> | **任何设计** | **Association**（最通用、最中性） | — |
> 
> ### 做题 SOP（3 步定位 Null hypothesis）
> 
> 1. **识别 study design**（找 stem 里 prevalence / incidence / cases vs controls / randomized 等线索）
> 2. **排除 H1 选项**（任何陈述"有关联 / 有差异 / 更多 / 更易"的都是 H1）
> 3. **在剩余选项里选措辞和 design 匹配的**：
>    - Cross-sectional → 选用 "association" / "prevalence" 的
>    - Cohort/RCT → 选用 "risk" / "incidence" 的
>    - Case-control → 选用 "OR = 1" 的
>    - **不确定时，选 "association" 永远安全**
> 
> ## 易混陷阱（普适）
> 
> ### USMLE Null hypothesis 题三大错误类型
> 
> | 错误类型 | 表现 | 例子 |
> |---|---|---|
> | **方向错** | 写成 H1（陈述"有关联"）| "Colon cancer is more prevalent in CRP+" |
> | **设计错** ⭐ | 方向对但术语和 design 不匹配 | Cross-sectional 用 "risk" / "incidence" |
> | **时序错** | 暗示因果方向（cross-sectional 无法判定）| "Cancer does not affect CRP" |
> 
> **正确选项 = 同时通过这三道关**：表达"无" + 措辞中性 + 不暗示时序。
> 
> ### Risk vs Prevalence vs Odds vs Association 区分
> 
> - **Risk** = 前瞻性概念（新发病例 / 起始人群）→ 仅 cohort/RCT 能算
> - **Prevalence** = 某时点患病比例 → cross-sectional 专属
> - **Odds** = case-control 用（无法算 incidence 时的替代）
> - **Association** = 中性万能词，任何 design 都适用 ⭐
> 
> ## 我为什么错
> 
> 选了 **D. The risk of colon cancer is the same for subjects with and without elevated CRP**。
> 
> - **不知道这个考点**：没意识到不同 study design 对应不同的"测量语言"
> - **概念部分对**：把"null = 表达无差异"理解对了一半（D 确实表达了"无差异"）
> - **没匹配 design**：stem 里 "prevalence" 和 "at a given point in time" 已经明确告诉是 cross-sectional，但没把这条信息和 D 的 "risk" 用词对应起来
> 
> **核心陷阱**：USMLE 把两个考点叠加在一题 ——
> 1. 你要知道 null = 无关联
> 2. 你**还要**知道 study design 决定术语
> 
> 只满足 (1) 不够，会被 D 钓到。**必须两个都满足才能选对**。
> 
> ## Memory Hook
> 
> **Null = "没有"** + **"没有"的措辞必须配 study design**
> 
> 口诀：
> - **"想证 A，先假非 A"** — Null 永远是研究者想证明的反面
> - **"Risk 是 cohort 的，Prevalence 是 cross-sectional 的，Odds 是 case-control 的，Association 是所有人的"**
> - 不确定时，选 **"no association"** 永远安全
> 
> 法庭类比：H0 = "无罪推定"，需要"超出合理怀疑"的证据（p < 0.05）才能推翻。Fail to reject H0 ≠ 证明无罪，只是"证据不够"。
> 
> ## 🤔 我的提问 / 卡点
> 
> - **Q: D 和 E 都说"无关联"，区别在哪？**
>   → D 用 "**risk**"，E 用 "**association**"。Risk 是 cohort/RCT 专属术语，cross-sectional 只能算 prevalence 不能算 risk。E 的 "association" 中性万能 → cross-sectional 唯一安全表达。
> 
> - **Q: 为什么 B 错？它也说"不影响"**
>   → B 说 "cancer does not affect CRP" — 暗示了**反向因果方向**（cancer → CRP）。Cross-sectional 无法判定时序，不能写出"谁影响谁"的措辞，必须用对称的"无关联"。
> 
> ## 🔗 关联
> 
> - 🔁 同主题错题：
>   - 首道 Hypothesis testing / Null hypothesis 题
>   - 关联到 study design 系列：
>     - [[mistakes/uworld-mistakes#^Q12684]] Cross-sectional 识别（本题正是其衍生考法）
>     - [[mistakes/uworld-mistakes#^Q12685]] Reporting bias（同日 Biostats）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/Biostats_Master]]
>   - [[完整笔记/专题笔记/Biostats_6指标决策树_纯净版]]（RR/OR/Prevalence 区分基础）
>   - 待生成草稿：`2026-05-12_Hypothesis_testing主笔记草稿_v1.md`（今日产出）
> - 🏥 跨学科：无（纯 Biostats）
> - 🌱 TODO（待生成衍生）：
>   - 等积累 3+ 道 Hypothesis testing 题（Type I/II / Power / p / CI）→ 请 Claude Code 整合 + 升级今日草稿 → 生成 [[完整笔记/专题笔记/_衍生_USMLE_统计推断]]
>   - 本题也是未来 [[完整笔记/专题笔记/USMLE_Study_Design决策树]] 的素材（"不同 design 对应不同测量术语"章节）
>   - 可补充进 [[完整笔记/专题笔记/_衍生_高频陷阱]]：USMLE 双重叠加陷阱（语义对 + design 不对）
> 
> ## ✅ 复盘行动
> 
> - [ ] 1 周后重做 Q3941
> - [ ] 默写 "Risk / Odds / Prevalence / Association" 各对应哪种 study design
> - [ ] 默写 H0 vs H1 逻辑（reject H0 ≠ 证明 H1，fail to reject ≠ 证明 H0）
> - [ ] 找 2-3 道类似 Null hypothesis 题（UWorld 搜 "null hypothesis"）
> - [ ] 关键习惯：以后看到 Biostats 题，**先识别 study design**，再用 design 排除"用错术语"的选项
> - [ ] 进阶：学习 Type I / II error + Power + p-value 解读
> 
> ---
> 
> 学科:: Biostats
> 主题:: Null Hypothesis
> 状态:: 
> 错因:: 

> [!example]- [2026-05-12] Biostats / OR-CI 表格判读 + Confounding (Q21248)
> ^Q21248
> 
> ## Stem 模式
> 
> **Vignette 套两题**（同一研究 abstract）：
> - **Item 1**：给 case-control 研究的 OR 表（含 **Bivariate + Multivariate** 双栏 + 95% CI），问哪个是该患者发病的"最显著危险因素"
> - **Item 2**：问该研究的"最大缺陷 / most concern"
> 
> 经典套路：双栏 OR 表 + 表脚 "(adjusted for age, sex, X)" + 故意把某个 bivariate OR 设得**很惊人**（如 11.84）但 multivariate CI 跨 1.0 → 钓不看 CI 的考生。
> 
> ## 核心概念
> 
> ### Item 1: OR 表判读三步法
> 
> 1. **只看 Multivariate (adjusted) 那栏** — Bivariate 没控制 confounder，不可信
> 2. **看 95% CI 是否跨 null value (1.0)** — 跨 1.0 = 不显著，无论点估计多大都不行
> 3. **看患者真的暴露了吗** — 显著 + 暴露 = 答案
> 
> ### Item 2: Confounding 应用
> 
> 看到"调整了 A, B, C"→ 立刻想"D, E, F 没调整呢？"= **Residual confounding**（残余混杂）
> 
> ## 普适规则
> 
> ### 95% CI 判读规则 ⭐
> 
> | 测量指标 | Null value | CI 跨 null → | CI 完全偏离 → |
> |---|---|---|---|
> | RR / OR / HR（比值类）| **1.0** | 不显著 | 显著 |
> | Mean difference / RD（差值类）| **0** | 不显著 | 显著 |
> 
> **口诀**：**"看比值盯 1，看差值盯 0"**
> 
> ### Bivariate vs Multivariate 角色
> 
> | 维度 | Bivariate (Unadjusted) | Multivariate (Adjusted) ⭐ |
> |---|---|---|
> | 控制 confounder? | ❌ | ✅ |
> | 哪个可信? | ❌ 容易被 confounding 扭曲 | ✅ **真实关联** |
> | 看哪个? | ❌ 不看 | ✅ 永远以此为准 |
> | 关注差异时机 | bivariate ≠ multivariate 差很大 → 强 confounding 信号 |
> 
> ### "Adjusted for" 的真实含义 ⭐⭐（关键概念）
> 
> 表脚 "Adjusted for X, Y, Z" 的潜台词：
> 
> > **"研究者怀疑 X、Y、Z 可能是 confounder（会干扰其他因子和结局的真实关联），所以在分析时把它们的影响扣除，看剩下因子的真实独立效应。"**
> 
> **不是**："X、Y、Z 是独立危险因素，所以我们把它们平衡掉"
> 
> **而是**："X、Y、Z 可能是干扰，我们想消除它们，看真相"
> 
> **类比**：调音师消除空调声、键盘声 → 不是因为这些声音重要，而是想让人声真实呈现。Confounder 就是研究里的"噪音"。
> 
> ### 为什么被 adjusted 的变量自己 multivariate 会"失去显著性"？
> 
> 当一个变量**同时**出现在因子列和表脚 adjusted 列表里（如 Q21248 的 CPB duration）：
> 
> 1. Bivariate 时它独自分析 → OR 包含"直接影响" + "通过其他变量的间接影响"
> 2. Multivariate 时模型先扣除它的影响（作为 confounder），再回头估它的"独立效应" → 已经被"用尽"的信号自然变小
> 3. 加上它和其他因子(如乳酸)可能高度相关 → **多重共线性**让信号被分走
> 
> → multivariate 失去显著性是**设计使然**，不代表它"没用"
> 
> → 真相可能是：CPB duration → 乳酸升高 → ARF（间接通过乳酸致病，不是直接独立危险因素）
> 
> ### Confounder vs Independent Risk Factor ⭐⭐（USMLE 高频陷阱）
> 
> | 概念 | 角色 | 处理方式 | 例子 |
> |---|---|---|---|
> | **Confounder（混杂变量）** | 干扰真实关联的第三方变量 | **要 adjust 掉**（消除影响）| 研究"咖啡→肺癌"时的吸烟 |
> | **Independent Risk Factor（独立危险因素）** | 真正独立致病的变量 | **不调整**，让它显示真实效应 | 研究"咖啡→肺癌"时的咖啡本身 |
> 
> **核心区别**：
> - 调整 confounder = 想让它的影响"消失"，剩下的关联才是真实的
> - 不调整 risk factor = 想让它的真实效应"显示出来"
> 
> ### USMLE OR 表题型问法精确解读 ⭐⭐
> 
> | 题目问法 | 怎么答 |
> |---|---|
> | "**Which is an independent risk factor**?" | 选 multivariate **CI 不跨 1.0** 的（显著）|
> | "Most **significant** risk factor for **this patient**" | multivariate 显著 **+ 该患者真的暴露** |
> | "Which factor's association is **explained by confounding**?" | 选 bivariate **显著** + multivariate **不显著** 的 |
> | "Which factor **lost significance** after adjustment?" | 选 bivariate 显著、multivariate 不显著的 |
> | "Which factor needs to be **controlled** in the analysis?" | 选**潜在 confounder**（表脚 adjusted 列表里的）|
> 
> ### 做题 SOP（OR 表题）
> 
> ```
>      看到 OR 表 + 问"显著危险因素"
>                |
>                ▼
>       Step 1: 锁定 Multivariate 栏
>                |
>                ▼
>       Step 2: 逐行看 CI 是否跨 1.0
>           跨 1.0 → 划掉（不是独立危险因素）
>           不跨 → 候选
>                |
>                ▼
>       Step 3: 候选 vs 患者状态
>           没暴露 → 划掉
>           暴露 → ✅ 答案
> ```
> 
> ### Item 2 干扰项排除模板
> 
> | 选项类型 | 适用场景 | 在 case-control 里是否成立 |
> |---|---|---|
> | Differential mortality | RCT / Cohort（有 follow-up）| ❌ Case-control 没有时间维度 |
> | Lack of power | 没显著结果时考虑 | ❌ 本题已有多个显著结果 → power 够 |
> | Limited adjustment for confounders | adjusted 变量少 + 临床上还有其他可能 confounder | ✅ 本题答案 |
> | Misclassification | 诊断标准模糊 / 主观 | ❌ pRIFLE 是客观分级标准 |
> 
> ## 易混陷阱（普适）
> 
> ### 三大 OR 表判读陷阱
> 
> | 陷阱 | 表现 | 修复 |
> |---|---|---|
> | **只看点估计 OR** | 被 OR 11.84 震住直接选 | 永远先看 CI |
> | **看错栏** | 只看 bivariate，忽略 multivariate | "Adjusted 才算数" |
> | **忽略表脚** | 没读 "(adjusted for X, Y, Z)" | 表脚告诉你哪些变量被当作 confounder 控制 — 这些变量在 multivariate 里失去显著性是设计使然（不是 bug）|
> 
> ### 三种 multivariate 表现的不同含义 ⭐
> 
> | Bivariate | Multivariate | 真相 |
> |---|---|---|
> | 显著 | **显著** | ✅ **真独立危险因素** |
> | 显著 | **不显著** | ❌ **伪危险因素**（表观关联其实来自 confounder）/ 或被相关变量"吃掉"信号 |
> | 不显著 | 显著（罕见）| 抑制效应（suppressor effect，偶见）|
> 
> ### "Significant" 的两层含义
> 
> - **统计显著（statistical significance）**：CI 不跨 null / p < 0.05
> - **临床显著（clinical significance）**：效应量大、对临床决策有意义
> - USMLE 默认问"statistically significant" — 用 CI 判
> 
> ### 干扰项配对陷阱（Item 1）
> 
> 出题人会**针对患者状态**设计陷阱：
> - 患者有 acyanotic → 给"acyanotic 是危险因素"的错选项（实际 cyanotic 才是）
> - 患者 CPB 150 min → 给"CPB duration"的错选项（已被调整掉）
> - 患者 moderate acidosis → 给"moderate acidosis"（其实 moderate 不显著，severe 也跨 1.0）
> 
> **永远先看 CI 排除不显著的，再核对患者状态**。
> 
> ## 我为什么错
> 
> 选了 **B. Duration of bypass 150 min**。
> 
> - **被 Bivariate OR 11.84 震住** — 数字最大 → 直觉觉得"它最危险"
> - **没看 Multivariate**：调整后 OR 7.47 但 CI 0.91-16.84 **跨 1.0 不显著**
> - **没看表脚**：(adjusted for age, sex, **and CPB duration**) — CPB duration 本身就是被调整的目标，它在多变量里失去显著性是设计使然
> - **不知道这个考点**：不知道 OR 表判读必须**先看 multivariate，再看 CI**
> 
> **核心陷阱**：USMLE 故意把 bivariate OR 设计得"很惊人"，钓只看点估计、不看 CI、不区分 adjusted/unadjusted 的考生。**点估计 + CI 是一体的，只看点估计 = 半个 Biostats**。
> 
> **Item 2 我做对了**：选 C. Limited adjustment for potential confounders
> - 思路：研究只调整了 age, sex, CPB duration，但术前 creatinine / proteinuria / ACE inhibitor 使用等临床上重要的肾功能相关 confounder 没调整 → 残余 confounding
> 
> ## Memory Hook
> 
> **OR 表三步：① 看 multivariate ② CI 不跨 1.0 ③ 患者真的暴露** — 三条同时满足才是答案。
> 
> **独立危险因素 = multivariate 显著（CI 不跨 1.0）** — 不是"不显著"！
> 
> **"Adjusted for X" 的潜台词** = "X 可能是干扰，我们想消除它，看真相" — 不是"X 重要所以平衡它"。
> 
> 类比：
> - **OR + CI 是"双胞胎"** — 永远一起判读，只看 OR = 只看身高不看体重
> - **Bivariate vs Multivariate = 生肉 vs 熟肉** — 没"调味"（调整 confounder）的是生肉，不可信
> - **OR 再大，跨 1.0 就废**
> - **被列入 adjusted for 列表 = 借给隔壁部门用了** — 它自己原本工作的时间就不够了，不是它没用，是工时分出去了
> 
> 口诀：
> - **"看比值盯 1，看差值盯 0"**（CI 跨 null = 不显著）
> - **"调过的才算数"**（adjusted 优先）
> - **"看到 adjusted for X, Y, Z → 这些就是被控制的 confounder"**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> - **Q: 为什么 CPB duration 同时出现在因子表和表脚 adjusted 列表里？multivariate OR 变小是 bug 吗？**
>   → 不是 bug，是"设计使然"。当一个变量被列入 adjusted 列表，它的解释力已经被"用尽"（用来校正其他变量），再估它自己的独立效应自然变小。加上它和其他因子（如乳酸）可能正相关 → 多重共线性让信号被分走。
> 
> - **Q: 是因为研究者认为它是独立危险因素所以要给他平衡掉？**
>   → ❌ 反了。"Adjusted for X" 的潜台词是"X 可能是 confounder（干扰），我们想消除它的影响，看真相"。**不是**"X 是独立危险因素所以平衡它"。Confounder 和 Independent Risk Factor 是两个完全不同的概念。
> 
> - **Q: 那"独立危险因素"到底怎么判断？**
>   → **Multivariate OR 的 95% CI 不跨 1.0**。本题真正的独立危险因素只有两个：hyperlactatemia ≥6 (OR 4.91, CI 1.26-19.05) + Cyanotic heart (OR 3.62, CI 1.11-11.63)。Item 1 答 hyperlactatemia 因为患者真的暴露（cyanotic 不符合：患者是 acyanotic）。
> 
> - **Q: 主笔记缺不少内容，要手动加还是让 Claude 生成草稿？**
>   → 工作流确定：刷题阶段我（Claude）生成错题卡 + 更新草稿；章节复习完让 Claude Code 整合草稿+错题→正式主笔记。**不手动改主笔记**。草稿用版本递增（v1 → v2 → v3），不每次新建。
> 
> ## 🔗 关联
> 
> - 🔁 同主题错题：
>   - **Q21248 Item 2 同 vignette** — Confounding（做对了，同 stem 两考点 = 高频考法）
>   - 同日 Biostats 系列：
>     - [[mistakes/uworld-mistakes#^Q12685]] Reporting bias
>     - [[mistakes/uworld-mistakes#^Q107800]] ROC 最佳 cutoff
>     - [[mistakes/uworld-mistakes#^Q3941]] Null hypothesis（同样涉及"CI 跨 null value"概念）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/Biostats_Master]]
>   - [[完整笔记/专题笔记/Biostats_6指标决策树_纯净版]]（RR/OR 区分基础）
>   - 待生成主笔记：Hypothesis testing 草稿 v3（本题填充 CI 章节 + 新增 OR 表判读 + Confounder vs Independent Risk Factor 概念）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/儿科]] / [[完整笔记/Peixuan分科笔记/外科]]：CPB 后 AKI 是儿心外术后高频并发症（本题考的是 Biostats，但临床背景可引）
> - 🌱 TODO（待生成衍生）：
>   - 等积累更多 OR/CI 题（forest plot / Kaplan-Meier 等）→ 请 Claude Code 整合 → 生成 [[完整笔记/专题笔记/_衍生_USMLE_OR_CI判读]] 或并入统计推断主笔记
>   - 本题已用于更新 Hypothesis testing 草稿（v3 新增"Confounder vs Independent Risk Factor"核心概念章节）
>   - 本题也是未来 [[完整笔记/专题笔记/_衍生_USMLE_Bias_5大鉴别]] 的 Confounding 章节实战案例（Item 2）
> 
> ## ✅ 复盘行动
> 
> - [ ] 1 周后重做 Q21248 整套 vignette
> - [ ] 默写 OR 表判读三步法
> - [ ] 默写 "CI 跨 null value" 规则（比值类跨 1.0，差值类跨 0）
> - [ ] 默写 Bivariate vs Multivariate 角色差异
> - [ ] 默写 Confounder vs Independent Risk Factor 区别（角色不同 / 处理方式不同）
> - [ ] 默写 USMLE OR 表 5 种题型问法精确对照（独立危险因素 / 最显著危险 / 被 confounding 解释 / lost significance / needs to be controlled）
> - [ ] 找 2-3 道类似 OR 表 / Forest plot 题（UWorld 搜 "odds ratio" / "confidence interval" / "multivariate"）
> - [ ] **关键习惯**：看到 OR/RR/HR 题 → 永远先问"CI 跨 null value 了吗？"
> - [ ] **关键习惯**：看到 unadjusted / adjusted 两栏 → 永远看 adjusted
> - [ ] **关键习惯**：表脚 "(adjusted for X, Y, Z)" 永远要读 — 它告诉你哪些变量被当作 confounder
> - [ ] **修正认知**：之前可能误以为"独立危险因素 = multivariate 不显著"，正确是"multivariate CI 不跨 1.0 才是独立危险"
> 
> ---
> 
> 学科:: Biostats
> 主题:: OR-CI 表格判读
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-12] Biostats / Study Design 判定 — Cohort vs Case-Control (Q20435)
> ^Q20435
> 
> ## Stem 模式
> 研究先按"有/无某诊断"分两组（matched control）→ 多年后查另一个疾病的发生率 → 问 study design。
> 
> ## 核心概念
> **Cohort 的本质 = "按 exposure 分组，比较 incidence"**
> - 时间方向（pro/retro）只决定数据收集方向，不改变 cohort 的本质
> - Retrospective Cohort：暴露分组后，从历史病历回查结局
> 
> ## 普适规则 — Study Design 判定 3 步 SOP
> ```
> Q1：研究问"A → B"？
>     → A = exposure, B = outcome（不管 A 叫不叫 "diagnosis"）
> 
> Q2：研究先按什么分两组？
>     ├─ 按 exposure 分 → COHORT
>     │   ├─ Outcome 已发生，回查历史 → Retrospective
>     │   └─ Outcome 未发生，前瞻追踪 → Prospective
>     ├─ 按 outcome 分 → CASE-CONTROL（always retro, 算 OR）
>     └─ 同时测 exposure + outcome → CROSS-SECTIONAL（算 prevalence）
> 
> Q3：算什么指标？
>     Cohort → RR / Incidence
>     Case-Control → OR
>     Cross-sectional → Prevalence
> ```
> 
> ## High-Yield 对比表 — Observational Study 四类
> 
> | 维度 | Case-Control | Cohort (Retro) | Cohort (Pro) | Cross-Sectional |
> |---|---|---|---|---|
> | **分组依据** | Outcome（有病/无病）| Exposure（暴露/未暴露）| Exposure | 都不分组，同时测 |
> | **方向** | 回顾找暴露 | 回顾查结局 | 前瞻追结局 | 横断面 snapshot |
> | **数据时间** | 历史 | 历史病历 | 未来追踪 | 当下 |
> | **算什么** | **OR** | **RR** | **RR** | **Prevalence** |
> | **能否算 incidence** | ❌ | ✅ | ✅ | ❌（只能算 prevalence）|
> | **适用** | 罕见病、长潜伏期 | 罕见暴露、多结局 | 因果证据最强（观察性中）| 现况调查、生成假设 |
> | **Stem 触发词** | "cases who had X vs controls who didn't" | "exposed vs non-exposed, review records" | "follow up for X years" | "at one point in time" |
> 
> ## 易混陷阱（普适）
> 
> ### ⚠️ 陷阱 1：Diagnosis ≠ Outcome
> "Diagnosis of X" 是中性词，可以是 exposure 也可以是 outcome。
> 判定标准 = 看研究问"A→B"的方向，不看哪个词带 "diagnosis"。
> 
> | "Diagnosis of X" 角色 | 例子 |
> |---|---|
> | Exposure | 精神疾病诊断 → 看是否导致 AMI |
> | Outcome | 吸烟 → 看是否导致肺癌诊断 |
> | Confounder | 糖尿病诊断 → 同时影响吸烟和 CVD |
> 
> ### ⚠️ 陷阱 2：Matched ≠ Case-Control
> Matching（年龄/性别匹配）是**控制混杂的统计手段**，cohort 和 case-control 都能用。
> 判定 study design 的**唯一标准**是"按什么分组"。
> 
> ### ⚠️ 陷阱 3：Retrospective Cohort ≠ Case-Control
> 两者都用"历史数据"，但：
> - Retrospective Cohort：按 **exposure** 分组 → 查 outcome
> - Case-Control：按 **outcome** 分组 → 查 exposure
> 
> ## 我为什么错（个性化）
> **选了 A（Case-Control）。真实错因：把"诊断"误认为"结局"**
> - 看到 "diagnosis of schizophrenia" → 大脑自动等价 "diagnosis = disease = outcome"
> - 于是误判：按 outcome 分组 → Case-Control ❌
> - 真相：精神疾病诊断在本题是 **exposure**，AMI 才是 outcome
> - 二次误导：matched control 触发了"case-control 标志"的条件反射
> 
> **核心教训**：读 stem 第一步永远是问"研究问什么因果方向"，而不是被名词触发条件反射。
> 
> ## Memory Hook
> 
> > **三句话保命口诀**：
> > 1. **"Diagnosis ≠ Outcome"** — 诊断只是标签，不代表它是结局
> > 2. **"看研究问什么，不看用什么词"** — A→B 中 A 就是 exposure
> > 3. **"Matched ≠ Case-Control"** — matching 是统计手段，谁都能用
> 
> > **类比 — 侦探办案**：
> > - Cohort：盯一群嫌疑人（exposed），看谁犯罪（outcome）
> > - Case-Control：先找罪犯（cases），回头查谁接触毒品（exposure）
> > - Cross-sectional：今天去监狱，同时数吸毒 + 犯罪人数
> 
> ---
> 
> ## 🤔 我的提问 / 卡点（学习路径）
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "为什么选 case-control 错？" | 判定 design 看**分组依据**，不看 matching |
> | （自己识别）"我没分清诊断和暴露因素" | **真正的根本错因** — "diagnosis" 是中性词，可以是 exposure 也可以是 outcome |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q7688]] Study Design 判定（Item 2）
>   - [[mistakes/uworld-mistakes#^Q20090]] Cohort vs Case-Control 鉴别
>   - [[mistakes/uworld-mistakes#^Q20283]] Cross-sectional 识别
>   - [[mistakes/uworld-mistakes#^Q20058]] Observational study 类型
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
> - 🏥 跨学科：暂无
> - 🌱 TODO（待生成衍生）：等 Biostats 章节复习完，请 Claude Code 整合 **Q7688 + Q20090 + Q20283 + Q20058 + Q20435** 这 5 道 Study Design 错题 → 生成 [[完整笔记/专题笔记/USMLE_Study_Design决策树]]
>   - **必须包含**：4 类 observational study 对比表 + 3 步判定 SOP + "Diagnosis ≠ Outcome" 陷阱专节 + "Matched ≠ Case-Control" 陷阱专节
>   - **素材已齐，明天可生成** ✅
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q20435（验证 3 步 SOP 是否内化）
> - [ ] 默写 Observational Study 4 类对比表（不看笔记）
> - [ ] 默写 Study Design 3 步判定 SOP
> - [ ] 明天让 Claude Code 生成 [[完整笔记/专题笔记/USMLE_Study_Design决策树]]
> - [ ] 下次看到 "diagnosis of X" → 强制问"X 是 exposure 还是 outcome"
> - [ ] 下次看到 "matched control" → 强制问"按什么分组"
> 
> ---
> 
> 学科:: Biostats
> 主题:: Study Design 判定
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-12] 神经 / Pseudodementia vs AD (AMBOSS-Pseudo78)
> ^AMBOSS-Pseudo78
> 
> ## Stem 模式
> 78 岁男 + **5 周** 健忘 + 危险行为（门没关 / 水龙头开着）+ 失眠 (6-7×/night) + 疲乏 + **lost interest in piano** + PMR + **blunt affect** + labs 正常 (TSH/B12/folate) + **"concerned about memory lapses"** → 问下一步治疗。
> 
> ## 核心概念
> **老年期抑郁可伪装成痴呆 (Pseudodementia)，认知缺陷在 SSRI 4-6 周后可逆**。USMLE 反复考"老人健忘 ≠ 自动 AD" — 必先排可治痴呆 8 大。
> 
> ## 普适规则
> 
> ### Pseudodementia 5 钩子（病人**自己**抱怨；AD 是被**家属**带来）
> 1. 起病数周-月（**快**，不是数年）
> 2. **病人自己关心**（自知力存在）⭐
> 3. 回答 **"我不知道"**（放弃式）— vs AD confabulation
> 4. **抑郁征核心**（≥ 5/9 DSM-5 MDD）
> 5. **抑郁先于认知**
> 
> ### DSM-5 MDD 9 项 = SIG E CAPS + 抑郁情绪（≥ 5/9，≥ 2 周）
> **S**leep / **I**nterest loss / **G**uilt / **E**nergy↓ / **C**oncentration↓ / **A**ppetite / **P**sychomotor agitation/retardation / **S**uicidal + **D**epressed mood
> 
> ### Pseudodementia vs AD 终极鉴别
> 
> | 维度 | Pseudodementia | AD |
> |---|---|---|
> | 起病 | **数周-月** | 数年 |
> | 自知力 | **过度自责** | 缺乏 ("我没问题") |
> | 主诉来源 | **病人自己** | 家属带来 |
> | 回答模式 | "我不知道" | 编造 / 错答 |
> | 抑郁征 | **核心** | 可有但非核心 |
> | 治疗 | **SSRI** | Donepezil → Memantine |
> | 预后 | **可逆** ⭐ | 不可逆 |
> 
> ### 治疗 — SSRI（老人 Citalopram ≤ 20 mg/d，QT 警告）
> 4-6 周认知应改善 → 不改善 = 重查 dementia
> 
> ## 易混陷阱（普适）
> 
> | 陷阱 | 表现 | 修复 |
> |---|---|---|
> | "老人 + 健忘 = AD" | 反射性选 Donepezil | 先查可治 8 大 (Pseudo/B12/甲减/神经梅毒/Lyme/NPH/cSDH/药物毒性) |
> | 漏看速度词 | 5 周 → 不可能 AD | "Over the past X weeks/months" 触发"AD？太快了" |
> | 漏看自知力 | concerned = pseudo 招牌 | "Patient is concerned about..." 必扫 |
> | 漏看抑郁标志 | PMR / blunt / 兴趣丧失 / 失眠 / 疲乏 5 个都在 stem | 强制症状交集 — 哪个病能解释最多？ |
> 
> ## 我为什么错
> 
> 选了 **A. Donepezil**（按 AD 治）。错因 = **pattern**（答题方法）。
> 
> - **反射性诊断**：看到 78 岁 + 健忘就跳 AD → Donepezil
> - **没扫全 stem**：5 个抑郁标志 (PMR / blunt / 兴趣丧失 / 失眠 / 疲乏) 全漏
> - **没识别 "concerned about memory"** = pseudo 金标准（AD 缺乏自知力）
> - **没用可治痴呆 8 大 schema**：labs 正常 + 抑郁征 + 速度快 → 直指 Pseudodementia
> 
> 核心陷阱：**老人 + 健忘 ≠ 自动 AD** — 必须先排可治痴呆 8 大。
> 
> ## Memory Hook
> 
> "**Pseudodementia patients complain; AD patients are brought in**"
> 
> 看到 "**concerned about memory + lost interest + sleep disturbance**" → 0.5 秒锁 Pseudodementia → **SSRI**（不是 Donepezil）
> 
> Pseudodementia 5 个"特别"：起病特别快 / 病人特别担心 / 回答特别消极 ("我不知道") / 抑郁特别明显 / 特别可治（SSRI 4-6 周→逆转）
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> - **Q: 5 周健忘为什么不是 AD？**
>   → AD 起病**数年**（"got lost in own neighborhood" stem 类型）。5 周 = 触发 "Pseudo / B12 / 甲减 / NPH / cSDH / 药物" 分支。
> 
> - **Q: Citalopram 老年人为什么 ≤ 20 mg/d？**
>   → QT 延长 risk — FDA 老人 (≥ 60) 上限 20 mg/d，>40 mg/d 有 Torsades 风险。
> 
> ## 🔗 关联
> 
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^AMBOSS-CJD57]] CJD 误选 FTD（同"反射性诊断 + 单一症状导向"）
>   - 等积累更多痴呆题 → AD / VaD / LBD 实战
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_老年痴呆鉴别决策树]]（可治痴呆 8 大 + Pseudo 5 钩子直接收录）
>   - [[完整笔记/Peixuan分科笔记/psych]]（MDD / SSRI）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/psych]](MDD 诊断标准 SIG E CAPS)
>   - [[完整笔记/Peixuan分科笔记/心内]](Citalopram QT 延长 / 老人 ≤ 20 mg/d)
> - 🌱 TODO：等积累 ≥ 4 道痴呆错题 → 升级 [[完整笔记/专题笔记/_衍生_老年痴呆鉴别决策树]] v2
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做
> - [ ] 默写 DSM-5 MDD 9 项（SIG E CAPS + 抑郁情绪）
> - [ ] 默写 Pseudodementia vs AD 终极鉴别表
> - [ ] 默写可治痴呆 8 大
> - [ ] 关键习惯：看到 "concerned about memory" → 立刻怀疑 Pseudo（不是 AD）
> 
> ---
> 
> 学科:: 神经
> 主题:: Pseudodementia 鉴别
> 状态:: 🟡
> 错因:: pattern

> [!example]- [2026-05-12] 神经 / CJD 招牌识别 (AMBOSS-CJD57)
> ^AMBOSS-CJD57
> 
> ## Stem 模式
> 57 岁男 + **2 个月**进展性认知下降（3 周内 ADL 不能）+ **diffuse involuntary muscle jerking** + **provoked by loud noises** + akinetic mutism + **EEG: triphasic periodic sharp-wave complexes** → 问诊断。
> 
> ## 核心概念
> **CJD = prion 病**，三联：**RPD (数周-月) + Startle myoclonus + EEG 周期性尖波**。12 月内致死，无治疗。
> 
> ## 普适规则
> 
> ### CJD 4 大金标准（2+ 几乎不会错）
> 1. **快速进展性痴呆**（数周-月，< 12 月致死）
> 2. **Startle myoclonus**（响声诱发）⭐ 招牌
> 3. **EEG triphasic periodic sharp-wave complexes**（1 Hz）⭐
> 4. **CSF 14-3-3 protein / RT-QuIC**
> 
> ### 5 种不自主运动鉴别 ⭐
> 
> | 运动 | 特点 | 标志病 |
> |---|---|---|
> | **Tremor**（震颤）| **节律性来回** | PD / 小脑 / ET |
> | **Chorea**（舞蹈）| 不规则流畅快速 | **Huntington** / Sydenham / SLE |
> | **Athetosis** | 缓慢扭转蛇形 | HD 晚期 / 脑瘫 |
> | **Myoclonus**（肌阵挛）⭐ | **突发、短促、闪电样** | **CJD** ⭐ / AD 晚期 / 缺氧 / 癫痫 |
> | **Tic** | 可短暂抑制 | Tourette |
> | **Dystonia** | 持续扭转 | 急性 EPS / 肌张力障碍 |
> 
> ### CJD vs FTD 镜像对照（选项常并列）
> 
> | 维度 | CJD | FTD |
> |---|---|---|
> | 病程 | **数周-月** | **数年** (6-9 年生存) |
> | 首发 | 快速认知 + 神经体征 | **行为 / 性格改变** |
> | 记忆 | 严重受累 | **相对保留**（MMSE 正常）|
> | 运动 | **Startle myoclonus** ⭐ | 晚期 parkinsonism |
> | EEG | **周期性尖波** | 非特异 |
> | 饮食 | 无特殊 | **Hyperorality + 偏甜** |
> 
> ## 易混陷阱（普适）
> 
> - **"jerking" ≠ 震颤 ≠ 舞蹈 = myoclonus**（独立概念，必须建立）
> - **"Blunt affect" 是多义症状**（PD / 抑郁 / 精分 / FTD / CJD / AD 晚期都可能）— 不能单独锁定方向
> - **修饰语必扫**："provoked by loud noises" = startle = CJD 招牌
> - **EEG 旁白必扫**：题 stem 给 EEG = 诊断锁定钥匙，不要忽略
> 
> ## 我为什么错
> 
> 选了 **I. FTD**。错因 = **pattern**（答题方法）。
> 
> - **症状词识别错**：把 myoclonus（闪电样）误读为帕金森样震颤
> - **被 blunt affect 带偏方向**：以为是 masked facies → 帕金森谱 → FTD（"最近邻"匹配）
> - **漏看 startle 修饰语**："provoked by loud noises" = CJD 招牌被忽略
> - **漏看 EEG**：题 stem 直接给 "triphasic periodic sharp-wave complexes" = CJD 锁定金标准
> - **漏看 2 个月**：太快 ≠ AD / FTD / PD / HD（这些都数年）
> 
> 核心陷阱：**被单一症状带偏 + 没做症状交集**。
> 
> ## Memory Hook
> 
> **"Myoclonus = 闪电、瞬间、被电了一下"** → CJD 招牌
> 
> CJD = "数周烂掉 + 响声电一下 + EEG 尖波" 三联
> 
> 看到 "**jerking provoked by loud noises / startle**" → 0.5 秒锁 CJD
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> - **Q: myoclonus 怎么和震颤区分？**
>   → Tremor = **节律性来回**（钟摆）；Myoclonus = **突发、短促、闪电样**（被电了）。CJD 的 myoclonus 还 provoked by startle。
> 
> - **Q: 为什么 FTD 排除？**
>   → FTD 数年进展（不是 2 月）+ 招牌是行为/语言改变（不是 mutism + EEG 异常）+ 无 myoclonus + 无周期性尖波。
> 
> ## 🔗 关联
> 
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^AMBOSS-Pseudo78]] Pseudodementia 误选 Donepezil（同"反射性诊断 + 单一症状导向"模式）
>   - 等后续 PD / HD / TD / Wilson 不自主运动题积累
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_老年痴呆鉴别决策树]]（CJD 4 大金标准 + 痴呆速度分类）
>   - [[完整笔记/Peixuan分科笔记/neuro]]
> - 🏥 跨学科：无（CJD 纯 Neuro）
> - 🌱 TODO：等积累 ≥ 3 道不自主运动错题（PD/HD/TD/Wilson）→ 生成 [[完整笔记/专题笔记/_衍生_不自主运动5种鉴别]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做
> - [ ] 默写 5 种不自主运动鉴别表
> - [ ] 默写 CJD 4 大金标准
> - [ ] 默写 CJD vs FTD 镜像对照
> - [ ] 关键习惯：看到不自主运动词 → 强制问"是震颤 / 舞蹈 / myoclonus / tic / dystonia 哪一种？"
> 
> ---
> 
> 学科:: 神经
> 主题:: CJD 招牌识别
> 状态:: 🟡
> 错因:: pattern

> [!example]- [2026-05-12] 神经 / Syringomyelia 病程演变 (AMBOSS-Syringo62)
> ^AMBOSS-Syringo62
> 
> ## Stem 模式
> 62 岁女 + **MVC 3 年前 (whiplash)** + 1 年进展性双上肢感觉异常 + **手指无痛烫伤数次** + 双侧上肢/上胸 **披肩样温觉↓ + 触觉正常** → 问 further evaluation most likely to show?
> 
> ## 核心概念
> **Syringomyelia 是时间轴疾病**：脊髓中央管空洞**从内向外扩展**，离中央近的纤维先废。"披肩痛温↓" 只是阶段 1，**阶段 2 = Horner**。
> 
> ## 普适规则
> 
> ### Syringomyelia 5 幕剧（从内向外烂）⭐⭐
> 
> ```
> 1️⃣ 前白连合 (anterior white commissure)
>    → 双侧披肩样痛温↓（"painless burns on hands"）
>    → 触觉 / 本体觉 / 运动 全部正常
> 
> 2️⃣ 外侧角 (T1-T2 lateral horn)
>    → 一级交感神经元 → 同侧 **Horner**（ptosis/miosis/anhidrosis）⭐
> 
> 3️⃣ 前角 (anterior horn)
>    → 上肢 **LMN 征**（biceps reflex ↓ 不是 ↑！萎缩 / flaccid）
> 
> 4️⃣ 外侧 CST
>    → 下肢 **UMN 征**（hyperreflexia + Babinski +）
> 
> 5️⃣ Sacral sparing 最后破（CST 最外侧）
>    → 骶段功能最后才丢
> ```
> 
> ⭐ **核心解剖逻辑**：空洞从中央向外扩展 → 谁离中央近谁先废
> 
> ### 病因
> - **Chiari I malformation**（最常见）⭐
> - 创伤后（whiplash / MVC 数年后）
> - 脊髓肿瘤（ependymoma）
> - 脊髓栓系（tethered cord）
> 
> ### Syringomyelia vs Central Cord Syndrome
> 
> | 特征 | Syringomyelia | Central Cord |
> |---|---|---|
> | 起病 | **慢性**（数月-年）| **急性**（创伤即刻）|
> | 年龄 | 年轻 | 老人 |
> | Stem | "Painless burns on hands" | "Fell + neck pain + weak arms" |
> | 病理 | 中央空洞 (cyst) | 中央灰质水肿 |
> 
> ## 易混陷阱（普适）
> 
> ### 干扰项配对（本题）
> 
> | 选项 | 为什么错 |
> |---|---|
> | A. **Exaggerated biceps reflex (↑)** | **方向反了**！Syrinx 在 C5-T1 损伤**前角细胞** → biceps ↓ (LMN)，不是 ↑。UMN 征出现在损伤平面**以下**（下肢）|
> | B. ↓ MMSE | Syringomyelia 不影响认知（MMSE↓ 见于 B12 SCD / Tabes paralytic dementia）|
> | C. ↓ Anal wink reflex | **Sacral sparing** 是 Syringomyelia 特征 — 骶段最后才累 |
> | D. Jaw deviation | CN V 运动核在脑桥，颈段 syrinx 累及不到 |
> | **E. Drooping of eyelid** ✅ | Horner 阶段 2 — 完美匹配病程下一步 |
> 
> ## 我为什么错
> 
> **知识缺口型**（不是答题方法问题）。错因 = **知识**。
> 
> 原话："以前只知道披肩征，从来没听过 Horner 跟这个有关系"
> 
> - 对 Syringomyelia 的知识结构是"**一个症状的疾病**"（披肩痛温↓）
> - 没建立"**时间轴疾病，按阶段发展**"的模型
> - 没意识到 **T1-T2 lateral horn = 一级交感** 这个关键解剖关联
> - Horner 在脑中只关联 Pancoast / 颈动脉夹层 / Wallenberg，**没关联 Syringomyelia**
> 
> 核心陷阱：**单症状疾病模型 vs 病程演变疾病模型** — 很多疾病不是"一个症状"，而是"按时间多症状"。
> 
> ## Memory Hook
> 
> **"5 幕剧：披肩 → Horner → 上肢软 → 下肢硬 → 骶段最后"**
> 
> 演员出场顺序 = 离中央距离的顺序（中央 → 外侧）
> 
> **看到 "painless burns on hands" + Chiari/whiplash 史** → 锁 Syringomyelia → **next step = Horner (ptosis)**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> - **Q: 为什么 biceps reflex 是 ↓ 不是 ↑？**
>   → Syrinx 累及 C5-T1 前角细胞 = LMN 损伤 → 反射 ↓ + 肌萎缩 + flaccid。UMN 征（↑）出现在损伤平面**以下**（下肢），不在上肢。
> 
> - **Q: Horner 怎么和 Syringomyelia 关联？**
>   → T1-T2 lateral horn = 一级交感神经元起点。空洞扩到外侧角时损伤一级交感 → 同侧 Horner = Syringomyelia 阶段 2 招牌。
> 
> ## 🔗 关联
> 
> - 🔁 同主题错题：
>   - 此为首道脊髓不全损伤错题，等后续 Central Cord / Brown-Séquard / Anterior cord / Cauda 积累
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/Horner综合征3级定位与病因]]（一级 Horner 来源题，5 幕剧 + Horner 关联完整）⭐
>   - [[完整笔记/Peixuan分科笔记/neuro]]
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/眼科]]（Horner ptosis vs CN III palsy 鉴别）
>   - [[完整笔记/Peixuan分科笔记/外科]]（颈脊髓 MRI / 减压手术指征）
>   - [[完整笔记/Peixuan分科笔记/儿科]]（Chiari I + Syringomyelia + Tethered cord 神经管发育谱）
> - 🌱 TODO：等积累 ≥ 3 道脊髓不全损伤错题 → 生成 [[完整笔记/专题笔记/_衍生_脊髓不全损伤综合征鉴别]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做
> - [ ] 默写 Syringomyelia 5 幕剧
> - [ ] 默写 Horner 3 级定位
> - [ ] 关键习惯：看到时间轴病（Syringomyelia / MS / PD）→ 问"现在在哪一阶段，下一阶段什么征？"
> 
> ---
> 
> 学科:: 神经
> 主题:: Syringomyelia 病程演变
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-12] 心血管 / Leriche 综合征 + PAD 三联 (AMBOSS-Leriche49)
> ^AMBOSS-Leriche49
> 
> ## Stem 模式
> 49 岁建筑工男 + **35 PY 吸烟** + BMI 34 + BP 169/98 + 父冠心病 + **6 月 ED (sildenafil 无效)** + 腰背 + 大腿痛 + 走路加重休息缓解 + HbA1c 6.2% (< 6.5%) → 问下一步 PE 体征。
> 
> ## 核心概念
> **Leriche = 主髂分叉 (aortoiliac) 闭塞**：三条下游血管同时缺血 → 三联（双侧大腿/臀 claudication + ED + 股动脉↓）。
> 
> ## 普适规则
> 
> ### Leriche 三联征 ⭐
> 1. **双侧大腿/臀部 claudication**（臀肌 + 大腿肌缺血）
> 2. **ED**（内髂动脉 → 海绵体灌注↓，sildenafil 无效）
> 3. **股动脉搏动 ↓/消失**（PE 体征）
> 
> ### Vascular vs Neurogenic Claudication 金表 ⭐
> 
> | 特征 | Vascular (PAD/Leriche) | Neurogenic (Lumbar spinal stenosis) |
> |---|---|---|
> | 走路加重 | ✅ | ✅（两者都加重）|
> | 休息缓解 | ✅ **站着就缓解** | ✅ **需坐下/弯腰** |
> | 站立不动 | 缓解 | ❌ 不缓解 |
> | 骑自行车 | 加重 | ✅ **不加重**（弯腰位）|
> | Pulse | ↓ | 正常 |
> | 影像 | CTA / MRA | MRI 腰椎 |
> 
> ⭐ **黄金口诀**：站立缓解 = Vascular；弯腰缓解 = Neurogenic
> 
> ### PAD 治疗优先级（USMLE 必考顺序）
> 1. **戒烟** > 一切
> 2. **Antiplatelet (ASA / clopidogrel) + Statin** = 降 MI/Stroke 死亡率（不改善走路）
> 3. **HbA1c < 7% + 控 BP**
> 4. Claudication 无 rest pain → **Supervised Exercise Therapy** ⭐ 首选
> 5. 二线：**Cilostazol**（PDE3i；**HF 禁用**）
> 6. CLI / 顽固症状 → Revascularization (PTA / Bypass)
> 
> ## 易混陷阱（普适）
> 
> ### 干扰项配对（本题）
> 
> | 选项 | 为什么错 |
> |---|---|
> | **A. ↓ Bilateral femoral pulses** ✅ | Leriche 体征 — 完美匹配 |
> | B. INO (Internuclear ophthalmoplegia) | MS / 卒中；此人双侧慢性 + 强血管高危 ≠ MS（young female + R&R）|
> | C. Palmar/plantar rash | Secondary syphilis；4 性伴 + 套不规律是诱饵 — 二期梅毒不引起 claudication |
> | D. JVD | 右心衰；CAD 风险因素 ≠ 当前 HF（无水肿/dyspnea/啰音）|
> | E. ↓ Anal tone | Spinal stenosis 是**坐下/弯腰缓解**；本题站立缓解 → 排除 |
> | F. Painless foot ulcer | DM autonomic；**HbA1c 6.2% < 6.5%** 排除 DM；PAD 溃疡 painful |
> 
> ### 性史 / 数字陷阱
> - **4 个性伴 + 套不规律**是 red herring（诱你选梅毒）
> - **HbA1c 6.2%** 故意贴近 6.5% — 让你以为 DM，实际**排除 DM**
> - **风险因素 ≠ 当前疾病**（CAD 风险 ≠ 当下 HF）
> 
> ## 我为什么错
> 
> "没思路" — **完全不认识 Leriche 这个名词**。错因 = **知识**（schema 缺失）。
> 
> - 没建立 "PAD 三联征" schema：ED + 大腿痛 + sildenafil 无效 → 不能 cluster 成一个诊断
> - 没有 "aortoiliac 闭塞同时影响 3 条下游 → 3 个症状" 的解剖映射
> - Stem 信号无法组成 cohesive picture → 任何选项都解释不掉全部信息 → 选不出来
> 
> 核心陷阱：**看到 ED 不要只想泌尿/心理** → 想血管/神经/激素四大方向；**sildenafil 无效**强烈提示**血管源**（不是 cGMP 问题）。
> 
> ## Memory Hook
> 
> **"主动脉分叉堵车，三条路同时瘫痪"** — 内髂 → ED / 臀肌 → 屁股痛 / 股总 → 腿痛 + 脉弱
> 
> **男性 + 双侧大腿臀痛 + ED + sildenafil 无效 + 双股动脉摸不到** → 0.5 秒锁 Leriche
> 
> "**Sildenafil 无效 ED**" → 血管源（不是 cGMP 问题）
> "**走路加重 + 站立缓解 + 脉↓**" → Vascular claudication
> "**坐下/弯腰缓解**" → Neurogenic claudication
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> - **Q: 为什么 sildenafil 无效就提示血管源？**
>   → Sildenafil = PDE5i 扩血管平滑肌（cGMP 增多）。但**没血流可扩 = 不起作用**（上游主髂闭塞 → 海绵体灌注↓）。心理性 / cGMP 异常 ED 用 sildenafil 有效。
> 
> - **Q: HbA1c 6.2% 是不是 DM？**
>   → < 6.5% = 排除 DM（pre-diabetes 5.7-6.4%）。本题故意贴近阈值钓选 F（DM 神经性溃疡）。
> 
> ## 🔗 关联
> 
> - 🔁 同主题错题：此为首道 PAD/Leriche 错题，等后续 Buerger / DVT / Compartment 积累
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]（PAD 章节）
>   - [[完整笔记/Peixuan分科笔记/外科]]（血管外科 PTA vs Bypass）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/心内]]（PAD = CAD 等危症，全身动脉粥样硬化）
>   - [[完整笔记/Peixuan分科笔记/endocrine]]（DM 风险因素 + ABI 假性升高 in CKD/DM 钙化）
>   - [[完整笔记/Peixuan分科笔记/neuro]]（neurogenic claudication 鉴别）
> - 🌱 TODO：
>   - 等下肢缺血题积累 → 生成 [[完整笔记/专题笔记/_衍生_下肢缺血鉴别]]（PAD / Buerger / DVT / Compartment）
>   - 等 ED 题积累 → 生成 [[完整笔记/专题笔记/_衍生_ED鉴别诊断]]（血管 / 神经 / 心理 / 内分泌 / Peyronie）
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做
> - [ ] 默写 Leriche 三联征
> - [ ] 默写 Vascular vs Neurogenic claudication 金表
> - [ ] 默写 PAD 治疗优先级（戒烟 → ASA+Statin → Exercise → Cilostazol → Revasc）
> - [ ] 关键习惯：看到 ED → 强制问"是血管 / 神经 / 心理 / 内分泌 / Peyronie 哪种？"
> 
> ---
> 
> 学科:: 心血管
> 主题:: Leriche 综合征 / PAD 三联
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-12] Biostats / RCT 质量评估 — Randomization Success 判定 (Q4121)
> ^Q4121
> 
> ## Stem 模式
> RCT 的 Table 1 显示两组 baseline characteristics（age, race, HTN 等）相似 → 问最可能的结论。
> 
> ## 核心概念
> **Baseline 相似 = Randomization 成功**
> - Randomization 是 RCT 独有工具，能控制 known + UNKNOWN confounders
> - Table 1（baseline characteristics）= randomization 的"体检报告"
> - 基线相似 → 混杂因素被均匀分配 → 两组可比
> 
> ## 普适规则 — Biostats 题黄金 SOP
> 
> ### 🎯 "题目给什么 → 只能推什么"
> | Stem 给的信息 | 只能推出的结论 |
> |---|---|
> | Table 1（baseline 相似）| Randomization 成功 ✅ |
> | Sample size + effect size + α | Power 评估 |
> | Outcome 数据 + p 值 | Positive / negative study |
> | 盲法描述 | Observer bias 控制 |
> | 分配方法描述 | Allocation concealment 评估 |
> 
> **铁律**：不给的信息 → 不能瞎推（USMLE 选项陷阱专坑这个）
> 
> ## 高频对比表 1 — RCT 4 大质量评估维度 ⭐
> 
> | 维度 | 评估什么 | 看什么信息判定 | 工具 |
> |---|---|---|---|
> | **Randomization success** | 两组可比性 / confounders 均匀分配 | **Table 1**（baseline 相似？）| Randomization |
> | **Adequate sample size** | 是否有足够 power | Sample size calculation（n + effect + α + β）| Power calculation |
> | **Power** | 1−β = 检测真实差异的能力 | n + effect size + α + variability，**与 baseline 无关** | 公式：Power = 1−β |
> | **Bias control** | Observer / performance / recall bias | 是否 blinded（single/double/triple）| Blinding |
> 
> ## 高频对比表 2 — RCT 3 大质控工具（按时间线）⭐
> 
> | 工具 | 发生时间 | 防什么 | 怎么做 | 怎么验证 |
> |---|---|---|---|---|
> | **Randomization** | 分组**那一刻** | Confounding（known + unknown）| 随机数表 / 计算机 | Table 1 基线相似 |
> | **Allocation concealment** | 分组**前** | **Selection bias** | 不透明信封 / 中央分配 | 描述分配方法 |
> | **Blinding** | 分组**后**整个过程 | **Observer / performance bias** | 安慰剂外观一致 / 编码药物 | 描述盲法实施 |
> 
> ### Allocation Concealment 速记
> - 定义：分组**前**，招募者和受试者都**不能预知**下一个人会被分到哪组
> - 没有它的灾难：医生预知分组 → 给重症选新药、轻症选安慰剂 → selection bias
> - 实现方法：不透明信封 / 中央分配系统 / 预编码药物
> - **vs Randomization**：随机化是"用什么方法分组"，AC 是"分组前能不能预知"
> - **vs Blinding**：AC 在分组**前**，blinding 在分组**后**
> 
> ## 高频对比表 3 — Randomization vs Matching（同样产生"基线相似"，机制完全不同）⭐
> 
> | | Randomization | Matching |
> |---|---|---|
> | **出现在** | RCT | Observational（cohort / case-control）|
> | **过程** | 先随机分组 → 后看基线 | 先选一组 → 按特征配对选另一组 |
> | **相似的本质** | 随机化的**副产品**（被动）| 人为强制的**结果**（主动）|
> | **控制 confounders** | known + **UNKNOWN** | **只控制 known** 的那些变量 |
> | **Stem 关键动词** | "**randomly assigned**" / "randomized" | "**matched**" / "selected to match" |
> 
> ## 易混陷阱（普适）
> 
> ### ⚠️ 陷阱 1：把 RCT 的"基线相似"误认为 matching
> RCT 里基线相似 = **randomization** 的副产品，**不是 matching**。
> **判定铁律**：看动词。"randomly assigned" → randomization；"matched" → matching。
> 
> ### ⚠️ 陷阱 2：把 "large-scale" 等同于 "power 大"
> "Large-scale" 是描述性词，不是统计判定。Power 需要 **n + effect size + α + variability** 4 类信息才能评估，光说"大规模"不够。
> 
> ### ⚠️ 陷阱 3：Randomization ≠ Allocation Concealment
> 一个研究可以"randomized"但**没有 allocation concealment**（如奇偶分配 — 医生能预知）。两者必须分开评估。
> 
> ### ⚠️ 陷阱 4：Randomization 防 confounding，Blinding 防 bias
> - **Randomization → 控制 confounding**（已知+未知混杂因素）
> - **Blinding → 控制 bias**(observer / performance bias)
> - 两者**不能互换**，是完全不同的工具
> 
> ## Power 深度速记 ⭐
> 
> ### 4 大决定因素
> | 因素 | 关系 | 比喻 |
> |---|---|---|
> | **Sample size (n)** | n ↑ → Power ↑ | 渔网大小，网越大越能捞鱼 |
> | **Effect size** | ES ↑ → Power ↑ | 差异越明显越容易看出 |
> | **α 水平** | α ↑ → Power ↑（但 Type I error 也↑）| 大门门槛 |
> | **Variability** | 变异 ↓ → Power ↑ | 数据越集中信号越清晰 |
> 
> ### ⚠️ 反直觉警告：α 和 Power 是**同向**变化 ⭐
> 
> **错误直觉**：α 大 = 标准松 = 研究质量差 = Power 小 ❌
> **正确逻辑**：α 大 = 拒绝 H₀ 的门槛低 = 真假差异都更容易被宣布"显著" = Power ↑ + Type I error ↑（同时上升）
> 
> | α 变化 | 大门比喻 | Power | Type I (α) |
> |---|---|---|---|
> | α ↑(标准**松**，如 0.10) | 大门**敞开**，谁都能进 | **↑**(真差异容易抓到) | **↑**(假差异也被误判) |
> | α ↓(标准**严**，如 0.01) | 大门**紧闭**，严查 | **↓**(真差异被漏掉) | **↓**(不冤枉无差异) |
> 
> **核心**：α 和 Power **同向**变化；α 和 β **反向**变化（Power = 1−β）。
> **代价**：调高 α 提升 Power 的同时增加假阳性 → 学术界不接受 → 实践中 α 固定 0.05 → 实际**调控 Power 只能靠 n**。
> 
> ### 📊 一张表锁死所有调整关系 ⭐⭐⭐
> 
> | 调整 | α (Type I) | β (Type II) | Power (1−β) |
> |---|---|---|---|
> | **α ↑**（门槛松）| ↑ | ↓ | **↑** |
> | **α ↓**（门槛严）| ↓ | ↑ | **↓** |
> | **n ↑**（样本量大）| **不变** | ↓ | **↑** |
> | **Effect size ↑**（效应大）| **不变** | ↓ | **↑** |
> | **Variability ↓**（数据集中）| **不变** | ↓ | **↑** |
> 
> **规律**：
> - **α 和 β**（n 固定时）→ **反比**（跷跷板）
> - **α 和 Power** → **正比**（因 Power = 1−β）
> - **n / Effect size / Variability** → **只影响 β 和 Power，不碰 α**
> 
> ### 🎯 终极口诀（背这一句就够）⭐
> 
> > **"α 和 β 反，β 和 Power 反，所以 α 和 Power 正"**
> > 
> > 推导：
> > - α ↕ β（反）
> > - β ↕ Power（反，因为 Power = 1−β）
> > - 反的反 = 正 → **α 和 Power 同向** ✅
> 
> ### ⚠️ 应用层易错点（2026-05-12 暴露的 3 个盲点）
> 
> **盲点 1：方向感 — 反比时要真的反过来**
> - 每次看到 α 变化，**先画箭头**：α ↑ → β ↓ → Power ↑
> - 陷阱：理论懂"反比"，应用时方向搞反
> 
> **盲点 2：n 是"独立变量"，不碰 α**
> - α 是研究者主动设定（默认 0.05），不是算出来的
> - 不管 n 多大，α 仍是 0.05
> - 口诀：**"n 只动 β 和 Power，不碰 α 和 Effect"**
> 
> **盲点 3：USMLE 题干约束词必读**
> - "**不增加假阳性**" / "without increasing Type I" → **排除调 α 的选项**
> - "**仅增加 Power**" → 只能选改 n / effect / variability
> - 陷阱：只看后半句"增加 Power"，忽略前半句的约束 → 错选"调高 α"
> 
> **黄金答题套路**：
> - 问"如何提升 Power" → 优先选 **"增加 sample size"**（唯一不动 α 的合法手段）
> - 问"如何降低 Type I" → 选"调低 α"（但代价是 Power 也降）
> - "p > 0.05 但仍想确认无差异" → 检查是否 **underpowered**（n 是否够）
> 
> ### 4 种假设检验结果
> | | H₀ 真（无差异）| H₀ 假（有差异）|
> |---|---|---|
> | **说"无差异"** | ✅ 正确 | ❌ Type II (β) |
> | **说"有差异"** | ❌ Type I (α) | ✅ **Power (1−β)** |
> 
> ### Power 判定铁律
> 评估 Power 需要：**n + effect size + α + variability**
> Table 1 完全不包含这些信息 → **Table 1 无法判 Power**
> 
> ## 我为什么错（个性化）
> **选了 C（Power is big）。真实错因：双层陷阱**
> 
> ### 错因 1（深层）：上一题（Q20435）的 matching 概念污染了本题判断
> - 刚学完"matched control 是 cohort 也能用"
> - 看到本题"两组相似" → 大脑联想"是不是 matching 做的？"
> - **忽略了 stem 关键词 "randomly assigned"** — 这才是真正的判定信号
> - 没识别"动词决定机制"的原则
> 
> ### 错因 2（表层）：过度联想 + 不懂 Power
> - 没把"randomization successful"当成"直接答案"
> - 觉得正确答案不会"这么简单"，转而选了听起来更复杂的 C
> - 实际上**完全不懂 Power 需要哪些信息**（不知道 Table 1 和 Power 无关）
> 
> **核心教训**：
> 1. **看动词**："randomly assigned" → randomization；"matched" → matching
> 2. **直球选答案**：Biostats 题往往有直接答案，不要绕弯
> 3. **题目给什么 → 只能推什么**：Table 1 只能判 randomization
> 
> ## Memory Hook
> 
> > **三句话保命口诀**：
> > 1. **"看动词，不看结果"** — Randomly assigned → randomization；Matched → matching
> > 2. **"题目给什么 → 只能推什么"** — Table 1 → randomization；n+effect → power
> > 3. **"Randomization 防 confounding，Blinding 防 bias，AC 防 selection bias"** — 三个工具不能互换
> 
> > **类比 — 抽签 vs 配对相亲**：
> > - **Randomization** = 抽签分组，运气好两边均匀（被动相似）
> > - **Matching** = 红娘按特征配对，故意造相似（主动相似）
> 
> > **Power 类比 — 侦探破案**：
> > - Power = 真有罪时成功定罪的概率
> > - n 大 = 证据多；Effect size 大 = 罪行明显
> > - Type I (α) = 冤枉好人；Type II (β) = 放过坏人
> 
> ---
> 
> ## 🤔 我的提问 / 卡点（学习路径）
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "我以为两组相似是被 matched 的结果，怎么区分？" | **真实错因暴露** — 上一题的 matching 概念污染了本题；判定铁律 = 看动词（randomly assigned vs matched）|
> | "Allocation concealment 这个概念以前没见过" | RCT 的 3 大质控工具（按时间线）：randomization（分组那一刻）+ AC（分组前）+ blinding（分组后）|
> | "对 Power 概念不熟悉" | Power = 1−β；4 大决定因素 = n + effect + α + variability；与 Table 1 无关 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q20435]] Cohort vs Case-Control（matched control 概念 — 上一题，导致本题概念污染）
>   - [[mistakes/uworld-mistakes#^Q7688]] Study Design 判定
>   - 本题是 **RCT 质量评估**首题，等后续题积累
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/心内]]（carvedilol 是 systolic HF 三大 mortality-benefit β-blocker 之一：carvedilol / metoprolol succinate / bisoprolol）
> - 🌱 TODO（待生成衍生）：
>   - 等 Biostats 章节复习完，请 Claude Code 整合 **RCT 质量评估类错题**（目前 Q4121，需积累到 3+ 道）→ 生成 [[完整笔记/专题笔记/USMLE_RCT质量评估]]
>     - **必须包含**：RCT 4 大质量评估表 + 3 大质控工具按时间线表 + Randomization vs Matching 区分表 + Allocation concealment 专节 + Power 4 大决定因素 + "题目给什么→只能推什么" SOP
>   - 等 Biostats 章节复习完，请 Claude Code 整合 **Bias 类错题**（Q3941 + Q20090 + Q4121 涉及的 selection / observer bias）→ 生成 [[完整笔记/专题笔记/USMLE_Bias_5大鉴别]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q4121（验证是否还会被 matching 概念污染）
> - [ ] 默写 **RCT 4 大质量评估维度表**
> - [ ] 默写 **RCT 3 大质控工具时间线表**（Randomization / AC / Blinding）
> - [ ] 默写 **Randomization vs Matching 区分表**
> - [ ] 默写 **Power 4 大决定因素** + 4 种假设检验结果
> - [ ] 给 [[完整笔记/Peixuan分科笔记/Biostats_Master]] 加 #薄弱点（Biostats 基础概念欠扎实）
> - [ ] 下次看到"baseline 相似" → 强制问"是 randomized 还是 matched？"（看动词）
> - [ ] 下次看到 Biostats 题 → 强制问"stem 给了什么数据？只能推什么结论？"
> 
> ---
> 
> 学科:: Biostats
> 主题:: RCT 质量评估 — Randomization Success
> 状态:: 🟡
> 错因:: 知识

---

## 2026-05-14

> [!example]- [2026-05-14] Heme-Onc / 抗凝药拮抗剂 4 对（复盘 self-test）
> 
> ## Stem 模式
> 
> "在吃 [Warfarin / UFH / Dabigatran / Apixaban] 的患者 + 急性出血（ICH / GI bleed / 大手术前）→ 拮抗剂 / 逆转策略?"
> 
> ## 核心概念
> 
> 不同抗凝药 → 不同拮抗剂；**不能一律 FFP**。每个 DOAC 有特异性逆转药，按靶点（IIa vs Xa）配对。
> 
> ## 普适规则
> 
> | 抗凝药 | 拮抗剂 | 起效 | 备注 |
> |---|---|---|---|
> | **UFH** | **Protamine sulfate** | 几分钟 | 与 heparin 负电荷结合 |
> | **LMWH**（Enoxaparin）| Protamine（只中和 60%）| 部分有效 | 效果不全，仅紧急时用 |
> | **Warfarin** + 严重出血/ICH | **4F-PCC + Vit K**（不是单独 FFP！）| PCC 几分钟；Vit K 6-24h | PCC 立刻补 II/VII/IX/X；Vit K 修复肝合成 |
> | **Dabigatran**（抗 IIa）| **Idarucizumab** | 5 分钟 | 单克隆抗体 |
> | **Xa-DOAC**（Apixaban / Rivaroxaban / Edoxaban）| **Andexanet alfa** | 几分钟 | 重组诱饵 Xa |
> | **Fondaparinux** | 无特异拮抗 | — | 4F-PCC 部分有效 |
> 
> ## 易混陷阱（普适）
> 
> - **Warfarin 严重出血 ≠ 单独 FFP**：FFP 因子浓度低、需大量输注、TACO 风险 → **4F-PCC + Vit K** 才是首选
> - **Idarucizumab 只对 Dabigatran**（抗 IIa），不能用于 Xa-DOAC
> - **Andexanet alfa 只对 Xa-DOAC**，不能用于 Dabigatran
> - **LMWH 用 Protamine 只中和 60%**，效果不全
> - UFH 静脉用量过大 → Protamine 也要分次用（避免低血压 / 过敏）
> 
> ## 我为什么错
> 
> - 选了：5/14 复盘 4 对全空（"以上都不记得"）+ 题 4 出血处理 4 道全部"不会"
> - 错因：**知识** — 这块完全零基础，从未系统接触
> - 核心陷阱：4 个药名 + 4 个拮抗剂名 = 8 个新词，不背就只能猜
> 
> ## Memory Hook
> 
> - **Idar-a-ru** → 抗 **II-a** (Dabigatran)
> - **And-ex-anet** → 抗 **X-a** (Apixaban / Rivaroxaban)
> - **Protamine** → "拉硫酸根" → 与 Heparin 负电荷结合
> - **Warfarin → 4F-PCC + Vit K** 三件套：**PCC 立刻补因子，Vit K 长效修肝**
> - 一句话：**"看到 Warfarin ICH 不要 FFP，先想 PCC + Vit K"**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "Warfarin ICH 为什么不直接 FFP？" | FFP 因子浓度低 + 需要大量输注（TACO 风险）+ 起效慢；**PCC = 浓缩 II/VII/IX/X + 几分钟起效** = 首选 |
> | "Dabigatran 和 Apixaban 拮抗剂为什么不一样？" | 作用靶点不同（IIa vs Xa），抗体 / 诱饵蛋白**特异性结合** → 必须配对 |
> | "LMWH 为什么 Protamine 只中和 60%？" | Protamine 主要中和 anti-IIa 活性；LMWH 主要靠 anti-Xa 活性，anti-Xa 部分中和不全 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本卡是抗凝药拮抗剂首张卡，等积累
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/hematology oncology]] / [[完整笔记/Peixuan分科笔记/心内]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/neuro]]（Warfarin ICH 紧急逆转最常见 stem）；[[完整笔记/Peixuan分科笔记/GI]]（DOAC GI 出血逆转）
> - 🌱 TODO（待生成衍生）：等抗凝出血题积累到 3+ 道 → 请 Claude Code 整合到 [[完整笔记/专题笔记/_衍生_抗凝药拮抗剂_4对]]
>   - **必须包含**：4 对拮抗剂表 + 起效时间 + 适应/禁忌 + Warfarin 急性出血 SOP（4F-PCC + Vit K 而非 FFP）+ 特异性配对原理（IIa vs Xa）
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 4 道出血处理情境题
> - [ ] 默写 4 对拮抗剂表（含起效时间）
> - [ ] 找 3 道 UW 抗凝出血题
> - [ ] 手动加 #考前必看 / #薄弱点 标签（高频 + 完全空白）
> 
> ---
> 
> 学科:: Heme-Onc
> 主题:: 抗凝药拮抗剂选择
> 状态:: 🟡
> 错因:: 知识

---

> [!example]- [2026-05-14] 肺 / PE 不稳定第一步 — TTE vs TEE，溶栓 vs 取栓（复盘 self-test）
> 
> ## Stem 模式
> 
> "SBP < 90 + 严重呼吸困难 + 怀疑 PE → 下一步?"
> 干扰项常包括：CTPA / TEE / 紧急外科取栓 / IVC filter。
> 
> ## 核心概念
> 
> 不稳定 PE = 高死亡率 → **床旁 TTE 评估 RV strain** → **tPA 溶栓**（**不是 TEE，不是取栓**）。
> 
> ## 普适规则
> 
> | PE 情境 | 诊断第一步 | 治疗第一步 |
> |---|---|---|
> | 稳定 + 低/中可疑 | **D-dimer**（阴性可排）| 抗凝待结果 |
> | 稳定 + 高可疑（Wells > 4）| **CTPA**（不做 d-dimer）| **经验性抗凝**同时进行 |
> | **不稳定**（SBP < 90 / shock）| **床旁 TTE**（看 RV strain）| **tPA 溶栓** + 抗凝 |
> | 抗凝禁忌（近期大出血 / ICH）| CTPA | **IVC filter** |
> | tPA 禁忌 / 溶栓失败 | — | 外科 / 导管取栓（catheter embolectomy） |
> 
> ## 易混陷阱（普适）
> 
> - **TTE ≠ TEE**
>   - **TTE**（Trans**t**horacic）= 床旁、无创、首选；不稳定 PE 看 RV
>   - **TEE**（Trans**e**sophageal）= 食管探头、需镇静；用于**主动脉夹层** / **心内膜炎** / **心房血栓**
> - **不稳定 PE → 溶栓 not 取栓**
>   - tPA 是一线（如无禁忌）
>   - 外科 / 导管取栓只在 tPA 禁忌或溶栓失败时
> - **Wells > 4 高可疑 → 直接 CTPA**，不做 d-dimer（浪费时间 + 假阴风险）
> - **不稳定不等 CTPA**：先床旁 TTE 看 RV → 立刻经验性 tPA（CTPA 需要搬病人去 CT 室，不稳定 PE 风险大）
> - **不要把 stroke LVO 取栓概念搬到 PE**：解剖位置不同，PE 是肺远端弥漫栓子，导管难达
> 
> ## 我为什么错
> 
> - 选了：诊断写 **TEE** / 治疗写 "取栓?"
> - 错因：**知识 + 易混**（TTE/TEE 缩写混；溶栓/取栓概念错搬）
> - 核心陷阱：把"血管内取栓 = stroke 的 LVO 治疗"概念错搬到 PE
> 
> ## Memory Hook
> 
> - **T-T-E** = **T**op (体表) + **T**horacic + **T**rauma bay = 急诊床旁不稳定 PE
> - **T-E-E** = **E**sophagus = 主动脉夹层（看降主动脉）/ 心内膜炎（看瓣膜）/ 房颤血栓
> - 不稳定 PE → **"溶栓 not 取栓"**（PE 是肺动脉远端弥漫栓子，导管难达 → 溶栓全身扩散更合理）
> - **Stroke LVO** 才取栓（颈内 / MCA M1 近端可达）
> - **TTE 看不稳定 PE 的 4 个征**：RV dilation / RV hypokinesis / **McConnell sign**（RV 自由壁运动减弱、心尖部正常）/ D-shaped LV
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "为什么 PE 不取栓但 Stroke 取栓？" | 解剖 + 导管可达性：PE = 肺动脉远端弥漫栓子，导管难全清；Stroke LVO = 近端大血管（颈内 / MCA M1），导管可达 |
> | "TTE 是看什么？怎么提示 PE？" | RV dilation / RV hypokinesis / **McConnell sign** / D-shaped LV → 急性右心衰提示大 PE |
> | "不稳定 PE 为什么不直接 CTPA？" | 不稳定 = 搬动风险大，先床旁 TTE 看 RV 决定是否经验性 tPA；CTPA 仅在能搬动 + 怀疑高时做 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本卡是 PE 第一张卡，等积累
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/pulmonary]] / [[完整笔记/Peixuan分科笔记/心内]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/neuro]]（stroke LVO 取栓窗口 ≤24h 对比 PE 不取栓）；[[完整笔记/Peixuan分科笔记/hematology oncology]]（抗凝禁忌时 IVC filter）
> - 🌱 TODO（待生成衍生）：等 PE / DVT / MI / Stroke / ALI 五急症错题积累到 3+ 道 → 请 Claude Code 整合到 [[完整笔记/专题笔记/_衍生_5急症第一件事决策表]]
>   - **必须包含**：诊断 vs 治疗双列 + Wells 切点（DVT≥2, PE>4）+ TTE vs CTPA 选择逻辑 + 抗凝禁忌分支 + tPA 禁忌时的 IVC filter / 外科取栓分支
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做"不稳定 PE 第一步"情境题
> - [ ] 默写 PE 5 情境 → 诊断 / 治疗第一步双列表
> - [ ] 找 3 道 UW 不稳定 PE 题
> - [ ] 找 1 道 TEE 适应症题（主动脉夹层 / 心内膜炎）对比记忆
> - [ ] 手动加 #考前必看 / #薄弱点 标签
> 
> ---
> 
> 学科:: 肺
> 主题:: PE 不稳定第一步
> 状态:: 🟡
> 错因:: 知识

---

> [!example]- [2026-05-14] 心血管 / Ruptured AAA vs 出血性胰腺炎陷阱 (Q4212)
> ^Q4212
> 
> ## Stem 模式
> 老年男性（>60）+ 吸烟史 + HTN / 动脉粥样硬化 + **突发**剧烈腹痛 + 低血压 / 心动过速 + **flank ecchymoses (Grey Turner sign)** + 无 rigidity / guarding → **Ruptured AAA**（腹膜后破裂型）
> 
> ## 核心概念
> **Grey Turner sign = "腹膜后出血"邮编，不是"胰腺炎"姓名。**
> 鉴别靠 demographics + 起病速度 + 伴随症状，**不是**靠体征本身。
> 
> ## 普适规则
> 
> **① AAA 急诊决策树（必背）**
> 
> | 场景 | 下一步 |
> |---|---|
> | 不稳定 + **已知** AAA | → 直接 OR（emergent repair） |
> | 不稳定 + **无既往**史 | → **床旁超声**确诊 → OR |
> | 稳定 + 症状性 | → **CT 腹部** |
> 
> **② Grey Turner sign 鉴别（按 USMLE 考频排序）**
> 
> | 病因 | Demographics + 关键线索 |
> |---|---|
> | Ruptured AAA | > 60 男性吸烟 + 突发崩溃 + 无 N/V |
> | Hemorrhagic pancreatitis | 酗酒 / 胆石 + 数小时渐进痛 + N/V / 发热 + 放射背 |
> | 抗凝相关腹膜后血肿 | 老年 + Warfarin / DOAC + INR ↑ |
> | 心导管术后股动脉穿刺并发症 | 介入术后突发侧腹痛 + 血压降 |
> | 骨盆骨折大出血 | 外伤史 |
> 
> **③ 主动脉破裂统一机制（推导口诀）**
> 高压血流穿透周围薄浆膜 / 筋膜：
> - 升主动脉 → 心包（小密封袋）→ **心包填塞**
> - 胸降主动脉 → 后纵隔 → 穿左纵隔胸膜 → **纵隔增宽 + 左侧血胸**
> - 腹主动脉破口朝后 / 侧 → **腹膜后填塞**（80%，可短暂稳定 → Grey Turner）
> - 腹主动脉破口朝前 → 穿壁层腹膜 → **腹腔大出血**（20%，到院前死亡）
> 
> ## 易混陷阱（普适）
> - ❌ **体征 ≠ 疾病**：经典体征（Grey Turner / Cullen / Murphy / Janeway）都指向"病理过程"而非"具体病"
> - ❌ **"Sudden onset" + 循环崩溃 ≠ 胰腺炎**：胰腺炎是 "acute" 但渐进性（数十分钟-数小时），不是"秒级崩溃"
> - ❌ **"No rigidity / guarding" 不能用来鉴别 AAA vs 早期胰腺炎**（两者都符合，因为都在腹膜后）
> - ❌ **不稳定患者 ≠ 先查 lab**：amylase / lipase 在急诊几乎从不是 next step（不影响处理 + 延误抢救）
> - ❌ **不稳定 + 已知 AAA ≠ 先做 CT**（转运延误致命，直接 OR）
> - ❌ **不稳定 + 无既往 AAA ≠ 直接 OR**（万一不是 AAA，开错刀 — 先床旁 US）
> 
> ## 我为什么错
> - 选了：**D. Serum amylase and lipase**
> - 错因：**pattern**（"看到 flank ecchymoses 就想到急性胰腺炎"——做了**体征 → 疾病**的一对一映射，跳过 demographics（62yo 男 + 30 包年吸烟 = AAA 经典画像）、起病速度（sudden collapse ≠ 胰腺炎）、伴随症状（无 N/V / 发热 / 酗酒史）的整合）
> - 核心陷阱：Grey Turner 不是胰腺炎专属，是"腹膜后出血"的多病因体征
> 
> ## Memory Hook
> **"老烟枪 + 突发腹痛 + 倒下 + 侧腹瘀斑 = AAA 破了，不是胰腺爆了。"**
> 
> Grey Turner 是**邮编**（腹膜后出血），不是**姓名**（具体病）。同邮编住户：AAA / 出血胰腺炎 / 抗凝血肿 / 外伤 / 介入术后血肿。
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | 急性胰腺炎不会 sudden onset？ | 可以 acute，但不会"秒级崩溃"；崩溃式起病 = **血管事件** |
> | 急性胰腺炎也没有腹膜刺激征吧？ | 早期对，晚期 / 重症可有（胰酶腹腔渗漏 → 化学性腹膜炎）|
> | Grey Turner sign 还见于什么？ | 抗凝血肿 / 心导管术后 / 骨盆骨折 / 腹膜后肿瘤出血 → 完整鉴别表 |
> | 主动脉哪段在腹腔，哪段在腹膜后？ | 全段主动脉都不在腹腔；腹主动脉全在腹膜后（SAD PUCKER 速记）|
> | 后纵隔出血为什么进左胸腔？ | 高压血流穿透薄的左侧纵隔胸膜 → "纵隔增宽 + 左血胸"是同一过程两时点 |
> | 腹主动脉在腹膜后，怎么破到腹腔？ | 前壁破口高压撕穿壁层腹膜；和胸主动脉穿胸膜同一机制 = **主动脉破裂统一机制** |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本题首张 AAA / 主动脉急症卡，等积累
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_主动脉急症决策树]] ⭐（本题落地的衍生笔记）
>   - [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别|读题策略 Part 7 — 体征 ≠ 疾病]] ⭐（本题贡献的方法论模块）
>   - [[完整笔记/Peixuan分科笔记/心内]] / [[完整笔记/Peixuan分科笔记/外科]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/GI]]（出血性胰腺炎是 AAA 最常考鉴别；Grey Turner 在心血管 / GI 共享）
> - 🌱 TODO（待生成衍生）：
>   - 累计 3+ 道"体征 ≠ 疾病"陷阱题（Grey Turner / Cullen / Murphy / Rovsing）→ 补入 [[完整笔记/专题笔记/_衍生_高频陷阱]] 新增章节"经典体征的多病因鉴别"
>   - 累计急诊影像选择题（CT vs US vs X-ray vs MRI）3+ 道 → 生成 [[完整笔记/专题笔记/_衍生_急诊影像决策]]
>   - 累计 aortic dissection 错题 → 补 _衍生_主动脉急症决策树 Part 6
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q4212，目标 < 60 秒选对
> - [ ] 默写 AAA 急诊决策树（4 分支：stable / unstable × known / unknown）
> - [ ] 默写 Grey Turner 5 大病因 + 鉴别表
> - [ ] 默写主动脉四段破裂统一机制
> - [ ] 找 3 道类似题：AAA stable 处理 / Aortic dissection / 出血性胰腺炎（反向题）
> - [ ] 建立"体征 ≠ 疾病"思维：先问"指向什么病理过程"，再问"哪些病能造成这过程"
> - [ ] 手动加 #考前必看 标签（高频 + 经典陷阱）
> 
> ---
> 
> 学科:: 心血管
> 主题:: Ruptured AAA vs 出血胰腺炎（Grey Turner 多病因鉴别）
> 状态:: 🟡
> 错因:: pattern

---

> [!example]- [2026-05-14] 内分泌 / 急诊 / Adrenal Crisis vs Anaphylaxis (Q17169)
> ^Q17169
> 
> ## Stem 模式
> 慢性病程（数月）+ 应激事件触发（手术 / 操作 / 麻醉）+ **难治性低血压**（refractory to fluids）+ **无过敏征**（无皮疹 / 喉水肿 / wheezing）+ **PAI 五联指纹**（Na↓ / K↑ / HCO3↓ / Glu↓ / Eos↑）→ **Adrenal crisis on chronic PAI**
> 
> ## 核心概念
> **PAI 危象主要由醛固酮缺乏驱动**（容量丢失 + 高钾），cortisol 缺乏使升压药无效（α₁ 受体需 cortisol 才能工作）。这就是为什么 PAI crisis 比单纯 cortisol 缺乏（如外源激素停药）更凶险 —— **原发缺三样，继发 / 三发只缺一样**。
> 
> ## 普适规则
> 
> **① PAI 五联实验室指纹（必背锁定法）**
> 
> | 指标 | 改变 | 机制 |
> |---|---|---|
> | **Na** | ↓（≈ 130）| Aldo↓ 排 Na + cortisol↓ 致 ADH↑ |
> | **K** | ↑（≈ 5.1）| Aldo↓ → K 潴留 |
> | **HCO3** | ↓（≈ 20）| Aldo↓ → H+ 排泌↓（正常 AG 代酸，HARDASS 的 A）|
> | **Glucose** | ↓（< 70）| Cortisol↓ → 糖异生↓ |
> | **Eos** | ↑（> 5%）| Cortisol↓ → 解除 Eos 抑制 |
> 
> **见任意 3 个 → 想 PAI；4 个 → 高度怀疑；5 个 → 几乎确诊**
> 
> **② Adrenal Crisis vs Anaphylaxis 鉴别**
> 
> | 维度 | Adrenal Crisis | Anaphylaxis |
> |---|---|---|
> | 病程 | 慢性背景 + 急性触发 | 纯急性，分钟内 |
> | 皮肤 / 气道 | 无急性皮疹 / 喉水肿 | **必有**皮疹 / 喉水肿 / wheezing |
> | SaO2 | 正常 | 多 < 90% |
> | Na / K / Glu | Na↓ / K↑ / Glu↓ | 正常 |
> | 对补液反应 | **Refractory** | 部分有效 |
> | 第一步处理 | **Hydrocortisone IV + 补液** | **IM epinephrine** |
> 
> **③ 三种 AI 鉴别（原发 vs 继发 vs 三发）**
> 
> | | Primary (PAI) | Secondary (垂体) | Tertiary (外源激素停药) |
> |---|---|---|---|
> | Cortisol | ↓ | ↓ | ↓ |
> | Aldosterone | **↓↓** | 正常 | 正常 |
> | ACTH | ↑↑ | ↓ | ↓ |
> | K | **↑** | 正常 | 正常 |
> | 皮肤色素 | **有** | 无 | 无 |
> | 危象严重度 | 最重 | 中 | 中 |
> | 治疗 | hydrocortisone + fludrocortisone | hydrocortisone | hydrocortisone |
> 
> **口诀**："原发缺三样，继发 / 三发只缺一样" → PAI crisis 最凶
> 
> **④ 应激分级 + Stress Dose Steroid（围手术期高频）**
> 
> | 级别 | 典型情境 | Stress Dose |
> |---|---|---|
> | 轻度 | 牙科 / 局部小手术 / 内镜（无镇静）| 维持原剂量 或 hydrocortisone 25 mg IV |
> | **中度** | **内镜 + 镇静**（本题）/ 疝 / 胆囊 / 关节镜 / 中等感染 | Hydrocortisone **50 mg IV** + 25 mg q8h × 24h |
> | 重度 | 大手术 / 重症脓毒症 / 严重创伤 / 烧伤 | Hydrocortisone **100 mg IV** + 50 mg q8h × 48-72h |
> | 危象 | 已发生 crisis | **100 mg IV bolus** + 200 mg/24h infusion |
> 
> **首选 hydrocortisone**（同时有糖 + 部分盐皮质活性），dexamethasone 用于不干扰 cortisol 测定时
> 
> **⑤ Eos↑ 完整鉴别（修正 "Eos↑ = 过敏" 反射）**
> 
> ```
> Eos↑ → 先看伴随线索：
> ├─ 伴 Na↓ / K↑ / Glu↓ ────→ ★ PAI / Addison's
> ├─ 伴皮疹 / wheezing ───→ Anaphylaxis
> ├─ 伴用药 + 皮疹 + 发热 ─→ DRESS
> ├─ 伴旅行 / 移民 ──────→ 寄生虫
> ├─ 伴哮喘 + 鼻息肉 ────→ AERD / EGPA
> ├─ 伴食管 / 食物过敏 ──→ 嗜酸性食管炎
> └─ 伴 AKI + 用药 + 皮疹 → AIN
> ```
> 
> **⑥ "应激" 完整清单**（PAI 患者遇到任何一个都警惕 crisis）
> - 手术 / 内镜 + 镇静 / 拔牙 / 介入操作
> - 感染（任何）/ 创伤 / 烧伤
> - DKA / 大出血 / MI / 卒中 / 分娩
> - 药物：**Etomidate**（11β-羟化酶抑制）/ 酮康唑 / Rifampin
> 
> ## 易混陷阱（普适）
> - ❌ **症状不特异 → 死记症状**：体重↓ / GI / 疲劳 单独看极不特异，**必须靠"组合 + 实验室指纹 + 慢性病程"三层锁定**
> - ❌ **Eos↑ = 过敏**：Eos↑ 在 PAI 是 cortisol 缺乏的"反向指纹"，不是过敏证据
> - ❌ **GI 症状几个月 = 来就诊的原因**：USMLE 不写废话，慢性病程是诊断核心舞台
> - ❌ **"refractory to fluids" 不当线索**：补液无效是 adrenal crisis 的**特征性表现**（α₁ 受体无 cortisol 不工作）
> - ❌ **SaO2 95% on room air = 正常**：注意 "on what FiO2"——若 on 2L NC 则隐性低氧；on RA = 真正常 = 排除呼吸源性休克
> - ❌ **Imaging unrevealing = 没线索**：在 USMLE 里 ≈ 90% 是引导你想内分泌 / 功能性病因
> - ❌ **答案选项陷阱**：PAI crisis 主要驱动因素 = **aldosterone deficiency**，不是 cortisol deficiency（UWorld 立场）
> 
> ## 我为什么错
> - 选了：**B. Anaphylaxis**
> - 错因：**pattern**（在两个看似合理诊断间错切换 — 看到 Na↓ / K↑ 想 A，又看到 Eos 12% + propofol 暴露切换到 B；默认 Eos↑ = 过敏的反射映射）
> - 核心陷阱：**症状不特异 → 看实验室指纹**。症状是干扰项，指纹才是锚点
> 
> **具体错位**：
> - ☑ 没整合"慢性背景 + 急性触发"双时间轴（数月病程 + 10kg 减重是 PAI 舞台，propofol 只是按下开关）
> - ☑ 不知 Eos↑ 是 PAI 经典指纹（默认 Eos↑ → 过敏）
> - ☑ 忽略阴性体征：stem 写 "no oropharyngeal abnormality, no wheezing, no skin rash" + SaO2 95% 共 5 条反向证据全部排除 anaphylaxis，被五联里 Eos 一项拽过去
> - ☑ 没用 "refractory to fluids" 做判别
> 
> ## Memory Hook
> 
> **🎯 指纹思维**（最重要的认知升级）：
> > "症状不特异时，回到实验室。**PAI 五联指纹 = 全 USMLE 内分泌最特征的组合**。看到 4-5 项同现 → 直接锁定，跳过症状迷雾。"
> 
> **一句话锁定**：
> > "数月减重 + 操作中突然倒下 + 补液无效 + 低钠高钾高嗜酸 = 肾上腺危象，先给氢可的松。"
> 
> **类比**：
> - **PAI 患者 = 没电池的备用发电机**：平时勉强，应激就完蛋
> - **Cortisol = 血管的"扩音器"**：没它，肾上腺素再吼血管也听不见
> - **"原发缺三样，继发 / 三发只缺一样"**：PAI 危象最凶
> 
> **🔍 阴性体征红圈扫读法**（USMLE 读题升级）：
> ```
> 做题流程：
> 1. 第一遍：定位阳性核心症状 → 初步诊断 1-2 个
> 2. 第二遍：扫所有 no / without / negative / normal / unremarkable → "红圈"标记
> 3. 第三遍：每个候选诊断 × 阴性体征核对
> 4. 反推：如果答案是 X，stem 应该写什么？现在写了什么相反的？
> ```
> 高频触发语言：no / no evidence of / negative for / without / denies / unremarkable / X is normal / imaging unrevealing / **no improvement with X**（最关键）
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | Cortisol 减少会嗜酸增高？ | 对，cortisol 是 Eos 生理抑制因子；缺乏时解除抑制 → PAI 指纹之一 |
> | 两者都低血压休克，如何鉴别？ | 病程（慢 / 急）+ 皮肤气道（有 / 无）+ SaO2（正常 / 降）+ 对补液反应（无效 / 有效）+ 实验室指纹（5 联 / 正常）|
> | GI 病史是否就是来就诊原因？ | 不，USMLE 不写废话；10kg 减重 + 数月慢性 = PAI 诊断核心舞台 |
> | Addison's 为什么有体重下降 + GI 症状？ | 4 通路：食欲↓（cortisol↓ 致食欲↓）+ 容量丢失 + 糖异生缺陷致肌肉分解 + 慢性疲劳致活动↓ |
> | 症状非特异认不出来怎么办？ | **指纹思维**：跳过症状看实验室；建立"实验室指纹诊断大全" |
> | 读题时忽略阴性体征怎么办？ | **红圈扫读法**：每道题强制扫 no / without 并核对每个候选诊断 |
> | 麻药算应激吗？ | 算（中度应激）；触发因素是 propofol + 操作 + 禁食 + 焦虑的复合应激 |
> | SaO2 95% 算降低吗？PAI 怎么解释？ | 正常下限，不算 hypoxemia；PAI 不影响 SaO2，95% 的作用是排除 anaphylaxis / PE 而非 PAI 证据；**必看 "on what FiO2"** |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本题首张内分泌 / 急诊 AI 卡，等后续 PAI / Cushing / 继发 AI / 应激剂量激素题积累
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_肾上腺皮质功能不全决策树]] ⭐（本题落地的衍生笔记）
>   - [[完整笔记/专题笔记/_衍生_实验室指纹诊断大全]] ⭐（PAI 五联触发本索引建立）
>   - [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别|读题策略 Part 5 + 6 — 指纹思维 + 慢性 / 急性双轴]] ⭐（本题贡献的方法论模块）
>   - [[完整笔记/Peixuan分科笔记/endocrine]] / [[完整笔记/Peixuan分科笔记/心内]]（休克鉴别）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/外科]]（围手术期 stress dose 激素管理）
>   - [[完整笔记/Peixuan分科笔记/感染]]（Waterhouse-Friderichsen → 急性 AI）
>   - [[完整笔记/专题笔记/_衍生_主动脉急症决策树]]（与昨日 Q4212 形成"难治性休克"系列）
> - 🌱 TODO（待生成衍生）：
>   - 累计 3+ 道"难治性休克鉴别"题（adrenal crisis / cardiogenic / 主动脉破裂失血 / 神经源 / 脓毒症）→ 生成 [[完整笔记/专题笔记/_衍生_难治性休克鉴别]]
>   - 累计 3+ 道"嗜酸增高鉴别"题 → 生成 [[完整笔记/专题笔记/_衍生_嗜酸增高鉴别诊断]]
>   - 累计 3+ 道阴性体征陷阱题后 → 生成 [[完整笔记/专题笔记/_衍生_读题策略_阴性体征]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q17169，目标 < 90 秒选 A
> - [ ] 默写 **PAI 五联指纹** + 每项机制
> - [ ] 默写 **Adrenal Crisis vs Anaphylaxis 6 项鉴别**
> - [ ] 默写 **三种 AI 鉴别表**（原发 / 继发 / 三发）
> - [ ] 默写 **应激分级 + stress dose**（4 个级别 + hydrocortisone 剂量）
> - [ ] 默写 **Eos↑ 6 路鉴别决策树**
> - [ ] 找类似题：① secondary AI ② 围手术期 stress dose ③ Waterhouse-Friderichsen ④ etomidate 诱发 AI ⑤ 长期激素停药致 crisis
> - [ ] 给 [[完整笔记/Peixuan分科笔记/endocrine]] 加 #要做题
> - [ ] **建立"指纹思维"习惯**：以后做内分泌 / 代谢题，先扫实验室异常组合再看症状
> - [ ] **建立"阴性体征红圈扫读"习惯**：每道 UW 题强制走三遍读题流程
> - [ ] **修正 "Eos↑ = 过敏" 反射**：见 Eos↑ 强制走 6 路决策树
> - [ ] **建立"慢性背景 + 急性触发"思维**：见"数月-数年症状" + "突发事件"默认想慢性病急性失代偿
> 
> ---
> 
> 学科:: 内分泌
> 主题:: Adrenal Crisis vs Anaphylaxis（PAI 五联指纹）
> 状态:: 🟡
> 错因:: pattern

---

> [!example]- [2026-05-14] 外科 / 程序性安全 / CVC 置入后必做 CXR (Q3504)
> ^Q3504
> 
> ## Stem 模式
> 严重感染（脓毒症 / 肾盂肾炎）+ 详细描述 CVC 置入步骤（位点 + 穿刺 + 置管 + 缝合 + 敷料）+ "next step in management" → **程序性安全题**：CVC 用之前必须 CXR 确认
> 
> ## 核心概念
> **CVC 置入完成 → 用之前必须做 portable CXR**，确认 tip 在 lower SVC + 排除气胸 / 血胸 / 异位。这是 patient safety 标准操作流程，**不是临床决策题**。位置未确认前不能给药 / 补液 / 输血。
> 
> ## 普适规则
> 
> **① CVC 三大穿刺点对比（USMLE 必背）**
> 
> | 维度 | **IJV（内颈）** | **Subclavian（锁骨下）** | **Femoral（股）** |
> |---|---|---|---|
> | 默认地位 | **首选**（超声引导）| 长期通路 / 患者舒适 | 急诊 / CPR 中 |
> | 气胸风险 | 低 | **最高** ★ | 无 |
> | 感染风险 | 中 | **最低** | **最高** ★ |
> | 可压迫止血 | ✓ | **✗** | ✓ |
> | DVT 风险 | 低 | 低 | **最高** |
> | CPR 中可用 | ✗ | ✗ | **✓** |
> 
> **② CVC 选位决策**
> 
> | 临床情境 | 首选位点 | 避免 |
> |---|---|---|
> | 一般 ICU 患者 | **IJV（超声）** | — |
> | 凝血障碍 | IJV / Femoral | SC（不可压迫）|
> | COPD / 肺气肿 | IJV / Femoral | SC（气胸代偿差）|
> | 拟血液透析 | IJV / Femoral | **SC**（中心静脉狭窄影响 fistula）|
> | CPR 中 / 心脏骤停 | **Femoral** | IJV / SC（干扰胸外按压）|
> | 长期 + 患者要活动 | SC / PICC | Femoral |
> 
> **③ CVC 置入流程 + 置后必做 CXR**
> 
> ```
> 1. 知情同意 + Time-out
> 2. Trendelenburg（IJV / SC）+ 严格无菌 + Chlorhexidine
> 3. 超声 / 标志定位
> 4. Seldinger 技术（针 → 丝 → 扩张 → 管 → 拔丝）
> 5. 抽血回确认 + 冲管
> 6. 缝合固定 + 敷料
> 7. ⭐ Portable CXR（IJV / SC 必做；Femoral 可省）⭐
>    确认：tip 在 lower SVC (T4-T6) + 无气胸 + 无血胸 + 无异位
> 8. ⭐ 确认后才能用 ⭐
> ```
> 
> **④ CVC 并发症（按时序）**
> 
> | 时间 | 高频并发症 | 关键处理 |
> |---|---|---|
> | **置入即刻** | 气胸（SC 最高）| 小 → 观察；大 / 有症状 → 胸管 |
> | | 动脉穿刺（颈动脉 / 锁骨下动脉）| 压迫；已置管 → 血管外科 |
> | | 空气栓塞（"machinery murmur"）| **左侧卧位 + Trendelenburg + 100% O2** |
> | | 心律失常（tip 入右房）| 回撤 1-2 cm |
> | | 心包填塞（穿心房，罕见致命）| 紧急心包穿刺 |
> | | 胸导管损伤（左侧）| chylothorax → 引流 + 禁脂 |
> | **早期（数天）** | 导管闭塞 | tPA 溶栓 |
> | **晚期（> 48-72h）**| **CRBSI** ⭐ | 拔管 + 培养 + 抗生素 |
> | | 血栓（导管相关 DVT）| 抗凝 ± 拔管 |
> | | 中心静脉狭窄（长期 SC）| 介入扩张 |
> 
> **⑤ CVC 并发症 stem 识别**
> 
> | Stem 关键词 | 诊断 |
> |---|---|
> | SC 置入后突发胸痛 + 单侧呼吸音↓ | 气胸 |
> | IJV 高压鲜红血回 | 颈动脉穿刺 |
> | 置入后突发低血压 + 缺氧 + 杂音 | **空气栓塞** |
> | tip 入右房后 VT | 导管诱发心律失常 → 回撤 |
> | 置入后突发休克 + Beck 三联 | 心包填塞 |
> | 留置 > 48h 新发发热 + 阳培养 | CRBSI |
> | 左侧 SC 后乳糜样积液 | Chylothorax |
> | 长期 SC 后上臂 / 面部水肿 | 中心静脉狭窄 |
> 
> **⑥ Procedure & Safety 通用原则 ⭐**
> 
> | 操作 | 置入后确认方式（金标准）|
> |---|---|
> | ET 管 | **Capnography（end-tidal CO2）** |
> | NG 管 | **CXR** |
> | CVC | **CXR** |
> | A-line | **动脉波形** |
> | 胸管 | **CXR** |
> | LP | 脑脊液流出 |
> 
> **铁律**：位置未确认前 → 不给药 / 不补液 / 不输血 / 不喂食
> 
> ## 易混陷阱（普适）
> - ❌ **临床优先级 = 跳过安全检查**：脓毒症 1 小时 bundle 紧迫，但不能跳过 CVC 位置确认；走外周 IV 给抗生素即可
> - ❌ **"治疗合理" = "下一步正确"**：A（抗生素）/ C（补液）治疗方向对，但**顺序错** — 未确认导管不能用
> - ❌ **"听呼吸音正常 = ET 在气管"**：食管插管也可能听到呼吸音；金标准是 **capnography**
> - ❌ **"抽出血回 = CVC 在静脉"**：抽血回只证明在血管内，**不证明在静脉而非动脉**；动脉穿刺也有血回
> - ❌ **超声引导第一针成功 = 可省 CXR**：理论可省，但实践仍多数做；本题盲穿（landmark）无资格省
> - ❌ **Bedside echo = CXR 替代**：技术可行但需熟练操作者；**CXR 是 standard of care**
> - ❌ **Femoral 是劣等位点**：不是！急诊 / CPR / 凝血障碍 / COPD 时是**首选**
> - ❌ **A-line 可给药**：严禁！误注会致远端组织坏死
> 
> ## 我为什么错
> - 选了：**A. Antibiotic through the catheter**
> - 错因：**pattern**（被"脓毒症 1 小时 bundle"劫持，直接跳到给抗生素，忽略"刚置完导管未确认"程序性前提 = 题型识别错位）
> - 核心陷阱：**"治疗合理但顺序错" — 临床优先级 ≠ 跳过安全检查**
> 
> **具体错位**：
> - ☑ 没识别题型：这是**程序性安全题**（procedure question），不是临床决策题
> - ☑ 被疾病严重度劫持：紧迫感跳过了安全检查
> - ☑ CVC 标准流程盲点：不知道置入后必做 CXR
> - ☑ 没注意 stem 详细描述置管步骤：USMLE 描述详细操作 = 在考程序细节
> 
> ## Memory Hook
> 
> **🎯 一句话锁定**：
> > "CVC 置完 → 先拍片，后用药。没拍片的 CVC 是危险品，不是通路。"
> 
> **🎯 类比**：
> CVC = 新装的电源插座 → 通电前必须测一下（CXR），否则烧设备（药物入错腔）
> SC + landmark = "盲打"，越盲打越要拍片
> 
> **🎯 USMLE 程序题识别信号**（重要方法论）：
> 看到这 4 个信号 → 是程序性安全题，不是临床决策题：
> 1. Stem 详细描述某个**操作过程**（CVC / 腰穿 / 胸管 / 内镜 / 手术）
> 2. 问 "best next step" 但操作刚结束
> 3. 选项里有"确认 / 影像"类（CXR / US）和"治疗"类（药 / 液）并存
> 4. 临床背景看似紧急（让你想跳步骤）
> 
> → 答题原则：**永远先选"确认 / 安全检查"，再选"治疗"**
> 
> **🎯 "三个统一安全原则"**：
> 1. 知情同意（除非救命急）
> 2. Time-out 三方核对（患者 + 操作 + 位点）
> 3. **影像 / 波形确认 → 才能用**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | 这道题考点是什么没明白 | 程序性安全题（patient safety），不是脓毒症治疗题 |
> | CVC 选位怎么决策 | IJV 默认首选；急诊 / CPR → Femoral；凝血 / 血透 → 避 SC；长期 / 活动 → SC / PICC |
> | CVC 三大位点优劣 | 气胸（SC↑↑）/ 感染（Femoral↑↑）/ 不可压迫（SC）|
> | 其他插管操作不熟 | 已整理"侵入操作大全"（ET / NG / CVC / A-line / Foley / 胸管 / LP / 腹穿 / PEG 等 10+ 项）|
> | 所有管子的置后确认方式 | ET → **Capnography**；NG / CVC / 胸管 → **CXR**；A-line → **动脉波形**；共同铁律：未确认前不能用 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本题首张 procedure & patient safety 卡，等后续 NG / ET / 胸管 / LP / Foley 题积累
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_侵入操作安全流程大全]] ⭐（本题落地的衍生笔记，覆盖 20+ 操作）
>   - [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别|读题策略 Part 1 — 题型识别 4 信号]] ⭐（本题贡献的方法论模块）
>   - [[完整笔记/Peixuan分科笔记/外科]]（侵入操作 + procedure safety）
>   - [[完整笔记/Peixuan分科笔记/感染]]（脓毒症 1h bundle vs procedure safety 优先级）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/pulmonary]]（气胸 — CVC 最常见严重并发症 / 胸管处理）
>   - [[完整笔记/Peixuan分科笔记/心内]]（心包填塞 — 与 Q4212 主动脉急症形成"心包填塞"系列）
> - 🌱 TODO（待生成衍生）：
>   - 累计 3+ 道脓毒症题（早期处理 / 抗生素时机 / fluid resuscitation / Surviving Sepsis bundle）→ 生成 [[完整笔记/专题笔记/_衍生_脓毒症1小时bundle]]
>   - 累计 3+ 道 CVC 并发症题 → 拆出 [[完整笔记/专题笔记/_衍生_CVC并发症大全]]
>   - 累计 3+ 道程序题（CVC / NG / ET / 胸管 / Foley / LP 后下一步）→ 整合"程序题识别 + 答题模板"补入 [[完整笔记/专题笔记/_衍生_读题策略_程序性安全题]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q3504，目标 < 60 秒选 D
> - [ ] 默写 **CVC 三大位点对比表**（IJV / SC / Femoral × 气胸 / 感染 / 止血 / DVT / CPR）
> - [ ] 默写 **CVC 选位决策**（凝血 / COPD / 血透 / CPR / 长期）
> - [ ] 默写 **CVC 标准流程 + 置后必做**
> - [ ] 默写 **CVC 并发症时序表**（即刻 / 早期 / 晚期）
> - [ ] 默写 **所有"管子"置后确认方式**（ET → capno；NG / CVC / 胸管 → CXR；A-line → 波形）
> - [ ] 找 3 道类似程序题：① NG 管置后 ② ET 管置后 ③ 胸管置后
> - [ ] 给 [[完整笔记/Peixuan分科笔记/外科]] 加 #要做题（procedure safety）
> - [ ] **建立"题型识别"习惯**：见 "best next step" + 操作刚完成 → 默认程序性安全题
> - [ ] **建立"优先级 ≠ 跳步骤"思维**：临床急迫不能省略安全确认
> - [ ] **建立"程序题答题模板"**：先选"确认 / 影像"，后选"治疗"
> 
> ---
> 
> 学科:: 外科
> 主题:: 程序性安全 — CVC 置入后必做 CXR
> 状态:: 🟡
> 错因:: pattern

---

> [!example]- [2026-05-14] 外科 / 创伤 / 肢体血管创伤 Hard vs Soft Signs (Q3354)
> ^Q3354
> 
> ## Stem 模式
> 穿透伤（枪伤 / 刀伤）+ **远端肢体异常表现叠加**（cool + feeble pulses）+ **伤口处血肿** → **2+ Hard signs → 立即手术探查**（跳过影像）
> 
> ## 核心概念
> 肢体血管创伤的核心决策 = **Hard signs vs Soft signs**：
> - **Hard signs（任 1 项）→ 立即 OR**，跳过影像
> - **Soft signs → IEI（伤侧远端 SBP / 健侧近端 SBP）→ ≤ 0.9 → CT angio → 选择性手术**
> 
> ## 普适规则
> 
> **① Hard signs 4 项（"4B's of Hard"）⭐ 必背**
> 
> | 项 | 4B 速记 | 中文 | 病理学含义 |
> |---|---|---|---|
> | 1 | **B**lood spurting | 搏动出血（pulsatile bleeding）| 动脉破口在喷 |
> | 2 | **B**ruit / thrill | 杂音 / 震颤 | AV fistula / 假性动脉瘤"在漏" |
> | 3 | **B**ulging hematoma | 扩大血肿（expanding）| "正在出血"到组织内 |
> | 4 | **B**loodless distal | 远端缺血（6P 任 1 项）| 远端"没血" = 主血管闭塞 / 内膜剥离 |
> 
> **② Soft signs 4 项（"HDBN"）**
> 
> | 项 | HDBN 速记 | 中文 |
> |---|---|---|
> | 1 | **H**istory of hemorrhage | 既往大量出血史（已止）|
> | 2 | **D**iminished pulses | 脉减弱**但还能摸到** |
> | 3 | **B**ony injury near vessel | 邻近骨损伤 |
> | 4 | **N**eurologic abnormality | 神经异常（孤立的）|
> 
> **③ 底层逻辑（最值得记的核心）**
> 
> | | Hard | Soft |
> |---|---|---|
> | 性质 | "**现在正在发生**" | "**过去 / 邻近 / 弱**" |
> | 临床决策 | 必须立即修 | 先评估 |
> | 时态 | 现在进行时 | 过去时 / 间接证据 |
> 
> **④ 完整决策树**
> 
> ```
> Penetrating extremity injury
>         │
>         ▼
> 检查 4B's of Hard
>         │
>    有 ≥ 1 项？
>    ┌──┴──┐
>    是    否
>    │     │
>    ▼     ▼
>  ⭐ 直接 OR    检查 HDBN of Soft
> （± 术中 angio） │
>              有 ≥ 1 项？
>              ┌──┴──┐
>              是    否
>              │     │
>              ▼     ▼
>             IEI    观察 / 系列查体
>          ┌────┴────┐
>         > 0.9     ≤ 0.9
>          │         │
>          ▼         ▼
>         观察     CT angio → 选择性手术
> ```
> 
> **⑤ 6P 缺血表现速记**（远端缺血 = Hard sign）
> 
> | P | 含义 |
> |---|---|
> | Pain | 疼痛（早期，与损伤不成比例）|
> | Pallor | 苍白 |
> | Paresthesia | 感觉异常 |
> | Paralysis | 瘫痪（晚期）|
> | Pulselessness | 无脉（晚期）|
> | Poikilothermia | 冷（cool to touch）★ 本题 |
> 
> **⑥ IEI（Injured Extremity Index）公式**
> 
> ```
> IEI = 伤侧远端 SBP / 健侧近端 SBP
> （类似 ABI）
> 
> > 0.9 → 正常，观察
> ≤ 0.9 → 异常 → CT angio
> ```
> 
> **⑦ ⭐ "质变升级"规则**（最容易掉的陷阱）
> 
> 单一 soft 表现 + 远端缺血任 1 项 = **整体升级为 Hard**：
> 
> | 单独看 | 组合后 | 整体分类 |
> |---|---|---|
> | Feeble pulses（Soft）| + cool / pale / paresthesia | **Hard**（distal ischemia）|
> | Small hematoma（不算 hard）| + 进行性扩大 | **Hard**（expanding）|
> | History of bleeding（Soft）| + bruit | **Hard**（bruit）|
> | Neurologic abnormality（Soft）| + 缺血表现 | **Hard**（distal ischemia）|
> 
> ## 易混陷阱（普适）
> - ❌ **"no active bleeding" = 排除 hard signs**：只排除 4B 的 1 项（Blood spurting），还有 3 项要核对
> - ❌ **Feeble pulses 一定是 Soft**：单独是 Soft，但 + cool / pale / 6P 任 1 项 = 整体升级为 Hard（distal ischemia）
> - ❌ **Stem 写"hematoma"无 "expanding"前缀就不算 hard**：创伤后**新发血肿** + 心动过速 + 低血压 → 高度可疑 expanding
> - ❌ **Hard signs 也要先做影像确认**：错！hard signs = 跳过影像直接 OR（影像 = 延误）
> - ❌ **Distal ischemia 必须 pulseless 才算**：错！6P 任 1 项就够（cool to touch 也算）
> - ❌ **AV fistula / pseudoaneurysm 是 Soft**：错！表现为 bruit / thrill = Hard sign
> 
> ## 我为什么错
> - 选了：**D. Doppler ultrasonography**
> - 错因：**pattern**（"看到 'no active bleeding' 就觉得排除了 hard sign"→ 走 soft sign 路径 → 选影像评估 = 反向阴性体征陷阱）
> - 核心陷阱：**"反向阴性体征陷阱" — 见 no X 不能直接排除整个类别，必须把完整 criteria（4 项 / 5 项）逐项核对**
> 
> **具体错位**：
> - ☑ 反向阴性体征陷阱：只核对一项阴性（no active bleeding）就以为排除整个类别
> - ☑ 未核对完整 4B 清单：忽略 hematoma（Bulging）+ cool / feeble（Bloodless distal）两条 hard signs
> - ☑ 未识别"质变升级"：feeble + cool 组合 ≠ 单纯 feeble
> - ☑ C/D 之间纠结说明已在错误路径：浪费时间在不重要的细节
> 
> ## Memory Hook
> 
> **🎯 完整记忆法套餐**：
> 
> **底层逻辑**（最核心）：
> - **Hard = "现在正在出问题"** → 直接 OR
> - **Soft = "过去 / 邻近 / 弱"** → 先评估
> 
> **首字母速记**：
> - **4B's of Hard**: **B**lood spurting / **B**ruit-thrill / **B**ulging hematoma / **B**loodless distal
> - **HDBN of Soft**: **H**istory hemorrhage / **D**iminished pulses / **B**ony injury / **N**eurologic abnormality
> 
> **对子法**（极端 vs 轻微）：
> 1. 喷血（Hard）vs 流过血（Soft）
> 2. 无脉（Hard）vs 弱脉（Soft）
> 3. 血管本身在出问题（Hard）vs 骨头打到附近（Soft）
> 4. 神经因缺血损伤（Hard）vs 单纯神经异常（Soft）
> 
> **一句话锁定**：
> > "枪伤 + 血肿 + 脚冷脉弱 = 立刻进 OR，别浪费时间做影像。"
> 
> **🎯 阴性体征扫读法 v2 升级**（基于昨日 Q17169 + 今日新陷阱）：
> 
> 见到 "no X" 时：
> 1. 先问：**X 属于哪个完整 criteria 清单？**（hard signs 4 项 / Light's / Wells / Jones 等）
> 2. **把完整清单列出**，逐项核对
> 3. 不止看缺失的那 1 项，**其他 3 项也要逐项扫**
> 4. ≥ 1 项满足 → 类别诊断成立
> 
> **🎯 类比记忆**：
> - **Hard signs = "红码"**：任 1 亮起 → 直接手术，不停留
> - **Soft signs = "黄码"**：做 IEI → 异常 → 影像 → 手术
> - **Q3354 陷阱**："no active bleeding" 只熄灭了 4B 中 1 个，剩 3 个还在亮
> 
> **🎯 类似"质变陷阱"USMLE 高频**：
> - **Light's criteria for exudate**（任 1 项即 exudate）
> - **SIRS criteria for sepsis**（任 2 项）
> - **Jones criteria for rheumatic fever**
> - **Wells score for PE / DVT**
> - **HEART score for ACS**
> - **APACHE / Ranson for pancreatitis**
> - **Centor criteria for strep**
> 
> → 看到所有 "criteria / signs / score" 类标准 → **逐项核对，不能只看 1 项就下结论**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | 看到 "no active bleeding" 就觉得排除 hard signs | 反向阴性陷阱；只排除 1 项（B-Blood spurting），还有 3B 要核对 |
> | 总记不住 hard / soft 各 4 项 | 5 套记忆法：底层逻辑 + 4B / HDBN + 对子 + 身体定位 + 故事法；推荐"底层逻辑 + 4B / HDBN"组合 |
> | Feeble pulse 是 Hard 还是 Soft？ | **单独是 Soft；+ cool / pale / paresthesia = 组合升级为 Hard（distal ischemia）**；Q3354 即此陷阱 |
> | 5/5 自测全中 | 4B / HDBN 记忆法已固化 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本题首张外科 / 创伤血管损伤卡，等后续 compartment syndrome / 急性动脉闭塞 / 颈部贯通伤 / 钝性血管伤积累
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/外周血管病专题_v1]] ⭐（C.3 Hard Signs 决策 + Rutherford 分级 + 黄金 6h 窗口）
>   - [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别|读题策略 Part 2 + 4 — criteria 完整核对 + 质变升级]] ⭐（本题贡献的方法论模块）
>   - [[完整笔记/Peixuan分科笔记/外科]]（血管创伤 + 创伤一般原则）
>   - [[完整笔记/Peixuan分科笔记/骨科]]（开放骨折 + compartment syndrome — 共享 6P）
> - 🏥 跨学科：
>   - [[完整笔记/专题笔记/_衍生_主动脉急症决策树]]（与 Q4212 同属"难治性休克 + 跳过影像直接 OR"系列）
>   - [[完整笔记/专题笔记/_衍生_侵入操作安全流程大全]]（与 Q3504 共享"临床优先级决策"方法论）
>   - [[完整笔记/Peixuan分科笔记/心内]]（与 Q4212 / Q3504 形成"紧急血管损伤"系列）
>   - [[完整笔记/Peixuan分科笔记/感染]]（穿透伤 → 破伤风预防 + 抗生素时机）
> - 🌱 TODO（待生成衍生）：
>   - ⭐ **立即可建**（与 Q3504 程序题方法论合并）：累计 5+ 道"临床决策 vs 影像延误"题（hard signs 直接手术 / 张力气胸不等 CXR / CVC 置后必拍片 / 心包填塞 echo / Rutherford IIb 跳影像）→ 生成 [[完整笔记/专题笔记/_衍生_临床优先级_跳过影像决策]]
>   - 累计 3+ 道创伤题（穿透 / 钝伤 / 开放骨折 / 头部 / 颈部贯通）→ 生成 [[完整笔记/专题笔记/_衍生_创伤评估与处理]]
>   - 累计 3+ 道肢体缺血题（hard signs / compartment / 急性动脉闭塞 / 慢性 PAD）→ 生成 [[完整笔记/专题笔记/_衍生_肢体缺血决策树]]
>   - ⭐ **方法论合并**：累计 3+ 道"反向阴性体征 / criteria 不完整核对"陷阱题 → 升级 [[完整笔记/专题笔记/_衍生_读题策略_阴性体征]] 添加 v2 章节"完整 criteria 清单核对"
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q3354，目标 < 60 秒选 E
> - [ ] 默写 **4B's of Hard**（Blood spurting / Bruit / Bulging hematoma / Bloodless distal）
> - [ ] 默写 **HDBN of Soft**（History / Diminished / Bony / Neuro）
> - [ ] 默写 **Hard vs Soft 决策树**（hard → OR；soft → IEI → CT → 选择性手术）
> - [ ] 默写 **6P 缺血表现**
> - [ ] 默写 **IEI 公式 + 阈值**
> - [ ] 默写 **质变升级规则**（feeble + cool = Hard）
> - [ ] 找类似题：① compartment syndrome ② 急性动脉闭塞（Rutherford 分级）③ 开放骨折处理 ④ 颈部贯通伤分区
> - [ ] 给 [[完整笔记/Peixuan分科笔记/外科]] 加 #要做题（血管创伤章节）
> - [ ] **建立"完整 criteria 清单"读题习惯**：见 "no X" 先想 X 属于哪个完整清单，把剩余项也核对
> - [ ] **建立"质变升级"思维**：单一软体征 + 远端异常 = 整体可能升级为硬体征
> - [ ] **强化"临床优先级 = 跳过影像"思维**：hard signs / 张力气胸 / 失代偿性休克 → 跳影像直接处理
> 
> ---
> 
> 学科:: 外科
> 主题:: 肢体血管创伤 Hard vs Soft Signs（criteria 完整核对）
> 状态:: 🟡
> 错因:: pattern

---

> [!example]- [2026-05-14] 外科 / 创伤 / 钝性胸创 BCI 评估 (Q19889)
> ^Q19889
> 
> ## Stem 模式
> 钝性胸部创伤 + **高危机制**（unrestrained + 车严重损坏）+ **稳定**生命体征 + **三件套部分已做**（CXR ✓ + eFAST ✓ + ECG ❌）→ 下一步 **ECG** 完成三件套筛查 BCI
> 
> ## 核心概念
> 钝性胸创评估遵循**诊断阶梯**：CXR + eFAST + ECG = **三件套基础筛查**。**高危机制 = 等同不稳定处理强度**（即必做三件套），但仍按阶梯顺序"便宜 → 贵"完成。ECG 是 BCI 筛查的**初筛工具**，不能跳过它直接做 troponin / echo / 入院观察。
> 
> ## 普适规则
> 
> **① 钝性胸创完整决策树**
> 
> ![[{97EDC4FC-B930-442E-84D2-8A302E2BF024}.png]]
> *(UWorld 官方决策图)*
> 
> 文字版：
> 
> ```
> Blunt chest trauma
>         │
>    ┌────┴────┐
>    不稳定    稳定
>    │         │
>    ▼         ▼
> 并行评估    有 high-risk mechanism
> + 复苏:     或 serious injury on exam?
> - eFAST     │
> - CXR     ┌─┴─┐
> - ECG    是   否
> - 干预    │   │
>           ▼   ▼
>      按"不稳定"  基础筛查:
>      处理:       CXR + ECG
>      eFAST       │
>      + CXR      异常?
>      + ECG      ┌─┴─┐
>      ↑         是  否
>      ★ 本题档次  │   │
>                  ▼   ▼
>               干预 出院 +
>                    镇痛 +
>                    回院 precautions
> ```
> 
> **② 高危机制清单**（USMLE 必背触发条件）
> 
> | 类别 | 具体情境 |
> |---|---|
> | **MVC** | **未系安全带 / 抛出车外 / 同车死亡 / 车辆严重损坏 / 气囊弹出 / 速度 > 40 mph** |
> | **坠落** | > 20 ft（成人）/ > 10 ft 或 2-3 倍身高（儿童）|
> | **行人 / 摩托** | 被撞击 |
> | **挤压 / 穿刺** | 重物 / 高能量 |
> | **爆炸** | 任何 |
> 
> **③ "严重损伤体征"等同触发**（与高危机制同等地位）
> 胸壁淤伤 / 皮下气肿 / 不对称呼吸音 / flail chest / 触诊压痛 + 捻发音 / JVD / 心音遥远 / 气管偏移
> 
> **④ BCI 评估三件套 + 加做**
> 
> ```
> 三件套（基础筛查，所有"按不稳定处理"患者）：
>   CXR + eFAST + ECG
> 
> 加做（仅在以下情况）：
>   - Troponin: ECG 异常 / 持续 tachycardia / 持续症状
>   - Echo (TTE): troponin 升高 / 持续低血压 / 新杂音 / 持续 ECG 异常
>   - TEE: 不稳定 + 怀疑主动脉损伤（替代 CT angio）
>   - CT chest: 怀疑主动脉损伤 / 隐匿气胸（稳定患者）
> ```
> 
> **⑤ BCI 评估算法（流程化）**
> 
> ```
> 三件套 → 全正常 + 无症状 → 出院 + 镇痛 + return precautions
>           │
>           异常?
>           │
>           ▼
>      ECG 异常 → 入院 24h 监护 + Troponin (0h + 4-6h) + Echo
>           │
>      Troponin 升高 → Echo 评估壁运动 + 心包 + 瓣膜 + 心血管会诊
>           │
>      Echo 异常 → ICU + 重症管理
> ```
> 
> **⑥ Troponin 在 BCI 的关键判读**
> 
> | 维度 | BCI | ACS |
> |---|---|---|
> | Troponin 升高含义 | **心肌挫伤** | 心肌梗死 |
> | 后续处理 | **Echo + 监护** | 冠脉造影 + PCI |
> | 抗血小板 / 抗凝 | ❌ **禁忌**（增内出血）| ✓ |
> | 溶栓 | ❌ 禁忌 | ✓ 部分适应 |
> | Troponin 阴性能否排除 | ❌ 不能完全（轻度可不升）| 部分可（结合临床）|
> 
> **⑦ 24h 观察的真正触发条件**
> 
> ```
> ❌ 不是"高危机制本身" → 自动观察
> ✓ 是 "ECG 异常" → 才需 24h 观察
> 
> 临床证据：
>   - ECG 正常 + 无症状 → 致命心律失常 < 0.1%
>   - ECG 异常 → 显著升高 → 必须 24h 监护
> 
> UWorld 立场：
>   高危 + 三件套全做且全阴性 + 无症状
>     = 可出院 + 镇痛 + return precautions
> ```
> 
> **⑧ 出院的具体要求（discharge criteria）**
> 
> 必须同时满足：
> - 三件套全阴性
> - 生命体征稳定
> - 疼痛口服镇痛可控
> - 能口服 + 活动
> - 可靠的回院系统 + 家庭照顾
> - **详细 return precautions**（突发胸痛 / 气短 / 心悸 / 晕厥 / 腹痛 / 意识改变 → 立即回院）
> 
> ## 易混陷阱（普适）
> - ❌ **稳定 + eFAST 阴性 = 可出院**：忽略高危机制 + 未做 ECG
> - ❌ **高危机制 = 自动入院观察 24h**：错！触发观察的是 ECG 异常，不是机制本身
> - ❌ **跳过 ECG 直接 troponin**：诊断阶梯不能跳级（本题陷阱）
> - ❌ **跳过 ECG 直接 echo / TEE**：同上
> - ❌ **BCI 心动过速 → β-blocker**：错！BCI 可致收缩力下降，β-blocker 加重低血压；窦速是生理反应，治原因
> - ❌ **BCI 跑 ACS 流程**：禁抗血小板 / 禁溶栓 / 不立即 cath；正确路径是 echo + 监护
> - ❌ **Troponin 阴性 = 排除 BCI**：轻度心肌挫伤可不升；必须结合 ECG + 临床
> - ❌ **流程图右路 "additional tests (eg, CT)" = 直接做 CT**：CT 只是 additional tests 中的一例，不是同义词；必须先完成三件套
> 
> ## 我为什么错
> - 选了：**B. Admit + 监测心肌酶**
> - 错因：**pattern**（"生命体征稳定 + eFAST 阴性，但有钝挫伤 + 可能滞后心脏问题 → 留院观察 + 心肌酶" — 诊断阶梯跳级 + 过度评估倾向）
> - 核心陷阱：**"诊断阶梯不能跳级" — 评估顺序是"便宜 → 贵；非侵入 → 侵入；快速 → 缓慢；筛查 → 确诊"，跳过 ECG 直接 troponin 是经典跨级错误**
> 
> **具体错位**：
> - ☑ 临床思路对（识别要评估 BCI ✓），但**跳过诊断阶梯**：直接跳到 troponin + 入院，跨过 ECG 这个初筛
> - ☑ 不熟悉 BCI 评估算法：不知道 ECG → 异常才加 troponin 的顺序
> - ☑ **过度评估倾向**：默认选最"保险"的"入院观察"，没意识到 ECG 阴性 + 三件套阴性可直接出院
> - ☑ 被"高危机制 = 24h 观察"直觉误导：实际 24h 观察的触发是 ECG 异常，不是机制
> - ☑ 流程图阅读错误：把"按不稳定处理"理解为"直接入院"，没看到这是指"完成三件套评估"
> 
> ## Memory Hook
> 
> **🎯 诊断阶梯（最值得记的核心方法论）**：
> 
> ```
> 钝性胸创评估阶梯（从下往上，越贵）：
> ┌──────────────────────────┐
> │ 5. TEE / Cardiac MRI    │ ← 特殊指征
> ├──────────────────────────┤
> │ 4. Echo (TTE)            │ ← troponin 升高时加
> ├──────────────────────────┤
> │ 3. Troponin (系列)       │ ← ECG 异常时加
> ├──────────────────────────┤
> │ 2. ECG ⭐ 本题考点        │ ← 三件套之一，快 + 便宜 + 敏感
> ├──────────────────────────┤
> │ 1. CXR + eFAST           │ ← 三件套之二，第一步
> └──────────────────────────┘
> ```
> 
> **🎯 一句话锁定**：
> > "钝挫伤 + 高危机制 + 稳定 = 先做完三件套（CXR + eFAST + ECG）→ ECG 阴性 + 其他阴性 = 可出院。不要跳过 ECG。"
> 
> **🎯 三件套（必背）**：
> - **CXR**：肺 / 纵隔 / 心影 / 气胸
> - **eFAST**：4 窗（心包 / 胸 / 腹 / 盆）
> - **ECG**：BCI 筛查（心律失常 / ST 改变 / 传导阻滞）
> 
> **🎯 "高危机制 = 不稳定处理强度"**（不是"高危 = 入院"）：
> - 等同 = 必做三件套（而非低危只 CXR + ECG）
> - 不等同 = 自动 24h 观察
> - 触发 24h 观察的是 **ECG 异常**，不是机制
> 
> **🎯 BCI vs ACS 反陷阱**：
> 
> | 维度 | BCI | ACS |
> |---|---|---|
> | Troponin 升高 → | Echo + 监护 | Cath lab + PCI |
> | 抗血小板 | **禁忌** | 给 |
> | β-blocker | **不常规**（致低 BP）| 给 |
> 
> **🎯 类比**：评估钝性胸创像装修房子检查 → 先看外观（eFAST / CXR），再看电路（ECG），有问题才砸墙（troponin + echo），最贵的内窥镜（TEE）留给特殊情况
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | 低危 vs 高危机制区别是 eFAST？ | 不，区别是**评估强度**：低危 = CXR + ECG；高危 = 三件套（+ eFAST）；不稳定 = 三件套 + 复苏 |
> | ECG 和 CXR 是不是都要做？ | 都要做，且 + eFAST（如高危）= 三件套 |
> | 高危 + 检查正常，24h 内会不会出现心律失常？要不要观察 24h？ | UWorld 立场：ECG 正常 + 三件套阴性 + 无症状 → 致命事件 < 0.1% → 可出院；24h 观察的触发是 ECG 异常 |
> | BCI 的 troponin 何时该做？ | ECG 异常时（UWorld 立场）；或持续 tachycardia / 持续症状（临床指南）；ECG 正常 + 无症状不需要 |
> | 流程图右路 "additional tests" 含义 | 不是直接 CT；指三件套完成后发现异常时的进一步检查 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q3354]] 肢体血管创伤（同日，hard signs 直接 OR — "跳过影像"反向案例）
>   - [[mistakes/uworld-mistakes#^Q3504]] CVC 程序题（同日，"程序题先确认后治疗"方法论互补）
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别|读题策略 — 新增"诊断阶梯不跳级"模块]] ⭐（本题贡献新方法论，等累计 3+ 道阶梯跳级题后正式补 Part 8）
>   - [[完整笔记/Peixuan分科笔记/外科]]（钝性胸创 + 创伤一般原则 + ATLS）
>   - [[完整笔记/Peixuan分科笔记/心内]]（BCI + 创伤性心包填塞 + 与 ACS 鉴别）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/pulmonary]]（鉴别：气胸 / 血胸 / 肺挫伤）
>   - [[完整笔记/专题笔记/_衍生_主动脉急症决策树]]（创伤性主动脉损伤鉴别）
>   - [[完整笔记/专题笔记/_衍生_侵入操作安全流程大全]]（与 Q3504 同属"程序 / 决策类"方法论系列）
>   - 今日 4 道创伤 + 程序题（Q4212 / Q3504 / Q3354 / Q19889）形成"紧急血管 + 程序 + 决策阶梯"系列
> - 🌱 TODO（待生成衍生）：
>   - ⭐ **本题方法论合并立即可建**：累计 3+ 道"诊断阶梯跳级"陷阱题（ECG 前 troponin / CXR 前 CT / 听诊前影像 / 阻断初筛直接做次级）→ 升级 [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别]] 添加 Part 8 "诊断阶梯不跳级"
>   - 累计 3+ 道创伤题（钝伤 / 穿透伤 / 头颈 / 腹部 / 多发伤）→ 生成 [[完整笔记/专题笔记/_衍生_创伤评估与处理]]（含 ATLS primary / secondary survey + 各部位决策树）
>   - 累计 3+ 道 BCI / 创伤性心损相关题 → 生成 [[完整笔记/专题笔记/_衍生_钝性心脏损伤BCI评估]]
>   - 累计 5+ 道胸部紧急情况题（BCI / 张力气胸 / 心包填塞 / 大量血胸 / 主动脉损伤）→ 生成 [[完整笔记/专题笔记/_衍生_胸部急症决策树]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q19889，目标 < 60 秒选 D
> - [ ] 默写 **钝性胸创完整决策树**（不稳 / 稳定 × 高危 / 低危）
> - [ ] 默写 **高危机制清单**（MVC unrestrained / 严重车损 / 坠落 > 20ft / 行人 / 摩托 / 挤压 / 爆炸）
> - [ ] 默写 **BCI 三件套 + 加做规则**（CXR + eFAST + ECG → 异常加 troponin → 升高加 echo）
> - [ ] 默写 **诊断阶梯**（CXR + eFAST → ECG → troponin → echo → TEE）
> - [ ] 默写 **24h 观察触发**（ECG 异常 = 触发；机制本身 ≠ 触发）
> - [ ] 默写 **BCI vs ACS 三差异**（Echo vs Cath / 不给抗血小板 / 不给 β-blocker）
> - [ ] 默写 **出院 criteria**（三件套阴性 + VS 稳定 + 痛可控 + 能口服 + 可靠回院 + return precautions）
> - [ ] 找类似题：① 心包填塞 ② 主动脉创伤 ③ 张力气胸 ④ 肺挫伤 ⑤ 钝性腹部创伤
> - [ ] 给 [[完整笔记/Peixuan分科笔记/外科]] 加 #要做题（创伤章节）
> - [ ] **建立"诊断阶梯不跳级"思维**（最重要的方法论收获）
> - [ ] **建立"高危机制 = 升级评估强度"思维**（≠ "高危 = 入院"）
> - [ ] **修正"过度评估倾向"**：稳定 + 三件套阴性 + 无症状 → 可出院，不要默认选"入院观察"
> - [ ] **建立 "UWorld 立场 ≠ 临床最保守"认知**：按指南 / 循证答题，不要被"万一"直觉拉走
> 
> ---
> 
> 学科:: 外科
> 主题:: 钝性胸创 BCI 评估（诊断阶梯不跳级）
> 状态:: 🟡
> 错因:: pattern

---

> [!example]- [2026-05-14] 心血管 / 电生理 / 先天性 LQTS (Jervell & Lange-Nielsen) (Q3910)
> ^Q3910
> 
> ## Stem 模式
> 儿童 + **先天性双侧感音神经性聋**（cochlear implants）+ **运动诱发晕厥**（无 postictal）+ **家族猝死**（兄弟游泳猝死）+ QT 520 ms → **Jervell & Lange-Nielsen syndrome (LQT1 纯合, AR)** → **β-blocker (propranolol or nadolol)**
> 
> ## 核心概念
> **遗传性离子通道病 ≠ 抗心律失常药治疗。**
> LQTS 的一线 = **β-blocker（Class II）**，几乎所有其他抗心律失常药（IA / IC / III）都**禁用**（延长 QT）。LQT1 对 β-blocker 反应最好，是首选。Class IB（Mexiletine）是例外——缩短 QT，LQT3 特别有用。
> 
> ## 普适规则
> 
> **① LQTS 双分类系统（USMLE 高频混淆点）**
> 
> ```
>                先天性长 QT 综合征
>                       │
>          ┌────────────┴────────────┐
>          ▼                         ▼
>     按"基因"分                  按"临床表型"分
>     LQT1, 2, 3...17             Romano-Ward vs J&L-N
>     (哪个通道坏了)              (聋 / 不聋 + AD / AR)
> ```
> 
> 一个患者**同时拥有两个标签**：基因标签（LQT1/2/3）+ 临床标签（Romano-Ward 或 J&L-N）。
> 
> **② Romano-Ward vs Jervell & Lange-Nielsen**
> 
> | | Romano-Ward | **J&L-N** |
> |---|---|---|
> | 遗传 | **AD**（杂合）| **AR**（纯合）|
> | 受累 | 仅心脏 | **心脏 + 双侧感音神经性聋** ★ |
> | 基因 | LQT1/2/3/...17 任一杂合 | **必是 KCNQ1 纯合（= LQT1 范畴）** |
> | 表型严重度 | 中 | 重 |
> | 占比 | 大多数 LQTS | 罕见（< 1%）|
> 
> **③ 杂合 vs 纯合的"基因剂量效应"**
> 
> ```
> KCNQ1 (LQT1) 基因：
> - 正常 / 正常 → IKs 100% → QT 正常 + 听力正常
> - 突变 / 正常（杂合）→ IKs 50% → LQT (Romano-Ward), 听力正常
> - 突变 / 突变（纯合）→ IKs ~0% → 严重 LQT + 聋 (J&L-N)
> 
> 为什么只有 LQT1 纯合能形成 J&L-N：
> - IKs 是"辅助型"复极 → 纯合可代偿存活
> - LQT2 (IKr) / LQT3 (Na) 是"主力型" → 纯合多胚胎死亡
> → LQT2 / 3 临床上几乎都是杂合 (Romano-Ward)
> ```
> 
> **④ LQT1 / 2 / 3 三亚型完整对比 ⭐⭐⭐**
> 
> | 维度 | **LQT1** | **LQT2** | **LQT3** |
> |---|---|---|---|
> | 基因 | KCNQ1 | KCNH2 (hERG) | SCN5A |
> | 通道 | IKs↓ | IKr↓ | INa 持续 |
> | 占比 | 35% | 30% | 10% |
> | **触发** | **运动 / 游泳** ★ | **听铃 / 惊吓 / 产后 / 低 K** | **睡眠 / 安静** |
> | Stem 关键词 | "drowned / swim / running" | "alarm clock / postpartum / startled" | "found dead in bed" |
> | **ECG T 波** | **宽底** | **切迹 / 双相** | **长 ST + 晚出 T** |
> | 性别偏好 | 1:1 | **女性多** | 男性多 |
> | 猝死率 | 中 | 中-高 | **最高** ⭐ |
> | β-blocker 反应 | **极好** ⭐⭐⭐ | 中等 ⭐⭐ | **较差** ⭐ |
> | **特殊治疗** | 严格避游泳 | **补 K + Mg** | **Mexiletine (IB)** ⭐ |
> | ICD 阈值 | 高 | 中 | **低** |
> | 运动限制 | **严格** + 避游泳 | 中度 | **不严格**（运动反保护）|
> | J&L-N 可能 | **可能（纯合）** | 极罕见 | 不出现 |
> 
> **⑤ 三型治疗共同 + 个性化框架**
> 
> ```
> 共同（所有 LQT）：
> 1. 避免延长 QT 药物（IA / III / macrolides / 抗精神病 / SSRIs / 抗呕吐 / methadone）
> 2. β-blocker（propranolol / nadolol）★ 一线
> 3. 严重 → ICD
> 4. β-blocker 失败 → LCSD
> 
> 个性化：
> - LQT1：严格避游泳 + 避剧烈运动
> - LQT2：补 K 至 4.5-5.0 + 补 Mg + 避惊吓 + 产后监护
> - LQT3：加 Mexiletine + ICD 阈值低 + 不严格限运动
> - J&L-N：同 LQT1 但更严重 → 早期考虑 ICD
> ```
> 
> **⑥ Vaughan Williams 抗心律失常药简化框架**
> 
> "1 钠 2 β 3 钾 4 钙"——心肌动作电位各时相对应：
> 
> | Class | 通道 | 代表药 | QT 效应 | LQTS 可用？|
> |---|---|---|---|---|
> | **IA** | Na（中速）| Quinidine, Procainamide, Disopyramide | **延长 QT** ⭐ | ❌ |
> | **IB** | Na（快速）| **Lidocaine** (IV), **Mexiletine** (口服) | **缩短 QT** | ✓ 安全；LQT3 特别用 |
> | **IC** | Na（慢速）| Flecainide, Propafenone | ↑QRS（不长 QT）| 谨慎 |
> | **II** | β-blocker | **Propranolol, Nadolol** ★, Metoprolol, Esmolol | 不影响 | ✓ **一线** |
> | **III** | K | **Amiodarone**, **Sotalol**, Ibutilide, Dofetilide | **延长 QT** ⭐⭐（amiodarone 例外）| ❌ |
> | **IV** | Ca (非 DHP) | Verapamil, Diltiazem | 不影响 | ✓ 安全 |
> | 其他 | — | **Adenosine** (SVT), **Magnesium** (TdP), Digoxin | 不影响 | ✓ |
> 
> **⑦ 必背 12 药 + 5 急救场景 + 3 禁忌组合**
> 
> 12 必背药：Quinidine / Procainamide / Lidocaine / Mexiletine / Flecainide / Propranolol / Nadolol / Metoprolol / Esmolol / Amiodarone / Sotalol / Verapamil + Diltiazem + Adenosine
> 
> 5 急救场景：
> 1. SVT 急性 → **Adenosine IV push**
> 2. 室速稳定 → **Amiodarone / Lidocaine IV**
> 3. 室颤 / 无脉室速 → **电除颤**
> 4. **Torsades de Pointes → Magnesium IV**（不论血 Mg）
> 5. WPW + 房颤 → **Procainamide / 电复律**（不用 AV 结阻滞剂）
> 
> 3 禁忌组合：
> 1. **LQTS + Class IA / III** → 延长 QT
> 2. **WPW + 房颤 + AV 结阻滞剂**（β / Ca / Adenosine / Digoxin）→ 致室颤
> 3. **结构性心脏病 / 心梗后 + Class IC**（Flecainide）→ 增死亡率（CAST 试验）
> 
> **⑧ Torsades de Pointes 急诊处理**
> 
> ```
> 1. 不稳定（无脉 / 持续）→ 电除颤
> 2. ⭐ Magnesium IV ⭐ 一线（1-2g bolus + 维持）
> 3. 停延长 QT 药 + 纠正 K / Mg / Ca
> 4. 反复发作 → 加快心率（overdrive pacing / Isoproterenol）
>    ★ 不用 β-blocker / 抗心律失常（急性期反加重）
> ```
> 
> **⑨ QT 延长完整病因表（基于 UWorld 官方表）⭐⭐⭐**
> 
> | 大类 | 子类 | 具体 |
> |---|---|---|
> | **Acquired**（获得性）| **药物** | • Macrolides & Fluoroquinolones |
> | | | • Antiemetics（**Ondansetron**）|
> | | | • Azoles（**Fluconazole**）|
> | | | • Antipsychotics / TCAs / **SSRIs**（尤 Citalopram）|
> | | | • Some opioids（**Methadone, Oxycodone**）|
> | | | • **Class IA**（Quinidine）|
> | | | • **Class III**（Dofetilide, Sotalol）|
> | | **电解质** | ↓ Magnesium / ↓ Potassium / ↓ Calcium |
> | **Congenital**（先天性）| Romano-Ward | AD，仅心脏 |
> | | **Jervell & Lange-Nielsen** | AR + **感音神经性聋** ★ |
> 
> > [!tip] Peixuan 口诀（5 行助记）
> > - **"IA，III 类 QT 长"**（抗心律失常）
> > - **"大环三环喹诺酮"**（Macrolides + TCA + Fluoroquinolones）
> > - **"抗精抗吐昂丹司琼"**（抗精神病 + Ondansetron）
> > - **"氯喹噻嗪阿唑钠"**（Chloroquine + Thiazide 致低 K 间接 + Azoles + Na 类）
> > - **"哪位鸦片镁钾钙（降低）"**（Methadone + opioids + ↓ Mg / K / Ca）
> 
> **⑩ 心源性 vs 癫痫晕厥鉴别（本题排除 A / C 的关键）**
> 
> | | **心源性**（本题）| 癫痫 |
> |---|---|---|
> | 起病 | 突发，无前驱 | 可有 aura |
> | 持续 | **< 1 min** | 数分钟 |
> | 恢复 | **立即清醒，无 confusion** ⭐ | **Postictal confusion** ★ |
> | 强直抽搐 | 罕见(短暂缺氧)| 常有 |
> | 舌咬伤 | 通常无 | **常有** |
> | 大小便 | 通常无 | **常有** |
> | 诱因 | 运动 / 听觉 / 应激 | 睡眠剥夺 / 闪光 / 停药 |
> 
> ## 易混陷阱（普适）
> - ❌ **遗传性离子通道病 → 用抗心律失常药**：错！LQTS 反而**禁用**大多数抗心律失常药（IA / III 延长 QT）
> - ❌ **Quinidine 是 LQTS 治疗**：错！Quinidine = IA = 经典 acquired LQTS 元凶
> - ❌ **Sotalol 是 β-blocker 所以 LQTS 可用**：错！Sotalol K 通道阻滞主导，仍延长 QT，禁忌
> - ❌ **Amiodarone 延长 QT 所以禁忌**：错！Amiodarone 致 TdP 罕见（多通道效应），可用于 LQTS（但谨慎）
> - ❌ **LQT2 / 3 也可以是 J&L-N**：错！J&L-N 几乎必是 LQT1 纯合（KCNQ1，少数 KCNE1）
> - ❌ **LQTS 都要严格限制运动**：错！LQT3 运动反而保护，不严格限制
> - ❌ **β-blocker 缩短 QT**：错！β-blocker 不直接缩短 QT，是通过抑制交感预防 TdP 触发
> - ❌ **Torsades 用 β-blocker 急救**：错！急性期会加重；急救用 Magnesium + 加快心率
> - ❌ **见到心律失常都查 ECG 看图**：USMLE 不要求看图诊断 LQT，stem 文字会给 QT 数字
> 
> ## 我为什么错
> - 选了：**E. Quinidine**
> - 错因：**知识**（认出疾病但**不知 β-blocker 是 LQTS 一线**；**抗心律失常药 Vaughan Williams 分类不熟**：误以为 Quinidine 是 III 类 / Sotalol 是单纯 β-blocker）
> - 核心陷阱：**"遗传性离子通道病 ≠ 抗心律失常药" + "Vaughan Williams 分类知识盲点"**
> 
> **具体错位**：
> - ☑ 认出疾病但不知一线治疗：知道 LQTS 但不知 β-blocker
> - ☑ "先天性病 → 抗心律失常药"反射误：误以为遗传性离子通道病要用针对性药；其实禁用大多数
> - ☑ 抗心律失常药分类不熟：Quinidine = IA（强延长 QT），Sotalol / Ibutilide = III
> - ☑ ECG 不会看 → 放弃读图：但 stem 文字已给 QT 520 ms，不需读图
> 
> ## Memory Hook
> 
> **🎯 触发口诀（最实用）**：
> > **"游泳 1，听铃 2，睡觉 3"**
> > - LQT1 → 游泳 / 运动
> > - LQT2 → 听铃 / 惊吓 / 产后 / 低 K
> > - LQT3 → 睡觉 / 安静
> 
> **🎯 ECG T 波口诀**：
> > **"1 宽 2 双 3 晚"**
> > - LQT1：宽底 T
> > - LQT2：切迹 / 双相
> > - LQT3：长 ST + 晚出 T
> 
> **🎯 治疗特殊点口诀**：
> > **"1 β 救命，2 补 K 防铃,3 美西律救场"**
> > - LQT1：β-blocker 最有效
> > - LQT2：β-blocker + 补 K + 避惊吓
> > - LQT3：β-blocker + Mexiletine + ICD 阈值低
> 
> **🎯 Vaughan Williams 框架**：
> > **"1 钠 2 β 3 钾 4 钙"** + **"1A 长，1B 短，2β 4 钙是真朋友，3 全长（除阿米奥），1C 不动 QRS 宽"**
> 
> **🎯 QT 延长病因口诀（Peixuan 5 行助记）**：
> > 1. **"IA，III 类 QT 长"**
> > 2. **"大环三环喹诺酮"**
> > 3. **"抗精抗吐昂丹司琼"**
> > 4. **"氯喹噻嗪阿唑钠"**
> > 5. **"哪位鸦片镁钾钙（降低）"**
> 
> **🎯 类比理解**：
> - LQTS 心脏 = **充电慢的手机**：复极慢 → 高心率时来不及充满 → 触发崩溃 (TdP)
> - β-blocker = **让手机用慢点**：减慢心率，给心脏足够时间复极
> - 游泳 / 听铃 / 惊吓 = **突然高负荷使用**：手机崩溃
> - Quinidine / Sotalol = **把充电速度调更慢**：火上浇油
> 
> **🎯 J&L-N "血统"识别**：
> > 聋 + LQT + AR → 必是 KCNQ1 纯合 = LQT1 范畴 → β-blocker 反应好 + 早期 ICD 考虑
> 
> **🎯 遗传性心律失常治疗哲学（最核心）**：
> > **"避诱因 + β-blocker + ICD"** = 90% 答案
> > 90% 的题选 β-blocker，10% 选 ICD（已发生心脏骤停或反复事件）
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | 遗传性离子通道病应该如何治疗？ | 不是用"对症"抗心律失常药；正确路径 = β-blocker + ICD + 避诱因 |
> | 三亚型临床症状再讲清楚 | 触发 / ECG / 性别 / 猝死率 / β-blocker 反应都有差异 |
> | LQT1 / 2 / 3 vs Romano-Ward / J&L-N 怎么对应？ | 双分类系统：基因层（LQT1 / 2 / 3）+ 临床层（RW / J&L-N）；J&L-N 必是 LQT1 纯合 |
> | 所有 LQT 治疗都一样吗？ | 共同框架 90% 同；个性化 10%：LQT2 补 K，LQT3 加 Mexiletine，LQT1 严格避运动 |
> | LQT2 / 3 是不是也是杂合？ | 是！LQT1 / 2 / 3 都默认杂合（Romano-Ward, AD）；只有 LQT1 纯合形成 J&L-N；LQT2 / 3 纯合多胚胎死亡 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本题首张心内 / 电生理 / 遗传性心律失常卡，等后续 Brugada / CPVT / ARVC / 获得性 QT 延长积累
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] ⭐（本题落地的衍生笔记，15 个 Part 全套）
>   - [[完整笔记/Peixuan分科笔记/心内]]（LQTS + Vaughan Williams + Torsades）
>   - [[完整笔记/Peixuan分科笔记/儿科]]（儿童心源性晕厥 + 先天性遗传病）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/感染]]（macrolides / fluoroquinolones / azoles → 获得性 LQTS — 开抗生素时常考点）
>   - [[完整笔记/Peixuan分科笔记/psych]]（抗精神病 / 抗抑郁致 QT 延长 — 精神科开药考点）
>   - 与 Q4212 主动脉急症形成"心内紧急"系列
> - 🌱 TODO（待生成衍生）：
>   - 累计 3+ 道遗传性心律失常题 → 生成 [[完整笔记/专题笔记/_衍生_遗传性心律失常综合征]]（含 LQT1-3 / Brugada / CPVT / ARVC / J&L-N / Andersen-Tawil / Timothy 全套）
>   - 累计 3+ 道获得性 QT 延长题（药物 + 电解质）→ 生成 [[完整笔记/专题笔记/_衍生_获得性LQTS病因清单]]
>   - 累计 3+ 道晕厥鉴别题 → 生成 [[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]]（心源 vs 神经 vs 血管迷走 vs 体位 vs 癫痫）
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q3910，目标 < 60 秒选 D
> - [ ] 默写 **Vaughan Williams 4 大类 + 代表药 + QT 效应**（用 "1A 长 1B 短 2β 4 钙是真朋友 3 全长"口诀）
> - [ ] 默写 **LQT1 / 2 / 3 三亚型对比**（基因 / 触发 / ECG / 猝死率 / β-blocker 反应 / 特殊治疗）
> - [ ] 默写 **三亚型触发口诀**（游泳 1 / 听铃 2 / 睡觉 3）
> - [ ] 默写 **三亚型 ECG 口诀**（1 宽 2 双 3 晚）
> - [ ] 默写 **三亚型治疗个性化口诀**（1 β 救命 / 2 补 K 防铃 / 3 美西律救场）
> - [ ] 默写 **J&L-N vs Romano-Ward 鉴别**（AR + 聋 vs AD 仅心；J&L-N = LQT1 纯合）
> - [ ] 默写 **Torsades 急诊处理**（Magnesium → pacing / Iso，禁 β-blocker）
> - [ ] 默写 **QT 延长 5 行口诀**（IA III / 大环三环喹诺酮 / 抗精抗吐昂丹 / 氯喹噻嗪阿唑钠 / 哪位鸦片镁钾钙）
> - [ ] 默写 **12 必背抗心律失常药**
> - [ ] 默写 **5 急救场景**
> - [ ] 默写 **3 禁忌组合**
> - [ ] 找类似题：① Brugada syndrome ② CPVT ③ 获得性 QT 延长 ④ TdP 急救 ⑤ Andersen-Tawil
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #要做题（电生理 + 抗心律失常药）
> - [ ] **建立"遗传性离子通道病 ≠ 抗心律失常药"思维**：LQTS 反而禁用大多数；β-blocker 是基础
> - [ ] **修正"看 ECG 才能诊断"误区**：USMLE 题 stem 文字会给 QT 数字，不必读图
> - [ ] **建立"基因 + 临床"双标签认知**：LQT1 / 2 / 3 基因层；Romano-Ward / J&L-N 临床层
> - [ ] **5 天专攻抗心律失常药计划**：Day1 框架 → Day2 12 药 → Day3 3 表 → Day4 题练 → Day5 默写
> 
> ---
> 
> 学科:: 心血管
> 主题:: 先天性 LQTS（J&L-N + LQT1 / 2 / 3 + Vaughan Williams + QT 延长病因）
> 状态:: 🟡
> 错因:: 知识

---

> [!example]- [2026-05-14] 心内 / 急救 / 心脏骤停 PEA 处理 (Q4725)
> ^Q4725
> 
> ## Stem 模式
> 患者突发无脉 + agonal breathing + 监护仪显示**有节律**（如房颤）→ **PEA (Pulseless Electrical Activity)** → **不可除颤** → CPR + Epi + 找 5H5T 可逆因
> 
> ## 核心概念
> **"有电活动 ≠ 有循环"**。监护仪显示节律但患者无脉 = PEA = 不可除颤。**"先看脉搏，后看节律"**——脉搏决定治疗，节律决定诊断。
> 
> ## 普适规则
> 
> **① 心脏骤停 4 种节律对照表（必背）⭐⭐⭐**
> 
> | 节律 | ECG 特征 | 脉搏 | 处理 | 是否除颤？|
> |---|---|---|---|---|
> | **VF**（室颤）| 完全混乱波形，无 QRS | 无 | CPR + **除颤** + Epi | ✓ **是** |
> | **Pulseless VT**（无脉室速）| 宽 QRS 规整 / 多形 | 无 | CPR + **除颤** + Epi | ✓ **是** |
> | **PEA**（无脉电活动）| **任何有形节律**（窦律 / 房颤 / 缓慢 / etc）| **无** ★ | CPR + Epi + 5H5T | ❌ **否** |
> | **Asystole**（停搏）| **直线**（确认 2 导联）| 无 | CPR + Epi + 5H5T | ❌ **否** |
> 
> **口诀**：**"V 除颤（VF + 无脉 VT），P/A 按压（PEA + Asystole）"**
> 
> **② 完整 ACLS 算法**
> 
> ![[{D20DE2F4-B2B2-475A-8530-4F4B105CE8BD}.png]]
> *(UWorld 官方流程图)*
> 
> 文字版：
> 
> ```
> 心脏骤停（无意识 + 无脉）
>         │
>         ▼
>    立即 CPR + 给氧 + 连监护
>         │
>         ▼
>    评估节律
>         │
>    ┌────┴────────────────────┐
>    ▼                          ▼
> 可除颤 (VF / pulseless VT)  不可除颤 (PEA / Asystole)
>    │                          │
>    ▼                          ▼
> Defibrillation (200J 双相)  CPR x 2 min
>    │                          + IV / IO access
>    ▼                          + Epi 1 mg q3-5 min
> CPR x 2 min                  + Treat reversible (5H5T)
>    + IV / IO                  │
>    + Epi 1 mg q3-5 min        ▼
>    │                       重新评估节律
>    ▼                       （循环或 ROSC）
> 重新评估节律
>    │
>    ▼
> 仍 VF? → 再除颤
>    + Amiodarone 300 mg（第 3 次除颤后）
>    │
>    ▼
> ROSC → 复苏后管理（targeted temp / ICU）
> ```
> 
> **③ 5H5T 可逆因（PEA / Asystole 必找）**
> 
> ```
> 5H：                          5T：
> 1. Hypovolemia 低血容量       1. Tension pneumothorax 张力气胸
> 2. Hypoxia 低氧               2. Tamponade (cardiac) 心包填塞
> 3. Hydrogen ion (酸中毒)       3. Toxins 毒物
> 4. Hypo / Hyperkalemia 钾异常 4. Thrombosis (PE) 肺栓塞
> 5. Hypothermia 低温           5. Thrombosis (MI) 冠脉栓塞
> ```
> 
> **针对性处理**：
> - Hypovolemia → IV 补液
> - Tension pneumo → 针刺减压
> - Tamponade → 心包穿刺
> - PE → 溶栓
> - 高 K → Ca + insulin / glucose + Kayexalate
> - MI → 心导管 / 溶栓
> 
> **④ ACLS 用药速查**
> 
> | 药 | 剂量 | 用途 | 时机 |
> |---|---|---|---|
> | **Epinephrine** | **1 mg IV / IO q3-5 min** | **所有 4 种骤停节律** ⭐ | 越早越好 |
> | **Amiodarone** | 300 mg IV bolus → 150 mg | VF / 无脉 VT | **第 3 次除颤后** |
> | **Lidocaine** | 1-1.5 mg/kg | VF / 无脉 VT 替代 | Amio 替代 |
> | **Magnesium** | 1-2 g | **Torsades de Pointes** | 任何时间 |
> | **Atropine** | 1 mg | **症状性窦缓 / AV 阻滞**（有脉）| ❌ **不用于 asystole**（2010 移除）|
> | **Ca / Bicarb** | — | 选择性（高 K / CCB 中毒 / 酸中毒）| 可逆因 |
> 
> **⑤ 三种"电击方式"区分**（USMLE 高频混淆）
> 
> | 维度 | **Defibrillation** | **Synchronized Cardioversion** | **Pacing** |
> |---|---|---|---|
> | 同步 R 波？| **否** | **是** | — |
> | 能量 | 高（200J 双相）| 低（50-200J 递增）| — |
> | **脉搏要求** | 必须**无脉** | 必须**有脉** | 有脉 |
> | 适应症 | VF / 无脉 VT | **有脉**的不稳定 SVT / 房颤 / 单形 VT | 症状性窦缓 / AV 阻滞 |
> | 患者意识 | 无 | 可能需镇静 | 清醒 |
> 
> **⑥ 三种"心律失常急救"分类决策树**
> 
> ```
> Step 1: 患者有脉吗？
>    │
>    ┌────┴────┐
>    无脉      有脉
>    │         │
>    ▼         ▼
> Step 2a:  Step 2b: 稳定吗？
> 评估节律     │
>    │      ┌──┴──┐
>    ▼     稳定   不稳
> ┌──┴──┐   │      │
> VF/VT  PEA/  ▼      ▼
> 除颤   Asys 抗心律 ⭐ Synchronized
>       CPR  失常    Cardioversion
>            药      （房颤 / SVT / 单形 VT
>            (按类   不稳定时）
>             型选)
> ```
> 
> **⑦ "看到房颤" 答题决策**（本题核心陷阱）
> 
> ```
> 看到 stem 提到房颤 → 必须先问：
> 
> 1. 有脉吗？
>    - 无脉 → PEA → CPR + Epi（不电击！）★ 本题
>    - 有脉 → 继续
> 
> 2. 血流动力学稳定吗？
>    - 不稳定（低 BP / 意识改变 / 胸痛 / 心衰）→ Synchronized Cardioversion
>    - 稳定 → 率控（β-blocker / CCB）或律转（amiodarone / cardioversion 择期）
> 
> 3. WPW 患者？
>    - 是 → Procainamide / Ibutilide / 电复律（不用 AV 结阻滞剂）
> ```
> 
> ## 易混陷阱（普适）
> - ❌ **看到房颤 = 复律**：必须先看脉搏；无脉房颤 = PEA = 不电击
> - ❌ **PEA 可以除颤**：错！PEA = 电活动正常但心肌不收缩，电击对"机械停跳"无效
> - ❌ **Asystole 给 atropine**：错！2010 AHA 已移除；asystole = CPR + Epi
> - ❌ **"有节律 = 有循环"**：错！PEA 关键就是节律和循环脱钩
> - ❌ **见骤停先评估 ABG / 实验室**：错！先 CPR；评估同步做
> - ❌ **第一次除颤就给 amiodarone**：错！第 3 次除颤后才给
> - ❌ **Defibrillation 和 Cardioversion 一样**：错！同步与否 + 脉搏要求完全不同
> - ❌ **Lidocaine 是 PEA 一线药**：错！Lidocaine 仅用于 VF / 无脉 VT
> - ❌ **"flatline shock"（直线电击）**：电视剧才有；真实临床绝不电击 asystole
> - ❌ **PEA 不需要找原因**：错！5H5T 必找；不像 VF 单纯电击就行
> 
> ## 我为什么错
> - 选了：**C. Defibrillation**
> - 错因：**pattern**（"看到房颤 + 速率 → 想复律 → 选除颤"——忽略 stem 写的 "no palpable pulse" + "agonal breathing" 关键词，被"还显示房颤"误导）
> - 核心陷阱：**"看到节律就反射性想电治疗，忘了先看脉搏"** — 节律决定诊断，**脉搏决定治疗**
> 
> **具体错位**：
> - ☑ 忽略"无脉"关键词：被"还显示房颤"拖偏
> - ☑ 混淆"有脉房颤"和"无脉房颤"：前者复律，后者 = PEA = CPR
> - ☑ 没按 ACLS 算法走：骤停永远先 CPR + 评估节律 + 二分
> - ☑ 4 种骤停节律记忆混淆：忘了 PEA = 不可除颤
> 
> ## Memory Hook
> 
> **🎯 核心口诀**：
> > **"V 除颤（VF + 无脉 VT），P/A 按压（PEA + Asystole）"**
> > **"先看脉搏，后看节律"**
> 
> **🎯 PEA 比喻**：
> > **"PEA = 电话有铃声但没人接"**
> > - 监护仪显示节律 = 铃声
> > - 心肌不收缩 = 没人接
> > - 电击没用（电铃声的话没意义）
> > - 治疗 = 找"为什么没人接"（5H5T）+ 持续敲门（CPR）+ 唤醒剂（Epi）
> 
> **🎯 "看到房颤" 答题三步**：
> > 1. 有脉吗？无脉 → PEA → CPR
> > 2. 不稳吗？是 → 同步电复律
> > 3. WPW 吗？是 → Procainamide / 电复律
> 
> **🎯 ACLS 时间窗**：
> > "3 个时间数字记牢"：
> > - **30:2** = CPR 按压：通气比
> > - **2 min** = 每周期 + rhythm check
> > - **3-5 min** = Epi 间隔
> 
> **🎯 5H5T 速记**：
> > H = "5 个 Hypo-"（Hypovolemia / Hypoxia / Hypothermia / Hypo-Hyperkalemia）+ H 离子（酸）
> > T = "5 个 T"（Tension pneumo / Tamponade / Toxins / Thrombosis × 2: PE + MI）
> 
> **🎯 关键反陷阱**：
> > **"V 字开头要除颤；P/A 开头要按压。"**
> > - V = Ventricular (VF + VT)
> > - P/A = Pulseless / Asystole
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | 知道这个知识点但时间长会混淆 | 建立"先脉搏后节律" + "V vs P/A"二分口诀；建议 ACLS 5 天巩固 |
> | 看到房颤直接想到电击是常见反射 | 关键不在节律是房颤，关键在**脉搏**；3 种"电"方式（defib / sync / pacing）适应症完全不同 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q3910]] LQTS（今日，电生理 + 抗心律失常药系列）
>   - 与今日 Q4212 / Q3504 / Q3354 / Q19889 / Q3910 共同构成 7 题"紧急决策"系列
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_ACLS急救决策树]] ⭐（本题落地的衍生笔记 — 12 个 Part 完整版）
>   - [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] ⭐（**姊妹笔记** — 药物对照视角）
>   - [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别|读题策略 — pattern 反射误]] ⭐（"看到节律就电"反射 = 模式识别错位）
>   - [[完整笔记/Peixuan分科笔记/心内]]（ACLS + 心律失常急救）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/外科]]（创伤性心包填塞 → PEA → 穿刺；张力气胸 → PEA → 针刺）
>   - [[完整笔记/Peixuan分科笔记/pulmonary]]（大块 PE → PEA → 溶栓）
>   - [[完整笔记/Peixuan分科笔记/感染]]（脓毒症休克 → 持续低血容量 → PEA）
>   - [[完整笔记/专题笔记/_衍生_主动脉急症决策树]]（心包填塞共享 — 难治性休克 / PEA 系列）
> - 🌱 TODO（待生成衍生）：
>   - ⭐ **立即可建**（与 Q3910 抗心律失常药合并）：累计 3+ 道 ACLS / 急救题 → 生成 [[完整笔记/专题笔记/_衍生_ACLS急救决策树]]（含 4 节律 + 5H5T + 用药 + 三种"电"方式对比 + ROSC 后管理）
>   - 累计 3+ 道"电击选择"题（除颤 vs 同步 vs 不电）→ 整合入 [[完整笔记/专题笔记/_衍生_ACLS急救决策树]] 子章节
>   - 累计 3+ 道 PEA 病因题（5H5T 各场景）→ 生成 [[完整笔记/专题笔记/_衍生_PEA可逆因鉴别]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q4725，目标 < 30 秒选 B
> - [ ] 默写 **4 种骤停节律对照表**（VF / 无脉 VT / PEA / Asystole × ECG / 脉搏 / 处理 / 是否除颤）
> - [ ] 默写 **ACLS 完整算法**（评估 → 可除颤分支 vs 不可除颤分支 → 用药 + 时间）
> - [ ] 默写 **5H5T 完整列表 + 每个对应处理**
> - [ ] 默写 **ACLS 用药 + 时机**（Epi q3-5min / Amio 第 3 次后 / Mg for TdP / Atropine 不用 asystole）
> - [ ] 默写 **Defibrillation / Synchronized Cardioversion / Pacing 三对比**（同步？能量？脉搏要求？适应症？）
> - [ ] 默写 **3 种心律失常急救分类**（无脉 / 有脉不稳定 / 有脉稳定）
> - [ ] 默写 **"看到房颤"答题三步**
> - [ ] 找类似题：① VF 处理时机 ② 同步复律适应症 ③ 5H5T 各因（PE / tamponade / 高 K / 张力气胸 / hypothermia）④ Asystole 处理 ⑤ ROSC 后管理
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（ACLS）
> - [ ] **建立"先看脉搏后看节律"思维**：永远先确认脉搏，再决定治疗
> - [ ] **修正"房颤 = 复律"反射**：必须先看脉搏 + 稳定性
> - [ ] **熟记"V 除颤 P/A 按压"口诀**：4 种骤停节律二分
> - [ ] **建立"PEA = 电话响没人接"比喻**：节律 ≠ 循环
> - [ ] **ACLS 5 天巩固计划**：Day1 4 节律 → Day2 5H5T → Day3 用药 → Day4 三种"电"方式 → Day5 全套默写
> 
> ---
> 
> 学科:: 心血管
> 主题:: 心脏骤停 PEA + ACLS 算法（先脉搏后节律）
> 状态:: 🟡
> 错因:: pattern
