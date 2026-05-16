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
> 主题:: Vaughan-Williams 抗心律失常药分类
> 状态:: 🟡
> 错因:: 知识

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

> [!example]- [2026-05-14] 心内 / 晕厥 / Volume-mediated Orthostatic Syncope (Q21638)
> ^Q21638
> 
> ## Stem 模式
> 摔跤运动员（搏击类）+ 比赛后晕厥 + 起立触发 + 前驱头晕 + **脱水四联指纹**（Hct↑ / BUN-Cr↑ / 干燥黏膜 / 低 K）→ **Volume-mediated Orthostatic Hypotension** due to **weight-cutting 致脱水**
> 
> ## 核心概念
> Orthostatic Hypotension (OH) **不是一种病，是一组机制**。两大型机制截然不同：
> - **Volume-mediated（容量型）**：池子里水不够，反射弧完好（HR 能 ↑ 但无效）
> - **Neurogenic（神经源型）**：水够但反射弧坏了（HR 不能 ↑）
> 
> 关键鉴别 = **HR 反应**：站起来 HR↑≥30 = 容量型；HR 几乎不动 = 神经源型。
> 
> ## 普适规则
> 
> **① 晕厥鉴别 4 大类（USMLE 必背）⭐⭐⭐**
> 
> | 维度 | **心源性** | **反射性（vasovagal）** | **Orthostatic** ★ | **癫痫** |
> |---|---|---|---|---|
> | 前驱症状 | **无**（突发）| 有（恶心 / 出汗 / 视暗）| **有**（头晕 / 视暗）| Aura |
> | 触发 | 运动 / 卧位 / 无诱因 | 情绪 / 疼痛 / 站久 | **站起来** ⭐ | 闪光 / 睡眠剥夺 |
> | 持续 | 数秒 | < 1 min | < 1 min | 数分钟 |
> | 恢复 | 立即清醒 | 立即清醒 | 立即清醒 | **Postictal confusion** |
> | 舌咬 / 失禁 | 罕见 | 罕见 | 罕见 | **常有** |
> | HR | 异常 | 缓慢（迷走）| 通常 ↑ 但脱水代偿不足 | 不定 |
> | 心脏体检 / ECG | 异常 | 正常 | 正常 | 正常 |
> | 关键体征 | 杂音 / 异常 ECG | — | **脱水四联** ★ | 抽搐 + postictal |
> 
> **② Orthostatic Hypotension 两型核心鉴别 ⭐⭐⭐**
> 
> | 维度 | **Volume-mediated**（Q21638）| **Neurogenic / Autonomic** |
> |---|---|---|
> | **机制** | 血容量不足 | 反射弧受损 |
> | **血容量** | 低 | 正常 |
> | **反射弧** | 完好 | 受损 |
> | **HR 反应** | **↑ ≥ 30 bpm** ⭐ | **不变 / ↑ < 10-15 bpm** ⭐ |
> | **Hct** | **↑**（浓缩）| 正常 |
> | **BUN/Cr** | **> 20**（prerenal）| 正常 |
> | **K** | 可低 | 正常 |
> | **黏膜** | **干燥** | 正常 |
> | **皮肤** | 干 | 出汗异常 |
> | **仰卧 BP** | 偏低 | **可正常 / 仰卧 HTN（反常）** |
> | **附带症状** | 脱水征 | **胃轻瘫 / 便秘 / 阳痿 / 神经源膀胱** |
> | **典型患者** | 年轻 / 急性 / 运动员 | **60yo DM / Parkinson / MSA / 高龄** |
> | **病程** | 急性（小时-天）| **慢性进行性**（月-年）|
> | **治疗反应** | **补液后快速改善** | **顽固，需药物** |
> 
> **③ 脱水四联指纹（必背）**
> 
> ```
> 见到这 4 个组合 → 锁定 hypovolemia：
> 1. Hct ↑（hemoconcentration，男 > 53%）
> 2. BUN/Cr 比 > 20（prerenal AKI）
> 3. 干燥黏膜
> 4. 低 K（利尿剂 / 出汗 / 醛固酮代偿）
> ```
> 
> **④ Orthostatic Hypotension 病因完整谱**
> 
> ```
> Volume-mediated（容量型）★ HR 能反应：
> - 脱水（呕吐 / 腹泻 / 出汗 / 限水 / 烧伤）
> - 失血（创伤 / GI 出血 / 月经）
> - 利尿剂
> - 静脉淤积（怀孕 / 静脉曲张 / 卧床）
> 
> Neurogenic（神经源型）★ HR 不反应：
> - 周围自主神经病
>   - **DM 自主神经病**（最常见）
>   - Amyloidosis / 副肿瘤 / HIV / 酗酒
> - 中枢自主神经病
>   - **Parkinson disease**
>   - **Multiple System Atrophy (MSA)**
>   - **Pure Autonomic Failure (PAF)**
>   - Lewy body 痴呆
> - 高龄 / 脊髓损伤（T6 以上）
> 
> Mixed / Other：
> - **PAI（昨日 Q17169）= 容量 + 反射混合**
> - 药物（α 阻滞 / TCA / 抗 HTN / 利尿）
> - 餐后 OH（老年 + 大餐 + 内脏淤积）
> - 心源性（HF / AS / 心动过缓）
> ```
> 
> **⑤ Orthostatic 诊断标准**
> 
> ```
> 床旁测试：
> 1. 仰卧 5 min → 测 BP + HR
> 2. 站立 1 / 3 min → 复测
> 
> 诊断阳性：
> - SBP ↓ ≥ 20 mmHg 或
> - DBP ↓ ≥ 10 mmHg
> 
> 分型（关键）：
> - 容量型：HR ↑ ≥ 30 bpm（反射保留尝试代偿）
> - 神经源型：HR 几乎不变 / ↑ < 10-15 bpm
> ```
> 
> **⑥ Orthostatic 治疗阶梯（按型不同）**
> 
> ```
> 容量型治疗（多数补液后解决）：
> 1. 补液 + 补电解质
> 2. 停"作恶"药物（利尿剂 / α 阻滞）
> 3. 治根本病因（出血止血等）
> 4. 体位渐变
> 
> 神经源型治疗（顽固，需长期管理）：
> 1. 非药物（首选）：
>    - 体位渐变（30 秒规则）
>    - 增 Na + 水（2-3 L/天）
>    - **弹力袜**（thigh-high）
>    - 床头抬高 10-20°
>    - 避热水浴 / 大餐 / 酒精
> 2. 药物（顽固病例）：
>    - **Fludrocortisone**（保 Na 增容量）
>    - **Midodrine**（α₁ 激动 → 血管收缩）⭐ 神经源 OH 关键药
>    - Droxidopa（NE 前体）
>    - Pyridostigmine
> 3. 治根本病（优化血糖等）
> ```
> 
> **⑦ 摔跤运动员 / 搏击运动 USMLE 高频考点 ⭐**
> 
> | 考点 | 临床表现 |
> |---|---|
> | **Weight-cutting 致脱水** | **本题** — orthostatic + 脱水四联 + 低 K |
> | **运动诱发猝死** | HCM / Brugada / 长 QT / **Commotio cordis**（胸前撞击 → R-on-T → VF）|
> | **AAS（合成代谢类固醇）滥用** | 男化 / 不孕 / HCM / 肝瘤 / 痤疮 / 心衰 |
> | **过度训练综合征** | 慢性疲劳 + 表现下降 + 抑郁 |
> | **Female Athlete Triad** | 月经异常 + 骨密度低 + 进食障碍 |
> 
> **⑧ DM 自主神经病的"三联证据"（神经源 OH 经典 stem）**
> 
> ```
> 长期 DM（> 10 年）+ HbA1c 高 + 以下任何组合：
> 1. 心血管：OH + 静息心动过速 + 心率变异性消失 + **仰卧 HTN**
> 2. 胃肠：胃轻瘫（早饱 / 餐后腹胀）+ 便秘 / 腹泻交替
> 3. 泌尿生殖：神经源性膀胱（残余尿 / 反复 UTI）+ **阳痿 (ED)**
> 4. 出汗：无汗症 / 异常出汗
> 5. 瞳孔：反应迟钝
> 
> → 见 DM 患者 + OH + 任何 2 项 = 自主神经病高度怀疑
> ```
> 
> ## 易混陷阱（普适）
> - ❌ **OH 就是脱水**：错！神经源型容量正常，反射坏了；不是所有 OH 都补液能好
> - ❌ **HR ↑ 就排除 OH**：错！HR ↑ 反而是容量型的特征（反射尝试代偿）
> - ❌ **HR 正常排除 OH**：错！神经源型 HR 几乎不变才是诊断特征
> - ❌ **仰卧 BP 正常排除 OH**：错！甚至仰卧 HTN 也支持神经源型（反常征）
> - ❌ **DM 患者晕厥 = 低血糖**：错！应同时考虑自主神经病致 OH（尤其慢性 DM + ED + 胃轻瘫）
> - ❌ **选对题不深挖机制**：直觉对 ≠ 机制懂；变形题会失误（本题最重要教训）
> - ❌ **OH 与心源性晕厥混**：心源无前驱，OH 有前驱（头晕）；心源任何体位发，OH 仅站起触发
> - ❌ **OH 治疗都用 midodrine**：容量型补液就够；midodrine 是神经源型才需要
> 
> ## 我为什么错
> - 选了：**E. Orthostatic hypotension**（**选对但机制不清楚**）
> - 错因：**知识**（机制深度不够 — 直觉 50-60% 对，机制清楚才能 90%+ 对；变形 stem 如老年 DM + 同样症状但 HR 不动会失误）
> - 核心陷阱：**"选对题不深挖机制 → 应付不了变形 stem"**
> 
> **本次学到的深层机制**：
> - ☑ Orthostatic 不是单一病因，是**容量型 vs 神经源型两大机制**
> - ☑ 关键鉴别 = **HR 反应**（容量型↑≥30，神经源型几乎不动）
> - ☑ 实验室不同：容量型有脱水四联，神经源型实验室正常
> - ☑ 治疗不同：容量型补液即可，神经源型需 midodrine
> - ☑ 摔跤运动员 weight-cutting 是 USMLE 高频背景考点
> 
> ## Memory Hook
> 
> **🎯 一句话锁定本题**：
> > "摔跤运动员 + 比赛后晕 + 脱水四联（Hct↑ / BUN-Cr↑ / 干燥 / 低 K）= Volume-mediated Orthostatic Hypotension。"
> 
> **🎯 晕厥鉴别"前 5 后"速记**：
> > **前**驱症状 → 反射性或 orthostatic（**有前驱**）
> > 突发**无**前驱 → 心源性
> > **5** 分钟以上无意识 → conversion disorder
> > 苏醒**后** confusion → 癫痫（postictal）
> 
> **🎯 OH 两型本质类比**：
> > **容量型 = "池子里水不够"**：年轻 / 急性 / HR 努力补救（但失败）
> > **神经源型 = "池子里水够但水泵开关坏了"**：老年 / 慢性 / HR 不动
> 
> **🎯 OH 病因 5 类速记 "湿干自主药老"**：
> > 1. **湿**（容量丢失）= Hypovolemia ★（本题）
> > 2. **干**（容量不补）= 摄入不足 / 烧伤
> > 3. **自主**（autonomic）= **DM** / Parkinson / MSA / 高龄
> > 4. **药**物 = α 阻滞 / TCA / 利尿 / 抗 HTN
> > 5. **老**（内分泌）= **PAI**（昨日 Q17169 — 与本题"指纹思维"互联）
> 
> **🎯 "脱水四联"指纹**（与昨日 PAI 五联思维联动）：
> > 1. Hct ↑（hemoconcentration）
> > 2. BUN/Cr 比 > 20（prerenal AKI）
> > 3. 干燥黏膜
> > 4. 低 K
> > 
> > 见到 → 想 **Hypovolemia** → 链回 [[完整笔记/专题笔记/_衍生_实验室指纹诊断大全]]
> 
> **🎯 神经源 OH 反常征**：
> > **"DM + OH + 仰卧 HTN + 胃轻瘫 + ED" = 自主神经病五联**
> > 越多组合越确诊，即使一个组合也要警惕
> 
> **🎯 摔跤运动员考点 3 类**：
> > 1. **Weight-cutting** → 脱水 + 低 K + orthostatic（本题）
> > 2. **运动中猝死** → HCM / Brugada / LQTS / commotio cordis
> > 3. **AAS 滥用** → 男化 / 不孕 / HCM / 肝瘤
> 
> **🎯 选对题深挖机制方法论**（最重要的学习态度）：
> > 直觉对 ≠ 机制懂。选对的题尤其要问：
> > 1. 为什么答案是这个？
> > 2. 如果 stem 改一个细节（年龄 / 实验室 / 体征），答案变吗？
> > 3. 这个诊断的"亚型 / 分型"是什么？
> > 4. 每种亚型的鉴别要点 + 治疗差异？
> > 
> > ⭐ 这就是 NBME 230 → 250 的关键瓶颈
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | 选对了但机制不清楚 | Orthostatic 两型本质区别（容量 vs 神经源）|
> | 60yo DM 同样症状 + 正常 Hct 怎么解释？ | 神经源型 OH：反射弧坏（HR 不动）+ 仰卧 HTN（反常）+ 自主神经三联（胃轻瘫 / 便秘 / ED）+ 治疗用 midodrine 而非补液 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q3910]] LQTS（同日，"运动诱发晕厥"鉴别 — Q3910 是 LQT1 不是 orthostatic）
>   - [[mistakes/uworld-mistakes#^Q17169]] PAI（同日，**"脱水四联"指纹思维**第二次应用 + adrenal crisis 也致 orthostatic）
>   - [[mistakes/uworld-mistakes#^Q4725]] PEA（今日，"先脉搏后节律"和"先 HR 反应后定型"思路类似）
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]] ⭐（本题落地的衍生笔记 — 11 个 Part 完整版）
>   - [[完整笔记/专题笔记/_衍生_实验室指纹诊断大全]] ⭐（Part 6.7 脱水四联指纹已沉淀）
>   - [[完整笔记/Peixuan分科笔记/心内]]（晕厥鉴别 + orthostatic hypotension）
>   - [[完整笔记/Peixuan分科笔记/外科]]（运动医学 + 搏击类运动相关疾病）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/endocrine]]（PAI 致 orthostatic — adrenal hypovolemia；DM 致自主神经病）
>   - [[完整笔记/Peixuan分科笔记/neuro]]（自主神经病 → orthostatic：DM / Parkinson / MSA）
> - 🌱 TODO（待生成衍生）：
>   - ⭐ **立即可建**（与今日 Q3910 / Q4725 / Q4212 合并）：累计已 4 道晕厥 / 休克相关题 → 生成 [[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]]（含 4 大类 + OH 两型 + 完整鉴别）
>   - 累计 3+ 道 OH 病因鉴别题 → 生成 [[完整笔记/专题笔记/_衍生_体位性低血压两型对比]]
>   - 累计 3+ 道运动员相关题（HCM / Commotio / AAS / weight-cutting / Female Triad）→ 生成 [[完整笔记/专题笔记/_衍生_运动员相关疾病]]
>   - ⭐ **方法论合并**：今日已累计 3 道 "**指纹思维**" 应用（PAI 五联 / 4B 血管创伤 / **脱水四联**）→ 已在指纹大全沉淀
>   - 累计 3+ 道 DM 慢性并发症题（视网膜 / 肾病 / 自主神经病 / 周围神经病）→ 生成 [[完整笔记/专题笔记/_衍生_DM慢性并发症]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q21638，目标 < 60 秒选 E + 能说明完整机制
> - [ ] 默写 **晕厥 4 大类鉴别表**（心源 / 反射 / 体位 / 非晕厥 × 前驱 / 触发 / 持续 / 恢复 / HR / ECG）
> - [ ] 默写 **OH 两型核心对比**（机制 / HR / Hct / BUN-Cr / 仰卧 BP / 附带症状 / 治疗）
> - [ ] 默写 **OH 病因 5 类**（湿干自主药老）
> - [ ] 默写 **脱水四联指纹**（Hct↑ / BUN-Cr↑ / 干燥 / 低 K）
> - [ ] 默写 **OH 诊断标准**（SBP↓≥20 / DBP↓≥10 / HR↑≥30 区分容量 vs 神经源）
> - [ ] 默写 **OH 治疗阶梯**（容量型补液 vs 神经源型 midodrine / fludrocortisone）
> - [ ] 默写 **DM 自主神经病三联 / 五联**（OH + 胃轻瘫 + 便秘 + ED + 仰卧 HTN）
> - [ ] 默写 **摔跤运动员 3 大考点**
> - [ ] 找类似题：
>   - ① 60yo DM + 慢性 OH + 仰卧 HTN（神经源型）
>   - ② Parkinson 患者 + OH（神经源 + 药物混合）
>   - ③ 老年人 + α 阻滞剂 + 起立晕厥（药物诱发）
>   - ④ MSA 患者（罕见但 USMLE 偶尔考）
>   - ⑤ Vasovagal syncope（鉴别）
>   - ⑥ HCM 运动猝死（鉴别）
>   - ⑦ Commotio cordis（胸前撞击致 VF）
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（晕厥章节）
> - [ ] **建立"前驱症状 + 触发"晕厥分类反射**
> - [ ] **建立"脱水四联指纹"诊断习惯**（与昨日 PAI 五联指纹合并形成"指纹思维"系统）
> - [ ] **建立"HR 反应分型 OH"思维**：见 OH 题立即问"HR 变化多少？"
> - [ ] **修正"选对就不深入"误区**：选对的题尤其要深挖机制 → 应对变形 stem
> - [ ] **建立"年龄 + 病程"OH 分型直觉**：年轻 + 急性 → 容量型；老年 + 慢性 → 神经源型
> 
> ---
> 
> 学科:: 心血管
> 主题:: Orthostatic Hypotension 两型（容量 vs 神经源）+ 晕厥 4 类鉴别
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-14] 心内 / 晕厥 / Classic Vasovagal Syncope → No Further Testing (Q21579)
> ^Q21579
> 
> ## Stem 模式
> 中年女性 + **情绪应激**（赶车）+ 经典前驱（**sweaty + warm**）+ **< 1 min** 失意识 + **立即清醒无 postictal** + 体检 / ECG / 体位测试均正常 → **Classic Vasovagal Syncope** → **No further testing**
> 
> ## 核心概念
> 经典 vasovagal **靠病史诊断**（history alone）：典型 prodrome + 触发 + 短暂 + 立即清醒 + 体检 ECG 正常 → **不需要任何检查**。检查只在**不典型 / 反复 / 红旗**时做。**典型 + 无红旗 → No further testing** 是 USMLE 越来越高频的"反向应用框架"题型。
> 
> **UWorld 官方速查表：Clues to etiology of syncope**（本地截屏）：
> 
> ![[{0AE45501-AAE4-4239-B13D-93EEEE90B76B}.png]]
> 
> ## 普适规则
> 
> **① 晕厥 6 大类完整分类系统 ⭐⭐⭐**
> 
> ```
> ① 反射性晕厥（Reflex / Neurally-Mediated）
>    - Vasovagal（情绪 / 看血 / 长站）★ 本题
>    - Situational（特定行为：排尿 / 排便 / 咳嗽 / 吞咽 / 举重）
>    - Carotid sinus hypersensitivity（颈部刺激，> 60 岁）
> 
> ② Orthostatic Hypotension
>    - 容量型（脱水 / 失血 / 利尿剂）
>    - 神经源型（DM / Parkinson / MSA / 高龄）
>    - 药物诱发（α 阻滞 / TCA / 抗 HTN）
> 
> ③ Cardiac Syncope ⚠️ 红旗类
>    - 心律失常（VT / VF / AV 阻滞 / LQT / Brugada）
>    - 流出道梗阻（HCM / AS / PE）
>    - 心衰致低 CO
> 
> ④ Cerebrovascular（罕见）
>    - Subclavian steal（手臂活动）
>    - Vertebrobasilar TIA（伴局灶征）
> 
> ⑤ 非晕厥（鉴别诊断）
>    - Seizure ⭐ 见规则 ⑪
>    - Psychogenic / Conversion
>    - 代谢（低血糖 / 低 Na）
> 
> ⑥ 其他特殊
>    - Post-prandial（餐后老年）
>    - Pregnancy supine hypotensive
> ```
> 
> **② 反射性晕厥 3 子型对比 ⭐**
> 
> | 维度 | **Vasovagal**（本题）| **Situational** | **Carotid sinus** |
> |---|---|---|---|
> | 触发 | 情绪 / 看血 / 长站 / 疼痛 | **特定生理行为** | 颈部刺激（剃须 / 紧领 / 转头）|
> | 典型患者 | 任何年龄（年轻多）| 中老年 + 慢病 | **> 60 岁** + 颈动脉粥样硬化 |
> | 前驱 | **典型 5 联**（sweat / warm / 恶心）| 短暂或无 | 短暂或无 |
> | HR | ↓（迷走）| ↓（迷走）| ↓（显著缓）|
> | 诊断 | 病史 | 触发因素特殊 | **Carotid massage**（HR↓ > 3s 或 SBP↓ > 50）|
> | 治疗 | 教育 + counterpressure | 治根本病 + 行为修改 | 起搏器（严重）|
> 
> **③ Situational Syncope 8 种触发场景**
> 
> | 触发 | 机制 | 经典 stem |
> |---|---|---|
> | **Micturition**（排尿）| Valsalva + 副交感 | 中老年男性 BPH + 夜间排尿 |
> | **Defecation**（排便）| Valsalva + 反射 | 老年便秘用力排便 |
> | **Cough**（咳嗽）| Valsalva 持续 | COPD + 长串咳嗽 |
> | **Swallow**（吞咽）| 食管刺激迷走 | 吞冷饮 / 冰激凌 |
> | **Weight-lifting**（举重）| Valsalva 屏气 | 健身房用力时 |
> | **Sneeze / Laugh** | Valsalva 短爆发 | 大笑 / 喷嚏后 |
> | **Trumpet / 吹奏 / 潜水** | 持续 Valsalva | 演奏 / 屏气潜水 |
> | **Post-prandial**（餐后）| 内脏血流↑ | 老年人 30 min after large meal |
> 
> **④ Vasovagal 双相反射机制（Bezold-Jarisch）**
> 
> ```
> T=0: 触发（情绪 / 疼痛 / 看血 / 长站）
>    ↓
> ─── 第 1 相：交感激活 (T=0-30s) ───
> - 心率 ↑ + 心肌强收缩
> - 出汗 ↑（汗腺胆碱能交感）★ prodrome
> - 温暖感（皮肤血流↑）★ prodrome
>    ↓
> ─── 第 2 相：心室异常感受 (T=30-60s) ───
> - 站立 → 下肢血液淤积 → 心室容量↓
> - 但交感激活让心室强烈收缩 → "空射"
> - 左室机械感受器（C 纤维）异常激活
> - 误传"心脏过满"信号到脑干
>    ↓
> ─── 第 3 相：反常迷走爆发 (T=60-90s) ───
> - 副交感 ↑↑↑ → HR ↓↓
> - 交感 ↓↓↓ → 血管扩张
> - BP 急剧↓
>    ↓
> ─── 第 4 相：晕厥 ───
> - 脑灌注↓ → 失意识
> - 倒地后水平体位 → 血液回流 → 立即清醒
> ```
> 
> **关键反陷阱**：晕厥时 HR ↓（迷走爆发），不是 ↑（很多人误以为心率代偿上升）。
> 
> **⑤ Vasovagal 5 联指纹（必背）**
> 
> | # | 元素 | 描述 | 本题 ✓ |
> |---|---|---|---|
> | 1 | **触发** | 情绪 / 疼痛 / 看血 / 长站 / 拥挤 / 排尿排便 | 赶车应激 ✓ |
> | 2 | **Prodrome** | sweat + warm + 恶心 + 视暗 / 听弱 | sweat + warm ✓ |
> | 3 | **短暂** | < 1 分钟 | 1 min ✓ |
> | 4 | **自发恢复** | 立即清醒 | ✓ |
> | 5 | **无 postictal** | 无 confusion / 失忆 / 抽搐 | ✓ |
> 
> **见这 5 个 → 直接诊断 vasovagal，不需要任何检查**
> 
> **⑥ 晕厥 7 维分类框架 ⭐⭐⭐**（最重要方法论）
> 
> 口诀：**"触前心醒，背伴ECG"**
> 
> | 维度 | 主作用 | 关键鉴别 |
> |---|---|---|
> | **1. 触发** | 区分各亚型 | 运动 = Cardiac；情绪 = Vasovagal；站起 = OH；排尿 = Situational |
> | **2. 前驱** | 反射 vs 心源 vs 癫痫 | 有前驱 ≈ 反射 / OH；无前驱 ≈ Cardiac；**aura（局灶）= Seizure** |
> | **3. HR** | 区分反射 vs OH 亚型 | ↓ = Vasovagal / Situational；↑ ≥ 30 = 容量 OH；不动 = 神经源 OH |
> | **4. 清醒** | 晕厥 vs 癫痫 vs Conversion | 立即 = 晕厥；延迟 = Seizure；> 5min = Conversion |
> | **5. 背景** | 调整概率权重 | > 60 → 心源↑；DM → 自主 OH↑；BPH → 排尿性 Situational |
> | **6. 伴随** | 排查严重病因 | 胸痛 → MI / PE；舌咬 → Seizure；腹痛 → AAA / 异位 |
> | **7. ECG** | 心源筛查 | 异常 = 锁定 Cardiac 亚型 |
> 
> **⑦ 晕厥 5 大类完整决策表**
> 
> | 维度 | **Vasovagal** | **Cardiac** | **OH 容量型** | **OH 神经源** | **Seizure** |
> |---|---|---|---|---|---|
> | 触发 | 情绪 / 看血 / 站久 | **运动 / 卧位 / 无** | **站起来** | **站起来** | 闪光 / 睡眠剥夺 / 停药 |
> | 背景 | 任何 | **> 60 / 心病史 / 家族猝死** | 年轻 + 急性脱水 | **> 60 / DM / Parkinson** | 癫痫病史 |
> | 前驱 | **Prodrome（全身）** | **无** | 有（头晕）| 有 | **Aura（局灶）** ⭐ |
> | HR | **↓** | 异常 | **↑ ≥ 30** | **不变** | 不定 |
> | 清醒 | **立即** | 立即 | 立即 | 立即 | **延迟 + postictal** ⭐ |
> | 伴随 | 无红旗 | **胸痛 / 心悸 / 呼吸困难** | 脱水四联 | 自主神经三联 | **舌咬 / 失禁 / 抽搐 / automatism** |
> | ECG | 正常 | **异常** | 正常 | 正常 | 正常 |
> | 下一步 | **不查** | Echo + Holter | 床旁 BP / HR | autonomic testing | **EEG + MRI** |
> 
> **⑧ 晕厥"红旗"10 条**（必查，提示心源性）
> 
> 口诀：**"运动卧 5 心家电杂老伤"**
> 1. **运动**中
> 2. **卧**位
> 3. **5** 分钟以上失意识
> 4. **心**悸 / 胸痛 / 呼吸困难
> 5. **家**族年轻猝死（< 50 岁）
> 6. 已知**结构性**心脏病
> 7. ECG / **电**生理异常
> 8. 心**杂**音
> 9. **老**年（> 60）
> 10. 严重外**伤**（提示突发无防御）
> 
> **⑨ Tilt-Table Testing 精确适应症 ⭐**
> 
> ```
> 4 大适应症：
> 1. 反复不明原因晕厥 + 床旁评估阴性
> 2. 鉴别 vasovagal vs OH（典型场景困难）
> 3. 怀疑 POTS（年轻女性 + 站立心悸 + BP 不降）
> 4. 评估治疗效果 / 长期随访
> 
> 不需要 tilt-table：
> ❌ 典型 vasovagal（本题）
> ❌ 单次发作
> ❌ 床旁 OH 测试已阳性
> ❌ 已知心源性 → 应做 Echo / Holter
> ❌ 已知癫痫 → 应做 EEG / MRI
> ```
> 
> **核心原理**：被动倾斜（60-70°）= 去掉"肌肉泵代偿"，纯粹考察自主神经反射 + 血容量。比主动站立更能诱发隐匿性 vasovagal / OH。
> 
> **⑩ "No further testing" 答题方法论 ⭐⭐⭐**
> 
> ```
> USMLE 答题 3 步：
> 1. 诊断已经清楚吗？（典型病史 + 无红旗 → 通常清楚）
> 2. 进一步检查能改变处理吗？（不能 → 不查）
> 3. 选项里有 "No further testing" 或 "observation"？很可能是答案
> 
> 经典 "No further testing" USMLE 场景：
> ★ 典型 vasovagal（本题 Q21579）
> ★ 典型 GERD（年轻 + 经典烧心 + 无报警征 → PPI 试验）
> ★ 单纯性头痛（无红旗 → 不做 CT）
> ★ 自限性病毒感染（流感 / 普通感冒 → 支持治疗）
> ★ 典型偏头痛（无红旗 → 不做影像）
> ★ 低风险 ACS 评分（HEART score 低 → 出院）
> ```
> 
> **⑪ Seizure 的 "Prodrome vs Aura vs Postictal" 三阶段 ⭐⭐⭐**（晕厥 vs 癫痫鉴别核心）
> 
> ```
> Seizure 5 期：
> T= -hours/days  ── Prodrome（前驱期，模糊）
>                    数小时-数天的非特异不适
>                    （烦躁 / 疲劳 / 头痛 / 情绪改变）
>                    ★ 不属于发作本身
>                          ↓
> T= -seconds     ── Aura（先兆，局灶性）⭐
>                    数秒-30 秒，局灶性症状
>                    ★ **已经是发作的一部分**（focal seizure）
>                    ★ 反映癫痫起源脑区
>                          ↓
> T= 0            ── Ictal phase（发作期）
>                    强直 / 阵挛 / 失张力 / 失神 / automatism
>                          ↓
> T= +minutes     ── Postictal phase（发作后期）⭐ 金标准鉴别
>                    意识混乱 / 嗜睡 / Todd 麻痹（15-30+ min）
>                          ↓
> T= +hours       ── Recovery（恢复期）
> ```
> 
> **晕厥 prodrome vs Seizure aura 本质区别**：
> 
> | 维度 | **晕厥 prodrome**（vasovagal）| **Seizure aura** |
> |---|---|---|
> | 时间 | 30-60s | **数秒-30s** |
> | 性质 | **全身性**（反射反应）| **局灶性**（癫痫本身）|
> | EEG | 正常 | **局灶性放电** |
> | 典型症状 | sweat / warm / 恶心 / 视暗 | **嗅觉 / 视觉 / déjà vu / 上腹 rising** |
> | 后续 | 渐进失意识 → 立即清醒 | 进入 ictal → **postictal confusion** |
> 
> **⑪a Seizure 内部两种"前驱"区别（关键概念）⭐**
> 
> | 维度 | **Seizure Prodrome（前驱期）** | **Seizure Aura（先兆）** |
> |---|---|---|
> | **时间** | 数小时-数天 | 数秒-30 秒 |
> | **性质** | 非特异，模糊不适 | **局灶性，特异** |
> | **是否癫痫电活动** | 否（推测是神经化学改变）| **是**（focal seizure 的开始）|
> | **EEG** | 通常正常 | **局灶性放电** |
> | **常见症状** | 烦躁 / 疲劳 / 头痛 / 失眠 / 情绪改变 | 嗅觉幻觉 / 视觉幻觉 / déjà vu / 上腹不适 / 麻木 |
> | **临床意义** | 患者自我警报 | 提示**癫痫起源部位** |
> 
> **核心区别**：prodrome 在发作"前"（不是发作本身），aura 是发作"开始"（已是 focal seizure）。USMLE stem 写 "felt anxious for several days before episode" = prodrome；写 "smelled burning rubber 10 seconds before LOC" = aura。
> 
> **⑪b Vasovagal vs Seizure 完整鉴别表 ⭐⭐⭐**（最终金标准）
> 
> | 维度 | **Vasovagal**（本题 Q21579）| **Seizure** |
> |---|---|---|
> | **触发** | 情绪 / 看血 / 长站 | 闪光 / 睡眠剥夺 / 停药 |
> | **前驱性质** | **Prodrome**（反射反应）| **Aura**（局灶发作）|
> | **前驱时长** | 30-60 秒 | 数秒-30 秒 |
> | **前驱症状** | 全身性（sweat / warm / 恶心 / 视暗）| 局灶性（嗅觉 / 视觉 / 感觉 / déjà vu）|
> | **意识** | 渐进失意识 | 突然失意识（局灶后扩散到全身）|
> | **抽搐** | **罕见**（短暂缺氧 "convulsive syncope" 可有）| **常有**（强直 / 阵挛）|
> | **舌咬伤** | 罕见 | **常有**（**侧舌咬** ⭐）|
> | **大小便失禁** | 罕见 | 常有 |
> | **持续** | < 1 min | 数分钟 |
> | **恢复** | **立即清醒** | **Postictal confusion**（5-30 min+）⭐ 金标准 |
> | **HR** | ↓（迷走介导）| 不定 |
> | **诊断** | 病史 | **EEG / MRI** |
> 
> > [!success] 终极金标准
> > **判断 seizure vs vasovagal = "postictal confusion"**
> > - **立即清醒 → 晕厥**
> > - **延迟清醒 + confusion → seizure**
> > 
> > 其他特征都可能"重叠"（如 convulsive syncope 也有短暂抽搐），唯独 postictal confusion 是 seizure 的"印章"。
> 
> **⑫ Seizure Aura 各脑叶定位（USMLE 高频）⭐**
> 
> | Aura 类型 | 起源脑叶 | 典型 stem 描述 |
> |---|---|---|
> | **嗅觉幻觉**（焦糊味）| **颞叶** | "smelled burning rubber" |
> | **Déjà vu**（"似曾相识"）| **颞叶** | "feeling I've been here before" |
> | **Jamais vu**（"陌生感"）| **颞叶** | "familiar place suddenly felt unfamiliar" |
> | **上腹 rising sensation** | **颞叶**（最常见 55%）| "something rising from stomach to chest" |
> | **视觉幻觉**（闪光 / 几何图案）| **枕叶** | "flashing lights / geometric patterns" |
> | **听觉幻觉**（嗡嗡 / 音乐）| **颞叶上回** | "buzzing sound / music" |
> | **躯体感觉异常**（一侧麻木）| **顶叶** | "numbness / tingling in one limb" |
> | **运动**（局部抽搐）| **额叶** | "twitching of one arm" |
> | **恐惧 / 焦虑**（强烈情绪）| **杏仁核 / 颞叶内侧** | "sudden intense fear without reason" |
> | **自主神经**（潮红 / 心悸 / 出汗）| **岛叶 / 颞叶** | ⚠️ 易误为 vasovagal |
> 
> **⑬ Déjà vu 详解**
> 
> ```
> Déjà vu = 法语"already seen"
> 体验："这个新场景我以前经历过"的强烈错觉
> 
> 两种来源：
> ① 正常生理（60-70% 健康人有过，多 15-25 岁）
>    - 偶发 + 数秒 + 无伴随 → 无病理意义
> ② 颞叶癫痫 aura ⭐ USMLE 考点
>    - 反复频繁 + 伴其他症状（嗅觉 / 上腹 / 恐惧）
>    - 后续 ictal phase（automatism / 失意识 / postictal）
> 
> 机制：
> 颞叶内侧"熟悉感开关"被错误激活
> （海马 + 杏仁核 + 内嗅皮层异常放电）
> ```
> 
> **相关词**：
> - **Déjà vécu**（"已经经历过"）：更强版本，几乎专属癫痫
> - **Jamais vu**（"从未见过"）：相反体验，也见于颞叶癫痫
> 
> **⑭ 颞叶癫痫"三联"特征（USMLE 必背）**
> 
> ```
> ① Aura（数秒）
>    - 上腹 rising / déjà vu / 嗅觉 / 恐惧
> ② Ictal phase（1-2 min）
>    - **Automatism**（自动症）★
>      - Lip-smacking（咂嘴）⭐ 最经典
>      - Chewing / picking at clothes / wandering
>    - Impaired awareness（意识受损）
> ③ Postictal（15-30+ min）
>    - Confusion / 头痛 / 嗜睡
>    - 不记得发作过程
> ```
> 
> 治疗：抗癫痫药（Carbamazepine / Lamotrigine / Levetiracetam）
> 
> **⑮ Convulsive Syncope 陷阱**（容易误为 seizure）
> 
> ```
> 晕厥时短暂抽搐 (myoclonic jerks)：
> - 脑灌注↓ → 皮层抑制解除 → 短暂运动激活
> - 持续 < 15 秒
> - **无 postictal**
> - 病史符合晕厥（有触发 + 前驱）
> → 仍是 vasovagal / OH，不是 seizure
> 
> 真正 seizure：
> - 抽搐 > 1 min
> - **Postictal confusion**
> - 舌咬伤 / 失禁
> - 无典型晕厥触发
> ```
> 
> ## 易混陷阱（普适）
> - ❌ **晕厥都要查 Holter / Echo / Tilt-table**：典型 vasovagal 病史诊断，不需检查
> - ❌ **Vasovagal = 单纯迷走过强**：错！是**双相反射**（先交感激活，后迷走爆发）
> - ❌ **晕厥时 HR 应该上升代偿**：错！vasovagal 时 HR 反而 ↓（迷走介导）
> - ❌ **Prodrome 有"冰冷苍白"**：错！典型 prodrome 是"sweat + warm"（第 1 相交感激活）；晚期才苍白
> - ❌ **Tilt-table 是 vasovagal 诊断金标准**：错！典型 vasovagal 靠病史；tilt-table 用于反复 / 不典型
> - ❌ **看到"心梗家族史"就选心源性检查**：错！本题父亲 MI 不算年轻猝死，不构成红旗
> - ❌ **反射性晕厥只有 vasovagal**：错！还有 Situational 和 Carotid sinus 两子型
> - ❌ **Situational = vasovagal**：错！触发不同，处理也不同（治根本病而非教育避诱因）
> - ❌ **运动中晕厥用 vasovagal 框架**：错！运动中 = Cardiac 红旗（HCM / LQT1 / AS）
> - ❌ **Seizure prodrome = Seizure aura**：错！prodrome 是数小时-天的模糊不适；aura 是数秒的局灶性发作开始 ⭐
> - ❌ **Déjà vu 一定是癫痫**：错！正常人 60-70% 有过；**反复 + 伴随症状**才是颞叶癫痫
> - ❌ **看到"晕厥 + 短暂抽搐"诊断 seizure**：错！可能是 convulsive syncope（无 postictal）
> - ❌ **颞叶癫痫的自主症状（心悸 / 出汗）= vasovagal**：错！岛叶 / 颞叶 aura 可包含这些；区别在 postictal
> 
> ## 我为什么错
> - 选了：**A. 24-h Holter monitoring**（思路："晕厥要排除心源性 → Holter 看看心律"；但忽略了 stem 已给出 vasovagal 完整 5 联指纹）
> - 错因：**pattern**（"过度评估倾向"反射 — 默认选"做更多检查"；**第 2 次掉进同陷阱**，与 Q19889 钝性胸创联动）
> - 核心陷阱：**"知道鉴别框架 ≠ 会答 '不查' 题"** — NBME 230 → 250 关键瓶颈
> 
> **具体错位**：
> - ☑ **过度评估倾向**（与 Q19889 第 2 次掉进同陷阱）
> - ☑ **学完晕厥框架后"反向应用失败"**：知道 4 类，但不会"如果无红旗就不查"
> - ☑ **没识别"经典 vasovagal" 5 联指纹**：情绪 + sweat + warm + 1min + 立即清醒
> - ☑ **被干扰项拽走**："心梗家族史 + 高血压 + amlodipine"是分散注意力的线索
> - ☑ **没用阴性体征确认排除**：体检 / ECG / 体位测试全正常 = 排除其他病因
> 
> ## Memory Hook
> 
> **🎯 一句话锁定**：
> > "赶车 + 出汗温暖 + 1 分钟晕 + 立即清醒 + 体检正常 = 经典 Vasovagal → No further testing"
> 
> **🎯 Vasovagal 5 联指纹**：
> > 触发 + Prodrome (sweat / warm / 恶心) + < 1 min + 立即清醒 + 无 postictal
> 
> **🎯 晕厥红旗 10 条口诀**：
> > **"运动卧 5 心家电杂老伤"**
> 
> **🎯 晕厥 7 维分类框架口诀**：
> > **"触前心醒，背伴 ECG"** — 每道晕厥题用这 7 个字扫一遍
> 
> **🎯 反射性晕厥 3 子型类比**：
> > - **Vasovagal** = "情绪型"（心理触发）
> > - **Situational** = "生理动作型"（排尿 / 咳嗽等）
> > - **Carotid sinus** = "颈部刺激型"（老人剃须）
> 
> **🎯 类比"金毛犬"理解 No further testing**：
> > 见到典型金毛犬不必做基因检测确认 → 5 个 vasovagal 特征都到位 = 形象明确 → 再做检查 = 浪费时间 + 钱 + 患者焦虑
> 
> **🎯 "过度评估倾向"修正**（与 Q19889 联动）：
> > 今日已 2 次掉进同一陷阱（Q19889 / Q21579）→ 下一次必须警惕
> > **见 "next step" 题 → 先问"诊断清楚吗？无红旗吗？" → 可能是"不查 / 观察 / 出院"**
> 
> **🎯 双相反射时序记忆**：
> > T=0-30s 交感激活（出汗 + 温暖）→ T=30-60s 心室异常感受 → T=60-90s 迷走爆发（HR↓ BP↓）→ 晕厥 → 倒地后立即清醒
> 
> **🎯 Seizure prodrome vs aura 终极鉴别**：
> > - **晕厥 prodrome** = 反射反应（全身：sweat / warm / 恶心，30-60s）
> > - **Seizure aura** = 局灶发作开始（局灶：嗅觉 / 视觉 / déjà vu / 上腹，数秒）
> > - **判别金标准** = **Postictal confusion**（seizure 有，晕厥无）
> 
> **🎯 颞叶癫痫 4 大经典 aura**（最高频考点）：
> > 1. **上腹 rising sensation**（最常见 55%）
> > 2. **Déjà vu / Jamais vu**
> > 3. **嗅觉幻觉**（焦糊味）
> > 4. **恐惧 / 焦虑感**（无外因）
> > → 后续常出现 **lip-smacking automatism**（咂嘴自动症）
> 
> **🎯 Déjà vu 判别口诀**：
> > "偶发 + 无伴随" = 正常（无病理）
> > "反复 + automatism / postictal" = 颞叶癫痫 aura
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | 先交感激活，再迷走激活，最后晕倒？ | 完全正确！双相反射（Bezold-Jarisch）|
> | OH 要进一步检查吗？Tilt-table 适应症？ | 多数 OH 床旁 BP / HR 就能确诊；Tilt-table 仅用于反复 / 不典型 / POTS |
> | 3 维（前驱 + HR + 清醒）就能分所有 syncope？ | 80% 适用，但需 4 补充维度；7 维框架是完整版 |
> | Situational 在哪里？ | 反射性 3 子型之一；8 种触发场景 |
> | Seizure 算是有前驱吗？ | 有，但 prodrome（数小时-天）和 aura（数秒局灶发作开始）完全不同；金标准是 postictal confusion |
> | Déjà vu 是啥？ | 法语"already seen"；正常人偶尔有（无意义），反复 + 伴 automatism = 颞叶癫痫 aura |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q21638]] Orthostatic Hypotension（同日，与本题对比：Q21638 是真 OH，本题是 vasovagal 不是 OH）
>   - [[mistakes/uworld-mistakes#^Q3910]] LQTS（同日，心源性晕厥代表，与本题反射性形成对比）
>   - [[mistakes/uworld-mistakes#^Q4725]] PEA（今日，急救场景的晕厥）
>   - [[mistakes/uworld-mistakes#^Q19889]] 钝性胸创（同日，**"过度评估倾向"陷阱第 2 次出现** ⭐）
> - 📚 主笔记：
>   - [[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]] ⭐（本题大量补充该衍生：Vasovagal 5 联 / 7 维框架 / Situational 8 种 / Seizure aura 详解 / 颞叶癫痫 / convulsive syncope）
>   - [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别|读题策略 — 反向应用框架]] ⭐（"知道分类不会用 → 不查"是本题方法论缺口）
>   - [[完整笔记/Peixuan分科笔记/心内]]（晕厥鉴别完整框架）
>   - [[完整笔记/Peixuan分科笔记/neuro]]（颞叶癫痫 + aura 定位 + 抗癫痫药）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/neuro]]（与癫痫鉴别 — 本题方法论核心补充）
>   - [[完整笔记/Peixuan分科笔记/psych]]（Conversion disorder 鉴别）
> - 🌱 TODO（待生成衍生）：
>   - 累计 3+ 道"No further testing"题（vasovagal / 典型 GERD / 偏头痛 / 病毒感染）→ 生成 [[完整笔记/专题笔记/_衍生_USMLE_NoTest题型]]
>   - 累计 3+ 道"过度评估倾向"陷阱题 → 升级 [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别]] 添加新 Part
>   - 累计 3+ 道反射性晕厥题（vasovagal / situational / carotid sinus）→ 补 _衍生_晕厥鉴别决策树 Part 3
>   - 累计 3+ 道癫痫题（focal / generalized / status / aura 定位）→ 生成 [[完整笔记/专题笔记/_衍生_癫痫aura脑叶定位]]
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q21579，目标 < 60 秒选 E
> - [ ] 默写 **Vasovagal 5 联指纹**
> - [ ] 默写 **Vasovagal 双相反射机制**（4 相时序）
> - [ ] 默写 **晕厥 6 大类完整分类系统**
> - [ ] 默写 **反射性晕厥 3 子型对比**（Vasovagal / Situational / Carotid sinus）
> - [ ] 默写 **Situational 8 种触发场景**
> - [ ] 默写 **晕厥 7 维分类框架**（"触前心醒，背伴 ECG"）
> - [ ] 默写 **晕厥 5 大类完整决策表**
> - [ ] 默写 **晕厥红旗 10 条**（"运动卧 5 心家电杂老伤"）
> - [ ] 默写 **Tilt-table 4 大适应症 + 5 个不需要场景**
> - [ ] 默写 **"No further testing" 答题三步**
> - [ ] 默写 **Seizure 5 期时序**（prodrome → aura → ictal → postictal → recovery）
> - [ ] 默写 **晕厥 prodrome vs seizure aura 核心区别**
> - [ ] 默写 **Seizure 内部 prodrome vs aura 区别表**
> - [ ] 默写 **Vasovagal vs Seizure 完整鉴别表 12 行**
> - [ ] 默写 **金标准**：postictal confusion = seizure 印章 ⭐
> - [ ] 默写 **颞叶癫痫 4 大 aura + automatism + postictal**
> - [ ] 默写 **Seizure aura 各脑叶定位表**（颞 / 枕 / 顶 / 额）
> - [ ] 默写 **Convulsive syncope 与真正 seizure 鉴别**
> - [ ] 找类似题：
>   - ① Situational syncope（排尿 / 咳嗽 / 排便 / 吞咽）
>   - ② Carotid sinus hypersensitivity（老年剃须）
>   - ③ 反复不明晕厥 → tilt-table
>   - ④ POTS（年轻女性）
>   - ⑤ 颞叶癫痫 + déjà vu / 嗅觉 aura + automatism
>   - ⑥ Convulsive syncope（晕厥伴短暂抽搐）
>   - ⑦ 其他 "No further testing"（典型 GERD / 偏头痛 / 自限感染）
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（晕厥）
> - [ ] 给 [[完整笔记/Peixuan分科笔记/neuro]] 加 #薄弱点（癫痫 aura）
> - [ ] **建立"反向应用框架"思维**：分类不只是确诊用，也用来"排除 + 不查"
> - [ ] **修正"过度评估倾向"**：第 2 次掉进，必须警惕（与 Q19889 联动）
> - [ ] **建立"7 维 + 红旗"扫读习惯**：每道晕厥题先用 7 维分类，再核对 10 条红旗
> - [ ] **建立"典型 + 无红旗 → No testing"反射**
> - [ ] **建立"prodrome vs aura"鉴别习惯**：前者全身反射，后者局灶发作；金标准是 postictal confusion
> 
> ---
> 
> 学科:: 心血管
> 主题:: 经典 Vasovagal → No Further Testing + Seizure aura 鉴别 + 颞叶癫痫
> 状态:: 🟡
> 错因:: pattern

## 2026-05-15

> [!example]- [2026-05-15] 心血管 / Type B 主动脉夹层降压**顺序** (复盘 self-test Q07)
> ^STQ20260515-07
> 
> ## Stem 模式
> 
> 58 岁男，撕裂样胸背痛，CT 确诊 Stanford **Type B**，BP 190/110，HR 105 → 问**最先**给哪个降压药？
> 
> ## 核心概念
> 
> 主动脉夹层降压**顺序**：**β-blocker（esmolol/labetalol）先降 HR < 60** → **再加 nitroprusside/NTG 降 SBP < 120**。
> 单纯先给 vasodilator → **reflex tachycardia + ↑dP/dt → 撕裂面扩展**。
> 
> ## 普适规则
> 
> ### 夹层降压 SOP
> 
> | 步骤 | 药物 | 目标 | 原理 |
> |---|---|---|---|
> | Step 1 | **IV β-blocker**（esmolol 首选 / labetalol）⭐ | HR < 60 | 降 dP/dt，减小血流冲击 |
> | Step 2 | + IV nitroprusside / NTG | SBP 100-120 | 进一步降压（HR 已控制后才能加） |
> | 镇痛 | IV morphine / fentanyl | 缓解疼痛 → 间接降 HR/BP | 必加 |
> 
> ### 分型与治疗（联动）
> 
> | 类型 | 累及范围 | 治疗 |
> |---|---|---|
> | **Type A**（Stanford A / DeBakey I/II）| 升主动脉 ± 弓 ± 降 | **立即外科**（替换升主动脉） |
> | **Type B**（Stanford B / DeBakey III）| 只累及左锁骨下远端 | **药物降压为主**（β-blocker + vasodilator）；并发症（破裂/缺血）才手术 / TEVAR |
> 
> ## 易混陷阱（普适）
> 
> - ❌ **单独 NTG / Nitroprusside / Hydralazine** → reflex tachycardia → 撕裂扩展（绝对错）
> - ❌ **Amlodipine / 口服降压**：起效太慢，急性夹层用不上
> - ⚠️ **β-blocker 禁忌**（重度 AS / 急性心衰 / AV block）→ 改用 **非二氢吡啶 CCB（diltiazem/verapamil）IV**
> - ⚠️ Type A 不要纠结药物 → **直接 OR**（药物只是过渡）
> 
> ## 我为什么错
> 
> - 选了：B（IV NTG）+ ?
> - 错因：**知识**（顺序题 — 知道夹层需降压但没记"先 HR 后 BP"原则）
> - 核心陷阱：看到 BP 190/110 第一反应"先扩血管"，忽略 HR 105 才是更重要的撕裂驱动力
> 
> ## Memory Hook
> 
> > **"先关水龙头（β-阻 HR），再开下水道（vasodilator）"**
> > 
> > 夹层 = **撕裂面被 dP/dt 推开** → 降 dP/dt 比降 BP 更优先
> > 
> > 顺序口诀：**"BB → NTG → 镇痛"**（永远 β 先）
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "BP 190 难道不该先降 BP 吗？" | 撕裂动力 = dP/dt（血压变化率），不是绝对压；HR↑会让 dP/dt 飙升 → 必须先压 HR |
> | "Type B 什么时候需要手术？" | 默认药物，**有并发症才手术**：破裂、malperfusion（肾/肠/肢端缺血）、难控疼痛/血压、夹层快速扩展 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本卡是夹层降压顺序首张，等积累
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/心内]] / [[完整笔记/专题笔记/_衍生_主动脉急症决策树]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/外科]]（Type A 立即手术）
> - 🌱 TODO：无（衍生 Part 6.5 已覆盖该顺序，对比检查 ✓）
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q07（验证"先 β 后 vasodilator"反射）
> - [ ] 默写 **夹层降压 3 步 SOP**
> - [ ] 默写 **Type A vs B 治疗分流**
> - [ ] 找 3 道 UW 夹层 / AAA 急诊题
> 
> ---
> 
> 学科:: 心血管
> 主题:: 主动脉夹层降压顺序（β-blocker 先于 vasodilator）
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-15] 神经 / 癫痫 vs 晕厥鉴别 — 舌咬部位陷阱 (复盘 self-test Q32)
> ^STQ20260515-32
> 
> ## Stem 模式
> 
> 28 岁男目击 LOC 后，问哪个特征**最可靠**区分 generalized tonic-clonic seizure vs vasovagal syncope？选项里有 "tongue biting on the tip" 和 "postictal confusion > 10 min"。
> 
> ## 核心概念
> 
> **舌侧缘（lateral）咬伤 = seizure 特异**；**舌尖（tip）咬伤 = syncope 也可见**。
> 选项写 "on the tip" 是**干扰项陷阱** — 真正最可靠区分点是 **prolonged postictal confusion（5-30+ min）**。
> 
> ## 普适规则
> 
> ### Seizure vs Syncope 鉴别铁律
> 
> | 特征 | Seizure | Syncope | 谁更特异？ |
> |---|---|---|---|
> | **舌咬部位** ⭐ | **侧缘（lateral）** | 偶尔**舌尖（tip）** | **侧缘 → seizure**（题干 "tip" 是陷阱） |
> | **Postictal confusion** ⭐⭐⭐ | **5-30+ min**（金标准）| < 1 min 完全清醒 | **延迟清醒 = seizure 印章** |
> | Aura | 局灶性（嗅 / 视 / déjà vu）| 全身性 prodrome（眼黑/出汗/恶心）| 局灶 → seizure |
> | Jerking | 持续节律性 1-2 min | 可有短暂 myoclonic（convulsive syncope）| 短暂抽搐 ≠ seizure |
> | Incontinence | 可有 | 也可有 | 不可靠 |
> | LOC 持续 | > 1 min | < 30 秒 | 时长 alone 不够 |
> | 触发 | 闪光 / 睡眠剥夺 / 戒酒 / 漏药 | 站立 / 疼痛 / 见血 / 排尿 | 看触发 |
> 
> ### "最可靠区分点"排序（USMLE）
> 1. ⭐⭐⭐ **Prolonged postictal confusion** → seizure 金标准
> 2. ⭐⭐ **Lateral tongue biting** → seizure
> 3. ⭐⭐ **局灶 aura**（déjà vu / 嗅幻觉 / automatism）→ seizure
> 4. ⭐ Witnessed prolonged jerking（> 1-2 min 持续抽搐）→ seizure
> 
> ## 易混陷阱（普适）
> 
> - ❌ "Tongue biting" 不分部位 → 错，**必须看部位**（tip = syncope 也行）
> - ❌ "Jerking" alone → 错，**convulsive syncope** 也有短暂 myoclonic jerks（脑灌注不足）
> - ❌ "Incontinence" → 两者都可见，**不可靠**
> - ❌ "LOC > 30 秒" → syncope 也可，不可靠
> - ✅ **Postictal confusion** 是最可靠的"印章"，几乎不会假阳性
> 
> ## 我为什么错
> 
> - 选了：C（tongue biting on the tip）
> - 错因：**干扰项**（被题干 "tip" 字眼吸引，忘了"侧缘 = 特异"细节，把"咬舌"笼统当 seizure）
> - 核心陷阱：USMLE 题干把"tip"明写 → **检验你知不知道 lateral 才是 specific**
> 
> ## Memory Hook
> 
> > **"咬侧不咬尖"** — Seizure 咬**侧缘**（lateral），syncope 偶尔咬**舌尖**（tip）
> > 
> > **最可靠印章 = postictal confusion > 5 min**（晕厥 < 1 min 立刻清醒）
> > 
> > 三件套优先级：**Postictal > Lateral tongue > 局灶 aura**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "Tip 咬舌为什么不算 seizure？" | Syncope 跌倒时舌头碰到牙也可能咬尖；只有**侧缘**是 tonic-clonic 时牙关紧咬咬住的特异部位 |
> | "Convulsive syncope 怎么和 seizure 区分？" | Jerks 短（< 15 秒）+ 无 postictal confusion + 触发是站立/疼痛 → 仍是 syncope |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q19889]] 经典 Vasovagal + Seizure aura 鉴别（2026-05-14 同主题）
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/neuro]] / [[完整笔记/Peixuan分科笔记/心内]] / [[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/Psych]]（PNES 非癫痫性发作鉴别）
> - 🌱 TODO：无（衍生 Part 8.3 已含 lateral 咬伤 + postictal confusion 金标准 ✓）
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q32（验证不被 "tip" 陷阱拐走）
> - [ ] 默写 **Seizure vs Syncope 7 行鉴别表**
> - [ ] 默写 **"最可靠区分点" 4 级优先级**
> - [ ] 反射训练：看到"tongue biting"先查部位（lateral？tip？）
> 
> ---
> 
> 学科:: 神经
> 主题:: Seizure vs Syncope 鉴别（舌咬部位 + postictal confusion）
> 状态:: 🟡
> 错因:: 干扰项

