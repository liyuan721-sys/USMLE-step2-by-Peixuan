---
tags:
  - USMLE-Step2
  - Ethics
  - QI
created: 2026-05-27
type: 专题笔记
---

# USMLE_患者安全_QI 工具与质量框架

> [!info] 本笔记定位
> 从 [[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]] (原 v1.3.15 大文件) 拆出，专注 **QI 工具方法论 + Healthcare Quality 框架 + Analysis Frameworks**。
> 4 子文件之一（另 3：[[完整笔记/专题笔记/USMLE/USMLE_患者安全_Safety文化与沟通]] / [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Cognitive诊断错误]] / [[完整笔记/专题笔记/USMLE/USMLE_患者安全_HFE与药物HAC]]）。
> 主索引：[[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]]（全局 §九 EOL / §十 9 大陷阱 / §十一 Memory Hooks 速查留索引文件）。

## §0 本文件目录

- §一 CK 题型套路（最常考的 3 种问法）
- §二 QI 工具 — Prospective vs Retrospective（FMEA / RCA / PDSA / Pareto / Lean / Six Sigma / Change Management）
- §十二 Healthcare Quality 框架与质量度量（STEEEP / Donabedian / HRO / BCA / Cost-Conscious Care）
- §13.12 Analysis Frameworks（RCA + Fishbone + 5 Whys + M&M + FMEA 升级）

---

## 一、CK 题型套路（最常考的 3 种问法）⭐

| 问法 | 套路 | 看哪一节 |
|---|---|---|
| **"Which intervention is most effective?"** | 选**系统改造**（forcing function / automation / standardization），不选 education / training | §三 防御层级梯队 |
| **"Which QI tool best fits this situation?"** | **事前选 FMEA，事后选 RCA**，监测稳态选 control chart，迭代试点选 PDSA | §二 QI 工具 |
| **"What is this called?"** | 名词配对（near-miss / sentinel / forcing function / Swiss Cheese / just culture） | §四 + §五 |

> [!tip] 答题原则
> **系统改造 > 提醒 > 培训**
> 看到 "most effective patient safety strategy" / "prevent future errors" → 优先 ① forcing function / ② automation / ③ standardization

### 1.1 Stem 细节解读 — Decisive vs 锦上添花 ⭐⭐⭐（v1.3.12 普适反射钩 — Q23111 锚定）

> [!warning] 普适原则（不只用在 Quality 题，所有 Ethics / Safety / Communication 题都适用）
> 看到 stem 描述主角的"**个人背景**"（leadership / experience / community trust / specialty / 工龄 / 资历）时，**先做 3 步判断**：
>
> **① 这条信息影响 4 个 wrong 选项里任何一个的对错吗？**
> - **不影响 → 锦上添花**（justify 正确选项的具体措辞）
> - **影响 → decisive**（直接决定选什么方向）
>
> **② 这条信息所在的逻辑链是"升级红线"吗？**
> - 升级红线 = adverse event 发生 / 内部协作失败 / capacity 丧失 / 利益冲突 / 病人自主权
> - **这些才是 decisive**
>
> **③ 一般规律**：
> - **个人 credential（leadership / experience / community trust）= 锦上添花**
> - **事件 severity（adverse event / harm / capacity / urgency）= decisive**

#### Q23111 拆解示范

| Stem 细节 | 性质 | 角色 |
|---|---|---|
| "Excessive **variations** in medication/imaging/LOS" | **Decisive** | 识别 systemic quality concern — 决定方向 |
| "**No adverse outcomes** observed" | **Decisive** | 决定不能选外部 board / 决定还有协作窗口 |
| "7 miles to alternate hospital" | **干扰** | 钓你选 refer out — 实际无关 |
| "Leadership experience" | **锦上添花** | Justify "participate on committee" 措辞 — 但不改方向 |
| "Community trust" | **锦上添花** | 同上 — 给 E 选项措辞背书 |

#### 拿掉锦上添花后答案变不变？

| 主角身份 | 答案方向 | 具体措辞调整 |
|---|---|---|
| 题里版本（FM + leadership + trust） | E：meet director + **participate on committee** | 主动领跑 |
| 普通家庭医生**无 leadership** | 仍 E 家族：meet director + **raise concerns / 提供 outpatient feedback** | 提醒不领跑 |
| Medical student rotation 发现 | 仍 internal team-based：**通过 attending / program director** 上报 | Entry point 不同 |
| **完全外人（家属 / 路人）+ no adverse event** | **方向变**：patient advocacy / letter to administrator | "Internal team" 路对外人不通 |
| **任何身份 + adverse event 已发生 + 内部协作失败** | **方向变到 D**：外部 board 合理 | 升级红线突破 |

> [!success] 结论
> **Leverage（credential）决定"主动到什么程度"，但不决定"选哪条路"**。路由 **adverse event 红线 + systemic concern 识别** 决定。
>
> 这条规则**普适所有 Ethics/Safety/QI 题** — 不只 quality concern 题。

#### 应用扩展场景

| 场景 | Decisive 信号 | 锦上添花 信号 |
|---|---|---|
| **Capacity assessment** | "Confused" / "unable to repeat back" / "MMSE 18" | "elderly" / "lives alone" / "widowed" |
| **Informed consent** | "Refuses despite understanding" / "comprehends risks" | "highly educated" / "PhD" / "former physician" |
| **End-of-life** | "Irreversible coma" / "no quality of life prospect" | "religious background" / "family preferences" |
| **Conflict resolution** | "Aggressive escalation" / "patient threat" | "respected senior staff" / "long-time employee" |
| **Fall prevention strategy**（Q107152 v1.3.13）| "80% classify high-risk" → wristbands 失效 | "AMBOSS table 推荐 visual cues" — 普适推荐 ≠ 本题适用 |
| **Unpredictable OB emergency**（Q105800 v1.3.14）| ">50% 无 risk factors" / "no risk factors in this patient" → checklist 失效 | "Checklist 是 evidence-based" — 普适推荐 ≠ unpredictable event 适用 |

**一句话锁**：**Decisive = 事件 / 临床事实；锦上添花 = 主角描述 / 普适推荐**。

#### 第三种细节：Stem-internal Linkage（Linked Vignette）⭐⭐（v1.3.13 — Q107152 新维度）

Linked vignette 题里，**Item 1 给的数字往往是 Item 2 的 decisive context**：

| Linked vignette 案例 | Item 1 数字 | 在 Item 2 的角色 |
|---|---|---|
| Q107151 → Q107152 | "80% classify as high risk" | **Decisive** — 让 wristbands / visual cues / bed alarms 失效（靠 discrimination 的策略全废） |
| Q106764 → Q106765 | "Drug-seeking suspect from chart" | **干扰** — Item 2 考 defensive medicine 与此无关（反例：linked 题 ≠ 同主题） |

**规则**：
- **Linked vignette ≠ 同主题**（不能 reflex-match 答案）
- **但 stem-internal 数字会跨题影响 decisive context**（先回顾 Item 1 关键数字再答 Item 2）

---

## 二、QI 工具 — Prospective vs Retrospective

### 2.0' 一句话锁定（5 工具条件反射版）⭐⭐⭐

> [!tip] 看 buzzword 直接锁工具，不犹豫
> | 工具 | 一句话核心 | Stem buzzword |
> |---|---|---|
> | **Six Sigma** | 减少变异 / 近零缺陷（统计驱动）| "reduce variation" / "near-zero defects" / "3.4 per million" / "6σ" / "statistical process control" |
> | **Lean** | 减少浪费 / 提高效率（去掉不增值步骤）| "eliminate waste" / "streamline" / "efficiency" |
> | **PDSA**（Plan-Do-Study-Act）| 小范围快速试错循环 | "small (rapid) test of change" / "pilot then scale" / "rapid cycle" |
> | **RCA**（Root Cause Analysis）| 事件**发生后**回溯找根因（retrospective）| "after a sentinel event" / "wrong-site surgery occurred" / "fishbone" |
> | **FMEA**（Failure Mode & Effects Analysis）| 事件**发生前**预判可能出错处（prospective）| "before operations begin" / "new unit not yet opened" / "proactively identify risks" |

> [!warning] 两条最高频一刀切
> - **Six Sigma（减变异）vs Lean（去浪费）**：3.4 per million / reduce variation → Six Sigma；eliminate waste / streamline → Lean（详见 §2.7.1）。
> - **RCA（事后 retrospective）vs FMEA（事前 prospective）**：出事**之后**查根因 → RCA；出事**之前**防漏洞 → FMEA（字眼陷阱详见 §13.12.8）。

### 2.0 Variation Management — Common Cause vs Special Cause ⭐⭐⭐（AMBOSS 增量 v1.2）

**Variation 定义**：医疗系统中 expected outcome vs actual outcome 的差异。一些 variation 是必要的（个性化照护）；不可预测的 variation 才是 QI 改进目标。

| 类型 | 性质 | 例子 | 管理策略 |
|---|---|---|---|
| **Common cause variation**（普通原因） | **Inherent 内生的**；stable + predictable 范围内但具体不可预测；**通常不能 trace 到 root cause** | 不同 demographic 患者反应差异 / 工作人员技能自然差异 | **Standardization**（protocols / checklists / clinical pathways）|
| **Special cause variation**（特殊原因）⭐ | **Specific cause + 非 inherent**；sporadic + unpredictable；**可以 trace 到 root cause + 可识别可解决** | Human error / wrong-patient coding / 临床流程被打断 | **RCA + 系统改造**（消除该 cause） |