> [!example]- [2026-05-15] 心血管 / Class IB 独特机制 — 缩短 QT (复盘 self-test Q38)
> ^STQ20260515-38
> 
> ## Stem 模式
> 
> 问：Class IB 抗心律失常药（lidocaine, mexiletine）相对其他类，**独特**的电生理效应是哪条？
> 
> ## 核心概念
> 
> **Class IB 独特 = 缩短 APD/QT**（所有其他 Na 通道阻滞剂要么不变要么延长 QT）。机制 → 临床：**LQT3（SCN5A 持续性晚 Na 电流）用 mexiletine** 正是为了把延长的 QT 拉回来。
> 
> ## 普适规则
> 
> ### Vaughan Williams Class I 三亚类核心对比 ⭐
> 
> | 亚类 | 代表药 | Na 通道结合 | APD/QT 影响 | 适应症 |
> |---|---|---|---|---|
> | **IA** | Quinidine, Procainamide, Disopyramide | 中等亲和 | **↑ QT**（也阻 K 通道）| AFib / VT；procainamide 用于 WPW + AFib |
> | **IB** ⭐ | **Lidocaine, Mexiletine** | 快结合快解离 | **↓ QT**（独特！）| **缺血性 VT**（lidocaine）/ **LQT3**（mexiletine） |
> | **IC** | Flecainide, Propafenone, Encainide | 慢结合慢解离 | **↑ QRS**（QT 微变）| **结构正常心脏**的 AFib（pill-in-pocket）；**禁用 post-MI**（CAST trial）|
> 
> ### 各类 ECG 标志
> 
> | 类 | 主要 ECG 变化 |
> |---|---|
> | IA | **QT ↑** |
> | IB | **QT ↓** ⭐ 独特 |
> | IC | **QRS ↑**（QT 基本不变）|
> | II（β-blocker）| **PR ↑** + HR ↓ |
> | III（amiodarone, sotalol, dofetilide）| **QT ↑↑** |
> | IV（diltiazem, verapamil）| **PR ↑** + HR ↓ |
> 
> ### IB → 临床 = LQT3 用 mexiletine
> 
> - LQT3 病因 = SCN5A 突变 → **late Na current 持续流入** → APD 延长 → QT 延长
> - Mexiletine 阻断 **late Na current** → 缩短 APD/QT → 救命
> - **β-blocker 在 LQT3 效果差**（不是肾上腺素触发），所以 mexiletine 是关键
> 
> ## 易混陷阱（普适）
> 
> - ❌ "PR prolongation" = II/IV 类（AV 阻断）特征，**不是 IB**
> - ❌ "QRS widening" = IC 类特征
> - ❌ 把 IB 当 III 类（"延长 QT"）→ 完全反了
> - ⚠️ Class III 也有缩短 QT 的例外吗？没有，III 一律 ↑ QT
> 
> ## 我为什么错
> 
> - 选了：D（PR prolongation）+ ?
> - 错因：**知识**（机制层面不熟 — 知道 Q31 临床用 mexiletine 治 LQT3，但没串到"IB → QT 缩短"机制）
> - 核心陷阱：Q31（临床应用）做对了 ≠ Q38（机制）能做对；**机制层面是反向题**，必须独立记忆
> 
> ## Memory Hook
> 
> > **"IB 短 QT，独此一家"**
> > 
> > 类联想：
> > - IA → A 字像 ↑ → **QT ↑**
> > - IB → B 字像 ↓ → **QT ↓** ⭐
> > - IC → C = "QRS Coupled" → **QRS ↑**
> > 
> > 临床闭环：**LQT3 → late Na 漏 → mexiletine 堵 → QT 回正**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "为什么只有 IB 缩短 QT？" | IB 快结合快解离 + 优先结合**激活/失活态** Na 通道 → 在缺血/去极化组织优先作用 → APD↓ |
> | "Lidocaine 为啥不用于 AFib？" | AFib 是房性 + 心房 Na 通道少受 IB 影响；IB 主要管缺血性室性心律失常 |
> | "Class III amiodarone 反例为什么没有？" | 没有；III 类核心机制 = K 阻断 → 一律 ↑ APD/QT |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本卡是 Class IB 机制首张，等积累
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/心内]] / [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/neuro]]（LQT3 syncope/猝死与神经病学交叉）
> - 🌱 TODO：无（衍生 Part 2.3 已覆盖 IB → QT↓ + LQT3 应用 ✓）
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q38（验证机制反射）
> - [ ] 默写 **Class I 三亚类 ECG 标志表**（IA↑QT / IB↓QT / IC↑QRS）
> - [ ] 默写 **5 类抗心律失常药 ECG 标志**
> - [ ] 反射训练：看到 "lidocaine/mexiletine" → 0.5 秒喊 "缩短 QT"
> 
> ---
> 
> 学科:: 心血管
> 主题:: Vaughan-Williams 抗心律失常药分类
> 状态:: 🔴
> 错因:: 知识

> [!example]- [2026-05-15] 内分泌 / Primary vs Secondary AI **独有**鉴别点 (复盘 self-test Q45)
> ^STQ20260515-45
> 
> ## Stem 模式
> 
> 问：哪个特征在**原发性肾上腺皮质功能不全（Addison）有，继发性没有**？选项含"低 cortisol / 低血糖 / 嗜酸 / 高 K + 色素沉着 / 乏力"。
> 
> ## 核心概念
> 
> **Primary 独有 = 高 K + 色素沉着**（aldo↓ + ACTH/α-MSH↑）。
> Secondary（垂体）只 cortisol↓，**aldo 正常**（RAAS 独立于 ACTH），所以**无高 K 无色素沉着**。
> 共同症状（低 cortisol / 低糖 / 嗜酸 / 乏力 / 低 Na）都不能用来鉴别。
> 
> ## 普适规则
> 
> ### Primary vs Secondary AI 鉴别铁律
> 
> | 特征 | Primary（1°，肾上腺烂）| Secondary（2°，垂体烂）| 鉴别价值 |
> |---|---|---|---|
> | **Cortisol** | ↓ | ↓ | 共同（无鉴别）|
> | **ACTH** | **↑↑** | ↓ | 实验室金标准 |
> | **Aldosterone** | **↓** | 正常（RAAS 独立）| 关键差异 |
> | **K⁺** | **↑（高 K）** ⭐ | 正常 | **独有 1°** |
> | **Na⁺** | ↓（双重机制：aldo↓ + ADH↑）| ↓（仅 ADH↑，cortisol 抑制 ADH↓）| 共同（程度不同）|
> | **色素沉着** | **有（掌纹/口腔/瘢痕）** ⭐ | 无 | **独有 1°** |
> | 低血糖 | + | + | 共同 |
> | 嗜酸 ↑ | + | + | 共同 |
> | 乏力 | + | + | 共同 |
> 
> ### 机制闭环
> 
> ```
> Primary (Addison)             Secondary (垂体)
> ───────────────────           ───────────────────
> 肾上腺 → 全废                 垂体 → ACTH↓
>   ├─ Cortisol↓ ←─┐              └─ Cortisol↓
>   └─ Aldo↓        │           Aldo 正常（RAAS）
>                   │
> ACTH↑↑（无负反馈） │
>   └─ α-MSH↑ → 色素 ⭐
> 
> Aldo↓ → K↑ + Na↓ ⭐
> ```
> 
> ### 病因速记
> 
> | 类型 | 常见病因 |
> |---|---|
> | **1° Addison**（美国）| **自身免疫性肾上腺炎**（最常，70%）；TB（发展中国家最常）；APS-2；adrenal hemorrhage（Waterhouse-Friderichsen）；转移癌 |
> | **2°**（垂体）| 长期外源 GC 突停 ⭐ 最常；垂体瘤 / Sheehan / 手术放疗 |
> | **3°**（下丘脑）| 慢性外源 GC 抑制 CRH |
> 
> ## 易混陷阱（普适）
> 
> - ❌ "低 cortisol / 低糖 / 嗜酸 / 乏力" → **共同症状，不能鉴别**
> - ❌ 选 fatigue 当鉴别点 → 经典分心选项
> - ⚠️ 2° AI 也有低 Na（cortisol↓ → ADH 反馈解除），但**没有高 K**
> - ⚠️ 长期外源 GC **突然停药** = 急性 2° AI（最常见原因，临床高频）
> 
> ## 我为什么错
> 
> - 选了：E（Fatigue）
> - 错因：**知识**（题问"独有"，但被共同症状选项分心；忘了 aldo↓ 才是 1° 的核心鉴别）
> - 核心陷阱：USMLE 题问"only in primary" → **必须锁定 aldo 驱动的高 K + ACTH 驱动的色素**
> 
> ## Memory Hook
> 
> > **"K 和黑只在 1°"** — High **K**alemia + Hyper**pigmentation** = Primary 独有
> > 
> > 机制闭环：
> > - 1° = **肾上腺全废** → cortisol↓ + **aldo↓**（→ K↑）+ ACTH↑（→ MSH → 色素）
> > - 2° = **只垂体死** → 只 cortisol↓，**aldo 不动**（RAAS 独立）
> > 
> > 共同症状 = 低 cortisol 直接后果（低糖 / 嗜酸 / 乏力 / 低 Na）→ **不能鉴别**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "为什么 2° 没有高 K？" | Aldo 主要受 RAAS（K + Ang II）调控，**不受 ACTH 调控**；ACTH↓ 不影响 aldo |
> | "为什么 1° 有色素沉着？" | ACTH 与 α-MSH 来自同一前体 POMC；ACTH↑↑ → α-MSH 副产物 → 黑素细胞 → 掌纹/口腔黏膜/瘢痕色素沉着 |
> | "2° 的 Na 为什么也低？" | Cortisol 平时**抑制 ADH**；cortisol↓ → ADH 解除抑制 → 水潴留 → 稀释性低 Na |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本卡是 Primary vs Secondary AI 鉴别首张，等积累
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/endocrine]] / [[完整笔记/专题笔记/_衍生_肾上腺皮质功能不全决策树]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/肾脏]]（高 K 急诊鉴别）；[[完整笔记/Peixuan分科笔记/感染]]（TB 致 1° AI）
> - 🌱 TODO：无（衍生 Part 2.1 已含 1° vs 2° 鉴别表 ✓）
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q45（验证"K + 黑 → 1°"反射）
> - [ ] 默写 **1° vs 2° AI 9 行鉴别表**
> - [ ] 默写 **AI 病因速记**（1°/2°/3°）
> - [ ] 反射训练：看到"hyperpigmentation + hyperK" → 0.5 秒喊 Addison
> 
> ---
> 
> 学科:: 内分泌
> 主题:: Primary vs Secondary AI 鉴别（高 K + 色素 = 1° 独有）
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-15] 外科 / 侵入操作安全 — 气管插管 gold std + Basilar fx 禁忌 (复盘 self-test Q48-Q49)
> ^STQ20260515-48-49
> 
> ## Stem 模式
> 
> **Q48**：60 岁男插管后，确认**气管 vs 食管**位置的金标准？
> **Q49**：18 岁高速 MVC 后 raccoon eyes + Battle sign + 鼻 CSF 漏，要减压胃 → 用什么管？
> 
> ## 核心概念
> 
> - **Q48 答案**：**Sustained ETCO2 waveform on capnography = gold standard**（区分气管 vs 食管）；**CXR 只确认深度 depth**，不区分位置
> - **Q49 答案**：Basilar skull fracture → **任何经鼻管禁忌**（NGT / Dobhoff / nasotracheal）→ **必须经口（OGT）**
> 
> ## 普适规则
> 
> ### Q48 — 气管插管位置确认 5 法对比
> 
> | 方法 | 区分气管 vs 食管？ | 确认深度？ | 可靠性 |
> |---|---|---|---|
> | **Sustained ETCO2 waveform（capnography呼气末二氧化碳监测）** ⭐ | **金标准** | × | **5-6 次稳定波 = 确定气管** |
> | Colorimetric CO2 detector | 是（弱版本）| × | 假阴性（心跳停 → 无 CO2 流） |
> | Bilateral breath sounds | 不可靠 | 部分 | 胃声可传播误导 |
> | Chest rise | 不可靠 | × | 主观 |
> | SpO2 > 92% | × | × | 延迟，不能即时确认 |
> | **CXR** | × | **确认深度（tip 2-4 cm above carina）** | 用于排除右主支气管插管 |
> 
> ### Q49 — Basilar skull fracture 三联征 → 经鼻管绝对禁忌
> 
> | 临床体征 | 提示 |
> |---|---|
> | **Raccoon eyes（双眶周淤青）** | 前颅窝骨折 |
> | **Battle sign（耳后淤青）** | 中颅窝骨折 |
> | **CSF rhinorrhea / otorrhea** | 硬膜撕裂 |
> | **Hemotympanum** | 中颅窝 |
> 
> **禁忌管路**：NGT / **Dobhoff**（也是经鼻细管）/ Nasotracheal intubation → 风险**经筛板进入颅内**
> **正确**：**Orogastric tube（OGT）** 经口
> 
> ### 通用"经鼻禁忌"红旗清单
> 
> - Basilar skull fracture
> - 严重颜面骨折 / Le Fort II/III
> - 鼻骨骨折
> - 鼻部肿瘤 / 重度鼻中隔偏曲
> - 食管狭窄 / 静脉曲张（相对禁忌）
> 
> ## 易混陷阱（普适）
> 
> ### Q48
> - ❌ "Bilateral breath sounds" → **不可靠**（食管插管也可传播气声到肺野）
> - ❌ "Chest rise" → 主观
> - ❌ "SpO2 > 92%" → 延迟指标
> - ❌ "CXR" → **是 depth 工具，不是 position 工具**（trap：很多学生选 CXR 觉得"客观"）
> - ✅ Capnography 是真正即时 + 客观的金标准
> 
> ### Q49
> - ❌ "改 Dobhoff" → **Dobhoff 也是经鼻**！同样禁忌
> - ❌ "等 CT 颈椎清" → 颈椎不是这里问题，颅底骨折才是
> - ❌ "PEG 现在做" → 急诊不做 PEG（择期）
> - ✅ **OGT 是唯一对的答案**
> - ⚠️ 同理：basilar fx 病人 **NPA（nasopharyngeal airway）也禁忌**
> 
> ## 我为什么错
> 
> ### Q48
> - 选了：E（CXR 确认 tip 2-4cm above carina）
> - 错因：**知识**（混淆了 position 确认 vs depth 确认；CXR 是 depth 工具）
> - 核心陷阱：CXR 看似"客观"，但**速度慢 + 只看深度，不能 0 秒区分气管/食管**
> 
> ### Q49
> - 选了：D（Dobhoff tube）
> - 错因：**知识**（不知道 Dobhoff = 也是经鼻管）
> - 核心陷阱：Dobhoff 名字像"特殊管"，但**插入路径仍是鼻 → 鼻咽 → 食管**，颅底骨折同样禁忌
> 
> ## Memory Hook
> 
> > **Q48** — **"听诊看胸都不算，CO2 波形才作数；CXR 只看深浅，不看对错"**
> > 
> > 一句口诀：**"位置看 CO2，深度看 X 光"**
> > 
> > **Q49** — **"鼻漏脑水 = 鼻子一律封死"**
> > 
> > 经鼻禁忌三联：**NGT / Dobhoff / Nasotracheal** 全部 OUT；**只剩 OGT**
> > 
> > 三联征口诀：**"熊猫眼 + 耳后青 + 鼻流水 = 颅底骨折"**
> 
> ---
> 
> ## 🤔 我的提问 / 卡点
> 
> | 我问的关键问题 | 学到了什么 |
> |---|---|
> | "Capnography 怎么区分气管 vs 食管？" | 食管无肺通气 → 无 CO2 流 → 几次后波形消失；气管持续呼气 → 5-6 次**稳定方波** = 确认气管 |
> | "为什么 CXR 不是金标准？" | CXR 拍片要 5-15 分钟 + 只能看气管隆突距离（depth），无法 0 秒识别"现在管在食管还是气管" |
> | "Dobhoff 不是用于喂食吗，为啥也禁鼻？" | 路径完全相同（鼻 → 咽 → 食管），细 ≠ 安全；颅底缺损时任何细管都可能误入颅内 |
> | "Basilar fx 临床急诊还能干啥？" | **避免擤鼻 / 经鼻吸引 / 经鼻通气**；评估 CSF leak（glucose+ / halo sign）；预防性抗生素有争议 |
> 
> ## 🔗 关联
> - 🔁 同主题错题：
>   - 本卡是侵入操作安全首张自测，等积累
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/外科]] / [[完整笔记/专题笔记/_衍生_侵入操作安全流程大全]]
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/neuro]]（颅底骨折评估）；[[完整笔记/Peixuan分科笔记/pulmonary]]（插管 + 通气）
> - 🌱 TODO：建议给衍生加补丁 — **明确写"任何经鼻管禁忌，包括 nasotracheal intubation 和 NPA"**（详见对话末尾增量清单）
> 
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q48 + Q49
> - [ ] 默写 **气管插管确认 5 法对比表**（capnography vs CXR vs auscultation）
> - [ ] 默写 **Basilar fx 三联征 + 经鼻禁忌清单**
> - [ ] 反射训练：
>   - 看到"confirm ET tube placement" → 0.5 秒喊 capnography
>   - 看到"raccoon eyes / Battle sign / CSF rhinorrhea" → 0.5 秒喊"经鼻一律 OUT，走 OGT"
> 
> ---
> 
> 学科:: 外科
> 主题:: 侵入操作安全（气管插管金标准 + Basilar fx 经鼻禁忌）
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-15] 心内 / WPW + Preexcited AF — 抗心律失常药选择 (Q3069)
> ^Q3069
>
> ## Stem 模式
> 已知 **WPW** + 急性发作 + **irregularly irregular** + 极快心率（>180）+ 血流动力学**稳定** → **Preexcited AF**
> （对比：WPW + 节律**齐** → AVRT，治疗完全不同）
>
> ## 核心概念
> Preexcited AF 稳定 → **Procainamide（Ia）**
> 机制：阻 Na⁺ 通道 → 直接抑制 accessory pathway（pathway 依赖 Na⁺ 电流，类心肌特性），同时不解除 AV 节点保护
>
> ## 机制图 — 为什么 WPW+AF 禁用 AV blocker
> ```
> 正常 AF（无 WPW）              Preexcited AF（WPW + AF）
> ═══════════════════           ═══════════════════════════
>   心房乱颤 350-600/min            心房乱颤 350-600/min
>        │                              │
>        ▼                        ┌─────┴─────┐
>   AV 节点（减速器）              │           │
>   慢钙离子通道                 AV 节点    Accessory Pathway
>   有不应期                    (慢, 安全)  (快, 类心肌, Na⁺ 通道)
>        │                        │            │
>        ▼                        ▼            ▼
>   心室率 100-160             心室 ~150    心室 200-300 ⚠️
>   （安全）                                可退化为 VFib（致命）
> ```
> **关键推论**：给 AV blocker（ABCD-V）→ 关掉左边"安全通道" → 全部冲动走右边旁路 → VFib
> → 所以 WPW+AF 必须用 **Procainamide**（直接降低旁路本身的传导）
>
> ## 普适规则 — WPW + 心动过速治疗决策树
> ```
> WPW + tachyarrhythmia
>     │
>     ├─ 血流动力学不稳定？
>     │   └─ YES → 同步电复律（任何节律都一样）
>     │
>     └─ 稳定 → 看节律
>         │
>         ├─ 规则齐（窄 QRS）→ AVRT
>         │   └─ Adenosine / 迷走动作 → 失败再电复律
>         │
>         └─ 不齐（宽 QRS, 变形态）→ Preexcited AF
>             └─ Procainamide（首选） / Ibutilide（备选）
>             └─ ⚠️ 禁用：ABCD-V
> ```
>
> ## 普适规则 — WPW 三种心律状态对照
>
> | 状态 | 节律 | Delta 波 | QRS | 治疗（稳定） | 治疗（不稳定） |
> |---|---|---|---|---|---|
> | **窦律 + WPW** | 齐 | Yes | Wide | 无需急性处理 / 长期可**消融** | NA |
> | **AVRT**（orthodromic 最常见） | 齐 | **No**（顺行经 AV 节点） | **窄** | **Adenosine** / 迷走 | 同步电复律 |
> | **Preexcited AF** | **不齐** | 间断有 | **宽** | **Procainamide** ⚠️ | 同步电复律 |
>
> **三状态记忆口诀**：
> - 窦律：有 Delta 波（旁路在"待机"，但还没参与心律失常）
> - AVRT：**Delta 波消失**（冲动顺着 AV 节点下传，旁路只参与逆传形成折返）→ QRS 变窄
> - Preexcited AF：**间断有 Delta 波**（冲动有时走 AV 节点、有时走旁路）→ QRS 宽且形态变化
>
> ## 普适规则 — Vaughan-Williams 抗心律失常分类（高频考点）
>
> | 类 | 机制 | 代表药 | 主要用于 | 特殊点 |
> |---|---|---|---|---|
> | **Ia** | Na⁺ 阻（中度）+ K⁺ 阻 → APD↑ | **Procainamide**, Quinidine, Disopyramide | SVT / VT / **WPW+AF** | QT↑ → torsades；procainamide → 狼疮样综合征 |
> | **Ib** | Na⁺ 阻（弱，偏好缺血/去极化心肌）→ APD↓ | **Lidocaine**, Mexiletine | **室性**心律失常（特别是缺血后 VT）| 对房性/SVT **无效** |
> | **Ic** | Na⁺ 阻（强）→ 传导↓↓，APD 不变 | **Flecainide**, Propafenone | AF（无结构性心脏病）| 有结构性心脏病禁用 |
> | **II** | β 阻 → AV 节点抑制 | Metoprolol, Esmolol | 速率控制 / 缺血保护 | **AV blocker** |
> | **III** | K⁺ 阻 → APD↑↑ | **Amiodarone**, Ibutilide, Sotalol, Dofetilide | AF / VT 广谱 | QT↑；amiodarone 多脏器毒性 |
> | **IV** | 非二氢吡啶 CCB → AV 节点抑制 | Verapamil, Diltiazem | SVT / 速率控制 | **AV blocker** |
> | 其他 | AV 节点阻 | **Adenosine**, **Digoxin** | AVRT/AVNRT（adeno）/ HF 房颤（dig）| **AV blocker** |
>
> **记忆要点**：
> - **"Ia 抑制 pathway，Ib 治室性，Ic 怕结构病"**
> - **Lidocaine ≠ Procainamide**：都是 Na⁺ 阻，但 Ib 偏爱去极化的心室肌，对房性无效
>
> ## 易混陷阱（普适）
>
> | 易混 | 区分关键 |
> |---|---|
> | AVRT vs Preexcited AF | **节律齐不齐**；齐=AVRT, 不齐=AF |
> | Adenosine 治 SVT vs WPW+AF 禁 adenosine | 看是 AVRT（齐）还是 AF（不齐）|
> | Procainamide vs Lidocaine（都阻 Na⁺）| Ia 治 SVT/AF，Ib 只治 VT |
> | Procainamide vs Amiodarone（WPW+AF）| Procainamide 经典首选；amiodarone 有争议（可能阻 AV 节点）|
> | 急性 vs 长期 WPW 管理 | 急性=药物/电；**长期根治=导管消融**（本患者已拒绝）|
>
> ## ⚠️ AV 节点阻滞剂"避雷家族"（WPW+AF 全员禁用）
> **ABCD-V**：**A**denosine / **B**eta-blocker / **C**CB（verapamil, diltiazem）/ **D**igoxin / **V**erapamil
> 机制：关闭 AV 节点这条"安全慢通道" → 房颤冲动全走旁路 → 心室率 250-300 → **退化为 VFib → 猝死**
> Digoxin 额外雷：**缩短旁路不应期** → 让旁路传得更快（双重打击）
>
> ## 我为什么错
> - 看到 "WPW + 心动过速 + 既往 SVT 病史" → 条件反射 = AVRT → 选 adenosine
> - **忽略了 "irregularly irregular" 这个 AF 标志词**
> - **不知道 WPW 也会发生 AF**（约 1/3 WPW 患者出现 preexcited AF）
> - 抗心律失常药 Vaughan-Williams 分类不熟，混淆 Ia / Ib（都是 Na⁺ 阻但适应症完全不同）
>
> ## Memory Hook
> - **"WPW 看节律：齐 adeno，不齐 procain"**
> - **"ABCD-V 全员避雷，留 P 单挑"**（Procainamide）
> - 类比：AV 节点 = 收费站（限速），旁路 = 没限速村路。AV blocker = 关收费站 → 车全涌村路 → 翻车
> - **"Ia 抑 pathway，Ib 治室性"**（解决 Procainamide vs Lidocaine 混淆）
>
> ---
>
> ## 🤔 我的卡点（学习路径）
> - Q：疾病机理懂，但药物机理 / 分类不熟 → **本次重点 = Vaughan-Williams 分类系统化**
> - 学到：
>   - Ia / Ib / Ic 同属 Na⁺ 阻但适应症完全不同（不能笼统记"Na 阻"）
>   - Lidocaine 对 SVT/AF 无效（Ib 选择性作用于室肌）
>   - Digoxin 在 WPW 是"双重雷"（不只是 AV 阻，还缩短旁路不应期）
>   - Amiodarone 在 WPW+AF 中**不是首选**（与笼统印象"广谱"相反）
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q3910]] J&L-N LQTS（首张抗心律失常药 / Vaughan-Williams 卡）
>   - [[mistakes/uworld-mistakes#^STQ20260515-38]] Class IB 独特机制 — 缩短 QT（Vaughan-Williams 三亚类对比）
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/心内]] / [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]]（本次增量更新：Part 8.4 + 新增 8.5 WPW 三状态对照 + Digoxin 双重雷 + 收费站/村路类比）
> - 🏥 跨学科：无
> - 🌱 TODO（待生成衍生）：
>   - ✅ Vaughan-Williams 衍生**已建**（[[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]]）；本次错题增量已并入
>   - 等心内"心律失常"章节复习完，请 Claude Code 整合 [WPW / AVRT / AVNRT / AF / SVT 急性处理 / 不稳定 vs 稳定] 类错题 → 生成 [[完整笔记/专题笔记/_衍生_心律失常急性处理决策树]]
>   - 等积累 AV blocker 相关错题（β / CCB / 地高辛 / 腺苷）→ 整合 → 可考虑生成 [[完整笔记/专题笔记/_衍生_AV节点阻滞剂适应症与禁忌]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q3069
> - [ ] **默写 Vaughan-Williams 7 类**（机制 + 代表药 + 适应症 + 主要副作用）
> - [ ] 默写 "WPW+AF 五大禁药"（ABCD-V）+ 为什么 digoxin 是双重雷
> - [ ] 默写 Ia vs Ib vs Ic 的区别（特别是为何 lidocaine 不能治 SVT）
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（抗心律失常药分类）
> - [ ] 找 3 道类似题：WPW+AVRT、WPW+AF、抗心律失常药副作用题
>
> ---
>
> 学科:: 心血管
> 主题:: Vaughan-Williams 抗心律失常药分类
> 状态:: 🔴
> 错因:: 知识

> [!example]- [2026-05-15] 心内 / 老年晕厥 — 间歇性 AV 阻滞识别 (Q4456)
> ^Q4456
>
> ## Stem 模式
> 老年人 + **无前驱**晕厥 + **反复发作头晕**（间歇性）+ ECG 示 **PR 延长 + QRS 延长**（双系统传导异常）+ LVH 但 **EF 正常** + 无体位性低血压 + QTc 正常 → **间歇性高度 AV 阻滞**（bradyarrhythmia）
>
> ## 核心概念
> Bradyarrhythmia ≠ 当下心率慢 → **bradyarrhythmia = 心率有"间歇性变慢/停搏"的潜在风险**
> ECG 当下"正常" **不能排除**间歇性 AV 阻滞。看**传导间期（PR、QRS）+ 病史（反复晕厥）**，不是看当下数字。
>
> ## 机制图 — 为什么"心率 64"也可以是 bradyarrhythmia
> ```
> 正常传导系统                       本患者的传导系统
> ═══════════════                    ═══════════════════════
>    SA 节点                            SA 节点 ✓ (64/min 正常)
>       │                                  │
>       ▼                                  ▼
>    AV 节点（PR < 200ms）              AV 节点（PR 延长）⚠️
>       │                                  │
>       ▼                                  ▼
>    His 束                             His 束 ⚠️ 纤维化
>       │                                  │
>       ▼                                  ▼
>    左右束支（QRS <120ms）             左右束支（QRS 延长）⚠️
>       │                                  │
>       ▼                                  ▼
>    Purkinje → 心室                    Purkinje → 心室
>
>    稳定 60-100 bpm                  现在：勉强能传 (64 bpm)
>                                     某一刻：传导突然完全失败
>                                     → 心室停搏几秒
>                                     → 晕厥
>                                     → 然后又自己恢复 ✓
>                                     → 下次再 ECG："看起来正常"
> ```
> **关键推论**：PR 延长 + QRS 延长 = **双系统弥漫病变**（AV 节点 + His-Purkinje）→ 提示 bifascicular/trifascicular block → 高风险进展为完全性 AV 阻滞
>
> ## 普适规则 — Cardiac Syncope 5 大病因鉴别（高频考点）
>
> | 病因 | 关键 stem 线索 | ECG 线索 |
> |---|---|---|
> | **Aortic stenosis / HCM** | 运动诱发晕厥 + 收缩期杂音 | LVH（但有杂音）|
> | **VT** | 无前驱 + 心肌病 / 既往 MI | 持续 VT，**EF 降低** |
> | **Sick sinus syndrome** | 前驱**疲劳 / 头晕** | **Sinus pauses** |
> | **Advanced AV block** | 反复**无诱因**晕厥 | **PR 延长 / Bifascicular block / Dropped QRS** |
> | **Torsades de pointes** | 无前驱 + **延长 QT 药物 / 低 K⁺/Mg²⁺** | QTc 延长 |
>
> > [!info] UWorld 原图（5 大病因 × clues 对照）
> > ![[{9F5BB061-E782-4E9F-AA9E-A54C94E7644D}.png]]
>
> ## 普适规则 — Syncope 4 大类鉴别（病史导向）
>
> | 类型 | 前驱 | 诱因 | 恢复 | 排除依据 |
> |---|---|---|---|---|
> | **Vasovagal** | 恶心 / 出汗 / 视物模糊 | 情绪 / 久站 / 疼痛 | 快 | 无前驱症状 |
> | **Orthostatic** | 站起头晕 | 体位变化 | 平躺即缓解 | 卧立 BP 差 < 20 mmHg |
> | **Cardiac** | **无前驱**或短暂心悸 | 任何时候 | 快，可能受伤 | 看 ECG / 超声 |
> | **Seizure** | Aura | — | **慢**（postictal confusion）| 无 postictal |
>
> ## 普适规则 — 传导系统病变常见病因（USMLE 高频）
>
> | 病因 | 机制 | 典型场景 |
> |---|---|---|
> | **特发性纤维化**（Lenègre/Lev 病）| 老化 + HTN 累积损伤 | 老年 + 长期 HTN（本题）|
> | **缺血性**（下壁 MI）| RCA → AV 节点供血 | 急性下壁 MI + 心动过缓 |
> | **药物**：β/CCB/Digoxin/Amiodarone | AV 节点抑制 | 老年人新用药后晕厥 |
> | **Lyme 病** | 莱姆心肌炎 | 年轻 + 旅行 + 红斑 |
> | **风湿热** | 急性期 PR 延长 | 儿童 + 链球菌感染后 |
> | **结节病 / 淀粉样变** | 浸润性心肌病 | 心肌肥厚 + 传导异常 |
> | **主动脉瓣手术**或 TAVR 后 | 主动脉环邻近 His 束 | 术后新发 AV block |
>
> ## 易混陷阱（普适）
>
> | 易混 | 区分关键 |
> |---|---|
> | "心率正常" vs "无心律失常" | **当下正常 ≠ 间歇性发作不存在**；看 PR/QRS 间期 + 反复发作病史 |
> | **LVH = 收缩功能差**❌ | **LVH = 舒张障碍（HFpEF）+ EF 正常或偏高**；除非失代偿期 |
> | Cardiac syncope vs Vasovagal | Cardiac **无前驱**；Vasovagal 有恶心/出汗/视物模糊前驱 |
> | Syncope vs Seizure | Syncope 恢复快无 postictal；Seizure 有 aura + postictal confusion |
> | TdP vs 其他 VT | TdP 需 **QTc 延长** + 多形性；本题 QTc 正常 → 排除 |
> | LVH 病因 | HTN（向心性 + 高电压无杂音）vs HCM（不对称 + 杂音）vs AS（杂音 + 运动晕厥）|
>
> ## 我为什么错
> - 看到 LVH + 高血压 + 老年人晕厥 → 想到"结构性心脏病 → 收缩力下降 → 晕厥"，选了 **C. Decreased contractility**
> - **根本错因 1**：**"心率 64 = 正常"** 的思维定式 → 没把 PR/QRS 延长这两个 ECG 异常和"间歇性 bradyarrhythmia"挂钩
> - **根本错因 2**：**LVH ≠ 收缩功能差**。LVH 主要造成舒张障碍（HFpEF），EF 通常正常甚至偏高。题目给了 EF 55% 就直接排除了 C
> - **根本错因 3**：忽略了 "intermittent" 暗示（反复发作 + 当下 ECG 正常 = 间歇性病变的典型表现）
> - **对传导阻滞的临床情景不熟**：没意识到老年 + 长期 HTN = 传导系统纤维化（Lenègre/Lev 病）的经典背景
>
> ## Memory Hook
> - **"心率正常 ≠ 没有心律失常"** —— 看传导间期 + 反复发作病史
> - **"PR 长 + QRS 长 + 老年晕厥 = pacemaker 候选人"**
> - **"LVH ≠ 收缩↓；LVH = 舒张↓ + EF 正常"**
> - 类比：间歇性 AV 阻滞 = 老化电线接触不良。平时灯亮（心率 64 正常），偶尔闪一下（晕厥）；ECG 拍到的是灯亮的瞬间，但电线本身（PR/QRS 延长）已经告诉你它有问题 → **别只看灯亮不亮，看电线**
>
> ---
>
> ## 🤔 我的卡点（学习路径）
> - Q：对传导阻滞的病因 + 临床情景不熟 → **本次重点 = 间歇性病变的识别陷阱 + 传导系统病因列表**
> - 学到：
>   - bradyarrhythmia 是"潜在风险"概念，不是"当下慢"概念
>   - PR 延长（AV 节点/His 上段）+ QRS 延长（His-Purkinje）= 双系统病变 = 高风险
>   - 老年 + 长期 HTN 的传导异常 = Lenègre/Lev 病（特发性纤维化）的经典背景
>   - LVH 默认 EF 正常（HFpEF），不要等同于 systolic dysfunction
>   - 反复发作 + 当下正常 = 间歇性病变的标志（适用于所有间歇性心律失常题）
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q3069]] WPW + Preexcited AF（同为心律失常急性识别；那题"快"，本题"慢"；共同点：都需根据 ECG 模式分类）
>   - [[mistakes/uworld-mistakes#^Q21579]] 经典 Vasovagal（Syncope 4 大类鉴别母题，本题增 Cardiac 子型详解）
>   - [[mistakes/uworld-mistakes#^Q21638]] Volume-mediated OH（Syncope 4 大类对照）
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/心内]] / [[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]]（本次增量并入 Part 5 Cardiac Syncope）/ [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]]（Part 7.6 扩展传导系统病变 7 大病因）
> - 🏥 跨学科：无
> - 🌱 TODO（待生成衍生）：
>   - ✅ 晕厥鉴别衍生**已建** v2（[[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]]）；本次错题增量已并入
>   - 等积累 3-5 道**缓慢性心律失常**错题（SSS / 一/二/三度 AV block / bifascicular block / 起搏器适应症）→ 整合 → 生成 [[完整笔记/专题笔记/_衍生_缓慢性心律失常与起搏器适应症]]
>   - 等积累 LVH 相关错题（HTN / HCM / AS / 主动脉缩窄 / HFpEF vs HFrEF）→ 整合 → 生成 [[完整笔记/专题笔记/_衍生_LVH病因与功能影响]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q4456
> - [ ] **默写 Cardiac Syncope 5 大病因表**（病因 + stem 线索 + ECG 线索）
> - [ ] **默写 Syncope 4 大类鉴别表**（前驱 / 诱因 / 恢复 / 排除依据）
> - [ ] **默写传导系统病变 7 大病因**（特发性纤维化 / 缺血 / 药物 / Lyme / 风湿热 / 浸润性 / 术后）
> - [ ] 记反射弧：**"老年 + 反复晕厥 + PR 延长 + QRS 延长" → 间歇性 AV block → EP study + pacemaker**
> - [ ] 记反射弧：**"LVH" 出现 → 默认 EF 正常 / HFpEF / 舒张障碍**
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（晕厥鉴别 + 缓慢性心律失常 + 传导阻滞病因）
> - [ ] 找类似题：间歇性 AV 阻滞 / SSS / Stokes-Adams 发作 / 起搏器适应症
>
> ---
>
> 学科:: 心血管
> 主题:: Cardiac Syncope / 间歇性 AV 阻滞 + 传导系统病变
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-15] 儿科 / 新生儿 — IDM 一过性 HCM (Q20421)
> ^Q20421
>
> ## Stem 模式
> **控制不佳的妊娠糖尿病母亲** + 新生儿 + **巨大儿（99th%）+ 肩难产 + 锁骨骨折** + 收缩期喷射性杂音 + 超声示 **室间隔肥厚 + 小 LV 腔** + **SpO₂ 95%（不发绀）** → **IDM-HCM（一过性肥厚型心肌病）**
>
> ## 核心概念
> IDM-HCM 由**胎儿高胰岛素血症**驱动，出生后母体葡萄糖供应中断 → 胰岛素正常化 → **1 岁前自发消退（spontaneous regression）**。
> 急性期支持治疗：**IV fluid + β-blocker**（降低收缩力、增加 LV 充盈、减轻动态 LVOT 梗阻）
> **禁用**：inotropes（加重梗阻）、利尿剂（减少 LV 容量加重梗阻）
>
> ## 机制图 — 为什么 IDM 妈生出心脏肥厚的宝宝
> ```
> 母亲控制不佳的糖尿病
>         │
>         ▼  (葡萄糖自由穿过胎盘；胰岛素不过胎盘)
>    胎儿高血糖
>         │
>         ▼  (胎儿胰岛 β 细胞代偿性增生)
>    胎儿高胰岛素血症 ⚠️ 核心驱动
>         │
>         ├─────────────┬─────────────┬─────────────┐
>         ▼             ▼             ▼             ▼
>    全身合成代谢↑   糖原+脂肪沉积   新生儿低血糖   红细胞生成↑
>    （anabolic）   于室间隔        （母体葡萄糖   （慢性宫内
>         │        ⚠️室间隔对       中断,胰岛素    缺氧→EPO↑）
>    Macrosomia    胰岛素特别敏感   还高）          │
>    肩难产        ↓               ↓              Polycythemia
>    锁骨骨折      室间隔肥厚      Hypoglycemia    高胆红素血症
>    臂丛损伤      + 小 LV 腔
>                  ↓
>                  动态 LVOT 梗阻
>                  ↓
>                  收缩期喷射性杂音
>                  + 呼吸窘迫
> ```
> **出生后**：母体葡萄糖中断 → 胰岛素正常化 → 室间隔逐渐变薄 → **1 岁前自愈**
>
> ## 普适规则 — IDM 并发症全图（"T 字诀"：全部 Transient）
>
> | 系统 | 并发症 | 机制 | 预后 |
> |---|---|---|---|
> | 生长 | **Macrosomia**（>90th%）| 胰岛素 = anabolic | — |
> | 产伤 | 肩难产 / **锁骨骨折** / **Erb palsy**（臂丛 C5-C6） | 巨大儿过产道 | 多数恢复 |
> | 代谢 | **新生儿低血糖**（最常见！最紧急！）| 母体葡萄糖中断，胰岛素仍高 | 一过性 |
> | 代谢 | 低钙、低镁 | 母体糖尿病干扰甲状旁腺 | 一过性 |
> | 血液 | **Polycythemia** + 高胆红素血症 | 慢性宫内缺氧 → EPO↑ | 一过性 |
> | 呼吸 | **RDS**（即使足月）| 高胰岛素延迟肺成熟 / 抑制 surfactant | 一过性 |
> | 心脏 | **Transient HCM** ⭐ | 室间隔糖原+脂肪沉积 | **1 岁前自愈** |
> | **结构畸形**（控制差的孕前糖尿病更高发）| **Caudal regression syndrome**、心脏畸形（VSD/TGA/situs inversus）、NTD | 早期器官形成期高血糖 | **永久** |
>
> **关键区分**：
> - **妊娠糖尿病（GDM）**：影响**晚期** → 大部分一过性问题（HCM、低血糖等）
> - **孕前糖尿病（pregestational）**：影响**早期器官形成** → 真结构畸形（caudal regression 等）
>
> ## 普适规则 — IDM-HCM vs 遗传性 HCM 鉴别（必背）
>
> | 特征 | IDM-HCM | 遗传性 HCM |
> |---|---|---|
> | 病因 | 高胰岛素 | β-myosin heavy chain 基因突变 |
> | 形态 | 室间隔肥厚 + 小 LV 腔 | 不对称室间隔肥厚 ± SAM |
> | LVOT 梗阻 | 动态 | 动态，可有 SAM |
> | 治疗 | 支持（IV fluid + β-blocker），**禁 inotropes / 利尿剂** | β-blocker / CCB / 手术 / ICD |
> | 预后 | **1 岁前自愈** | 终身存在，**SCD 风险** ⚠️ |
> | 家族史 | 无 | 常有 |
>
> ## 普适规则 — 新生儿心脏杂音 / 心脏病速查（针对你的卡点）⭐
>
> ### 1. 是否发绀（SpO₂）= 第一分诊关键
>
> | SpO₂ 正常（>92%）| SpO₂ 低 / 发绀 |
> |---|---|
> | 左→右分流 或 阻塞性 | 右→左分流 或 混合 |
> | VSD, ASD, PDA, **IDM-HCM** ⭐, AS, PS, CoA | TOF, d-TGA, TAPVR, Truncus, Tricuspid atresia, HLHS, Ebstein |
> | 通常**不**导管依赖 | 多数**导管依赖** → 需 **PGE1** |
>
> ### 2. 杂音性质 → 病因定位
>
> | 杂音 | 时相 / 性质 | 位置 | 提示病变 |
> |---|---|---|---|
> | **Systolic ejection murmur**（喷射性）| 收缩期，crescendo-decrescendo | RUSB（AS）/ LUSB（PS）/ 左胸（HCM）| **流出道梗阻**：AS / PS / **HCM / IDM-HCM** ⭐ |
> | **Holosystolic**（全收缩）| 收缩全程，plateau 形 | LLSB（VSD）/ apex（MR）| **分流或反流**：VSD / MR / TR |
> | **Continuous "machinery"**（机器样）| 整个心动周期 | 左锁骨下 | **PDA** |
> | **Diastolic decrescendo** | 舒张期 | LSB | AR / PR |
> | **Diastolic rumble** | 舒张中晚期 | apex | MS（罕见于新生儿）|
> | **Fixed split S2** | — | — | **ASD** |
> | **Single S2** | — | — | TOF / d-TGA / HLHS / truncus |
>
> ### 3. 杂音随动作变化（识别 HCM 的金标准）
>
> | 动作 | 前负荷变化 | HCM 杂音 | AS 杂音 |
> |---|---|---|---|
> | **Valsalva**（屏气用力）| ↓ 静脉回流 → ↓ LV 容量 | **↑↑**（梗阻加重）| ↓ |
> | **下蹲 / 抬腿 / 握拳** | ↑ 静脉回流 → ↑ LV 容量 | ↓ | ↑ |
> | **站立**（突然）| ↓ 静脉回流 | ↑ | ↓ |
>
> **逻辑**：HCM = **动态**梗阻，LV 越小、梗阻越重 → 减少前负荷 = 加重杂音；AS = **固定**梗阻，前负荷↑ = 流过梗阻血流↑ = 杂音响
>
> ### 4. 新生儿先心病快速识别表
>
> | 病变 | SpO₂ | 杂音 | 关键特征 | 治疗 |
> |---|---|---|---|---|
> | **VSD** | 正常 | **Holosystolic LLSB** | 最常见 CHD | 小→自闭 / 大→手术 |
> | **ASD** | 正常 | **Fixed split S2** + RUSB 收缩中期 | 反常栓塞风险 | 多数自闭 |
> | **PDA** | 正常 | **Continuous machinery** 左锁骨下 | 早产儿多见 | **Indomethacin** 关闭 |
> | **AS / 二瓣化** | 正常 | Systolic ejection RUSB → 颈部 | Ejection click | β-blocker / 手术 |
> | **CoA** | 正常 / 上下肢差 | 后背可闻 | **上下肢血压差** + Turner 综合征 | 手术 |
> | **IDM-HCM** ⭐ | 正常 | **Systolic ejection** + IDM 背景 | 室间隔肥厚 + 小 LV | **支持 + β-blocker** → 自愈 |
> | **TOF** | ↓ | Systolic ejection LUSB（PS 杂音）+ single S2 | Tet spells（蹲位缓解）/ Boot-shaped heart | 手术 |
> | **d-TGA** | ↓↓ | **常无杂音** + single S2 | **生后立即发绀** | **PGE1** + 房隔造口 + 手术 |
> | **HLHS** | ↓↓ | Single S2 + 弱搏动 | 全发绀 + 休克样 | **PGE1** + 分期手术 |
> | **TAPVR** | ↓ | Fixed split S2 | "Snowman" 心影 | 手术 |
> | **Truncus** | ↓ | Systolic + 单一 S2 | 常合并 22q11 缺失 | 手术 |
>
> ### 5. PGE1（前列腺素 E1）适应症 = 维持 PDA
>
> **用 PGE1**（导管依赖型，发绀）：HLHS / d-TGA / Critical AS or PS / Severe TOF / Tricuspid atresia / Pulmonary atresia / CoA(critical) — 共同点：**生存依赖 PDA 维持**
> **不用 PGE1**：**IDM-HCM** ⭐ / VSD / ASD / 简单 PDA / TTN / 胎粪吸入
>
> ## 易混陷阱（普适）
>
> | 易混 | 区分关键 |
> |---|---|
> | IDM-HCM vs 遗传性 HCM | IDM = **transient**（1 岁前自愈）；遗传性 = 终身 + SCD 风险 |
> | IDM-HCM vs HLHS（你的选项 A/C/D 思路）| HLHS **必然发绀**（SpO₂<92%）；本题 SpO₂ 95% 直接排除 |
> | HCM 杂音 vs AS 杂音 | **Valsalva**：HCM↑，AS↓；动作试验是鉴别金标准 |
> | Systolic ejection vs Holosystolic | Ejection = **流出道梗阻**（AS/PS/HCM）；Holo = **分流/反流**（VSD/MR/TR）|
> | 妊娠糖尿病 vs 孕前糖尿病 | 妊娠 → **晚期** → 一过性问题；孕前 → **早期器官形成** → 真结构畸形 |
> | IDM-HCM 治疗：用 β-blocker | **禁用 inotropes / 利尿剂**（减容量加重动态梗阻，与 HFrEF 治疗相反！）|
>
> ## 我为什么错
> - **卡点 1：对杂音不熟** → 看到"systolic ejection murmur"没立刻定位到"流出道梗阻"（AS/PS/HCM），更没把它和超声"室间隔肥厚"对应起来 → 没识别出 HCM
> - **卡点 2：IDM 心脏影响没条件反射** → 看到"母亲控制不佳的糖尿病 + 巨大儿 + 锁骨骨折"应该立刻在脑中铺开 IDM 并发症列表，**心脏 = 一过性 HCM** 是其中一项，但没建立这个反射
> - 因此走错路径：把"心脏结构异常 + 新生儿"过度联想成严重 CHD（HLHS / 需要移植 / 需要 PGE1）
> - **根本错因**：
>   - ☑ **不知道这个考点**：IDM-HCM 这个独立疾病实体
>   - ☑ **概念混淆**：把"结构异常 = 严重 = 不可逆"等同
>   - ☑ **模式识别没建立**：IDM 三联征（巨大儿 + 锁骨骨折 + 室间隔肥厚）没形成整体识别
>
> ## Memory Hook
> - **"IDM 三联征：巨大儿 + 锁骨骨折 + 室间隔肥厚 → 全部 transient"**
> - **"IDM 的 T 字诀"**：**T**ransient HCM、**T**ransient hypoglycemia、**T**ransient polycythemia、**T**ransient RDS — 全是 transient
> - **"新生儿 SpO₂ 95% = 不发绀 = 不是导管依赖型 CHD = 不需要 PGE1"**
> - 杂音口诀：**"喷射看梗阻（AS/PS/HCM），全收缩看分流（VSD/MR/TR），机器声看 PDA，分裂固定看 ASD"**
> - HCM Valsalva：**"动态梗阻怕空腔" → Valsalva 减容量 → 腔更小 → 梗阻更重 → 杂音更响**
> - 类比：IDM-HCM = 婴儿吃太胖的心脏。母亲血糖太高 → 胎儿一直"加餐"（高胰岛素）→ 室间隔被"喂胖"。出生后"断奶"（母体糖供应停）→ 几个月就"瘦回来"
>
> ---
>
> ## 🤔 我的卡点（学习路径）
> - Q1：对杂音不熟 → **本次重点 = 杂音 6 大模式 + HCM/AS 鉴别动作试验**
> - Q2：IDM 心脏影响没条件反射 → **本次重点 = IDM 并发症全图（特别是 HCM 部分）**
> - 学到：
>   - 杂音分类先按**时相**（systolic/diastolic/continuous）→ 再按**性质**（ejection/holo/rumble）→ 再按**位置**
>   - HCM vs AS 的金鉴别 = **Valsalva 反应方向相反**
>   - IDM 几乎所有问题都是 **transient**（除非控制差的孕前糖尿病 → 真结构畸形）
>   - "新生儿心脏异常" ≠ 一定严重 / 一定 PGE1 / 一定手术 → 先看 SpO₂ 分诊
>   - 妊娠糖尿病 vs 孕前糖尿病 = 影响时期不同 → 并发症性质不同
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - （首题，等后续儿科 / 新生儿 / IDM / 杂音题积累）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/儿科]]
>   - [[完整笔记/Peixuan分科笔记/newborn care and screening]]
>   - [[完整笔记/专题笔记/_衍生_新生儿先心病系统化总结]]（本次新建，三轴：时间 / 紫绀 / 杂音）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/endocrine]]（母体糖尿病的胎儿影响 / 胰岛素 anabolic 作用）
>   - [[完整笔记/Peixuan分科笔记/OB]]（妊娠糖尿病管理）
>   - [[完整笔记/Peixuan分科笔记/心内]]（HCM vs IDM-HCM / 杂音鉴别）
> - 🌱 TODO（待生成衍生）：
>   - ✅ 新生儿先心病系统化总结**已建**（[[完整笔记/专题笔记/_衍生_新生儿先心病系统化总结]]）；本次错题增量已并入
>   - 等积累 3-5 道 **IDM 相关**错题（HCM / 低血糖 / 多血症 / RDS / 产伤 / caudal regression）→ 整合 → 生成 [[完整笔记/专题笔记/_衍生_IDM糖尿病母亲婴儿并发症全图]]
>   - 等积累 3-5 道 **HCM 谱系**错题（遗传性 HCM / SAM / SCD / 运动员猝死 / β-blocker vs 手术 / Valsalva 动作）→ 整合 → 生成 [[完整笔记/专题笔记/_衍生_HCM谱系（遗传性vsIDM）]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q20421
> - [ ] **默写 IDM 并发症全图**（按系统分类，10+ 条）
> - [ ] **默写 IDM-HCM vs 遗传性 HCM 鉴别表**
> - [ ] **默写 新生儿先心病快速识别表**（11 种病变 × SpO₂ / 杂音 / 治疗）
> - [ ] **默写 杂音 6 大模式**（ejection / holosystolic / continuous / diastolic decrescendo / diastolic rumble / fixed split S2）
> - [ ] **默写 HCM vs AS 的 Valsalva / 下蹲反应**（这是高频考点）
> - [ ] **默写 PGE1 适应症 vs 非适应症**
> - [ ] 给 [[完整笔记/Peixuan分科笔记/儿科]] 加 #薄弱点（新生儿心脏病 + IDM + 杂音）
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（杂音识别 + HCM）
> - [ ] 记反射弧：**"母亲糖尿病 + 巨大儿 + 锁骨骨折" → 立刻把 IDM 所有 transient 并发症过一遍**
> - [ ] 记反射弧：**"新生儿 SpO₂ 正常" → 不是导管依赖型 CHD → 不需要 PGE1**
> - [ ] 记反射弧：**"systolic ejection murmur" → 流出道梗阻（AS / PS / HCM）→ 用 Valsalva 鉴别 HCM**
> - [ ] 找类似题：HLHS（导管依赖 → 对比）、d-TGA、TOF、CoA、其他 IDM 并发症题
>
> ---
>
> 学科:: 儿科
> 主题:: 新生儿先心病 / 杂音 + 时序鉴别
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-15] 儿科 / 心内 — VSD 婴儿期心衰发病机制 (Q16280)
> ^Q16280
>
> ## Stem 模式
> **1 月龄** + **不发绀**（never turned blue, SpO₂ 95%）+ **喂养困难 + 进食时出汗苍白** + 呼吸急促 + 双肺啰音 + 肝大 3 cm + **4/6 holosystolic LLSB 杂音 + thrill** + 宽脉压（90/46）→ **中-大型 VSD 引起左→右分流 → 高输出量心衰**
>
> ## 核心概念
> VSD 心衰 = **容量超载型 high-output failure**（不是泵衰竭，LV 收缩力**正常**）
> 根本血流动力学异常 = **肺血流增加（pulmonary overcirculation）**
> 发病时机依赖 **PVR 下降曲线**：胎儿期高 → 出生后渐降 → **1-2 月降至最低 = 分流峰值 = 症状最重**
>
> ## 机制图 — VSD 自然病程时序（解答"为什么不在出生时发病"）
> ```
> 胎儿期（in utero）
> ─────────────────
>    PVR 高（=SVR）→ 双侧压力相等 → **几乎无分流** → 无症状 ✓
>
> 出生 0-2 周（postnatal transition）
> ─────────────────────────────
>    肺开始呼吸 → PVR 开始↓
>    脐带剪断 → SVR↑
>    PVR 还没降到底（肺血管重塑需 4-8 周）
>    分流较小 → 症状轻（杂音可能已出现）
>
> ** 1-2 月龄 ⭐（本题）**
> ─────────────────────────────
>    PVR 降至接近成人水平
>    SVR/PVR 差最大 → 左→右分流 ↑↑↑ 达峰值
>    ↓
>    肺血流↑↑ → 肺淤血 → 肺静脉回流↑
>    ↓
>    左房 + 左室容量超载（要泵 = 体循环 + 分流量）
>    ↓
>    **高输出量心衰**（LV 收缩力正常但跟不上回流）
>
> 多年后（未治疗）
> ─────────────────
>    持续肺血流↑ → 肺血管**重塑**（平滑肌增生 + 内膜增厚）
>    PVR ↑↑↑ 缓慢上升
>    ↓
>    PVR > SVR → 分流**反转**为右→左
>    ↓
>    **Eisenmenger 综合征** → 发绀 + 杵状指 → 不可逆
> ```
>
> ## ⭐ VSD 心衰的解剖时序（解答"1 个月怎么就右心衰了？"）
>
> **关键澄清**：VSD 婴儿期的肝大 ≠ 严格意义的右心衰，而是**左心容量超载 + 体循环淤血的早期表现**
>
> ### 血流路径决定哪个心腔最重
> ```
> 左室收缩
>    │
>    ├──→ 主动脉（正常路径）
>    │
>    └──→ 经 VSD → 右室（"路过"，舒张期排空到肺动脉）
>                    │
>                    ▼
>                肺血流↑↑
>                    │
>                    ▼
>                肺静脉回流↑ → 左房 → 左室
>                    │
>                    ▼
>                ⚠️ 真正的容量负荷最重处：LA + LV
>                （LV 要泵的总量 = 体循环血量 + 分流量）
> ```
>
> ### 谁先衰？
>
> | 心腔 | 受累程度 | 机制 |
> |---|---|---|
> | **LA + LV** ⭐最重 | 重 | 肺循环回流的血量 = 体循环 + 分流量 → 长期容量过载 |
> | **RV** | 中 | 收缩期被左室"挤入"额外血液，但舒张期就排空了（不像真正的容量滞留）|
> | **RA** | 最轻 | VSD 不涉及房水平 |
>
> **→ VSD 心衰本质 = 左心衰为主**
>
> ### 那 1 个月就摸到 3 cm 肝大怎么解释？
>
> | 机制 | 解释 |
> |---|---|
> | **(a) 婴儿肝脏解剖差异** ⭐ | 婴儿正常肝缘可达**肋下 1-2 cm**（成人不可触及才算正常）；血管床顺应性高 → 轻度静脉压↑即反映为肝大；本题 3 cm = **轻度淤血**，非严重右心衰 |
> | **(b) 体循环淤血早期征象** | 大量分流 → 整个循环系统轻度压力升高 → 敏感的婴儿肝静脉先反映出来 |
> | **(c) 左心衰传导（晚期机制）** | 左心衰 → 肺静脉压↑ → 肺动脉压↑ → 右室后负荷↑ → 体循环淤血 → 肝大；这是后期机制，1 月龄通常还没到这步 |
>
> ### VSD 心衰症状出现的解剖时序（先后顺序）
>
> ```
> 1️⃣ 肺淤血（最先）
>    → 呼吸急促 + retractions + 双肺啰音
>
> 2️⃣ 左心容量超载 + 交感激活
>    → 喂养困难（婴儿版"运动不耐受"）
>    → 出汗 + 苍白（交感激活 + 灌注不足）
>    → 心动过速
>
> 3️⃣ 体循环淤血（婴儿敏感的肝脏先反映）
>    → 肝大（轻度，3 cm 在婴儿属于早期信号）
>    → 体重不增
>
> 4️⃣ 真正的双室泵衰竭（晚期，如未治疗）
>    → 严重肝大 + 腹水 + 颈静脉怒张
> ```
>
> **结论**：本题 1 月龄的肝大 = 第 3 步**早期体循环淤血**，**不是**第 4 步严重右心泵衰竭。
> UWorld 措辞 "signs of right-sided heart failure (eg, hepatomegaly)" 在临床上偏松——更准确应说"**体循环淤血征象**"。
>
> ## 普适规则 — 婴儿心衰 vs 成人心衰对照（识别陷阱）
>
> | 成人心衰 | 婴儿心衰 | 解剖/生理基础 |
> |---|---|---|
> | 爬楼气短 / 运动不耐受 | **Poor feeding**（吃奶 = 婴儿最大体力活动）| 吃奶能量消耗约 = 成人慢走 |
> | 端坐呼吸 | **Diaphoresis with feeds**（喂奶时出汗）| 交感激活 |
> | 夜间阵发性呼吸困难 | 呼吸急促 + retractions（轻度回缩）| 同肺淤血机制 |
> | 下肢水肿 | **肝大 + 体重不增** | 婴儿无重力依赖性水肿 |
> | 颈静脉怒张 | 难评估 → **肝大替代** | 婴儿颈短 |
> | BNP↑ | BNP↑ | 同 |
> | "正常肝缘不可触及" | **正常肝缘可达肋下 1-2 cm** | 婴儿肝解剖位置低 + 软 |
>
> **关键陷阱**：婴儿肝缘 3 cm = **轻度异常**（不是严重右心衰）；正常婴儿可达 1-2 cm
>
> ## 普适规则 — VSD 杂音反直觉规律（高频考点）
>
> | 特征 | 表现 | 机制 |
> |---|---|---|
> | 时相 | **Holosystolic**（全收缩）| 整个收缩期跨 VSD 压差都存在 |
> | 位置 | **LLSB**（左下胸骨缘）| 经典位置 |
> | 性质 | "Blowing"吹风样 | — |
> | 强度 | **小 VSD 杂音越响** ⚠️反直觉 | 小孔 → 高湍流 → 大声 |
> | Thrill | **≥4/6 一定有 thrill** | 4/6 = 触觉震颤 |
> | **大 VSD** | 杂音**反而轻** | 压差小 → 湍流少 |
> | **Eisenmenger 后** | 杂音**消失** | 双侧压力又相等，无压差 = 无杂音 |
>
> ## 普适规则 — 左→右分流 3 大 CHD 鉴别
>
> | 病变 | 杂音 | S2 | 经典特征 | 发病时机 | 治疗 |
> |---|---|---|---|---|---|
> | **VSD** ⭐ | Holosystolic LLSB + thrill | 正常 | 最常见 CHD | **1-2 月**（PVR 谷底） | 小→自闭 / 大→手术 |
> | **ASD** | RUSB ejection + **Fixed split S2** | **固定分裂** | 多无症状到成人 | **儿童期到成年**（更迟）| 多数自闭 / 大→介入 |
> | **PDA** | **Continuous "machinery"** 左锁骨下 | 正常 | 早产儿 / 母亲风疹 | 早产儿出生即可见 | **Indomethacin**（早产）/ 手术 |
>
> **时序记忆**：**VSD 最早（1-2 月）→ PDA 看胎龄 → ASD 最晚**（依赖各自的"压差出现窗口"）
>
> ## 易混陷阱（普适）
>
> | 易混 | 区分关键 |
> |---|---|
> | "肝大 = 右心衰" | 肝大 = **体循环淤血征象**；可由左心衰、容量超载或右心衰任一原因；婴儿肝更敏感 |
> | "心衰 = 收缩力差" | VSD 心衰 = **容量超载 + LV 收缩力正常**（high-output failure）→ 选项 A（contractility ↓）错 |
> | "VSD 增加 LV afterload" | ❌反直觉：VSD 是 LV "**减压阀**"——血液经 VSD 走低阻肺循环，afterload **↓**或正常 → 选项 C 错 |
> | "VSD 右→左分流" | 当下 SpO₂ 95% / never turned blue → ❌排除；右→左是 **Eisenmenger 晚期**才出现 |
> | "先心病出生立刻发病" | **左→右分流 CHD 都"延迟发病"**（依赖 PVR 下降）；发绀型才出生立即发病 |
> | 小 VSD vs 大 VSD 杂音 | **小 VSD 杂音更响**（湍流大）；大 VSD 杂音反轻 |
> | VSD vs IDM-HCM（[[mistakes/uworld-mistakes#^Q20421]]）| VSD = 分流 + 进行性恶化；IDM-HCM = 流出道梗阻 + 一过性自愈；两题共用"婴儿不发绀 + 收缩期杂音"的分诊框架 |
>
> ## 我为什么错 / 卡点
> - **卡点 1：对 VSD 发病时序不清晰** → 不理解为什么"先天性"病偏偏 1 个月才发作
>   - 学到：左→右分流 CHD 都依赖 **PVR 下降曲线**，**胎儿期压力相等无分流**，PVR 降到底（1-2 月）才达分流峰值
> - **卡点 2：误以为 1 个月就严重右心衰** → 不理解婴儿肝大的真实含义
>   - 学到：婴儿肝大 ≠ 严格右心衰；本质是**左心容量超载 + 体循环淤血**；婴儿肝脏解剖上更敏感（正常可达 1-2 cm）
> - **根本错因（如果选错）**：
>   - ☑ 时序生理理解空缺：把 CHD 和"出生立刻发病"等同
>   - ☑ 心衰类型混淆：没区分容量超载心衰 vs 泵衰竭
>   - ☑ 婴儿解剖知识空缺：正常婴儿肝缘 1-2 cm 可触及
>
> ## Memory Hook
> - **"PVR 决定 VSD 的脸色——高时安静，低时心衰，再高就发紫"**（一句话概括 4 阶段）
> - **"VSD 婴儿不在出生时哭，在 1 个月时哭"**（PVR 降的过程）
> - **"婴儿肝缘 1-2 cm 是正常的"**（不要看到肝大就联想严重右心衰）
> - **"婴儿心衰 = 看吃奶"**：poor feeding + diaphoresis with feeds = 婴儿版"运动不耐受"
> - **"小 VSD 大声响，大 VSD 反而轻；Eisenmenger 后杂音消失"**
> - **"VSD 反而帮 LV 减压"**（afterload ↓ 不 ↑，反直觉考点）
> - 类比：VSD = 左右两室之间的"违章小门"
>   - 胎儿期：两边客流量一样 → 没人挤
>   - 出生 1-2 月：右室那边突然变空旷（PVR 降）→ 左室人群拼命往右挤 → 肺这边人满为患 → 肺水肿 + LV 累
>   - 多年后：肺被挤怕了装防爆门（血管重塑）→ 右室压力暴涨 → 反过来从右往左挤 → 全身缺氧（Eisenmenger）
>
> ---
>
> ## 🤔 我的卡点（学习路径）
> - Q1：1 个月就右心衰太快？
>   → 学到：**不是真正的右心衰**，是**左心容量超载 + 体循环淤血**的早期表现；婴儿肝脏解剖敏感（正常可触 1-2 cm，3 cm 属轻度异常）
> - Q2：VSD 心衰发病时序逻辑
>   → 学到：依赖 **PVR 下降曲线**；胎儿期 PVR=SVR 无分流，1-2 月 PVR 最低分流峰值，未治疗多年后 PVR 反弹 → Eisenmenger
> - Q3：VSD 心衰是什么类型？
>   → 学到：**容量超载型 high-output failure**，LV 收缩力**正常**（不是泵衰竭）
> - Q4：左→右分流 CHD 解剖时序
>   → 学到：VSD 最早发病（1-2 月）；PDA 看胎龄；ASD 最晚（成年期才有症状）
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q20421]] IDM-HCM（同为新生儿/婴儿不发绀心脏病；那题流出道梗阻 + 一过性自愈，本题分流 + 进行性恶化；共用"婴儿不发绀 + 收缩期杂音"分诊框架）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/儿科]]
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[完整笔记/Peixuan分科笔记/newborn care and screening]]
>   - [[完整笔记/专题笔记/_衍生_新生儿先心病系统化总结]]（本次增量并入：Part 1.3 VSD 4 阶段时序 + 新增 Part 1.5 婴儿心衰 vs 成人心衰对照 + Part 4.1 VSD 行扩展反直觉规律 + Part 8 陷阱）
> - 🏥 跨学科：无
> - 🌱 TODO（待生成衍生）：
>   - ✅ 新生儿先心病系统化总结**已建** v1.1（[[完整笔记/专题笔记/_衍生_新生儿先心病系统化总结]]）；本次错题增量已并入 v1.2
>   - 等积累 3-5 道**左→右分流 CHD**错题（VSD / ASD / PDA + Eisenmenger）→ 整合 → 生成 [[完整笔记/专题笔记/_衍生_左向右分流CHD时序与Eisenmenger]]（重点：PVR 时序、发病窗口、手术时机、为何"先心病不一定生后发病"）
>   - 等积累 3-5 道**婴儿心衰**错题（VSD / 大 PDA / CoA / 心肌病 / IDM-HCM）→ 整合 → 生成 [[完整笔记/专题笔记/_衍生_婴儿心衰识别（吃奶/出汗/肝大）]]（重点：婴儿心衰 vs 成人心衰对照、婴儿肝大的真实意义、容量超载 vs 泵衰竭）
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q16280
> - [ ] **默写 VSD 自然病程 4 阶段**（in utero / postnatal transition / infancy / late childhood）+ 每阶段 PVR 状态 + 临床
> - [ ] **默写 VSD 心衰症状出现的解剖时序**（肺淤血 → 喂养困难 → 体循环淤血 → 严重双室衰）
> - [ ] **默写婴儿心衰 vs 成人心衰对照表**（特别是"婴儿肝缘 1-2 cm 正常"这一条）
> - [ ] **默写左→右分流 3 大 CHD 鉴别**（VSD / ASD / PDA 杂音 + S2 + 发病时机 + 治疗）
> - [ ] **默写 VSD 杂音反直觉规律**（小 VSD 大声 / 大 VSD 小声 / Eisenmenger 后消失）
> - [ ] 给 [[完整笔记/Peixuan分科笔记/儿科]] 加 #薄弱点（先心病时序 + 婴儿心衰识别）
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（VSD 时序 / Eisenmenger）
> - [ ] 记反射弧：**"1-2 月龄 + 喂养困难 + 出汗 + 不发绀 + LLSB holosystolic + thrill" → 大 VSD + 高输出量心衰**
> - [ ] 记反射弧：**婴儿肝缘 ≤2 cm 正常；> 2 cm 早期淤血；> 4-5 cm 才考虑严重右心衰**
> - [ ] 记反射弧：**任何先天性左→右分流 CHD 发病时机 → 跟 PVR 下降曲线走**（不是"出生立刻发病"）
> - [ ] 找类似题：大 PDA（同左→右分流时序）、ASD（时序更晚）、Eisenmenger（晚期表现）、CoA 婴儿心衰
>
> ---
>
> 学科:: 儿科
> 主题:: 新生儿先心病 / 杂音 + 时序鉴别
> 状态:: 🔴
> 错因:: 知识