**管理目标**：
- ✅ **减少 special cause variation**（找到并消除）
- ✅ **适当管理 common cause variation**（接受其存在，用 standardization 控制范围）

> [!warning] CK 易混
> - "Special cause = inherent" ❌ — Special 是**非 inherent**，可追根可解决
> - "Common cause 用 RCA" ❌ — Common cause **不能** trace 到 root cause；用 standardization
> - "Standardization 解决 special cause" ❌ — Standardization 针对 **common** cause

> [!success] 海浪 vs 海啸类比 ⭐（视觉记忆 hook — v1.3.9 新增）
> ```
> Common Cause = 海浪 🌊
> ├─ 总在波动（小幅度，~2-4% 背景波动）
> ├─ 无法预测具体哪一天高 / 哪一天低
> ├─ 没有 single root cause（多因素叠加 → "天然 noise"）
> └─ 管理：建防波堤（**Standardization** — protocols / checklists / clinical pathways）
>           ※ 不是消除波动，是把波动控制在可接受范围内
>
> Special Cause = 海啸 🌊🌊🌊
> ├─ 突然出现（远超基线，~12% 异常 spike）
> ├─ 有明确 root cause（地震 = root cause；wrong-patient ID / 流程被打断 / equipment failure）
> ├─ Sporadic + unpredictable + 可识别可解决
> └─ 管理：找到震源并预警（**RCA + 系统改造** — 消除该 cause）
> ```
>
> **一句话**：海浪日日有 → 建防波堤（standardize）；海啸罕见但致命 → 查震源（RCA）。
>
> **Control chart 读图反射**：
> - 所有点在 control limits 内波动 = 海浪 = common cause = stable process（用 standardization 优化整体水平）
> - **出 control limits 的点 / 7+ 点同侧 / 趋势** = 海啸 = special cause = **trigger RCA**

### 2.1 四大核心工具对比

| 工具 | 时机 | 用途 | Stem 触发词 ⭐ |
|---|---|---|---|
| **FMEA** (Failure Mode and Effects Analysis, 故障模式与影响分析) | **Prospective 事前** ⭐ | 新流程 / 新单位 / 新设备开张前找潜在故障 | "before operations begin" / "new ICU opening" / "anticipate problems" / "has not yet opened" |
| **RCA** (Root Cause Analysis, 根因分析) | **Retrospective 事后** | 出事后追根因 | "after a sentinel event" / "wrong-site surgery occurred" / "patient died from..." |
| **PDSA cycle** (Plan-Do-Study-Act, 戴明环) | 迭代改进 | 小范围试验 → 测 → 修改 → 推广 | "test small-scale change before full implementation" / "pilot then scale" |
| **Control chart / Run chart** | 持续监测 | 看已稳定流程是否在 control limits 内 | "monitor monthly infection rates over time" / "track trends" |

### 2.2 FMEA 详解 — Q19553 错题考点 ⭐

**核心**：**Prospective + 多学科团队 + 系统性**找潜在故障。

**5 步流程**：
1. 组多学科团队（医生 / 护士 / 呼吸治疗师 / 药剂师...）
2. 定义 FMEA 主题（ventilator alarm / med administration / handoff...）
3. 绘制流程图（每个步骤画出来）
4. 识别 **Failure modes**（每步可能出什么错）+ **Effects**（出错的后果）+ **Causes**（为什么会出）
5. 用 **hazard decision matrix** 估算可能性 + 严重度 → 排优先级 → 制 action plan

> [!warning] 易混
> - FMEA ≠ RCA — **时间方向相反**（prospective vs retrospective）
> - FMEA ≠ Control chart — control chart 是**已稳定流程后的监测**，FMEA 是**事前预防**
> - "New ICU 还没开" → 一定选 FMEA（其他工具需要数据 / 事件）

### 2.3 RCA 详解

**核心**：**Retrospective + sentinel event 强制触发 + 找系统根因（不是 blame 个人）**。

**典型 stem**：
- 手术做错部位
- 病人因为给错药死了
- Newborn 抱错家庭

**5 Whys 技术**：反复问 "为什么" 5 次直到挖到系统根因（疲劳 / UI 设计 / 培训缺失），不停在"她粗心"。

### 2.4 PDSA Cycle（升级 v1.2 + SMART + PDCA 区分）

**4 步循环**（Plan → Do → Study → Act）：
- **Plan**：定义改进领域 + 设计 corrective action；用 **SMART criteria** 设定目标
- **Do**：测试 new action + 文档化 unexpected observations
- **Study**：分析 **before/after 数据** + 与预测对比；用 measurement tools（Pareto / Control chart / Run chart）
- **Act**：根据数据决定**推广**（positive impact）或**修改后重来**（begin a new cycle）

**stem 触发**："pilot then scale" / "试点一个病房" / "小范围测试新协议" / "迭代式改进"

#### 2.4.1 SMART Criteria（Plan stage 必备）⭐⭐⭐

CK 高频名词。Plan stage 设定 objective 时用：

| 字母 | 含义 |
|---|---|
| **S**pecific | 行动 / 影响 / 目标人群 / 责任**明确** |
| **M**easurable | 量化指标 |
| **A**ssignable | 责任**分配**到具体团队 + 资源可达 |
| **R**ealistic | 与 mission 一致，可达成 |
| **T**imely | 时间框架**明确**，有截止 |

#### 2.4.2 PDCA vs PDSA 区别

| 模型 | 第三步重点 | 适用 |
|---|---|---|
| **PDCA**（Plan-Do-**Check**-Act） | **Check** = 检查 compliance（是否按计划执行）| Business settings；PDSA 的 precursor |
| **PDSA**（Plan-Do-**Study**-Act）⭐ | **Study** = 分析 data + reflection + **continuous learning** | **Health care 首选** ⭐ |

> [!tip] CK 区分
> CK 一般考 **PDSA**（health care 标准）；PDSA 强调 **learning > compliance**

### 2.5 Control Chart vs Run Chart

| 工具 | 内容 | 有 Control Limits | 用途 |
|---|---|---|---|
| **Run chart**（time plot） | 时间 vs 单一指标的折线 | ❌ 无 | 看趋势（rising / falling）；**不能判断 stable/unstable** |
| **Control chart**（Shewhart chart）⭐ | Run chart + **upper/lower control limits** + 中线 | ✅ 有 | 判断流程是否在 control 内；**出界点 = special cause variation** |

**Stem 触发**："monthly infection rates plotted over 12 months" / "track variation over time"

### 2.6 Pareto Chart — 80/20 找最大问题 ⭐（AMBOSS 增量 v1.2）

**结构**：条形图（按 frequency / cost 降序排列）+ 累计百分比折线（overlaid line）。

**用途**：识别**最重要的少数类别**（80/20 原则 — 80% 问题来自 20% 原因）→ 优先改这些。

**Stem 触发**：
- "identify highest-ranking reason for patient transfer delays"
- "which category causes most defects"
- "rank improvement priorities"

> [!info] 3 大 Measurement Tools 速查（CK 配对题）
> | 工具 | 看什么 | Limits | 何时用 |
> |---|---|---|---|
> | **Pareto chart** | 按频率排序的 bar + 累计 % 线 | — | **找最大问题 / 优先排序** |
> | **Control chart** | 时间趋势 + control limits | ✅ 有 | **判断 common vs special cause variation** |
> | **Run chart** | 时间趋势 + central line（mean/median） | ❌ 无 | **看趋势**（不能判 stability）|

### 2.7 4 大 QI Methodology — Model for Improvement / Lean / Six Sigma / Change Management ⭐⭐⭐（v1.3.15 升级 — AMBOSS 4 联表锚定）

> [!info] Methodology vs Tool 边界
> - **Methodology**（改进哲学）= 怎么思考问题 → PDSA / Lean / Six Sigma / Change management 4 大
> - **Tool**（具体工具）= 怎么执行 → FMEA / RCA / Control chart / Pareto / Run chart
>
> 同一个 **PDSA** 在 §2.1 / §2.4 作为 **tool** 与 FMEA / RCA 并列；在 §2.7 作为 **methodology** 与 Lean / Six Sigma / Change management 并列 —— 不矛盾，是不同抽象层。

#### 4 大 Methodology 主表（AMBOSS 4 联）

| Methodology | 核心 (Core) | Example | Stem 触发词 ⭐ |
|---|---|---|---|
| **Model for Improvement / PDSA cycle** ⭐ | **Incremental cycles** of planning, piloting, assessing, refining（迭代改进）| 新 check-in procedure + weekly patient satisfaction survey | "cyclical" / "iterative" / "pilot then refine" / "small-scale change before full implementation" / "ongoing data collection to adjust" |
| **Lean** ⭐⭐ | **Reduce waste** + optimize workflow（消除浪费 + 优化流程）| Streamlining scheduling → 减 wait time / no-show | "reduce waste" / "eliminate unnecessary steps" / "streamline" / "reduce no-show / wait time" / "value stream" |
| **Six Sigma** | **Near-elimination of defects** through statistically driven process（统计学驱动近零缺陷，6σ = 99.99966% = 3.4 defects/million）| Controlling wrong-site surgery rate to < 0.00001% | "near zero defects" / "6σ" / "3.4 per million" / "statistical process control" / "catastrophic error elimination" / "reduce variation" |
| **Change management** ⭐（新增 v1.3.15）| Engaging **personnel** to adopt + implement organizational change（人因驱动 — 让员工接受变革）| 找 frontline early adopters lead EHR implementation | "**champion**" / "**early adopter**" / "engage staff in adoption" / "culture change for new system" / "physician buy-in" / "resistance to change" |

#### Lean 的 8 大 Waste（医疗版 — TIMWOODS 记忆法）

```
T - Transportation        不必要搬运（病人 / 标本 / 物资）
I - Inventory             库存过多
M - Motion                不必要动作（HCP 走动）
W - Waiting ⭐ (最常考)    等待时间（病人候诊 / lab 报告 / 转诊）
O - Overproduction        过度生产 / 检查 / 医嘱
O - Overprocessing        过度处理
D - Defects               缺陷（need rework）
S - Skills underused      人才浪费（高资 HCP 做低端工作）
```

#### Six Sigma DMAIC 流程

```
D - Define     定义问题（如 wrong-site surgery rate 偏高）
M - Measure    测量当前缺陷率（baseline data）
A - Analyze    找根因（统计学 + control chart + Pareto）
I - Improve    实施改进（process redesign）
C - Control    维持改进（statistical process control 长期监控）
```

#### Change Management 关键概念

| 概念 | 含义 | CK Stem 信号 |
|---|---|---|
| **Champion** ⭐ | 变革推动者（关键意见领袖 / 院领导支持） | "physician champion leading the rollout" |
| **Early adopter** ⭐ | 早期采纳者（先试用 → 影响其他人）| "identify early adopters in each department" |
| **Stakeholder engagement** | 利益相关者全员参与 | "engage frontline staff in design" |
| **Culture change** | 组织文化转变（不只是流程改）| "shift from blame to just culture" |
| **Resistance to change** | 抗拒变革（自然反应，要主动管理）| "staff reluctant to adopt new EHR" |

> [!tip] CK 经典 stem
> 医院要推新 EHR / 新临床路径 / 新 safety protocol — 怎么让员工真的用起来？→ **Change management**（找 champion / 找 early adopter / engage stakeholders）。**不是** education alone（培训不解决"愿不愿意用"）。

---

### 2.7.1 Lean vs Six Sigma 关键区分 ⭐⭐⭐（最高频考点 — v1.3.15 新增）

CK / AMBOSS 反复在 Lean 和 Six Sigma 之间钓选项。**5 维对照**：

| 维度 | **Lean** | **Six Sigma** |
|---|---|---|
| **目标** | 减 **waste / inefficiency**（浪费 / 低效） | 减 **defects / variation** 到 6σ（缺陷 / 变异） |
| **核心问题** | "这一步有没有 **value**？" | "这一步**错误率**有多少？" |
| **场景** | wait time / no-show / 流程冗余 / 候诊堵塞 | wrong-site surgery / medication error / never events / catastrophic |
| **关键词** | streamline / workflow / value / waste | defect / variation / statistical / 99.99966% / control chart |
| **工具** | Value stream map（价值流图）/ Lean 8 waste | Control chart / Capability analysis / DMAIC / statistical process control |

> [!success] 记忆诀窍（v1.3.15 视觉 Hook）
> - **Lean = 流畅** 🌊 — 去除堵点，让流程跑得**顺**（重点在"流不流畅"）
> - **Six Sigma = 精准** 🎯 — 消除错误，让结果**零缺陷**（重点在"准不准"）
>
> 一句话决策：
> - 题干说 "**等太久 / no-show / 走太多路 / 不必要步骤**" → **Lean**
> - 题干说 "**手术错位 / 用错药 / 5σ → 6σ / 统计学**" → **Six Sigma**

> [!warning] Lean 反 pattern
> "Lean = 减病人数 / 砍预算" ❌ — Lean 减的是 **waste（无价值步骤）**，不减 value。砍病人数是 cost-cutting 不是 Lean。

---

### 2.7.2 Swiss Cheese Model vs Lean — Mental Model vs Methodology 区分 ⭐⭐（v1.3.15 新增）

很多人会把 Swiss Cheese 当成 QI methodology，**但它根本不是**。

| 概念 | 性质 | 用法 |
|---|---|---|
| **Swiss Cheese Model** | Patient safety **mental model**（思维模型 — 解释错误为什么发生） | 多层 safeguard 像奶酪片，每片有洞（vulnerabilities）。**洞对齐时 hazard 穿过所有层 → adverse event**。用于**事后解释**或**事前思考防御层**。详见 §3.2 |
| **Lean** | QI **methodology**（方法学 — 主动改进流程） | 主动**识别并消除 waste**，优化 workflow。用于**改造流程减低效**。详见 §2.7 |

> [!danger] CK 关键区分
> - 题目问"**用哪种 model 解释**这次 adverse event" → **Swiss Cheese Model**
> - 题目问"**用哪种 QI methodology 防止再次发生**" → 看具体故障：
>   - 减 wait / waste → **Lean**
>   - 减 defect / variation → **Six Sigma**
>   - 迭代试点 → **PDSA**
>   - 让员工接受 → **Change management**

**类比**：
- Swiss Cheese = **解剖图**（告诉你身体怎么坏的）
- Lean / Six Sigma / PDSA / Change mgmt = **治疗方案**（怎么治）

> [!tip] 同类区分提示
> **RCA**（§2.3 / §13.12）也是**分析工具**（事后找根因），不是改进 methodology。同样道理：
> - Swiss Cheese / RCA / Fishbone / 5 Whys = **分析框架**（理解 error）
> - PDSA / Lean / Six Sigma / Change mgmt = **改进方法**（防止 error）
> - FMEA / Control chart / Pareto = **QI 工具**（具体操作）

---

### 2.7.3 4 步选择法 — Methodology Decision Tree ⭐（v1.3.15 新增）

```
看到 QI 场景，按顺序问自己：

├─ 1. 是不是 "小试点 + 迭代 + 反复调整"？      → PDSA / Model for Improvement
│     ✓ 关键词：cyclical / iterative / pilot then refine
│
├─ 2. 是不是 "减 waste / 等待 / 冗余步骤"？     → Lean
│     ✓ 关键词：streamline / waste / wait time / no-show
│
├─ 3. 是不是 "把错误降到接近零 + 统计学"？      → Six Sigma
│     ✓ 关键词：6σ / 99.99966% / statistical / catastrophic
│
└─ 4. 是不是 "让员工接受变革 / champion"？      → Change management
      ✓ 关键词：champion / early adopter / buy-in / culture

如果题目问 "为什么 error 发生" 而不是 "怎么改" → Swiss Cheese Model
如果题目问 "找出 error 根本原因 + 系统分析"   → RCA（§2.3）
如果题目问 "新流程上线前预防 error"            → FMEA（§2.2）
```

> [!warning] 4 高频陷阱
> 1. **PDSA vs Lean**：都能"改善满意度"，区分点是**是否 cyclical/iterative**。强调"试点再扩展"= PDSA；强调"消除等待 / 流程冗余"= Lean
> 2. **Six Sigma 关键词陷阱**：看到 6σ / 99.99966% / 3.4 per million / statistical process control → 直接 Six Sigma
> 3. **Change management 容易漏选**：题目重点在"**人**"而不是"流程"时选这个 — champion / early adopter / culture / buy-in 是强信号
> 4. **Swiss Cheese ≠ QI methodology**：它是 error analysis 工具，不是改进方法。同理 RCA / Fishbone / 5 Whys 也是分析工具不是 methodology

---

### 2.7.4 4 大 Patient Safety System Design Models 钉死表 ⭐⭐⭐（v1.4 新增 — Q21477 + Q7-2026-05-27 双反复错驱动）

> [!danger] 5-25 + 5-27 反复错触发 🔴
> Q21477 SCM 5-25 选 hard stops + 5-27 Q7 选 PDSA — 两次都不识别 Swiss Cheese Model；本节为治本钉死。
>
> **核心区分**：**System Design Models（如何防 error）** vs **Error Analysis Tools（已发生 error 怎么分析）** — SCM/Hard stop/Automation 是设计层，RCA/FMEA/CCA/M&M 是分析层；PDSA 跨两个层（既是 methodology 又是分析 cycle）。

#### 4 大模型主表（Stem 暗号词钉死）

| 模型 | 核心 | Stem 暗号词 ⭐ | 经典应用 |
|---|---|---|---|
| **Swiss Cheese Model (SCM)** ⭐ | 多个不同性质 barrier **simultaneously / concurrently** 叠加 — 单层都有"洞"但叠加难一次穿透 | "implemented **simultaneously**" / "multiple measures **concurrently**" / 列举 ≥ 2 **不同性质**维度（教育 + 物理 + 个人防护 + 免疫）| 感染控制 bundle（洗手 + 口罩 + 通风 + 疫苗 + 教育）/ 手术安全 / 用药安全 |
| **Hard stop (Forcing function)** | **1 个物理设计强制不能错**（USP-level prevention）| "**physically** incompatible connector" / "**hard limit** prevents overdose" / "**cannot enter** wrong value" | 麻醉气体不同接口（O₂ 接不上 N₂O）/ 给药泵 dose-range hard limit / Tall Man Lettering 强制视觉差异 |
| **Automation** | **计算机替代易错人工**（认知卸载）| "**automated** dose calculation" / "**smart pump** algorithm" / "**EHR alerts**" / "**CDSS** alert" / "**barcode** scanning" | Smart pump auto-dose / EHR drug-drug interaction alert / Barcode medication administration (BCMA) |
| **PDSA (Plan-Do-Study-Act)** | **Iterative cycles + 反复 refine**（不一次到位）| "**repeated cycles**" / "**small-scale change before** full implementation" / "**pilot → measure → refine → expand**" / "**iterative testing**" | 新 check-in 流程 pilot 1 周 + measure 满意度 + refine 后 expand / Lab workflow 试点改进 |