> [!example]- [2026-05-15] 心内 / Acute Pericarditis 首选治疗 (Q12374)
> ^Q12374
>
> ## Stem 模式
> Pleuritic 胸痛（吞咽/深呼吸加重）+ 病毒前驱（sore throat + myalgia 数日前）+ Friction rub（LSB, scratchy）+ 弥漫 PR depression → **Acute Viral/Idiopathic Pericarditis**
>
> ## 核心概念
> Viral/Idiopathic pericarditis 一线 = **NSAID + Colchicine 联用**
> - NSAID：抗炎止痛（治当下）
> - Colchicine：抑制中性粒细胞 → 复发率减半（防未来）
>
> ## 普适规则 — 不同病因心包炎用药对照表 ⭐
>
> | 病因 | 首选 | 禁用/避免 | 理由 |
> |---|---|---|---|
> | Viral / Idiopathic | **NSAID + Colchicine** | 一线 steroid（↑复发） | 抗炎+防复发 |
> | **Post-MI <1 周**（peri-infarction）| **Aspirin（高剂量）** | **NSAID / Steroid**（妨碍愈合，↑ rupture）| 心肌脆弱期 |
> | Dressler（post-MI 2-10 周）| NSAID + Colchicine 或 ASA | — | 心肌已愈合 |
> | **Uremic** | **透析**（治本）| NSAID（肾毒性）| 清除尿毒素 |
> | Autoimmune (SLE/RA) | 治原发病 + NSAID ± steroid | — | 控免疫病 |
> | Bacterial (purulent) | **引流 + IV 抗生素** | 单 NSAID | 化脓需引流 |
> | TB | 抗结核 + steroid | — | 防 constrictive |
>
> ## Aspirin 剂量决定作用
> - **81 mg（low-dose）= 抗血小板**（不抗炎，治不了 pericarditis）
> - **650-1000 mg q6-8h（high-dose）= 抗炎**（pericarditis / 川崎 / 风湿热可用）
>
> ## 易混陷阱（普适）
> 1. **抗凝在 pericarditis 中是禁忌**（致心包出血/tamponade）— vs ACS 必用抗凝 → 靠 pleuritic（pericarditis）vs pressure（ACS）鉴别
> 2. **Low-dose ASA ≠ 抗炎**（剂量决定一切，看到 "low-dose aspirin" 治 pericarditis 直接排除）
> 3. **Steroid 一线 = 错**（仅在 NSAID 禁忌/失败、或 TB/autoimmune 才用，单用 steroid ↑ 复发率）
> 4. **Acetaminophen / Opioid ≠ 治疗**（无抗炎作用）
> 5. **Post-MI 早期"反射性"用 NSAID = 大错**（必须切换为 high-dose ASA）
>
> ## 我为什么错
> - 选 D（正确），但用药记忆模糊 — "蒙对"而非"掌握"
> - 根本陷阱：不同病因 pericarditis 用药差异不熟；如换成 post-MI <1 周 / uremic / SLE 场景大概率翻车
>
> ## Memory Hook
> - **NSAID = 灭火器**（灭当下炎症）
> - **Colchicine = 防火门**（防复发）
> - **Steroid = 拆迁队**（用力过猛，留隐患）
> - **Aspirin = 特殊型号灭火器**（剂量足才抗炎）
> - 口诀："**病毒心包炎 → 布洛芬 + 秋水仙**；**心梗 1 周内心包炎 → 只用阿司匹林**（其他 NSAID 让心脏裂）"
>
> ---
>
> ## 🤔 我的提问 / 卡点
> - Q：心包炎首选治疗记不清？→ A：viral/idiopathic 默认 NSAID + colchicine；其他病因按对照表切换
> - Q：不同机制心包炎用药如何区分？→ A：按"病因决定治疗"——viral 抗炎、post-MI 早期单 ASA、uremic 透析、bacterial 引流、TB 抗结核+steroid
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - （首题，等后续 pericarditis / post-MI 并发症 / ACS 鉴别题积累）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[完整笔记/专题笔记/_衍生_高频陷阱]]（剂量决定作用 / 反射性用药陷阱 — 本次新增"low-dose ASA ≠ 抗炎"+"Steroid 一线 ↑ 复发"两条普适陷阱）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/肾脏]]（uremic pericarditis → 透析为首选，非 NSAID）
>   - [[完整笔记/Peixuan分科笔记/感染]]（viral prodrome → coxsackie/adeno/echo/influenza/HIV）
> - 🌱 TODO（待生成衍生）：
>   - 等心内 post-MI 并发症章节复习完 → 请 Claude Code 整合 [pericarditis 不同病因用药 + post-MI 时间轴并发症] → 生成 [[完整笔记/专题笔记/_衍生_心包炎用药对照_按病因]]
>   - 等积累 3+ 道 ACS vs pericarditis 鉴别题 → 生成 [[完整笔记/专题笔记/_衍生_胸痛鉴别速查]]（pleuritic vs pressure、抗凝禁忌区）
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做：换 post-MI <1 周 / uremic / SLE 场景能否切换正确用药
> - [ ] 默写"不同病因心包炎用药对照表"（凭记忆画）
> - [ ] 默写 Aspirin 剂量-作用映射（low vs high）
> - [ ] 找 3 道类似题：post-MI 早期、uremic、bacterial purulent
>
> ---
>
> 学科:: 心血管
> 主题:: 胸痛鉴别 / 各病因（症状 + 治疗）
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-15] 心内 / Costochondritis（胸痛鉴别）(Q4650)
> ^Q4650
>
> ## Stem 模式
> 年轻女性 + Sharp **localized** 胸骨旁痛 + **动作/呼吸加重** + 运动后起病 + **触诊压痛可重现** + 生命体征/ECG/CXR 正常 → **Costochondritis（肋软骨炎）**
>
> ## 核心概念
> Costochondritis = 临床 + 排除性诊断的肌骨胸痛
> - 决定性体征 = **Tenderness to palpation**（按压可重现疼痛）
> - 自限性（数周-1 年）
> - 初始管理 = **Reassurance + NSAID/APAP**（不需检查）
>
> ## 普适规则 — 胸痛鉴别系统对照表 ⭐⭐⭐
>
> | 类别 | 性质 | 加重 | 缓解 | 决定性体征 | 首选 |
> |---|---|---|---|---|---|
> | **Costochondritis** | Sharp, **localized** | Movement / Inspiration | 休息 | **Palpation tenderness** ⭐ | Reassurance + NSAID |
> | **ACS / Angina** | Dull pressure, **radiating** | Exertion | Rest, nitrates | ECG/troponin 异常 | ECG → Troponin → Stress |
> | **Pericarditis** | Sharp, pleuritic | Inspiration, **lying flat** | **前倾** | Friction rub + PR depression | NSAID + Colchicine |
> | **GERD** | **Burning** | **Postprandial, supine, bending** | Antacids | 无压痛 | PPI trial |
> | **PE** | Pleuritic, sudden | Inspiration | — | Tachycardia + hypoxia + ↑ D-dimer | CTA |
> | **Aortic dissection** | **Tearing, radiating to back** | — | — | BP 双臂不等 / 纵隔增宽 | CT angiography |
> | **Esophageal spasm** | **Crushing**, mimics ACS | Cold/hot drinks | **Nitrates（迷惑点！）** | ECG/troponin 正常 | Manometry |
>
> ## 三个 P 鉴别胸痛（核心口诀）⭐
> - **P**alpation 阳性 → **肌骨**（Costochondritis）
> - **P**leuritic + **P**ositional（前倾缓解）→ **心包**（Pericarditis）
> - **P**ostprandial + supine 加重 → **消化**（GERD）
>
> ## 五大加重诱因鉴别表（核心卡点）⭐
>
> | 加重诱因 | 病种 | 机制 |
> |---|---|---|
> | **Movement / Palpation / Inspiration** | **Costochondritis / 肌骨** | 胸壁运动牵拉炎症 |
> | **Inspiration / Lying flat**（前倾**缓解**）| **Pericarditis** | 心包脏壁层摩擦 |
> | **Postprandial / Supine / Bending** | **GERD** | 体位促胃酸反流 |
> | **Exertion / Emotion**（休息缓解）| **Stable angina** | 氧需-氧供失衡 |
> | **Cold / hot drinks** | **Esophageal spasm** | 食管平滑肌痉挛 |
>
> ## 胸痛鉴别决策树（完整版）
>
> ```
> 胸痛
> ├── 生命体征不稳 / 急性发作？
> │   ├── YES → ACS / PE / Dissection / Pneumothorax → 立即 ECG + CXR + Troponin
> │   └── NO → 继续
> │
> ├── Tenderness to palpation？
> │   ├── YES → Costochondritis（最常见！）→ Reassurance + NSAID
> │   └── NO → 继续
> │
> ├── Pleuritic（呼吸加重）？
> │   ├── YES + friction rub / PR depression → Pericarditis
> │   ├── YES + tachycardia / hypoxia → PE
> │   └── NO → 继续
> │
> ├── Exertional + relieved by rest？
> │   ├── YES → Stable angina → Stress test
> │   └── NO → 继续
> │
> ├── Burning + postprandial / supine？
> │   ├── YES → GERD → PPI trial
> │   └── NO → 继续
> │
> └── Crushing + mimics ACS but ECG/troponin normal → Esophageal spasm → Manometry
> ```
>
> ## 易混陷阱（普适）
> 1. **"动作加重" ≠ "GERD"** — GERD 是 postprandial/supine/bending；movement/inspiration 加重是肌骨或心包
> 2. **Tenderness to palpation 是 costochondritis 的指纹** — 看到就锁定，看不到就排除
> 3. **家族 MI 史 ≠ 必须做心源性检查** — 体征+ECG 阴性时，年轻女性 ACS 仍极低
> 4. **Esophageal spasm 是迷惑点**：nitrates 能缓解（因为是平滑肌），但 ECG/troponin 正常
> 5. **能用一根手指指出来 = 体表/肌骨；弥漫/放射 = 内脏**
> 6. **临床诊断 ≠ 需要进一步检查** — 病史+体征足够时，加做检查 = 过度医疗
>
> ## 我为什么错
> - 选 C（Esophageal pH testing）→ 把"sharp, localized, left of sternum"误读为 GERD
> - 根本陷阱：
>   - 没建立胸痛鉴别系统树（不知按"机械/内脏/心源"分层）
>   - **忽略了决定性体征 "tenderness to palpation"** — 这是 costochondritis 金标准
>   - 混淆"加重诱因"—— 把 movement/inspiration 误读为 GERD-like
>   - 可能被父亲 MI 史分散注意力
>
> ## Memory Hook
> - **"一根手指能指出来 + 按一下就疼 + ECG/CXR 正常 → Costochondritis → 安抚就行"**
> - Costochondritis = **挫伤后的瘀青** — 按了痛，自限性
> - 胸痛 5 大鉴别 = **5 把钥匙开 5 把锁** — 每病一个独家"加重诱因"
> - Tenderness to palpation = **costochondritis 的指纹**
>
> ---
>
> ## 🤔 我的提问 / 卡点
> - Q：胸痛鉴别不熟悉？→ A：靠"三个 P"分流 + 决定性体征锁定（palpation tenderness → 肌骨；friction rub → 心包；radiating to back → dissection）
> - Q：为什么不需要进一步检查？→ A：临床诊断已成立 + 危险病因被基础检查排除 → reassurance 即治疗
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q12374]] Acute viral pericarditis（pleuritic + friction rub + PR depression → NSAID + colchicine）— 同 family "胸痛鉴别 / 各病因"
>   - （胸痛鉴别 2/3 道，再积累 1 道触发衍生笔记）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[完整笔记/专题笔记/_衍生_高频陷阱]]（动作加重 ≠ GERD / 家族史诱导反射陷阱）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/消化腺]]（GERD 加重诱因 + PPI trial 流程）
>   - [[完整笔记/Peixuan分科笔记/骨科]]（肌骨胸痛归属）
> - 🌱 TODO（待生成衍生）：
>   - ⭐ **接近触发**：本题 + Q12374 已积累 2 道，再 1 道（ACS / PE / dissection / esophageal spasm 任一）→ 请 Claude Code 整合 → 生成 [[完整笔记/专题笔记/_衍生_胸痛鉴别速查]]（5 大类 + 三个 P + 加重诱因表 + 决策树）
>   - 等 GI 章节复习完 → 整合 GERD 阶梯诊断（empirical PPI → endoscopy → pH testing）→ 生成 [[完整笔记/专题笔记/GERD诊断流程]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做：不看选项说出诊断 + 处理
> - [ ] 默写"胸痛鉴别系统对照表" + "三个 P 鉴别口诀"
> - [ ] 找 3-5 道类似题：GERD / esophageal spasm / stable angina / PE 各 1 道
> - [ ] **关键提醒**：以后胸痛题第一步问"有无 tenderness to palpation" → 直接锁定/排除 costochondritis
>
> ---
>
> 学科:: 心血管
> 主题:: 胸痛鉴别 / 各病因（症状 + 治疗）
> 状态:: 🔴
> 错因:: 知识

## 2026-05-16

> [!example]- [2026-05-16] 心内 / Statin 不耐受处理 (Q17515)
> ^Q17515
>
> ## Stem 模式
> ASCVD 患者（近期 MI + DES）服 high-intensity statin (rosuvastatin) 出现肌痛 → 自行停药 → 问下一步降脂方案
>
> ## 核心概念
> Statin intolerance ≠ statin discontinuation。Mild myalgia 时优先在 statin 类内调整（换药 / 降阶 / rechallenge），而不是放弃 statin 改用其他类。
>
> ## 普适规则：Statin 副作用处理 SOP
> ```
> 出现肌肉症状
>   │
>   ▼
> CK 检测 + 评估严重程度
>   │
>   ├─ Rhabdomyolysis（CK >10× ULN + 肌红蛋白尿）→ 永久停 statin → 改 ezetimibe / PCSK9i
>   │
>   └─ Mild myalgia（90% 患者）
>         ├─ ① 查 TSH（亚临床甲减 ↑ 风险）+ 药物相互作用 + Vit D
>         ├─ ② 短暂停药 2-4 周 → 症状消失 → rechallenge 同药
>         ├─ ③ 换另一种 high-intensity statin（atorva ↔ rosuva）
>         ├─ ④ 降到 moderate-intensity（prava / pitava / fluva — 肌毒最低）
>         ├─ ⑤ 隔日服药（every-other-day dosing）
>         └─ ⑥ 仍不行 → Ezetimibe / PCSK9i 替代
> ```
>
> ## Statin 强度速查表
>
> | 强度 | LDL ↓ | 代表药 | 适应证 |
> |---|---|---|---|
> | High | ≥50% | Atorva 40-80 / Rosuva 20-40 | ASCVD / LDL≥190 / DM 高风险 / 10yr ≥20% |
> | Moderate | 30-49% | Atorva 10-20 / Rosuva 5-10 / **Prava / Pitava / Fluva** | High 不耐受；10yr 7.5-20% |
>
> ## 降脂药定位（普适）
>
> | 药物 | 地位 | 适应证 |
> |---|---|---|
> | Statin | 1st line 永远 | ASCVD / 高 LDL / 高风险 |
> | Ezetimibe | 2nd line add-on | Statin 最大量仍不达标 / 完全不耐受 |
> | PCSK9i | 3rd line add-on | Statin + Ezetimibe 仍不达标 / Very high-risk ASCVD |
> | Fibrate | **不在 ASCVD 链** | **TG ≥500** 防胰腺炎 |
> | Fish oil | 特殊 | TG ≥500 辅助；icosapent ethyl 例外（REDUCE-IT） |
>
> ## 易混陷阱（普适）
> - ❌ Myalgia 立刻弃 statin 改 ezetimibe → 应先换药/降阶
> - ❌ LDL 不达标直接上 PCSK9i → 应先加 ezetimibe
> - ❌ ASCVD 患者用 fibrate 防 MI → fibrate 只防胰腺炎（TG ≥500）
> - ❌ "Lifestyle only" 用于二级预防 → 二级预防必须药物 + lifestyle
> - ❌ Fish oil 防 ASCVD → 证据不一致（除 icosapent ethyl）
>
> ## 我为什么错（个性化）
> - 我选了：E（蒙对）
> - 我的思路：不熟悉降脂药使用原则，凭"感觉 statin 还是要用"蒙
> - 根本错因：☑ 不知道这个考点 ☑ Statin 强度分级不清 ☑ 二线药适应证模糊
> - 核心陷阱：以为"肌肉痛 = 不能用 statin" → 错。Mild myalgia 是可处理的，不是禁忌
>
> ## Memory Hook
> - "**统计 + 依折 + 单抗**"（Statin → +Ezetimibe → +PCSK9i）
> - "**轻痛换药，重溶弃药**"（Myalgia 换 / Rhabdo 弃）
> - "**TG <150 / 150-499 / ≥500**" — 只有 ≥500 才用 fibrate 防胰腺炎
>
> ---
>
> ## 🤔 我的提问 / 卡点
> - Q: 降脂药的治疗升级是什么？→ 学到：Statin → +Ezetimibe → +PCSK9i 的"加药链" vs Myalgia 换药的"换药链"，两条线不混
> - Q: ASCVD risk 记忆方法及临床应用？→ 学到："病高糖险"4 类直接用 statin；"5-7.5-20"三个分水岭；Pooled Cohort 9 变量；Risk Enhancers 8 条
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - （首题，心内降脂药主题，等后续 statin add-on / PCSK9i / TG 管理 / ASCVD risk 计算题积累）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[完整笔记/专题笔记/USMLE降脂药与ASCVD风险管理]]（今日新建，16 Part 完整框架）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/endocrine]]（statin 前查 TSH；DM + ASCVD risk）
>   - [[完整笔记/Peixuan分科笔记/肾脏]]（CKD 是 risk enhancer）
>   - [[完整笔记/Peixuan分科笔记/免疫，疫苗]]（RA / SLE 慢性炎症是 enhancer）
> - 🌱 TODO（待生成衍生）：
>   - 等积累 5+ 道降脂药/Statin 副作用题后 → 生成 [[完整笔记/专题笔记/_衍生_Statin副作用速查]]
>   - 等积累 ASCVD risk 计算题后 → 生成 [[完整笔记/专题笔记/_衍生_ASCVD_RiskEnhancers]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q17515（盲做）
> - [ ] 默写 Statin 强度分级表（high/moderate 代表药 + 剂量）
> - [ ] 默写 Myalgia vs Rhabdo 鉴别 5 点
> - [ ] 默写 "病高糖险"4 类 + "5-7.5-20"三阈值
> - [ ] UWorld 搜 "statin" / "ASCVD primary prevention" 做 5-10 题
>
> ---
>
> 学科:: 心血管
> 主题:: Statin 不耐受 / ASCVD 降脂药选择
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-16] 心内 / 肥厚性心肌病 HCM 临床表现与治疗 (Q2686 + Q22660)
> ^Q2686-Q22660
>
> **Stem 模式**
> - 年轻人 + 运动性晕厥/胸痛/呼吸困难
> - 家族年轻猝死史（"grandfather/father died suddenly at age 40 from heart attack"）
> - 左下胸骨缘 systolic murmur（**不放射颈部**，区分 AS）
> - S4 gallop + prominent LV impulse
> - Echo: 非对称性室间隔肥厚 + 动态 LVOT 梗阻
>
> **核心概念**
> - AD 遗传 sarcomere 突变 → 非对称室间隔肥厚 → **动态 LVOT 梗阻**
> - 反直觉核心：**LV 容量越小，梗阻越重**（与 AS 的固定梗阻完全相反）
> - 所有治疗围绕一条：**增加 LV 血容量**
>
> **普适规则 — 治疗决策树**
> ```
> 无症状 → 定期随访
> 有症状 → β-blocker (metoprolol) 一线
>          ↓ 不耐受 (如哮喘)
>          非二氢吡啶 CCB (verapamil / diltiazem)
> SCD 高危 (晕厥/家族猝死/持续 VT) → 加 ICD
> 房颤 → 控律 + 抗凝
> 难治性 + LVOT 梗阻 → 室间隔消融 / 心肌切除
> 难治性 + 无梗阻 → 心脏移植
> ```
>
> **β-blocker 两个机制（必背）**
> 1. Negative chronotropy → 延长舒张期 → ↑ LV 充盈 → ↑ LV 舒张末容量
> 2. Negative inotropy → ↑ LV 收缩末容量
> 整周期 ↑ LV 容量 → LVOT 梗阻 ↓
>
> **HCM 禁忌药对照表（高频陷阱）**
>
> | 药物 | 机制 | 为何禁 |
> |---|---|---|
> | DHP-CCB (amlodipine) | ↓ 后负荷 | LV 排空更彻底 → 梗阻 ↑ |
> | ACEI / ARB (lisinopril) | ↓ 前+后负荷 | 同上 |
> | 硝酸酯 (isosorbide) | ↓ 前负荷 | LV 装血少 → 梗阻 ↑ |
> | 利尿剂 | ↓ 前负荷 | 同上 |
> | Digoxin | 正性变力 | 收缩更猛 → 梗阻 ↑ |
>
> **共同机制**：所有"减少 LV 容量"的药都加重 HCM 梗阻
>
> **杂音随动作变化（vs AS 鉴别）**
>
> | 操作 | LV 容量 | HCM | AS |
> |---|---|---|---|
> | Valsalva / 站立 | ↓ | 变响 ⬆ | 变弱 ⬇ |
> | 蹲下 / 抬腿 / 握拳 | ↑ | 变弱 ⬇ | 变响 ⬆ |
>
> 一句话锁定：**"杂音随 Valsalva 变响" = HCM**
>
> **易混陷阱（普适）**
> - HCM vs AS：都引起 exertional syncope，但 AS 杂音放射颈部 + Valsalva 变弱 + 老年人为主
> - HCM 哮喘患者 → verapamil（不是 diltiazem，因 diltiazem 有轻度血管扩张）
> - HCM 选 ICD 看 SCD 风险（晕厥史 / 家族猝死 / 持续 VT），不是默认全装
> - Septal ablation / myectomy = 难治 + 有梗阻 才用，不是一线
> - Valve replacement = AS 的治疗，HCM 不需要
>
> **我为什么错（个性化）**
> 这两题都做对了 ✅，记录关键判断点供未来复习：
> - Q2686 一线 → metoprolol（β-blocker 默认一线）
> - Q22660 哮喘患者 → verapamil（β-blocker 相对禁忌时的替代）
> - 关键识别点：看到 "asthma" + HCM → 立刻想到非二氢吡啶 CCB
>
> **Memory Hook**
> - HCM 的心室 = **挤压过紧的水管**
> - 越想让水快流（脱水/扩血管/加快心率），管子被挤得越扁
> - 解决办法：**让水管多装水，把肥厚的壁撑开**
> - HCM 怕"**空、瘪、猛**"：怕心室空（脱水）、怕血管瘪（扩血管药）、怕收缩猛（正性变力药）
>
> ---
>
> 🤔 **我的提问 / 卡点**
> 暂无 — 这两题做对后直接归纳，未深入提问。未来复习时可主动测试：
> - 为什么 β-blocker 改善 LVOT 梗阻？（答：两个负性 → ↑ LV 容量）
> - 哮喘 + HCM 选什么？为什么不选 diltiazem？（答：verapamil；diltiazem 有轻度血管扩张）
> - HCM 杂音 Valsalva 变响 vs AS 变弱，机制？（答：动态 vs 固定梗阻）
>
> 🔗 **关联**
> - 🔁 同主题错题：
>   - （首批 HCM 题，等后续题积累）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[完整笔记/专题笔记/_衍生_新生儿先心病系统化总结]]（Part 3.3 HCM vs AS Valsalva 反向动作试验已涵盖；本卡补成人 HCM 治疗 + 5 禁忌药）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/pulmonary]]（哮喘 → β-blocker 相对禁忌 → 选 verapamil）
> - 🌱 TODO（待生成衍生）：
>   - 等心内章节再积累 2-3 道杂音相关题后，请 Claude Code 整合「HCM / AS / MVP / MR 杂音随 Valsalva-蹲下变化」→ 生成 [[完整笔记/专题笔记/_衍生_杂音动作鉴别表]]
>   - 等收集到 "动态梗阻 vs 固定梗阻" 相关题目（HCM / AS / 主动脉夹层等）→ 生成 [[完整笔记/专题笔记/_衍生_HCM_vs_AS对比]]
>
> ✅ **复盘行动**
> - [ ] 1 周后默写 β-blocker 治疗 HCM 的两个机制
> - [ ] 默写 HCM 禁忌药 5 类 + 共同机制（↓ LV 容量）
> - [ ] 默写 HCM vs AS 杂音随 Valsalva / 蹲下变化表
> - [ ] 找 3 道运动员晕厥鉴别题（HCM / AS / 长 QT / Brugada / ARVC）
>
> ---
>
> 学科:: 心血管
> 主题:: HCM 临床表现与治疗
> 状态:: 🟢
> 错因:: 知识