#### SCM 三原则（再钉一次）⭐

1. **任何单一 barrier 都有"洞"**（人会忘洗手 / 口罩戴错 / 疫苗漏接种 / 设备失灵）
2. **Harm 发生 = 所有洞对齐贯穿**（hazard 穿过每层 → 后果实现）
3. **多层 overlapping → 洞对齐概率指数下降**（5 层叠加 = 5 个独立小概率乘积 ≈ 趋近 0）

#### 经典 SCM 应用 — USMLE 高频 ⭐

| 场景 | 多层 barrier |
|---|---|
| **感染控制 bundle** | 洗手 + 口罩 + 通风 + 疫苗 + 教育（5 片奶酪）— Q21477 经典 |
| **手术安全** | 术前 marking + time-out + count + 双人核对 + 设备检查 |
| **用药安全** | 电子开药 (CPOE) + pharmacist 复核 + barcode (BCMA) + smart pump + double-check |
| **跌倒预防** | Bed alarm + 物理 barrier + sitter + low bed + 鞋子 + 评估 risk score |

#### 4 大模型钉死决策树 ⭐

```
看到 Patient Safety 题，扫 stem → 识别"如何防 error"路径
    │
    ├─ "Multiple measures **simultaneously** / concurrently"
    │  + 列举 ≥ 2 不同性质维度
    │     → **Swiss Cheese Model**（多片奶酪同时叠加）⭐
    │
    ├─ "**Physically** incompatible / cannot enter wrong"
    │  单一物理设计强制
    │     → **Hard stop / Forcing function**
    │
    ├─ "**Automated** / smart pump / EHR alert / barcode"
    │  计算机替代人工
    │     → **Automation**
    │
    └─ "**Repeated cycles** / iterative / pilot then refine"
       小规模试点 + 反复调整
         → **PDSA**
```

#### 反 pattern 警示 ⭐⭐⭐

| 误选 | 为什么错 |
|---|---|
| 见 5 个措施反射 → PDSA（"5 个 cycles"）❌ | PDSA 关键不在"措施数量"，在"**时序 iterative**"（一轮做完看效果再下一轮）；本题 stem 是 **simultaneously concurrent** 上线，不是 cycles |
| 见"多层防御"反射 → Hard stop（"hard stops 复数"）❌ | Hard stop = **物理单点强制**（如气体接口不兼容）；SCM 才是多层叠加 |
| 见 fishbone / RCA 反射 → SCM ❌ | Fishbone / RCA 是**分析工具**（已发生 error 怎么分析），SCM 是**设计模型**（如何防 error） |
| 见"automation 自动" 反射 → SCM ❌ | Automation 是单一 layer（很好的 layer），但单独不是 SCM；SCM 是 **多 layer 叠加** |

#### 一句话锁 ⭐

- **"同时上 N 个不同性质 barrier = Swiss Cheese（多片奶酪同时摆）"** ⭐
- **"反复试 cycles = PDSA（先做一小批再扩）"**
- **"物理不让错 = Hard stop（接口不兼容）"**
- **"计算机替手算 = Automation（EHR alert / smart pump）"**
- 类比：感染 bundle = SCM；新流程 pilot then scale = PDSA；麻醉气体接口不兼容 = hard stop；smart pump 自动算剂量 = automation

---


---

## 十二、Healthcare Quality 框架与质量度量（AMBOSS QI 章节整合 v1.1）⭐

> [!info] 整合来源
> AMBOSS Quality Improvement 章节 5 个核心概念，CK 名词配对题 + framework 应用题高频出现。
> 本节与 §二（QI 工具）互补：§二 是"用什么工具改"，§十二 是"评估什么维度 / 衡量什么指标"。

### 12.1 STEEEP — 6 大 Healthcare Quality Aims（IOM 框架）

CK 考点：**名词记忆 + 配对场景**。

| 字母 | 维度 | 中文 | 实例（CK stem 触发词） |
|---|---|---|---|
| **S**afety | 安全 | 避免 / 减少 iatrogenic injury | Forcing function / checklist / time-out / 防 medication error |
| **T**imeliness | 及时 | 减少有害延迟 | Door-to-needle / staggered shifts / telemedicine / same-day appointments |
| **E**ffectiveness | 有效 | 循证 + 避免无效治疗 | 不开 abx for viral URI / 不做 imaging for nonspecific LBP |
| **E**fficiency | 效率 | 最小资源最高质量 | 避免 overutilization / unnecessary imaging / 重复检查 |
| **E**quitable | 公平 | 不论 gender / race / SES 公平 access | Health disparity 监测 / 公平 referral |
| **P**atient-centered | 以病人为中心 | 尊重 preference / values / 个性化 | Shared decision-making / 家庭参与 / cultural sensitivity |

> [!tip] 记忆
> **"STEEEP"** — 5 个 E（Effectiveness / Efficiency / Equitable / 含 S 安全 T 及时 P 病人中心）→ 6 维评估任何 QI 项目

### 12.2 Donabedian Model — 5 类 Healthcare Quality Measures ⭐⭐⭐

**CK 高频"这属于哪类 measure"配对题** — 必须能秒分辨。

| 类型 | 中文 | 度量什么 | 经典例子 ⭐ |
|---|---|---|---|
| **Structural** | 结构 | **资源 / 设施 / 人员配置** | • 床位数<br>• Physician-to-patient ratio<br>• 营养师数量<br>• ICU 设备配置 |
| **Process** | 过程 | **流程执行率**（做没做） | • Cancer screening 接受率<br>• HbA1c 检测频率<br>• 流感疫苗接种率<br>• 洗手依从率 |
| **Outcome** | 结果 ⭐ | **最终临床结局** | • Mortality rate<br>• Nosocomial infection rate<br>• Maternal mortality<br>• 平均 HbA1c 水平 |
| **Balancing** | 制衡 | **一个干预对另一系统的影响** | • 缩短住院日 → readmission 率变化<br>• 增加营养师 → cost-benefit 分析 |
| **Composite** | 综合 | **整合多类为单一分** | • Afib 综合指标 = 专家数（structural）+ 抗凝率（process）+ stroke 率（outcome） |

> [!danger] 关键易混区分（CK 考点核心）
> | 表述 | 类型 | 为什么 |
> |---|---|---|
> | "**做** HbA1c 检测的患者比例" | **Process** | 流程执行率 |
> | "患者**平均** HbA1c 水平" | **Outcome** | 真实临床结局 |
> | "护士 / 床位 / 设备数量" | **Structural** | 资源配置 |
> | "**接种**疫苗的儿童比例" | **Process** | 流程执行 |
> | "**感染率** / **死亡率**" | **Outcome** | 终末结局 |
> | "缩短住院 → readmission **是否上升**" | **Balancing** | 干预对另一系统的影响 |

#### 12.2.x Outcome 不变诊断顺序 ⭐⭐⭐（v1.3.9 新增 — Q22359 锚定）

**CK 高频 stem**：QI intervention 实施后 outcome 不变 → 哪个 indicator 该测才能 better understand？

```
Outcome unchanged after QI intervention
     │
     ▼
① ⭐ Process indicator — checklist / compliance 完成率（FIRST）
     │
     ├─ Low compliance（busy times 漏做）
     ├─ High variation（不同班次完成不一致）
     ├─ Complexity 问题（checklist 太长）
     └─ Staffing 不足
     │
     ▼
② Structural — 知识 / 资源是否到位（已测则跳过）
     │
     ▼
③ Patient-related factors — 患者本身 severity
     （不是常 primary 解释 — patient factors 影响但不 systematically alter intervention results）
```

> [!success] Q22359 经典 stem（CLABSI checklist 不见效）
> ICU 实施 CLABSI 防控 checklist + 训练 → 6 月后：① Structural ✓（knowledge ↑）② Outcome ✗（CLABSI rate unchanged）③ Balancing ✓ 已测（documentation time ↑）→ 缺哪个 indicator？
>
> **答案 = Process variation and compliance**（D ✓）— checklist 完成率 / 不同班次 variation。
>
> **反 pattern**：
> - A "counterbalancing costs" ❌（balancing 已测）
> - B "organizational structures" ❌（structural 已测）
> - C "patient-related factors" ❌（patient factors 不 systematically alter intervention results）
>
> **反射钩**：见 "outcome unchanged + structural OK + balancing already measured" → 0.5 秒锁 **process compliance**

> [!tip] 4 indicator 关系示意
> 实施 QI → ① **Structural**（资源足？） → ② **Process**（实际执行了？） → ③ **Outcome**（病人结局改善？） → ④ **Balancing**（引入 cost / 不良 trade-off？）
>
> "**做了"= Process ⭐；"结果"= Outcome；"资源"= Structural；"副作用"= Balancing**

### 12.3 High-Reliability Organizations (HROs) — 5 Principles of Reliability

**HROs 定义**：在**高风险 + 复杂环境**下**持续少错的组织**（航空 / 核电 / 一流医院）。

| Principle | 中文 | 含义 | CK 关联 |
|---|---|---|---|
| **1. Preoccupation with failure** | 警惕失败 | 对潜在故障**高度敏感**；**near-miss 当 learning** 不当 "无害不管" | ↔ §四 near-miss reporting |
| **2. Reluctance to simplify** | 拒绝简化 | 承认系统复杂性，不偷工减料；但 standardization 仍有效率价值 | ↔ §三 防御层级 |
| **3. Sensitivity to operations** | 关注一线 | **Situational awareness** — 一线人员对系统整体感知 | ↔ §3.3 Time-out |
| **4. Commitment to resilience** | 接受不完美 + 训练韧性 | 接受 error 不可避免；训练应对而非追求 zero-error | ↔ §五 Just culture |
| **5. Deference to expertise** ⭐ | 重经验 > 重等级 | 让**最有经验的人**决策，**不论职称** | ↔ §六 closed-loop / 团队扁平化 |

> [!warning] CK 陷阱反 Pattern
> - "HRO 追求 **zero error** environment" ❌ — Principle 4: 接受不可避免，重点 resilience
> - "HRO 必须由 attending / senior 拍板" ❌ — Principle 5: 重经验 > 等级，护士经验丰富时听护士
> - "HRO 反对所有 standardization" ❌ — Principle 2: complexity + standardization 都需要
> - "HRO = no-blame culture，从不惩戒" ❌ — 同 Just culture，reckless behavior 仍要罚

#### AMBOSS Systems Approach to Error Prevention — 4 Components 补充版 ⭐⭐⭐（v1.3.6 新增 — Q22079 锚定）

AMBOSS 给出的 **Systems Approach 4 Components**（与 §12.3 上面的 HRO 5 Principles 互补，**侧重设计哲学**）：

| Component | 内容 |
|---|---|
| **① Culture of safety** | Prioritize **safety-promoting resources** + 强调 reporting + learning（不 blame）|
| **② Resilience** ⭐⭐ | **Systems design to prevent errors** — 把 human error 视为 inevitable，设计 workflow processes 来 **anticipate + minimize consequences** of error |
| **③ Team-based vigilance** | **Safety oversight by entire team**（不只 attending）— 每个 member 持续 monitor errors + 可 candidly speak up without retaliation |
| **④ Comprehensive analysis** | **Avoid simplistic explanations** — 仔细 examine all factors 包括 **latent factors**（system-level vulnerabilities），不只 focus on individual personnel |

#### Examples of Systems Approach

| Example | 内容 |
|---|---|
| **Human factors engineering** | Reduce human effort needed for safe action（见 §13.6 HFE 3 档分级）|
| **Swiss cheese model** | Multiple **overlapping layers** to block errors（"holes" — 见 §3.2）|

#### 核心反直觉 — "Zero Adverse Events ≠ Zero Human Error" ⭐⭐⭐

> [!danger] CK 高频陷阱
> 直觉以为"safety goal = 让 staff 不犯 error"。**错** —— Human error 在 complex 环境**不可避免**；clear organizational goals of "zero human error" 是**不现实** + **dangerous**：
> - 不 address latent errors within systems
> - **促进 culture of fear**（员工怕被 blame → 不 report errors → 学习机会消失）
>
> **正确 goal**：**Zero adverse events**（zero harm to patients）— 通过 **systems + processes that REDUCE reliance on human effort**（checklists / standardization / automation / forcing functions / preprogrammed limits）。
>
> **Resilience to error 核心**：human error → **systems anticipate + minimize consequences**（例：infusion pump preprogrammed dosing limits 即使 staff 输错 dose 也不出 harm）。

#### Q22079 4 大反 pattern 分析

| 反 pattern | 例 | 为什么错 |
|---|---|---|
| **① "Increase reliance on human effort"** | A 选项 | ❌ 反向 — Systems approach 是**减少** human effort reliance，不增加 |
| **② "Delegate safety to specific group"** | B 选项 | ❌ 违反 team-based vigilance 原则；safety 是**全员**责任 |
| **③ "Workflow processes minimize consequences"** ✅ | C 正解 | Resilience to error 完美 example — anticipate + minimize harm from inevitable errors |
| **④ "Event analyses to identify personnel involved"** | D 选项 | ❌ Individual-focused / blame-oriented；违反 Comprehensive Analysis（应 examine system + latent factors）|
| **⑤ "Zero human errors goal in high-risk settings"** | E 选项 | ❌ 不现实 + dangerous + culture of fear；应 zero adverse events 不是 zero human errors |

#### 一句话锁

> [!success]
> 「**Systems Approach 4 Components：Culture of safety + Resilience + Team-based vigilance + Comprehensive analysis**」
> 「**Goal = Zero adverse events（zero harm）不是 Zero human error**」
> 「**Resilience = design workflow to minimize consequences of inevitable errors**（preprogrammed limits / checklists / automation）」

### 12.4 Cost-Conscious Care + Antibiotic Stewardship Programs (ASPs)

**核心理念**：高 **value** = quality / cost — 在保证质量前提下避免 overutilization。

**Overutilization 4 大反 pattern**（CK 高频 stem）：
- ❌ 不必要的 **imaging**（如 nonspecific LBP 的 MRI）
- ❌ 不必要的 **antibiotics**（viral URI / acute bronchitis）
- ❌ 不必要的 **opioid prescriptions**
- ❌ 不必要的 **screening**（Pap smear for limited life expectancy / cancer screening 临终病人）

**原则**：
- ✅ 循证决策（不依从 patient demand）
- ✅ Generic > Brand-name（同效更便宜）
- ✅ 个性化（life expectancy 短 → 不做 screening）
- ✅ 透明告知 cost 给病人

**Antibiotic Stewardship Programs (ASPs)** ⭐：
- **多学科团队**（ID 医生 + 临床药师 + 护士 + 微生物实验室）
- 监测 + 优化抗生素使用
- 减少 **C. difficile** + **multidrug-resistant organisms (MDROs)** + 节省成本
- CK 关键词："reduce inappropriate antibiotic prescribing" / "decrease antibiotic resistance"

> [!tip] CK 高频 stem
> 病人 demand 抗生素 for viral URI / acute bronchitis → **patient education + antibiotic stewardship**（不 prescribe / 不开 placebo / 不顺从 demand）
> 参考 [[完整笔记/专题笔记/_衍生_Ethics精简框架]] §12.13 Antibiotic Stewardship Counseling 子节（reframe as "chest cold" / delayed Rx）

### 12.5 Benefit-Cost Analysis (BCA)

**用途**：经济学方法比较 intervention 的 cost vs benefit，辅助 budget priority 决策。

**两大指标**：

| 指标 | 定义 | 实施 cutoff |
|---|---|---|
| **Benefit-cost ratio** | Benefits / Net costs | **> 1** 才实施 |
| **Net benefit** ⭐（preferred measure） | Benefits − Costs | **> 0** 才实施 |

**特点**：
- 两者都用 **monetary terms**（钱衡量）→ 适合跨 intervention 排序
- 评估**immediate cost**（项目花费）+ **long-term benefit**（如 prevention 现在花钱，5 年后省钱）

> [!info] BCA vs Cost-Effectiveness Analysis (CEA)
> | 方法 | Cost 单位 | Benefit 单位 | 用途 |
> |---|---|---|---|
> | **BCA** | $ | $ | 跨 intervention 直接比金额排序 |
> | **CEA** | $ | Clinical outcome（QALY / 寿命年 / mmHg 降低）| 比"性价比"但不要求 benefit 折算成钱 |
>
> CK 一般考概念区分，不算具体数字。

### 12.6 Integrated Care + Feedback Loops（次要考点）

**Integrated care 定义**：多学科 + 跨级别（primary / specialty / inpatient / community）协调的连续性照护。

**4 原则**：
- Education + shared decision-making
- 服务针对个人 / 社区需求
- 持续改进 access / quality / efficiency
- **Performance improvement through feedback loops**（PDSA 是常用工具）

> [!info] Feedback loop 与 PDSA 关系
> Integrated care 用 **PDSA cycle**（§2.4）作为持续改进引擎；CK 偶尔考 "performance improvement through feedback loops" = PDSA 应用。

### 12.7 Variation Reduction Strategy — High Variation 后果 + Data-Driven Feedback 干预 ⭐⭐（v1.3.3 新增 — Q106289 + Q106290 锚定）

#### High Variation in Care 的后果 ⭐

**核心铁律**：对有 well-established practice guidelines 的医疗条件，**high variation in care = ↑ costs + ↓ quality + ↓ value**（quality / cost 比下降）。

| 维度 | 影响 |
|---|---|
| **Cost** | ↑（unnecessary use of services / overuse / 重复检查）|
| **Quality** | ↓ 或 unimproved（与 evidence-based guidelines 偏离）|
| **Patient outcomes** | Worse maternal + fetal outcomes（CD 案例：infection / emergency hysterectomy / 新生儿 respiratory distress）|
| **Patient satisfaction** | Not improved + 不 reduce malpractice litigation |
| **Value**（quality/cost 比）| ↓ |

**经典 stem 模式**：
- Cesarean delivery 率在 NTSV（**N**ulliparous **T**erm **S**ingleton **V**ertex）presentations 中**high variation among hospitals / OBs**（55% 高于 regional + 30% 个体差异，远高于推荐 ~16%）→ high variation → ↑ cost + 无 outcome 改善

#### Variation Reduction 干预选择 — Data-Driven Feedback 首选 ⭐⭐⭐