> [!example]- [2026-05-16] Heme / LMWH 逆转剂局限（自测反向题）(STQ20260516-05)
> ^STQ20260516-05
>
> ## Stem 模式
> 抗凝逆转剂配对反向题（"哪个 INCORRECT"），选项含 LMWH → protamine 完全逆转 anti-Xa
>
> ## 核心概念
> Protamine 对 UFH 是 100% 中和（强碱性 + UFH 强酸性 → 离子结合中和），但对 LMWH **只能逆转 ~60% 的 anti-Xa 活性**。LMWH 分子链短 → 与 protamine 结合位点少 → 反转不完全。
>
> ## 普适规则：抗凝逆转剂速查
>
> | 抗凝药 | 逆转剂 | 完整性 |
> |---|---|---|
> | **Warfarin**（严重出血）| **4-factor PCC + IV vitamin K** | 完全（PCC 即时 + Vit K 维持）|
> | Warfarin（INR 高无出血）| Vitamin K oral / hold dose | — |
> | **UFH** | **Protamine sulfate** | **完全（100%）** |
> | **LMWH**（enoxaparin / dalteparin）| Protamine（**部分**）| **~60% anti-Xa；无完全逆转剂** ⭐ |
> | Fondaparinux | **无逆转剂**（rFVIIa 试验性）| — |
> | **Dabigatran**（II 抑）| **Idarucizumab**（monoclonal Fab）| 完全 |
> | **Apixaban / Rivaroxaban / Edoxaban**（Xa 抑）| **Andexanet alfa** | 完全（昂贵；备 4F-PCC 替代）|
> | Argatroban / Bivalirudin（DTI IV）| **无逆转剂** + 半衰期短（停药即可）| — |
> | tPA / Alteplase（溶栓）| **Cryoprecipitate + TXA**（如出血）| — |
>
> ## 易混陷阱（普适）
> - ❌ LMWH 严重出血 → protamine 完全逆转 → **错**（只逆转 ~60%）
> - ❌ Apixaban 严重出血 → idarucizumab → **错**（那是 dabigatran 的；Xa 抑用 andexanet）
> - ❌ Warfarin 严重颅内出血 → 单独 vitamin K → **错**（必须 PCC，Vit K 单独要 12-24h 才起效）
> - ❌ Fondaparinux 用 protamine → **错**（无效，化学结构不同）
>
> ## 我为什么错（个性化）
> - 我选了：D（apixaban / rivaroxaban → andexanet）— 这是正确配对
> - 漏看反向题词："哪个 **INCORRECT**" → 应选 LMWH-protamine 这条
> - 根本错因：☑ 反向题阅读 ☑ LMWH-protamine 不完全的细节没记牢
> - 核心陷阱：**反向题陷阱** — "INCORRECT/EXCEPT" 题型每周至少错 1 道
>
> ## Memory Hook
> - "**短链短抓**"：LMWH 分子短 → protamine 抓不全 → 只能逆 60%
> - "**Da-bi 找 Ida**" / "**Xa 找 Andex**"（Dabigatran → Idarucizumab；Xa 抑 → Andexanet）
> - "**反向题先圈题干 INCORRECT/NOT/EXCEPT**"（自定 SOP）
>
> ---
>
> ## 🤔 我的提问 / 卡点
> - 暂无（自测错点，未在对话中深入）
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - （首张抗凝逆转剂卡，等后续 warfarin reversal / DOAC reversal 题积累）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/hematology oncology]]
>   - [[完整笔记/专题笔记/急性血栓事件_抗凝抗板专题_v1]]
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/心内]]（机械瓣 / AFib 抗凝选择）
>   - [[完整笔记/Peixuan分科笔记/外科]]（围术期抗凝桥接 + 逆转）
> - 🌱 TODO（待生成衍生）：
>   - 累计 3+ 道反向题（INCORRECT/EXCEPT）→ 生成 [[完整笔记/专题笔记/_衍生_反向题陷阱SOP]]
>   - 累计 3+ 道抗凝逆转题 → 整合到 [[完整笔记/专题笔记/急性血栓事件_抗凝抗板专题_v1]] 增量
>
> ## ✅ 复盘行动
> - [ ] 1 周后默写完整抗凝逆转剂表（9 个药 + 逆转剂 + 完整性）
> - [ ] 自测反向题前先圈出 "INCORRECT/NOT/EXCEPT" — 形成 SOP
> - [ ] UWorld 搜 "anticoagulant reversal" 做 5 题
>
> ---
>
> 学科:: Heme-Onc
> 主题:: 抗凝逆转剂完整性 + 反向题陷阱
> 状态:: 🟡
> 错因:: pattern