| 干预 | 有效性 | 为什么 |
|---|---|---|
| **Data-driven feedback** ⭐⭐⭐（正解）| **最有效** | Provide physician with **individual clinical performance data vs benchmarks / peers** → 提升 awareness of how 自己 practice 与 evidence-based 差异 → 改善 clinical decision-making |
| **Passive education**（expert-led workshops）| 较弱 | 不针对个人 practice pattern；不显示个体偏差 |
| **Patient-centered approach** | 较弱 | 改善 satisfaction + outcomes 但 **不针对** physician practice style modifying |
| **Increased malpractice insurance coverage** | 无效 | 不 address 心理 discomfort with litigation；不减 unnecessary services |
| **Defensive medicine education** | 无效 | 不 address physician 自己 practice variation 来源 |

#### Variation 源头 — Physician Practice Style ⭐

> [!info] 核心 insight
> 同一医院、同一 case mix、同一 patient demographics → **OB 个体之间 CD 率仍可 30%+ 差异** → 这种差异**主要来自 physician individual practice style**（subjective decision-making + attitudes + perceptions about treatment），不是 patient factor。
>
> 这就是为什么 **individual performance data feedback** 比 group education 有效 — 让 physician 看到 "我比同事高出多少 / 比 benchmark 高出多少"，触发 self-correction。

#### 与 §12.2 Donabedian 联动

| Donabedian 维度 | 在 variation reduction 中的角色 |
|---|---|
| **Structural** | 提供 EHR + data analytics infrastructure 才能 feedback |
| **Process** | Data-driven feedback **本身** 是 process measure（physician 接收 feedback 频率 + 行动率）|
| **Outcome** | Variation reduction 后看 outcome（mortality / 并发症 / cost）改善 |
| **Balancing** | 监测 feedback 是否 induce 反向 overuse / 患者满意度下降 |

#### 4 大反 pattern（CK 钓饵）

| 反 pattern | 例 | 为什么错 |
|---|---|---|
| **① High variation 自动 = ↑ quality** | "More services = better care" | ❌ 对有 guidelines 的条件，high variation = ↓ quality |
| **② 用 patient-centered 解决 physician variation** | 强推 shared decision-making 减 CD | Patient-centered 改善 satisfaction，**不改** physician practice style |
| **③ Increased malpractice 保险 = 减 defensive medicine** | C 选项 | Insurance 不 address physician 心理 discomfort with litigation 来源 |
| **④ Workshops 比 individual feedback 强** | National experts workshop | Passive education **弱于** individualized data-driven feedback |

> [!success] 一句话锁
> 「**High variation in well-guidelined conditions = ↑ cost + ↓ quality + ↓ value**」
> 「**Reduce variation 首选：Data-driven feedback on individual performance vs benchmarks**」（不是 workshop / patient-centered / malpractice insurance）

### 12.8 Healthcare Value = Quality / Total Cost Ratio ⭐⭐（v1.3.6 新增 — Q22780 锚定）

#### 反射钩

> [!info]
> Stem 给 intervention（如 intraoperative pathology eval / EHR upgrade / new workflow）+ 问 "best assesses whether intervention improves **healthcare value**" → 反射 **value = quality outcomes / total costs ratio** → 必须**对比 quality 与 cost**，不是单测一个 metric。
> ❌ 单测 reoperation rate（quality only）❌ 单测 operation time（cost indicator only）❌ 仅 short-term costs（不全）

#### Value 核心公式

```
              Quality
   Value  =  ─────────
            Total Cost
```

#### Value 定义详解 ⭐

| 维度 | 内容 |
|---|---|
| **Quality** | Patient outcomes（**mortality / morbidity**）+ Safety（**adverse events**）+ Patient care metrics（**satisfaction / wait times**）|
| **Costs** | **Total costs**（**not only short-term**）— per patient over the **entire course of treatment**；可从 patient / health care system / society 不同 perspective 评估 |
| **High-value care** | Optimize quality 同时 minimize total costs + waste（avoiding unnecessary treatment / complications） |

#### Q22780 经典 Stem 解析

**Intraoperative pathology 评估 negative margins** intervention：
- **Short-term cost ↑**：additional staff + reduced revenue from lower case volumes + extended operation time
- **Long-term cost ↓**：fewer surgical complications + unnecessary reoperations + frees up OR for other surgeries
- **Quality ↑**：reduced reoperation rate / improved patient morbidity / patient satisfaction
- **Value assessment**：comparing **quality outcomes** （reoperation rate）to **total costs** per patient（including long-term offset）

#### 4 大反 pattern（CK 钓饵）⭐

| 反 pattern | 例（Q22780 选项）| 为什么错 |
|---|---|---|
| **① Quality-only metric** | "Compare reoperation rates before/after" | Only **quality indicator**；不 capture cost；only **partial** info |
| **② Cost-only metric** | "Quantify operation time increase" | Only **cost indicator**；不 capture quality；only **partial** info |
| **③ 单维度 + 不全 cost** | "Patient complication rates vs operation volume" | Operation volume = **short-term cost only**（少 case → 少 revenue），不含 long-term cost benefits |
| **④ Compare quality outcomes to TOTAL costs ratio** ✅ | B 选项 — 正解 | Quality numerator + total cost denominator + per patient + entire course |

#### Single Metric Trap — Healthcare Quality 评估通用原则 ⭐

> [!danger] 任何单一 metric 都是 partial info
> - **Reoperation rate alone** = quality 一面，不知 cost
> - **Operation time alone** = cost 一面，不知 quality
> - **Length of stay alone** = cost-related，但若 patient discharged too early → ↑ readmissions（quality ↓）→ Balancing measure 需求（见 §12.2 Donabedian）
> - **Mortality alone** = outcome，但不 capture morbidity / satisfaction / cost
>
> **High-value care 评估必须同时看 quality + cost ratio**，不是单 metric 优化。

#### Cost Perspectives — 3 大视角（细节考点）

| Perspective | 关注什么 cost |
|---|---|
| **Patient** | Out-of-pocket + lost wages + caregiver burden |
| **Health care system** | Direct medical costs + administrative overhead |
| **Society** | Productivity loss + community-level impact |

CK stem 一般用 health care system perspective（hospital / payer）；偶尔考 patient OOP cost。

#### 与既有 §十二 节联动

```
§12.1 STEEEP（Healthcare quality 6 维）— Quality 定义
    │
    ▼
§12.2 Donabedian（5 类 measures）— Structural / Process / Outcome / Balancing / Composite
    │
    ▼
§12.4 Cost-conscious care — 避免 overutilization
    │
    ▼
§12.5 Benefit-cost analysis（BCA）— $ vs $ monetary terms
    │
    ▼
§12.8 Healthcare Value Formula ⭐ ← 这里
    │
        Quality（§12.1 STEEEP / §12.2 Donabedian outcomes）
    =  ──────────────────────────────────────────────────
              Total Costs（§12.5 包括 long-term）
```

#### 一句话锁

> [!success]
> 「**Value = Quality / Total Cost；单 metric 都是 partial info**」
> 「**Quality includes outcomes + safety + patient metrics；Cost includes TOTAL（long-term + short-term）**」
> 「**Long-term cost 常 offset short-term cost**（intraop pathology 例：减 reoperation ↓ long-term cost）」

---


---

### 13.12 Analysis Frameworks — RCA + Fishbone + 5 Whys + M&M + FMEA 升级 ⭐⭐

#### 13.12.1 RCA Process — 3 步（升级 §2.3）

1. **What happened?** — 描述 error 情境
2. **Why did it happen?** — 分析所有 risk factors / 系统 / 设备 / 环境
3. **What can be done to prevent recurrence?** — Update tech / double check / checklist / staff education

> [!info] RCA Overview + Principles 速记表（AMBOSS / v1.3.9 新增）⭐
>
> | 维度 | 内容 |
> |---|---|
> | **Overview & uses** | Retrospective + comprehensive + systematic error analysis tool；conducted **after sentinel event** or cluster of patient safety incidents |
> | **Principles** ⭐ | ① Uncovers **fundamental factors** leading to variations in performance + opportunities for error<br>② **Focuses on systems, NOT individual performance**（**no blame**）<br>③ Generates **action plan** for organizational process improvements |
>
> **Sentinel event 定义**：patient safety incident **unrelated to patient's underlying condition** → death / severe temporary harm / permanent harm

> [!success] Q18751 经典案例 — Wrong Patient Error (WPE) → Interprofessional Rounds ⭐（v1.3.9 新增）
>
> **Stem**：两 CAP patients in ICU + senior resident 同时管 + electronic order for IV vancomycin 给 **Patient B 而非 Patient A**（**WPE**）→ 2 天后 Patient B 急性肾损伤 → RCA → 哪个 change prevent future？
>
> **答案 = Daily team-based interprofessional rounds**（**C** ✓）
>
> **WPE 防错机制流程**：
> ```
> Senior resident enters order for wrong patient
>      │
>      ▼
> ① Pharmacist on rounds reviews order → 注意 patient B 不需 vancomycin
>      │
>      ▼
> ② Nurse on rounds 注意 medication change for B → 与既往评估不符
>      │
>      ▼
> ③ Team discussion → 早发现 + correct order
>      │
>      ▼
> Sentinel event prevented
> ```
>
> **反 pattern 4 类**：
> - ❌ A "Didactic training EMR"（knowledge OK 但 didactic inferior to hands-on；本题非 knowledge 缺口）
> - ❌ B "Time off + sleep breaks"（fatigue 非主因 — 错发生 at beginning of shift + 2 天 unnoticed 不解释 fatigue）
> - ❌ D "Fewer handoffs"（非 handoff 问题 — same resident throughout）
> - ❌ E "ID specialist verbal approval"（redundancy 但不解决 root cause = lack of team-based oversight；order 仍可到 wrong patient + remain undetected）
> - ✅ C "Interprofessional rounds"（直接 address suboptimal teamwork root cause）
>
> **典型 Sentinel Event 6 类**：WPE / wrong-site / wrong-procedure / Med error 致 harm / RSO / Patient suicide / Newborn abduction / Unanticipated death
>
> **反射钩**：见 "sentinel event + RCA + suboptimal teamwork as root cause" → 0.5 秒锁 **interprofessional rounds**（不是 didactic / 不是 fatigue / 不是 handoff / 不是 specialist approval）