> [!example]- [2026-05-16] 心内 / Vaughan Williams 全表 ECG 双向锁死（自测）(STQ20260516-15)
> ^STQ20260516-15
>
> ## Stem 模式
> 配对反向题："哪个 Vaughan Williams class 配 ECG 标志正确"
>
> ## 核心概念
> 抗心律失常药 4 大类的**核心 ECG 标志**必须**双向**记住：见到 ECG 改变能反查 class，给 class 能正答 ECG。Class IB 是**唯一缩短 QT 的**（独家），Class IC 是**最强 QRS 增宽**（最强），IA/III 都延长 QT（双胞胎），II/IV 都延长 PR（双胞胎）。
>
> ## 普适规则：双向锁死表 ⭐⭐⭐
>
> | Class | 代表药 | APD 影响 | **核心 ECG 标志** | 双向锁死 |
> |---|---|---|---|---|
> | **IA** | Quinidine, Procainamide, Disopyramide | **延长** | **QT 延长** + QRS 轻度增宽 | 看到 QT 长 → IA/III 选 |
> | **IB** | **Lidocaine, Mexiletine** | **缩短** | **QT 缩短** ⭐**独家** | 看到 QT 短 → 只能是 IB |
> | **IC** | Flecainide, Propafenone | 不变 | **QRS 显著增宽** ⭐**最强** | 看到 QRS 强增宽 → IC |
> | **II** | β-blocker | — | **PR 延长** + HR↓ | 看到 PR 长 → II/IV 选 |
> | **III** | Amiodarone, Sotalol, Ibutilide, Dofetilide | **延长** | **QT 延长** | 看到 QT 长 → IA/III 选 |
> | **IV** | Verapamil, Diltiazem | — | **PR 延长** + HR↓ | 看到 PR 长 → II/IV 选 |
>
> ## 双向锁死口诀 ⭐（Peixuan 自创，反复打磨）
>
> > [!success] 4 行锁死
> > - **QT 缩短 → IB**（独家！只可能是 IB）
> > - **QRS 显著增宽 → IC**（最强！4 大类里增宽幅度最大）
> > - **QT 延长 → IA 或 III**（双胞胎，看副作用 / 临床场景区分）
> > - **PR 延长 → II 或 IV**（双胞胎，看是否影响哮喘 / HF 区分）
>
> ## 易混陷阱（普适）
> - ❌ IA → QT 缩短 → **错**（IA 延长 QT，Quinidine syncope = TdP 经典）
> - ❌ IB → QRS 增宽 → **错**（IB 不影响 QRS，只缩短 QT）
> - ❌ III → PR 缩短 → **错**（Class III 是 K 阻滞 → QT 延长）
> - ❌ IV → QT 延长 → **错**（Class IV 是 Ca 阻滞 → PR 延长 + HR↓）
> - ❌ Sotalol 是 β-blocker 所以不影响 QT → **错**（K 阻滞主导，QT 延长 + TdP 高风险）
>
> ## 我为什么错（个性化）
> - 我选了：A（IA → QT 缩短）
> - 我的思路：把 IA 和 IB 完全记反了；只记住 IB → QT 缩短，反向题时把"短"错配给了 IA
> - 根本错因：☑ 单向记忆（只记 IB → 短，没双向记 IA → 长）☑ 反向题没有锁死表
> - 核心陷阱：5/15 Class IB 强化追踪 Week 1 Q1 做对了（mexiletine → QT 短），以为记牢了；但**整张 4 大类表没建起来** → 反向题立刻露馅
>
> ## Memory Hook
> - **"独家 / 最强 / 双胞胎"** 三档分组：
>   - **独家**：QT 短 = IB
>   - **最强**：QRS 强增宽 = IC
>   - **双胞胎**：QT 长 = IA / III；PR 长 = II / IV
> - 类比：**4 大类像 4 个家庭** — IB 是独子（独家），IC 是大力士（最强），IA/III 是延长 QT 的姊妹，II/IV 是延长 PR 的姊妹
>
> ---
>
> ## 🤔 我的提问 / 卡点
> - Q: Class IB 强化追踪 Week 1 Q1 做对了，为什么今天还错？
>   → 学到：**单点掌握 ≠ 全表掌握**。Mexiletine 单药 → QT 短 是点；4 大类 ECG 双向锁死是面。强化追踪要扩展到全表。
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q3910]] J&L-N LQTS（首张电生理卡）
>   - [[mistakes/uworld-mistakes#^STQ20260515-38]] Class IB 独特机制 — 缩短 QT
>   - [[mistakes/uworld-mistakes#^STQ20260516-16]] CAST 临床应用反向（同日同根问题）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]]（Part 12.10 双向锁死表已增量）
> - 🏥 跨学科：
>   - [[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]]（LQTS 触发与 Class IB Mexiletine 治疗）
>   - [[完整笔记/Peixuan分科笔记/儿科]]（先天 LQTS → 触发 / 治疗用药选择）
> - 🌱 TODO（待生成衍生）：
>   - 已有 [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] — 本次增量进 Part 12.10
>
> ## ✅ 复盘行动
> - [ ] 1 周后默写"双向锁死 4 行口诀"
> - [ ] 1 周后默写 4 大类 ECG 标志 + 代表药
> - [ ] Class IB 强化追踪 Week 1.5 加做 3 题（覆盖 IA/IB/IC + II/IV 全表）
> - [ ] UWorld 搜 "antiarrhythmic ECG" / "Vaughan Williams" 做 5 题
>
> ---
>
> 学科:: 心血管
> 主题:: Vaughan Williams 4 大类 ECG 双向锁死
> 状态:: 🔴
> 错因:: 知识

> [!example]- [2026-05-16] 心内 / CAST trial 临床应用反向（自测）(STQ20260516-16)
> ^STQ20260516-16
>
> ## Stem 模式
> "哪个患者**最安全**用 flecainide" — 选项里混入 post-MI / EF↓ / HCM / 严重 AS / lone AFib
>
> ## 核心概念
> CAST 试验（1989）：post-MI 患者用 flecainide / encainide 抑制 PVC → **死亡率反而上升 2-3 倍**。机制：缺血 / 瘢痕组织里 IC 药造成**慢传导 + 折返** → 致命性 VT/VF。**铁律**：Class IC **仅用于结构正常的心脏**（lone AFib / pill-in-the-pocket）。
>
> ## 普适规则：Class IC（Flecainide / Propafenone）使用决策
>
> ```
> 患者是否有结构性心脏病 / 心肌缺血史？
>   │
>   ├─ 否（年轻 + 心超正常 + 无 CAD / MI / HF）
>   │     ↓
>   │     ✅ 可用 Flecainide / Propafenone（pill-in-the-pocket AFib 转复）
>   │
>   └─ 是（任一）：
>       - Post-MI（即使 5 年前 — 瘢痕依然在）
>       - CAD / 缺血性心肌病
>       - HFrEF（EF ↓）
>       - HCM
>       - 严重 AS / 主动脉狭窄
>       - 持续性 VT 病史
>       ↓
>       ❌ 绝对禁忌 — CAST 试验：死亡率 ↑ 2-3 倍
>       ↓
>       ✅ 替代：Amiodarone / β-blocker / Sotalol（评估 QT）
> ```
>
> ## "结构性心脏病"扩展定义（USMLE 高频考点）
>
> | 类型 | 例子 | Flecainide 可否 |
> |---|---|---|
> | **缺血** | Prior MI（任何时间）/ CAD / 不稳定型心绞痛 | ❌ 禁 |
> | **HFrEF** | EF < 40% / NYHA II-IV | ❌ 禁 |
> | **肥厚** | HCM / 严重 LVH | ❌ 禁 |
> | **瓣膜** | 严重 AS / 严重 MR | ❌ 禁 |
> | **心肌病** | 扩张 / 限制 / ARVC | ❌ 禁 |
> | **传导异常** | LBBB / 二度 III 度 AVB | ❌ 谨慎（IC 进一步抑传导）|
> | **结构正常** | Lone AFib / SVT 在年轻健康人 | ✅ 可 |
>
> ## 易混陷阱（普适）
> - ❌ "5 年前的 MI 不算结构性病" → **错**（瘢痕永久存在 → 永久禁 IC）
> - ❌ "HCM 心率快用 flecainide" → **错**（HCM 是结构性病，禁 IC；用 β-blocker / 非 DHP CCB）
> - ❌ "Lone AFib 必须 amiodarone" → **错**（年轻健康心脏首选 flecainide / propafenone pill-in-pocket，避免 amiodarone 长期毒性）
> - ❌ 把 CAST 用于 IA / III 类 → **错**（CAST **仅针对 IC**；IA/III 在 SHD 也用，但有 QT 监测）
>
> ## 我为什么错（个性化）
> - 我选了：A（65 岁，5 年前 MI）
> - 我的思路：误以为 "5 年前的 MI 已远期 = 可以用"
> - 根本错因：☑ 知识 — 不知道 CAST 应用没有"时间窗豁免" ☑ pattern — 选项里有"35 岁健康女性 lone AFib"才是正解，但没识别这个 pattern
> - 核心陷阱：**"远期 MI" 干扰项** — USMLE 故意用 5 年 / 10 年的远期 MI 测试是否真的懂 CAST。瘢痕永久 → 永久禁
>
> ## Memory Hook
> - "**CAST 没有时间窗**" — MI 1 天前 vs 10 年前 → 都禁 IC
> - "**心脏有疤就别 C**" — 任何 SHD（缺血 / 肥 / 衰 / 瓣 / 心肌病）都禁 Class IC
> - **类比**：IC 是"强力胶水" — 健康木板上能用（lone AFib），有裂缝的木板（SHD）用了反而裂得更大（折返 VT）
> - **配对**：lone AFib + 健康心 → flecainide ✓；任何 SHD → amiodarone（或 β / sotalol）
>
> ---
>
> ## 🤔 我的提问 / 卡点
> - Q: 5 年前的 MI 为什么也禁？
>   → 学到：瘢痕组织是永久解剖结构，IC 在瘢痕周围造成慢传导 → 折返环不需要"急性缺血"，只需要"传导不均"。这就是 CAST 没有时间窗的根本原因。
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^STQ20260516-15]] Vaughan Williams 双向锁死（同日同根问题）
>   - [[mistakes/uworld-mistakes#^STQ20260515-38]] Class IB 独特机制（Class I 三亚类系列）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]]（Part 2.4 CAST 试验 + Part 14 陷阱表已有，本次扩 Part 12.11 反向应用决策树）
> - 🏥 跨学科：
>   - [[完整笔记/专题笔记/急性血栓事件_抗凝抗板专题_v1]]（post-MI 患者用药选择交叉）
> - 🌱 TODO（待生成衍生）：
>   - 累计 3+ 道"远期 MI 干扰项"题 → 拆出 [[完整笔记/专题笔记/_衍生_远期病史干扰项陷阱]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后默写 "Class IC 禁忌：缺/HFrEF/肥/瓣/心肌病/传导/✅ 结构正常"
> - [ ] 1 周后默写 CAST 试验机制（瘢痕 + 慢传导 + 折返）
> - [ ] Class IB 强化追踪 Week 1.5 Q3 覆盖此点
> - [ ] UWorld 搜 "flecainide" / "antiarrhythmic post-MI" 做 5 题
>
> ---
>
> 学科:: 心血管
> 主题:: CAST 试验临床应用反向 (Class IC 禁忌)
> 状态:: 🔴
> 错因:: 知识

> [!example]- [2026-05-16] 心内 / 酒精性心肌病 AIC (Q2692)
> ^Q2692
>
> **Stem 模式**
> 慢性进展性 dyspnea + 长期大量饮酒 ≥5 yr + HFrEF (EF↓, LV dilated) + 冠脉造影干净 + MCV↑ + AST/ALT>2:1 + 三系轻度受累
>
> **核心概念**
> AIC = 乙醇/乙醛直接毒性 → 收缩力↓ → eccentric hypertrophy → LV cavity dilation。属于**病因可去除的 DCM** → **完全戒酒**是唯一能逆转 LV 功能的治疗，效果远超任何 HFrEF 标准药物。
>
> **普适规则 — 心衰题答题三步法**
> 1. **形态**：echo/CXR → HFrEF(DCM) vs HFpEF(HCM/RCM)
> 2. **病因**：扫 social hx + family hx + labs + 影像 → 有无可去除毒物 / 可治原发病
> 3. **治疗匹配**：
>    - 病因可去除 → **优先病因治疗**（戒酒 / 控速 / 停药 / 血运重建）
>    - 病因不可去除 → 标准 HFrEF（ACEi/ARNI + BB + MRA + SGLT2i + 利尿剂）
>
> **可逆性 DCM 病因对照（必背）**
>
> | 病因 | Stem 线索 | 最佳治疗 | 可逆性 |
> |---|---|---|---|
> | Alcohol | >80g/d × >5yr, AST/ALT>2:1, MCV↑ | 完全戒酒 | 高 |
> | Tachycardia-induced | 长期 AF/SVT, HR>100 | 控速 | 高 |
> | Peripartum (PPCM) | 产前 1m ~ 产后 5m | HFrEF 标准药 + 后续避孕 | 中-高 |
> | Doxorubicin | 累积>400 mg/m² | 停药 + HFrEF | 部分 |
> | Viral myocarditis | 病毒前驱症 + troponin↑ | 支持治疗 | 部分自发 |
> | Ischemic CMP | CAD 危险因素 / 既往 MI | 血运重建 + ACEi/BB | 部分 |
> | Idiopathic/Familial | 家族史 | 标准 HFrEF | 低 |
>
> **慢性酒精三大实验室指纹（一眼锁定）**
> - MCV >100（无 B12/叶酸缺乏的大细胞）
> - AST/ALT >2:1（"AST is higher"）
> - 三系轻度受累（贫血 + 血小板↓ ± WBC↓）
>
> **易混陷阱（普适）**
> - 问 "reverse LV dysfunction" → 选**病因治疗**，不选 HFrEF 标准药
> - 问 "manage HFrEF" → 才选 ACEi/ARNI+BB+MRA+SGLT2i
> - 看到 HFrEF 不要条件反射 ACEi —— 先问"病因能不能拿掉"
> - 长 pack-year 吸烟史是红鲱鱼，冠脉干净就排除 ischemic
> - 酒精性肝炎用激素 ≠ AIC 用激素（AIC 激素**无效**）
>
> **我为什么错**
> 选 C (ACEi)。看到 EF 25% 条件反射 "HFrEF → ACEi"，忽略了：
> ① 长期饮酒史藏在 social hx 一句话里没当回事
> ② 没扫 MCV 和 AST/ALT 比值（3 条酒精指纹全漏）
> ③ 没注意问题措辞 "**reverse** LV dysfunction" → 暗示病因可去除
> **根本错因**：形态诊断做对（DCM），病因诊断漏掉（酒精），所以治疗选错。
>
> **Memory Hook**
> "心肌是被酒泡了 15 年的海绵 —— ACEi 是用力拧，戒酒才是把海绵拿出来晾干。拧得再用力，不拿出来都没用。"
>
> **🤔 我的提问 / 卡点**
> - 卡点：看出来扩心病，没想到病因是酒精
>   → 学到：DCM 题必须**形态 + 病因**双确诊，否则治疗必错
> - 隐性卡点：没扫 CBC/LFT
>   → 学到：USMLE 给完整 labs 不是装饰，**MCV + AST/ALT 比值**是必扫项
>
> **🔗 关联**
> - 🔁 同主题错题：（首题，等心衰病因学错题积累）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[完整笔记/专题笔记/_衍生_实验室指纹诊断大全]]（Part 5.5 慢性酒精性多系统指纹 — 本卡触发新建）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/消化腺]]（AST/ALT>2:1 + MCV↑ 同源指纹）
>   - [[完整笔记/Peixuan分科笔记/hematology oncology]]（酒精性 macrocytosis 鉴别）
> - 🌱 TODO（待生成衍生）：
>   - 心内章节复习完 → 整合 AIC + PPCM + Tachy-induced + Doxo + Ischemic CMP → [[完整笔记/专题笔记/_衍生_DCM病因学与可逆性对照]]
>   - 已建指纹大全 Part 5.5（慢性酒精性多系统指纹）；继续积累 2-3 道酒精多系统题后 → 拆 [[完整笔记/专题笔记/_衍生_慢性酒精中毒实验室指纹]]（MCV/AST-ALT/三系/B1B6 完整版）
>
> **✅ 复盘行动**
> - [ ] 1 周后重做 Q2692（重点：能否一眼锁定 alcohol clue + MCV/LFT）
> - [ ] 默写心衰题三步法 + 可逆性 DCM 对照表
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（心衰病因学）
> - [ ] UWorld 搜 alcoholic / peripartum / tachycardia-induced CMP 各 2 题
> - [ ] 强制习惯：见完整 CBC+LFT 必扫 MCV 和 AST/ALT
>
> ---
>
> 学科:: 心血管
> 主题:: 酒精性心肌病 (AIC) / DCM 病因学
> 状态:: 🟡
> 错因:: pattern

> [!example]- [2026-05-16] 心内 / Malignant Pericardial Effusion (Q20254)
> ^Q20254
>
> ## Stem 模式
> 癌症病史（尤其肺癌）+ 亚急性 dyspnea + CXR **心影大 + 肺野清** + Beck triad（不必全）→ 心包积液 ± 早期 tamponade
>
> ## 核心概念
> CXR 心影大 + 肺野清 = **心包积液**（不是心衰！）
> 首选下一步 = **Echocardiography**（确诊 + 评估量 + 评估 tamponade + 指导穿刺）
>
> ## 普适规则
>
> **心影大 CXR 鉴别表（4 病因）**：
> | 病因 | 肺野 | 啰音 | 起病 | 首选下一步 |
> |---|---|---|---|---|
> | CHF | **淤血/水肿** | 有 | 慢性+急性恶化 | BNP + Echo |
> | Pericardial effusion | **清** | 无 | 亚急性 | **Echo** |
> | Tamponade | **清** | 无 | 急性恶化 | Echo → 穿刺 |
> | Dilated CM | 可清可淤 | ± | 慢性 | Echo |
>
> **Pericardiocentesis 适应症决策树**：
> - Tamponade（血流动力学不稳）→ 急诊穿刺
> - 怀疑恶性/化脓/结核 → 诊断性穿刺（送 cytology/culture）
> - 病因明 + 量小 + 稳定 → 治原发病 + Echo 随访（**不穿**）
>
> **MPE 速查**：
> 最常见原发瘤 = **Lung > Breast > GI > Lymphoma > Melanoma**
> ECG: ↓QRS voltage, **electrical alternans**
> Echo: large effusion ± RA/RV collapse
> 防复发: pericardial window / 长期 catheter
>
> ## 易混陷阱（普适）
> - "心影大"≠ 一定心衰，**必须先看肺野**
> - 心包积液给 **furosemide** = 降 preload → 加重/诱发 tamponade（致死陷阱）
> - 创伤性 tamponade → **穿刺救命**
> - 主动脉夹层 → tamponade → **绝对不穿**（拔塞子致死，直接 OR）⭐
> - CKD (Cr↑) → CT 造影禁忌（即使想做 CTA 排 PE 也不行）
>
> ## 我为什么错
> - 选了 D. Furosemide therapy
> - 思路："心影扩大 → 心衰 → 利尿剂"
> - 根本错因：
>   - 没看清 "lungs are clear bilaterally" + "no edema" 两个关键阴性体征
>   - 被单一影像锚定（anchoring bias），忽略 "lung cancer a year ago" 这个最响的钟
> - 核心陷阱：**心影大 ≠ 心衰，鉴别点在肺野**
>
> ## Memory Hook
> - **"癌症 + 心影大 + 肺野清 = MPE，找 Echo"**
> - 画面：**心脏 = 桃子在塑料袋里**
>   - 心衰 = 桃子肿 + 袋外漏水（肺水肿）
>   - MPE = 桃子正常 + **袋里灌满水**（心包积液）→ 影子大但肺干净
> - **"心包积液给利尿，前负荷掉人难逃"**
>
> ## 🤔 我的提问 / 卡点
> 1. **"Pericardial effusion 不需要 pericardiocentesis 吗?"** → 学到了穿刺适应症决策树（稳不稳 + 啥病因 + 量多大）
> 2. **"创伤性 vs 主动脉夹层心包压塞处理是否相反?"** → 学到了"创伤穿，夹层切"原则；夹层时心包血肿是止血塞子，穿刺致死
> 3. **"Cardiac Tamponade 如何评估?"** → 学到 Beck triad + Pulsus paradoxus + ECG (low voltage + electrical alternans) + Echo (RA/RV collapse + IVC plethora)
> 4. **"Pulsus paradoxus vs Kussmaul 怎么分?"** → 学到 P 看袖带（血压）, K 看脖子（JVP）; P→Tamponade, K→Constrictive
> 5. **"Constrictive 也有 equalization?"** → 学到都有, 但 Constrictive 是"舒张中晚期"均衡 + RV 曲线 Square root sign
> 6. **"为什么 Restrictive LV>>RV?"** → 学到 LV 壁厚 (10-12mm) >> RV 壁厚 (3-5mm), 浸润性病在 LV 影响更大
> 7. **"Restrictive 为什么 BNP 高?"** → 心肌本身被浸润 → 室壁张力↑ → BNP↑↑; Constrictive 心肌正常 → BNP 不高
> 8. **"JVP 波形各段对应什么?"** → 学到 a-c-x-v-y 5 段; 异常模式 (Cannon a/Giant a/Giant v/X 深 Y 消失/M-W 双谷)
> 9. **"RV 曲线和 JVP 一样吗?"** → 不一样但对应; JVP Y 谷 ≈ RV Dip; 都反映同一右心系统
> 10. **"Low voltage ECG 都见于什么?"** → 学到 5C5O 分类 (心内 vs 心外); 经典反差 "壁厚 + low voltage = Amyloid"
>
> ## 🔗 关联
> - 🔁 同主题错题：（首道心包病题，等后续 tamponade/constrictive/pericarditis 题积累）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/心内]]
>   - [[草稿/2026-05-16_心包心肌病谱_主笔记草稿_v2]]（今日生成 ⭐ — 心包病谱 + 限制性 CM + JVP 深度专题 + RV 曲线 + BNP + Low Voltage ECG）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/hematology oncology]]（恶性肿瘤心包转移 / Amyloid）
>   - [[完整笔记/Peixuan分科笔记/肾脏]]（CKD → 造影剂禁忌，排除 A 选项的关键背景）
>   - [[完整笔记/Peixuan分科笔记/外科]]（创伤性 tamponade / 主动脉夹层手术）
> - 🌱 TODO（待生成衍生）：
>   - 等积累 3-5 道心包病题后，请 Claude Code 整合 → [[完整笔记/专题笔记/_衍生_心包疾病谱]]（Pericarditis → Effusion → Tamponade → Constrictive）
>   - 整合"心影大 CXR 鉴别"主题错题 → [[完整笔记/专题笔记/_衍生_心影大鉴别诊断]]
>   - 整合"Tamponade 禁忌操作"（不穿夹层 / 不利尿 / 不溶栓）→ [[完整笔记/专题笔记/_衍生_Tamponade禁忌]]
>   - 整合"Low Voltage ECG 鉴别"（5C5O）→ [[完整笔记/专题笔记/_衍生_LowVoltage鉴别]]
>   - 整合"JVP 波形鉴别"（草稿 v2 第五章已有完整 13 节素材）→ [[完整笔记/专题笔记/_衍生_JVP波形鉴别]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q20254
> - [ ] 默写"心影大 CXR 鉴别表"（4 病因 × 5 鉴别点）
> - [ ] 默写 MPE 三联：**癌症史 + 心影大 + 肺野清 → Echo**
> - [ ] 默写 Pericardiocentesis 适应症决策树（稳/不稳 × 病因）
> - [ ] 默写"创伤穿 vs 夹层切"原则
> - [ ] 默写 Tamponade 禁忌三药（利尿/扩血管/β-阻）
> - [ ] 找 UWorld 心包病题练 5-10 道（pericarditis / effusion / tamponade / constrictive 全谱）
>
> ---
>
> 学科:: 心血管
> 主题:: Malignant Pericardial Effusion / 心影大鉴别
> 状态:: 🟡
> 错因:: pattern

> [!example]- [2026-05-16] 心内 / 主动脉狭窄 AS 体征 (Q4277)
> ^Q4277
>
> **Stem 模式**
> 老年人 + 劳力性晕厥前兆/晕厥 + RUSB 收缩期杂音 + **slow-rising, delayed carotid pulses** (pulsus parvus et tardus) + 无 CAD 史 → **Severe AS**
>
> **核心概念**
> Severe AS = 瓣叶**钙化僵硬** → 关闭无震动 → A2 减弱 + A2 延迟（与 P2 重合）→ **Soft and single S2**。同时左室对压力超负荷反应是**向心性肥厚（壁厚腔小）→ S4**，不是离心性肥厚 → **本期不会有 S3**（S3 要等失代偿期）。
>
> **普适规则 — 心音预测三步法**
> 1. **病变本质**：压力超负荷？容量超负荷？瓣叶钙化？
> 2. **心室适应**：向心性（壁厚腔小）or 离心性（腔大壁薄）？
> 3. **心音映射**：
>    - 压力超负荷 / 向心性肥厚 → **S4**（AS / HTN / HCM）
>    - 容量超负荷 / 离心性肥厚 → **S3**(MR / AR / DCM / HF / 妊娠 / 甲亢)
>    - 瓣叶钙化动不了 → 关闭音**变软**（AS → soft A2）
>    - 瓣叶能动 + 关闭压差大 → 关闭音**增强**（MS 早期 → loud S1；HTN → loud A2；PAH → loud P2）
>
> **Severe AS 体征"四联征"**
> | 体征 | 机制 |
> |---|---|
> | **Soft / single S2** | 钙化瓣震不起来 + A2 延迟与 P2 合并 |
> | **Late-peaking crescendo-decrescendo systolic murmur** (RUSB) | 严重狭窄需更长喷射时间，杂音峰值后移 |
> | **Pulsus parvus et tardus** | 颈动脉脉搏弱而延迟 |
> | **S4** (非 S3) | 向心性肥厚 → 心房推血进僵硬左室 |
>
> **心音 - 疾病速查（必背）**
> | 心音 | 提示疾病 |
> |---|---|
> | Loud S1 | **MS 早期** / 短 PR / 高输出 |
> | Soft S1 | MS 晚期（瓣钙化） / MR / 长 PR |
> | **Soft / single S2** | **Severe AS** ⭐ / 严重 PS |
> | Paradoxical S2 splitting | Severe AS / LBBB / HCM |
> | Wide fixed S2 splitting | **ASD** |
> | **S3** | 容量超负荷：DCM / 严重 MR / AR / HF / 妊娠 / 甲亢 / 儿童正常 |
> | **S4** | 压力超负荷 / 顺应性↓：**AS** / HCM / HTN / 缺血 |
>
> **易混陷阱（普适）**
> - "左室肥厚 ≠ 左室扩大" —— AS 是**壁厚但腔小**，没有 S3 的解剖基础
> - **S3 vs S4 是对偶**：腔大软 → S3；腔小硬 → S4
> - **MS Loud S1 vs AS Soft A2**：关键不是"狭窄"，是**瓣叶能不能动**
> - Severe AS 是 **late-peaking**，不是 early-peaking（后者是轻-中度 AS）
> - AS 不影响 S1；MS 才 Loud S1
>
> **我为什么错**
> 选 B (Audible S3)。错误推理链：
> AS → 左室压力大 → 左室扩大 → S3
> **第 2 步就错**：AS 是**向心性肥厚（壁厚腔不大）**，根本没"扩大"，所以没有 S3 的解剖基础。
> **根本错因**：
> ① 概念混淆：把"压力超负荷→向心肥厚"和"容量超负荷→离心肥厚"搞反
> ② 没建立"病理生理 → 结构 → 心音"三段映射
> ③ 跳步：直接从"AS"推到"S3"，省了中间结构改变这一步
>
> **Memory Hook**
> - **"4 个壁，3 个腔"**：S4 = 壁厚（向心），S3 = 腔大（离心）
> - **"压力 → 壁厚 → S4；容量 → 腔大 → S3"**
> - AS 体征"三软一硬一延迟"：S2 软、A2 软、carotid 软；杂音硬；carotid 延迟
> - 类比：**MS 早期 = 风顶开的门关上很响；AS = 生锈卡住的门关不响**
>
> **🤔 我的提问 / 卡点**
> - 卡点 1：AS 为什么不是 S3？
>   → 学到：S3 = 容量超负荷 + 腔扩大，AS 是压力超负荷 + 向心肥厚（壁厚腔小），机制完全相反
> - 卡点 2：为什么 MS Loud S1 但 AS Soft A2？
>   → 学到：**关键不是"狭窄"，是瓣叶能不能动**。MS 早期瓣叶能动 + 被高房压顶得远 → 关得猛 → Loud；AS 瓣叶钙化僵硬 → 关闭无震动 → Soft
>
> **🔗 关联**
> - 🔁 同主题错题：（首题，等瓣膜病/心音错题积累）
> - 📚 主笔记：[[完整笔记/Peixuan分科笔记/心内]] / [[草稿/2026-05-16_瓣膜病心音机制框架_v1]]（今日新建草稿）
> - 🏥 跨学科：（暂无）
> - 🌱 TODO（待生成衍生）：
>   - 等瓣膜病错题积累 3-5 道 → [[完整笔记/专题笔记/_衍生_瓣膜病心音与杂音速查]]（AS/AR/MS/MR/MVP × S1/S2/S3/S4/杂音/动作鉴别）
>   - 等 S3/S4 类错题积累 → [[完整笔记/专题笔记/_衍生_S3_S4机制与病因鉴别]]（容量 vs 压力超负荷决策树）
>
> **✅ 复盘行动**
> - [ ] 1 周后重做 Q4277（重点：能否一眼锁定 severe AS 三联征 + 预测 S4 不是 S3）
> - [ ] 默写"心音预测三步法"
> - [ ] 默写"压力 vs 容量超负荷 → 向心 vs 离心 → S4 vs S3"映射
> - [ ] 默写"MS Loud S1 vs AS Soft A2"的瓣叶机制
> - [ ] 给 [[完整笔记/Peixuan分科笔记/心内]] 加 #薄弱点（瓣膜病心音）
> - [ ] UWorld 搜 aortic stenosis / S3 gallop / S4 gallop 各 2-3 题
> - [ ] 见瓣膜病题强制问：压力 or 容量？瓣叶能动否？
>
> ---
>
> 学科:: 心血管
> 主题:: AS 体征 / S3 vs S4 机制（压力 vs 容量超负荷）
> 状态:: 🟡
> 错因:: 知识

> [!example]- [2026-05-16] 儿科 / Tetralogy of Fallot (Q2429)
> ^Q2429
>
> ## Stem 模式
> 数月-数岁婴儿 + **喂奶/哭闹时发紫**（Tet spell）+ **Single S2** + LUSB **crescendo-decrescendo** 杂音 + 4 肢 BP 相等 + 中心性紫绀（唇舌）→ TOF
>
> ## 核心概念
> TOF = 最常见的紫绀型先心病（>1 岁），**胚胎漏斗部间隔前上偏移**导致 4 个缺陷
> Tet spell = RVOT 阻塞动态加重 + SVR 下降 → 右→左分流↑ → 紫绀
> 首选下一步：诊断 = Echo；急性 Tet spell = Knee-to-chest + O₂ + Morphine
>
> ## 普适规则
>
> **TOF 4 缺陷（PROVe）**：
> - **P**ulmonary stenosis (RVOT 阻塞) — 杂音来源
> - **R**V Hypertrophy — boot-shaped 心影来源
> - **O**verriding aorta — 骑跨 VSD
> - **V**SD（大型）
>
> **先心病诊断 5 步框架**（最关键）：
> 1. **紫**绀吗？→ 紫绀走 5T+H, 非紫绀走 VAPP/阻塞
> 2. **时**间窗？→ 24-48h / 数周 / 数月 / 成年 各对应不同病
> 3. **S**2？→ Single (5T) / 固定分裂 (ASD) / 响亮 P2 (PH)
> 4. **杂**音？→ 位置 + 形状（Holosystolic / Crescendo-decrescendo / Continuous）
> 5. **压**力差？→ 4 肢 BP, 排除 CoA
>
> **杂音形状鉴别**：
>
> | 形状 | 病 |
> |---|---|
> | Holosystolic (▭▭▭) | VSD / MR / TR |
> | Crescendo-decrescendo (▲▼) | **TOF / AS / PS** |
> | Continuous machine-like | PDA |
> | 收缩+舒张 | Truncus |
>
> **Tet Spell 急性处理 7 步 (KOMI-PB-bicarb)**：
> K**nee-chest → **O**₂ → **M**orphine → **I**V fluids → **P**henylephrine (↑SVR) → **B**eta-blocker (↓RVOT 痉挛) → **bicarb**（纠酸）
> 禁忌：β-agonist（加重痉挛）/ Diuretics（减 preload）
>
> ## 易混陷阱（普适）
> - **紫绀必想 5T+H**，绝不选 VSD/ASD/PDA（左→右不会紫绀，除非 Eisenmenger）⭐
> - **VSD 杂音 = Holosystolic at LLSB；TOF 杂音 = Crescendo-decrescendo at LUSB**（不要混）⭐
> - **TOF 杂音来源是 RVOT 阻塞（PS），不是 VSD**（大 VSD 压差小无杂音）
> - **Single S2 强烈提示 RVOT 阻塞 / 共干**（TOF, Truncus, severe PS, TGA）⭐
> - **固定分裂 S2 → ASD**（USMLE 经典 100% 锁定）
> - TGA / HLHS 在 24-48h 发病, 不可能 3 月才表现
> - Tet spell 诱因：哭闹 / 喂奶 / 排便 / 早晨醒来（Valsalva → SVR↓）
> - Squatting 缓解机制：↑SVR → ↓ 右→左分流
>
> ## 我为什么错
> - 选了 C. Isolated VSD
> - 思路："婴儿 + 心脏杂音 → VSD（最常见先心病）"
> - 根本错因：
>   - **完全忽略了紫绀这个核心特征** — VSD 不会紫绀
>   - 没听 Single S2 这个关键线索
>   - 没听杂音"形状"（c-d ≠ holosystolic）
>   - 没识别 tet spell 模式（喂奶/哭闹时发紫 = TOF 教科书）
> - 核心陷阱：**没立起来"先紫绀分类→后细分"的诊断框架，只是堆症状找最像的**
>
> ## Memory Hook
> - **TOF 4 缺陷**：**PROVe** (PS, RVH, Overriding aorta, VSD)
> - **紫绀型 5T+H**：TOF, TGA, Truncus, Tricuspid atresia, TAPVR, HLHS
> - **非紫绀型 VAPP**：VSD, ASD, PDA + 阻塞 (CoA, AS, PS)
> - **CXR 4 大经典征**：
>   - **Boot-shaped** → TOF ⭐
>   - **Egg-on-string** → TGA
>   - **Snowman** → TAPVR (supra)
>   - **"3" sign** → CoA
> - **杂音口诀**：VSD 全平台 / TOF 菱形 / PDA 机器响 / ASD 固定分裂
> - **诊断 5 步**：**"紫-时-S-杂-压"** ⭐⭐⭐（必背！）
> - **Tet spell 处理**：屈膝吸氧 + 镇静补液 + 缩血管减痉挛 + 纠酸
>
> ---
>
> ## 🤔 我的提问 / 卡点
> 1. **"先心病的诊断框架没见立起来，不知道该怎么想"** ⭐ 核心卡点
>    → 学到了 **5 步法（紫-时-S-杂-压）**，每步砍掉一半选项
>    → 学到了**第 0 层分类**：先紫绀 vs 非紫绀（决定走 5T+H 还是 VAPP）
>    → 学到了**时间窗砍选项**（24-48h vs 数月 vs 成年）
>    → 学到了 **S2 一秒判半题**（固定分裂→ASD; Single→5T 紫绀型）
>    → 学到了**杂音"位置+形状"**比单看位置更精确
>    → 学到了用 4 肢 BP 锁定 CoA
>
> ## 🔗 关联
> - 🔁 同主题错题：（儿科先心病首道，等积累 ASD/VSD/PDA/CoA/TGA 后建立横向链接）
> - 📚 主笔记：
>   - [[完整笔记/Peixuan分科笔记/儿科]]（先心病章节）
>   - [[草稿/2026-05-16_先心病诊断框架_主笔记草稿_v2]]（今日生成 ⭐ 待章节复习后整合）
>   - [[完整笔记/专题笔记/_衍生_新生儿先心病系统化总结]]（已有相关衍生 — 时间×紫绀×杂音三轴）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/心内]]（心脏听诊 — 杂音形状 / S2 异常 / 成人 TOF post-repair 并发症）
> - 🌱 TODO（待生成衍生）：
>   - 等积累 5-8 道先心病题后，整合 → [[完整笔记/专题笔记/_衍生_先天性心脏病完整图谱]]
>   - 整合 "Tet Spell 处理 SOP" → [[完整笔记/专题笔记/_衍生_TetSpell处理]]
>   - 整合 "心脏杂音定位+形状鉴别" → [[完整笔记/专题笔记/_衍生_心脏杂音鉴别]]
>   - 整合 "S2 异常鉴别" → [[完整笔记/专题笔记/_衍生_S2异常鉴别]]
>   - 整合 "儿科 CXR 经典征" → [[完整笔记/专题笔记/_衍生_儿科CXR经典征]]
>
> ## ✅ 复盘行动
> - [ ] 1 周后重做 Q2429
> - [ ] 默写诊断 5 步法（紫-时-S-杂-压）⭐ 最重要
> - [ ] 默写 5T+H 紫绀型 + VAPP 非紫绀型完整列表
> - [ ] 默写 TOF 4 缺陷（PROVe）+ Tet spell 处理 7 步（KOMI-PB-bicarb）
> - [ ] 默写 4 大 CXR 经典征（boot, egg, snowman, 3 sign）
> - [ ] 默写 S2 异常对应病（固定分裂→ASD, Single→5T, 响亮 P2→PH）
> - [ ] 默写杂音形状鉴别（Holosystolic / Crescendo-decrescendo / Continuous）
> - [ ] **用框架强制做 10 道先心病题**，每题写下 5 步答案，不要跳步
> - [ ] 在 [[完整笔记/Peixuan分科笔记/儿科]] 加 #薄弱点 先心病
>
> ---
>
> 学科:: 心血管
> 主题:: TOF / 先心病紫绀分类与 5 步诊断框架
> 状态:: 🟡
> 错因:: pattern

> [!example]- [2026-05-16] 心内/药理 / Digoxin Toxicity (Q4454)
> ^Q4454
> 
> **Stem 模式**：老年 + HFrEF + AFib + 用药列表含 **digoxin** + furosemide + 数日恶心/食欲↓/乏力 + 缓慢 AFib 室率（55/min）+ ECG 无新发缺血 → 问 most helpful diagnostic study
> 
> **核心概念**：怀疑窄治疗窗药物中毒 → 第一步永远是**测血药浓度**（Blood medication level）
> 
> **普适规则 — 窄治疗窗药物中毒 SOP**：
> ```
> 老年/CKD/脱水 + 窄治疗窗药物在用药列表 + 多系统亚急性症状
>         ↓
> 第一步：血药浓度 + 相关电解质 + 肾功
>         ↓
> 不是：心超 / CXR / stress test / LP / TFT
> ```
> 
> | 窄治疗窗药物 | 经典中毒表现 | 第一步 | 解毒 |
> |---|---|---|---|
> | **Digoxin** | GI（恶心/呕吐/食欲↓）+ 神经（confusion/黄绿视/乏力）+ 缓慢心律/AV block | 血 dig level + K⁺ + Cr | DigiFab |
> | Lithium | 震颤、共济失调、意识改变 | 血锂浓度 | 水化/透析 |
> | Warfarin | 出血 | PT/INR | Vit K / FFP / PCC |
> | Theophylline | N/V、震颤、癫痫、心律失常 | 血药浓度 | 活性炭/透析 |
> | Phenytoin | 眼震、共济失调 | 血药浓度（游离） | 支持 |
> | Vancomycin | 肾毒、耳毒 | trough level | 停药/调整 |
> 
> **Digoxin 毒性"DIG-SICK"**：
> - **D**igestive（N/V、食欲↓）
> - **I**rregular bradycardia（缓慢心律 / AV block / 室早）
> - **G**reen/Yellow vision（黄视/绿视）
> - **S**enior（老年）
> - **I**ncreased by diuretics（利尿剂诱发）
> - **C**onfusion（神经症状）
> - **K**⁺ low（低钾放大毒性）
> 
> **易混陷阱（普适）**：
> - 看到 HFrEF 患者新发症状 → 本能想"HF 失代偿 → 查心超"= 错误启发式
> - HF 急性加重 vs 药物毒性鉴别：
>   - HF 加重：戏剧化、单系统（肺水肿/JVD↑/水肿↑）、数小时-1 天
>   - 药物毒性：多系统、非特异、数日-数周亚急性
> - 用药列表 ≠ 背景信息，是**核心嫌疑人清单**
> - 即使 digoxin 浓度正常也不能完全排除中毒（临床表现 + 电解质 + 心律共同判断），但**第一步**仍是查浓度
> 
> **我为什么错**：
> - 选了 E（Echocardiography）
> - 思路：看到 EF 25% + HF + 心律异常 → "心脏问题 → 查心超看 EF"
> - 根本错因：
>   - ☑ 完全忽略用药列表，没把 digoxin 当线索
>   - ☑ 不认识 digoxin toxicity 临床综合征（GI + 神经 + 缓慢心律三联）
>   - ☑ 错误启发式："HF 患者出问题 → HF 失代偿"
> - 核心陷阱：**用药列表必须当核心信息读，不是背景**
> 
> **Memory Hook**：
> - "老奶奶 + furosemide 脱水 → digoxin 堵车出不去 → 全身中毒"
> - 公式：**老年 + Digoxin 在用药列表 + 任何新发症状 → 先查 [dig level + K⁺ + Cr]**
> 
> ---
> 
> **🤔 我的提问 / 卡点（学习路径）**：
> - Q1: "为什么 AFib + HFrEF 这个组合会想到用药？"
>   → 学到：这两个诊断 = 高度标准化的 4-5 类药物"套餐"（β-blocker + ARNI/ACEi + 利尿剂 + 抗凝 ± digoxin），看到组合就该激活"逐药扫描"反射；老年慢病 + 多药 + 新发症状 → 药物副作用先验概率 > 病情加重
> 
> **🔗 关联**：
> - 🔁 同主题错题：（首题，等后续 digoxin / 窄治疗窗药物中毒题积累）
> - 📚 主笔记 + 已有衍生：
>   - [[完整笔记/Peixuan分科笔记/心内]]（AFib + HFrEF 用药管理）
>   - [[草稿/2026-05-16_老年多药患者诊断思维_v1]]（今日生成 ⭐ 待章节复习后整合 — 方法论侧）
>   - [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] **Part 6.1**（Digoxin Toxicity 综合管理 — 药物本身侧；今日同步整合 v1.5）⭐
> - 🏥 跨学科：[[完整笔记/Peixuan分科笔记/肾脏]]（老年 + 利尿剂 → AKI → 经肾药物清除受损）
> - 🌱 TODO（待生成衍生）：
>   - ~~等积累 2-3 道 digoxin 题 → 整合 Digoxin_中毒与管理~~ **已落地** Vaughan Williams Part 6.1（2026-05-16）
>   - 等积累 5+ 道窄治疗窗药物中毒题 → 整合 [[完整笔记/专题笔记/_衍生_窄治疗窗药物速查]]（覆盖 lithium / warfarin / theophylline / phenytoin / vancomycin 等）
> 
> **✅ 复盘行动**：
> - [ ] 1 周后重做此题（2026-05-23）
> - [ ] 默写 "DIG-SICK" + 窄治疗窗药物 SOP 表
> - [ ] 训练新阅读习惯：stem 用药列表逐药扫描"能解释症状吗？"
> - [ ] 找 3 道类似题：UWorld 搜 "digoxin toxicity" / "drug toxicity elderly" / "narrow therapeutic window"
> - [ ] 把"HF 患者新发 GI 症状 → 先怀疑药物毒性"加进 [[完整笔记/专题笔记/_衍生_高频陷阱]]
> 
> ---
> 
> 学科:: 心血管
> 主题:: Digoxin toxicity / 老年多药患者用药列表逐药扫描
> 状态:: 🟡
> 错因:: pattern