#### 13.12.2 Fishbone (Ishikawa / Cause-and-Effect) Diagram ⭐⭐

**用途**：RCA 的**可视化工具**，把多 contributing factors 分类成 branches。

**步骤**：
1. 鱼头 = 问题
2. 主鱼骨 = 主要类别（People / Process / Equipment / Environment / Materials / Management）
3. 细鱼骨 = 各类细分因素
4. 视觉化 → 找 **multifactorial solutions**

#### 13.12.3 5 Whys Approach — 完整例子 ⭐⭐

**例**：病人给错药。

| Why | 问 | 答 |
|---|---|---|
| 1st | 为什么给错药？ | Nurse 没完成 patient identification |
| 2nd | 为什么 identification 不完整？ | 病人没 wristband |
| 3rd | 为什么没 wristband？ | Procedure 时取下没换 |
| 4th | 为什么没换？ | Wristband **printer 坏了** |
| 5th | 为什么 printer 坏？ | **IT 资源不足修不了** ⭐ ← Root cause |

> [!tip] 铁律
> Root cause 在**系统层 / 资源层**，**不停在 "nurse 粗心"**。

#### 13.12.4 FMEA — 7 步完整版（升级 §2.2 的 5 步）

| 步 | 内容 |
|---|---|
| 1 | Choose **specific system component**（如 medication administration）|
| 2 | **Process mapping**（每步骤画 flow）|
| 3 | Identify **failure modes**（可能错什么）|
| 4 | Identify **failure causes**（为什么会错）|
| 5 | Identify **failure effects**（错了的后果 + severity）|
| 6 | **Prioritize**（probability × severity 排序）|
| 7 | Implement **corrective measures proactively** |

#### 13.12.5 Morbidity and Mortality (M&M) Review ⭐⭐（新概念）

**定义**：**Retrospective peer review**，定期讨论 patient care errors / complications。

**特点**：
- Traditional：单科 + 关注 **individual actions**
- Modern ⭐：跨科 + 关注 **systemic causes**（不 blame 个人）
- **内容法律保护** — 多数州 inadmissible in malpractice lawsuits ⭐

> [!info] 4 大 Error Analysis Tools 区分（CK 名词配对）⭐⭐⭐（v1.3.4 升级为 4 工具）
> | 工具 | 时间方向 | 事件数 | 用途 |
> |---|---|---|---|
> | **RCA** | **Retrospective** | **单一 sentinel event** | 深挖一个事件的 underlying causes（active + latent factors）|
> | **FMEA** | **Prospective** | 新流程 / 新单位 | 预防多个 future potential vulnerabilities |
> | **Common Cause Analysis** ⭐ v1.3.4 | **Retrospective + aggregate** | **多事件**（机构层）| 找跨事件 **common themes + trends**（聚合多 RCAs）|
> | **M&M** | Retrospective | 周期性 + 多 case | Peer review 教育 + system-level improvements via interdisciplinary discussion |

#### 13.12.6 Process Mapping

**定义**：用 flowchart 把流程可视化 → 找问题节点。FMEA 第 2 步 + RCA 辅助工具。

#### 13.12.7 Common Cause Analysis ⭐⭐（v1.3.4 新增 — Q22581 锚定）

**定义**：**Retrospective + aggregate** analysis — 聚合机构内**多个 errors / 多个 RCAs** 的数据，找跨事件的 **common themes + trends + patterns**。

##### 与 RCA 的关键区别 ⭐

| 维度 | RCA | Common Cause Analysis |
|---|---|---|
| **范围** | **单一事件** 深挖 | **多事件聚合** 找模式 |
| **时机** | 触发：sentinel event 后 | 周期性 / 大量 errors 累积后 |
| **输出** | 这一个 event 的 underlying causes | 跨事件**共同主题**（如"夜班 fall 高发"/"某药 ADE 集中"）|
| **行动方向** | Fix this specific event 的 root cause | **System-level / institutional** priorities |
| **数据来源** | 单事件深度访谈 + 文档 | 多 RCAs 数据库 + incident reports 聚合 |

##### Stem 触发关键词

| Stem 元素 | 暗示 Common Cause Analysis |
|---|---|
| "**most common themes + trends**" across multiple errors | Common cause analysis（CK 经典 stem 语言）|
| "Aggregate data from multiple RCAs" | 同上 |
| "Identify which problems most frequently lead to errors" | 同上 |
| "Institution-level safety prioritization" | 同上 |

##### USMLE 高频陷阱

> [!warning] Common cause analysis vs 其他 3 工具区分
> - **"过去多事件 + 找 themes"** → Common Cause Analysis（不是 RCA — RCA 是单事件）
> - **"过去单事件 + 找 underlying causes"** → RCA
> - **"未来 potential vulnerabilities"** → FMEA
> - **"周期 peer review 多 case + 教育目的"** → M&M
>
> Q22581 stem 给"infusion pump errors"已发生**多次** + recommend RCA → 但 RCA primary purpose 仍是**这些 particular events** 的 underlying causes（不是跨所有未来事件的 vulnerabilities — 那是 FMEA；也不是跨所有事件的 themes — 那是 Common cause analysis）。

##### 4 工具决策树 ⭐

```
错误分析需求
    │
    ├─ 事件已发生（retrospective）？
    │    │
    │    ├─ 单一 sentinel event → 找具体 underlying causes
    │    │    → RCA（§13.12.1）
    │    │
    │    ├─ 多事件聚合 → 找跨事件 themes / trends
    │    │    → Common Cause Analysis（§13.12.7）⭐
    │    │
    │    └─ 多事件周期复盘 → 跨科 systemic improvements
    │         → M&M Review（§13.12.5）
    │
    └─ 事件未发生（prospective）→ 防 future vulnerabilities
         → FMEA（§13.12.4）
```

#### 13.12.8 RCA-FMEA 字眼陷阱反射钩 ⭐⭐⭐（v1.4 新增 — Q22581 + Q8-2026-05-27 第 3 次同型错驱动）⚠️⚠️

> [!danger] 反复错 #考前必看 + #难记 第 3 次错
> [[mistakes/uworld-mistakes_2026-05#^Q22581]] 字眼陷阱反复错（5-24 Q19553 + 5-25 入库 + 5-27 Q8 第 3 次同型错）。**字眼陷阱反射钩完全未建立** — 本节为最后强化。

##### 核心陷阱句式 ⭐⭐⭐

> [!warning] USMLE 出题人专门用 **FMEA 句式当 RCA 钓饵**
> 选项里看到 **"future" + "potentially cause" + "vulnerabilities"** 三连 = **FMEA 语言**。
> 如果 stem 是 retrospective（"errors HAVE occurred"），这种选项就是**钓饵**，不是 RCA 答案。

##### 字眼 → 工具识别表 ⭐

| 选项字眼 | 描述哪个工具 | 在 retrospective stem 里的角色 |
|---|---|---|
| "**future**" + "**potentially cause**" + "**vulnerabilities**" | **FMEA** 语言 | ❌ 钓饵（stem retrospective 时） |
| "**underlying causes**" + "**past events / have already occurred**" | **RCA** 语言 | ✅ 正解（stem retrospective 时） |
| "**aggregate patterns from multiple unrelated**" | **CCA** 语言 | 仅 stem 强调"multiple unrelated themes"时正解 |
| "**personnel responsible**" + remediation | **personnel-focused**（违反 RCA "no blame" 原则）| ❌ 永远错 |
| "**statistical likelihood**" / "**calculate probability**" | **risk modeling**（既不是 RCA 也不是 FMEA） | ❌ 干扰项 |

##### Stem 时间方向校验 SOP ⭐⭐⭐

```
Step 1: 扫 stem 找时间方向暗号
    │
    ├─ "errors HAVE occurred" / "resulting in harm" / "internal review identifies past errors"
    │     → ⭐ retrospective → 答案应描述 "past events underlying causes"
    │
    └─ "before operations begin" / "new unit / not yet opened" / "anticipate potential failures"
          → ⭐ prospective → 答案应描述 "future potential vulnerabilities"

Step 2: 扫选项找匹配描述
    │
    ├─ 找 "underlying causes" + "past / already occurred"
    │     → 这是 RCA 描述 → 若 stem retrospective → 选这个 ✓
    │
    ├─ 找 "future vulnerabilities" + "potentially cause"
    │     → 这是 FMEA 描述 → 若 stem prospective → 选这个 ✓
    │     → 若 stem retrospective → ❌ 钓饵，跳过
    │
    └─ 注意：RCA 也找 system-level latent factors，但**primary purpose 句式**必须用 "underlying causes of past events"，不是 "future vulnerabilities"

Step 3: 校验匹配 → 选答案
```

##### 类比 4 件套（钉死）⭐

| 工具 | 类比 | 适用场景 |
|---|---|---|
| **RCA** | **法医验尸** | 已死，查死因（单一事件 underlying causes）|
| **FMEA** | **工程师审图** | 还没造，找潜在缺陷（新流程 prospective vulnerabilities）|
| **CCA** | **法医统计办公室** | 多案聚合找全市模式（multiple events trends）|
| **M&M** | **科室病例讨论会** | Confidential 教育学习（peer review）|

##### 一句话锁 ⭐⭐⭐

- **"RCA = 已发生过去事件 underlying causes（过去 why）；FMEA = 未发生未来事件 potential vulnerabilities（未来 what could）"** ⭐
- **"选项里看到 'future' + 'potentially' + 'vulnerabilities' 三连 = FMEA 语言"** ⭐⭐⭐
  - 若 stem 是 retrospective（"errors HAVE occurred"）→ 这是钓饵
  - 若 stem 是 prospective（"new unit / not yet opened"）→ 这是正解
- **"RCA 也找 system-level latent factors，但 primary purpose 句式必须是 'underlying causes of past events'"** — 不能因为 RCA 也涉及 system 层就选 "future vulnerabilities" 描述

##### 每日浩斯宾前 10 秒默写（CK 救命）⭐⭐⭐

```
1. RCA = past underlying causes（单一事件 / retrospective）
2. FMEA = future potential vulnerabilities（事前 / prospective）
3. CCA = multiple aggregate themes（多事件聚合）
4. M&M = confidential interdisciplinary discussion（peer 教育）
5. 选项 "future + potentially + vulnerabilities" 三连 → FMEA 语言
6. 选项 "personnel responsible" → 违反 RCA no-blame 原则
7. Stem "errors HAVE occurred" + 选项 "future vulnerabilities" → ❌ 钓饵
```

##### 反 anchor 训练

- 见 stem **任何形态**前 — **先校验时间方向**：past 还是 future？
- 见选项**任何字眼** — **先匹配时间方向**：future vulnerabilities 字眼必须配 prospective stem
- **不字母 anchor / 不字眼 anchor** — 必须 stem 时间方向 × 选项字眼**双向校验**

> [!tip] 同型反 pattern 联动学习
> 本节字眼陷阱 + [[完整笔记/专题笔记/USMLE/USMLE_答案选项策略]] §二 Letter Anchor + §13.4 Cognitive Biases 是 USMLE 三大"反 pattern" 元方法 — 都教你**不被 surface feature 钓走**，永远回到 stem + 选项内容**双向校验**。

#### 13.12.9 Error Reporting Systems (ERS) — Effective Implementation + ERS vs RCA 边界 ⭐⭐⭐（v1.5 新增 — Q106640 锚定）

> [!info] ERS (Incident Reporting Systems / IRS) 与 §13.11 配套
> §13.11 是 IRS 基础概念；本节聚焦 **effectiveness 决定因素 (IRCSF)** + **ERS vs RCA 边界**（front-line vs external committee 分工）。

##### ERS 5 大 Effective Implementation Characteristics — IRCSF 缩写 ⭐⭐⭐

| 字母 | 特征 | 详解 |
|---|---|---|
| **I** ⭐ | **Investigation + response + feedback** | 每个 report 触发系统 investigation + 反馈给 submitter + transparency → 增 confidence + sustain reporting culture（Q106640 核心答）|
| **R** | **Report all front-line personnel** | Not only nurses + MDs — 包括 pharmacists / techs / housekeeping / transporters 等（CK 反 pattern 钓饵：限定 nurse + MD）|
| **C** | **Clear criteria for what to report** | 减 underreporting **near-miss events**（避免依赖 individual judgment）|
| **S** | **Safety from retribution** | Confidentiality + anonymity + focus on **systems** not individual mistakes |
| **F** | **Faster + simpler reporting process** | 减 time + effort → 增 submission rate |

##### ERS vs RCA 边界 ⭐⭐（关键边界）

| 工具 | 谁做 | 时机 | 内容 |
|---|---|---|---|
| **ERS submission** | **Front-line personnel** | 事件后立刻 | 简短描述 incident — 触发后续 investigation |
| **RCA** | **External committee（QI committee）** | ERS 触发后 OR sentinel event 后 | Multistep — collect data + causal flowchart + identify root causes + measure changes |

> [!danger] ❌ 反 pattern — Submit RCA with each ERS report
> 让 front-line submit RCA **错位**：
> - RCA 应 **external committee** 做（front-line 没 access to all data）
> - 增 reporter burden → **减 reporting rate** → ERS 失效

##### Near-miss Events 重要性（USMLE 高频）⭐

**Near-miss** = errors caught **before** causing patient harm（如 pharmacist intercept wrong med order before admin）。

**Near-miss reporting 是 ERS 核心价值**，但常被 underreport 因为：
- "No harm done" 心态 → 觉得不值得报
- 个人判断 → 不知道是不是 reportable

→ 必须 **clear criteria** (IRCSF 的 C) define 什么算 reportable + **culture** 鼓励上报 near-miss

##### ERS 反 pattern 5 类（CK 高频钓饵）⭐

| 反 pattern | 例 | 为什么错 |
|---|---|---|
| **① Add burden to reporters**（submit RCA）| Q106640 Choice A | RCA = external committee 工作；front-line submit RCA 增 burden → 减 reporting rate |
| **② Individual judgment for reporting**（无 clear criteria）| Q106640 Choice C | 导致 underreport **near-miss events** — near-miss 是 ERS 核心价值 |
| **③ Rely on ERS to identify most serious hazards** | Q106640 Choice D | ERS = qualitative + incomplete cross-section；适 identify **trends / patterns**，不是 picking 最 serious cases |
| **④ Limit to nurses + MDs only** | Q106640 Choice E | 应 encourage **ALL front-line personnel** — pharmacist / tech / housekeeping 等 |
| **⑤ No feedback to reporter**（缺 closure）| — | Reporter 看不到 outcome → 信心下降 → reporting rate 降 → ERS 失效 |

##### 一句话锁 ⭐

- **"ERS effectiveness = IRCSF（Investigation+response / Report all front-line / Clear criteria / Safety from retribution / Faster simpler）"** ⭐
- **"ERS = front-line submit 简短；RCA = external committee 做 multistep"**（分工边界）⭐
- **"Near-miss 是 ERS 核心价值；需 clear criteria 防 underreport"** ⭐
- **"ERS 不是 picking 最严重案例工具，是 trend identification 工具"** ⭐

##### 类比 — 餐厅意见箱

- **ERS** = 收集意见（submit）+ 餐厅每天读 + 写回复 + 改菜单（structured response + feedback）→ 顾客继续提意见
- **不读不回复** = 没人再提（ERS effective failure）
- **要求顾客写完整 RCA 分析** = burden 大 → 没人提（front-line 不该 submit RCA）

##### 与 §13.12.1-8 联动学习

| §13.12 工具 | 在 ERS 流程中的位置 |
|---|---|
| §13.12.1 RCA | ERS 报告触发后由 external committee 做 |
| §13.12.2 Fishbone | RCA 的视觉工具 |
| §13.12.4 FMEA | 与 ERS 互补 — ERS 看过去，FMEA 看未来 |
| §13.12.5 M&M | 跨多 ERS reports 的 case-based discussion |
| §13.12.7 Common Cause Analysis | 聚合多 ERS / RCAs 找 patterns |
| §13.12.8 RCA-FMEA 字眼陷阱 | 区分 ERS report 触发的 retrospective vs prospective 分析 |
| §13.12.9（本节）⭐ | ERS effectiveness 决定因素 + 与 RCA 边界 |


---

## 🔗 关联

- 🔁 **同主题错题**（聚焦 QI / Analysis Frameworks）：
  - [[mistakes/uworld-mistakes_2026-05#^Q22581]] RCA primary purpose 字眼陷阱（5-27 错 #考前必看 + #难记）
  - [[mistakes/uworld-mistakes_2026-05#^Q21477]] Swiss Cheese vs PDSA / Hard stop / Automation 4 大模型混（5-27 错 🔴）
  - [[mistakes/uworld-mistakes_2026-05#^Q19553]] FMEA prospective 详解
  - [[mistakes/uworld-mistakes_2026-05#^Q22359]] Donabedian 4 类 indicator CLABSI
  - [[mistakes/uworld-mistakes_2026-05#^Q106289]] / [[mistakes/uworld-mistakes_2026-05#^Q106290]] Variation Reduction Strategy
  - [[mistakes/uworld-mistakes_2026-05#^Q22780]] Healthcare Value = Quality/Cost Ratio
  - [[mistakes/uworld-mistakes_2026-05#^Q23111]] Stem 细节 Decisive vs 锦上添花
- 📚 **配套子文件**（拆分姐妹笔记）：
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Safety文化与沟通]]（防御层级 / Error 分类 / Safety Culture / Communication / Disclosure / IRS / SBT）
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Cognitive诊断错误]]（Cognitive Biases / Diagnostic Error Prevention / CDSS / Cognitive Overload）
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_HFE与药物HAC]]（HFE / Tall Man / Med Reconciliation / HACs / Surgical Safety / Patient-Centered Counseling）
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]]（主索引 + §九 EOL + §十 9 大陷阱 + §十一 Memory Hooks）
- 📚 **主笔记 / 跨学科**：
  - [[完整笔记/Peixuan分科笔记/Ethics_Master]]
  - [[完整笔记/专题笔记/感染/感染_CLABSI完整体系]]（§12.2.x Outcome 不变诊断顺序 Q22359 锚）
  - [[完整笔记/专题笔记/USMLE/USMLE_老年Fall3层防护]]（§13.9 HAC Falls 配套）