> [!example]- [2026-05-16] 心内 / Symptomatic Bradycardia → Atropine 1st line (Q2141)
> ^Q2141
>
> ## Stem 模式
> HR 30 + syncope/lightheadedness/疲劳 + BP 82/44 + 嗜睡 + 末梢冷 + capillary refill 3s + ECG **sinus bradycardia**（结上）+ 无 BB/CCB 用药史 → "most appropriate next step?"
>
> ## 核心概念
> 症状性 sinus bradycardia + 不稳定 → **Atropine 1 mg IV** 是 ACLS 1st line（结上水平有效）
> 完整决策树 + 缓 vs 速反向用药逻辑见 [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] **Part 7.6 / 7.6.y / 7.6.z**（今日同步整合 v1.6）
>
> ## 普适规则（精简，详细去 Part 7.6）
> - **1st line**: Atropine 1 mg IV (q3-5 min, max 3 mg)
> - **2nd line**: TCP / TVP（同时可 dopamine 5-20 mcg/kg/min 或 epi 2-10 mcg/min）
> - **结上有效，结下无效**（Mobitz II / 3° → 别等 atropine，直接起搏）
> - **缓时禁 5 药**：β-blocker / non-DHP CCB / Digoxin / Adenosine / Amiodarone
>
> ## 易混陷阱 — D vs E 干扰项（Q2141 核心学习点）⭐
>
> | 选项 | 用于什么 | 为什么本题错 |
> |---|---|---|
> | A. Adenosine | SVT 终止折返 | **加重缓** + 用错心律 |
> | B. Amiodarone | AF / VT / VF | 负性变时 → **加重缓** |
> | **C. Atropine ✅** | 症状性窦缓 / 结上 AV 阻滞 | 1st line |
> | **D. Glucagon** | **明确 BB / CCB 中毒**特异解毒 | Stem **无 BB/CCB 用药史** → 没指征；"看到缓 + 低 BP 就想 BB 中毒"是 trap |
> | **E. Norepinephrine** | 脓毒症休克 / 严重低血压（升 α）| 本题低血压是**缓的果不是因**（HR↓→CO↓→BP↓）；NE 不增 HR + α 收缩加重外周缺血；**先 ↑HR，BP 自动回升** |
>
> ## Memory Hook
> - **缓 vs 速反向**："治速的药 = 缓时全禁"（BB / CCB / Digoxin / Adenosine / Amiodarone）
> - **缓 + 低 BP 反射弧**：先 atropine 升 HR，**不**先 NE 升 α
> - **缓 + 低 BP + 有 BB/CCB 史** → Glucagon（特异）；**没 BB/CCB 史** → Atropine（一般）
> - **结上 atropine，结下起搏**（Mobitz II / 3° 不要试 atropine）
>
> ---
>
> ## 🤔 我的提问 / 卡点
> - 卡点 1：缓 + 低血压时为什么不选 NE 升压？
>   → 学到：缓时低血压是 HR↓→CO↓→BP↓ 的果，**先纠正 HR，BP 会自动回升**；NE 升 α 但不增 HR，且加重外周缺血
> - 卡点 2：Glucagon 什么时候用？
>   → 学到：**仅明确 BB / CCB 中毒**才用（机制：绕过 β 受体直接 ↑cAMP）；没用药史就别选
>
> ## 🔗 关联
> - 🔁 同主题错题：
>   - [[mistakes/uworld-mistakes#^Q4456]] 老年间歇性 AV 阻滞（PR 长 + QRS 长 → EP study + PPM；结下水平 atropine 无效）
>   - [[mistakes/uworld-mistakes#^Q4454]] Digoxin toxicity（缓 + GI + 神经三联，"治速的药"用错时致命）
> - 📚 主笔记 + 已有衍生：
>   - [[完整笔记/Peixuan分科笔记/心内]]（心律失常 / ACLS）
>   - [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] **Part 7.6 + 7.6.y + 7.6.z**（今日同步整合 v1.6 — 缓 vs 速反向 / 5 大禁用药 / D vs E 陷阱）⭐
>   - [[完整笔记/专题笔记/_衍生_晕厥鉴别决策树]]（症状性缓属心源性晕厥红旗）
> - 🏥 跨学科：
>   - [[完整笔记/Peixuan分科笔记/感染]]（Lyme carditis → AVB）
>   - [[完整笔记/Peixuan分科笔记/neuro]]（Cushing 反射 = HTN + 缓 + 不规则呼吸）
>   - [[完整笔记/Peixuan分科笔记/endocrine]]（甲减 → 缓）
> - 🌱 TODO：
>   - 等积累 ACLS 心动过速 + 不稳定 SVT/AF/VT 错题 → 整合 [[完整笔记/专题笔记/_衍生_ACLS用药决策树]]（缓 vs 速 用药逻辑对称）
>
> ## ✅ 复盘行动
> - [ ] 默写"症状性缓 ACLS 流程"（atropine → TCP/TVP → dopamine/epi infusion）
> - [ ] 默写"缓时禁用 5 大类"（BB / CCB / Digoxin / Adenosine / Amiodarone）
> - [ ] 默写"D vs E 干扰项 — 没 BB 史不选 Glucagon；缓的低血压先升 HR 不升 α"
> - [ ] 默写"结上 atropine，结下起搏"
> - [ ] UWorld 搜：symptomatic bradycardia / AV block management / BB toxicity 各 2-3 题
>
> ---
>
> 学科:: 心血管
> 主题:: Symptomatic bradycardia ACLS / Atropine 1st line / Glucagon-NE 干扰项
> 状态:: 🟢
> 错因:: 知识
