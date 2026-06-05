---
tags:
  - USMLE-Step2
  - Ethics
  - Patient-Safety
created: 2026-05-27
type: 专题笔记
---

# USMLE_患者安全_Safety 文化与沟通

> [!info] 本笔记定位
> 从 [[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]] (原 v1.3.15 大文件) 拆出，专注 **防御层级 + Error 分类 + Safety Culture + Communication + Disclosure + IRS + SBT + Abuse Reporting + Stress 管理**。
> 4 子文件之一（另 3：[[完整笔记/专题笔记/USMLE/USMLE_患者安全_QI工具]] / [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Cognitive诊断错误]] / [[完整笔记/专题笔记/USMLE/USMLE_患者安全_HFE与药物HAC]]）。
> 主索引：[[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]]。

## §0 本文件目录

- §三 Patient Safety 防御层级（Swiss Cheese + Time-out 详解）
- §四 Error 分类与命名（5 大类 + Sentinel + Hazard/Risk + Adverse Event）
- §五 Safety Culture（Just Culture + Voluntary Reporting + Safety Epidemiology + Hand Hygiene Case + Just Culture 时序）
- §六 Communication Tools（SBAR + Closed-loop + Time-out + I-PASS + Collaboration + Psychological Safety 待加 B 增量）
- §七 Disclosure of Medical Errors
- §13.10 Initial Management + Disclosure SOP + Apologize 措辞
- §13.11 Incident Reporting Systems (IRS)
- §13.13 Simulation-Based Training (SBT)
- §13.14 Navigating Stressful Situations in Residency
- §13.15 Abuse Identification & Mandatory Reporting

---

## 三、Patient Safety 防御层级 — 强度梯队（核心 ⭐⭐⭐）

CK 反复考"哪个干预最有效" → 答案永远按这个梯队选**最高层**：

```
最强 ═════════════════════════════════════════════════════════ 最弱
  │
  ├── ① Forcing function / Hard stop（物理上不可能错）        ★★★★★
  │     例：氧气接口与氮气接口物理不兼容；infusion pump 强制上限
  │     Stem 关键词："prevent incorrect action by design"
  │
  ├── ② Automation（电脑自动算）                              ★★★★☆
  │     例：smart infusion pump 自动算剂量 + preset limits
  │     Stem 关键词："computerized algorithm" / "auto-calculation"
  │
  ├── ③ Standardization / Protocol / Checklist               ★★★★
  │     例：WHO surgical safety checklist / order set
  │     Stem 关键词："implement a standardized protocol"
  │
  ├── ④ Swiss Cheese Model — Overlapping barriers ⭐           ★★★★
  │     多层不完美防御叠加 → 漏洞错位则不会通过
  │     Stem 关键词："multiple layers" / "combination of barriers"
  │     Q21477 考点
  │
  ├── ⑤ Time-out / Universal protocol                        ★★★
  │     例：手术 / 高风险操作前暂停核对（patient + site + procedure）
  │     Stem 关键词："pause before procedure begins"
  │     Q106239 考点
  │
  ├── ⑥ Closed-loop communication                            ★★★
  │     接收者复述指令回去确认
  │     例："Give 5 mg morphine IV" → "Confirming 5 mg morphine IV"
  │
  ├── ⑦ Double-check / Independent verification              ★★
  │     两人独立核对（如 high-alert med 给药前）
  │
  ├── ⑧ Reminder / Alert / Pop-up                            ★★
  │     EHR 弹窗（容易 alert fatigue）
  │
  └── ⑨ Education / Training                                 ★
        培训永远是最弱的；CK "most effective" 题几乎不选
```

### 3.1 "Which is most effective?" 解题铁律

> [!danger] 铁律
> 1. 看选项 → 在梯队里找**最高层**的那个
> 2. 同一层级中：优先**物理 / 自动 > 人为流程 > 提醒 > 培训**
> 3. 遇到这些词优先选 **automation / forcing function**：
>    - medication overdose / dose calculation error
>    - look-alike / sound-alike drug
>    - wrong infusion rate
>    - prevent future errors

### 3.2 Swiss Cheese Model 详解 — Q21477 错题考点

**核心**：每层防御都有"洞"（vulnerabilities）— 但**叠加多层 + 洞错位** → 危险无法穿透。

```
hazard →  [██░██░██]  ← 防御层 1（如 hand hygiene，有洞）
          [██░░██░░]  ← 防御层 2（如 vaccination，有洞）
          [░██░██░░]  ← 防御层 3（如 PPE，有洞）
          [██░░░██░]  ← 防御层 4（如 ventilation）
                        ↓
                   ✗ 大多数 hazard 被挡住
                      （只有当 4 层洞对齐时才穿透）
```

**stem 模式**：
- 诊所同时上多个**互补**干预（口罩 + 手卫生 + 通风 + 疫苗 + 教育）
- 关键词：**"overlapping" / "multiple barriers" / "layers of defense"**

> [!warning] Swiss Cheese ≠ Forcing function
> - Swiss Cheese = **多层不完美防御叠加**
> - Forcing function = **单一物理 hard stop**（如氧气接口形状）
> - Q21477 (Choice B) 错答：clinic 没有物理 hard stop，只是叠加多层 imperfect 屏障

### 3.3 Time-out 详解 — Q106239 + Q107227 双锚

**核心**：操作 / 手术 / 关键步骤**正式开始前**全员暂停核对。

#### Time-out 3 大核心要素 ⭐⭐⭐（Q107227 锚定，v1.3.14）

```
Time-out（在 skin incision / 针刺前立即做）
    │
    ├─ ① Right Patient — Patient identity（≥2 identifiers — 姓名 + DOB / MRN）
    │      ✓ 不用床号 / 房间号（必须用不会变的 2 个）
    │
    ├─ ② Right Procedure — Type of procedure being performed
    │      ✓ "We are performing paracentesis on this patient"
    │
    └─ ③ Right Site — Site / Location（laterality + 解剖位置）
           ✓ 配 "YES + initials" site marking
```

#### Patient Safety Procedures 完整流程 ⭐

| 阶段 | 内容 | 时机 |
|---|---|---|
| **Preoperative verification** | Patient ID + operative site + procedure type + side（≥2 providers + patient/surrogate + 2 identifiers）| Preop holding area |
| **Site marking** | "YES" + initials on operative site（不 mark non-operative sites）+ permanent marker | 操作前任何时间 |
| **Time-out** ⭐ | 重新核对 patient ID + procedure + site + side + 团队全员参与 | **Immediately prior to skin incision / 针刺** |

#### 3 要素之外的信息归哪个流程 ⭐

| 内容 | 归哪个流程 | 不在 time-out 因为 |
|---|---|---|
| **Indication for procedure** | Informed consent | 与患者讨论时已完成 |
| **Medications taken** | Medication reconciliation | 早期评估 + 团队接班时完成 |
| **Names of team members + roles** | Team safety debriefings | Time-out 之前已熟悉 |
| **Potential complications** | Informed consent | 与患者讨论 risks 时完成 |

**适用场景（CK 高频）**：
- 手术开台前：核对 patient + site + procedure（防 wrong-site surgery）
- 手术 counting 前：让 surgeon 知道 nurse 要 count → 减少 interruption
- 高风险用药前
- **任何 invasive 操作**（paracentesis / LP / 中心静脉置管 / 关节注射）

**为什么 time-out 有效**：
1. 把所有人**注意力同步**到 safety 步骤
2. 提升 **situational awareness**（团队群体警觉）
3. 给低年资 / 护士**发声窗口**（不打断式提醒）

> [!tip] Memory Hook
> **"三 Right"**：Right Patient + Right Procedure + Right Site ⭐
> Time-out ≠ informed consent / med rec / debriefing 的替代 — 是**简短聚焦的 3 要素 safety check**。

> [!warning] Q106239 (Choice A) 陷阱
> RSO（retained surgical objects）成因 = **distraction / interruption / low situational awareness**，**不是** intimidation / authority 问题。
> - **Time-out（D）** 解决 awareness + interruption
> - **Authority/intimidation 培训（A）** 解决不存在的问题（团队问的是 tools / sutures，不是质疑权威）

---

## 四、Error 分类与命名

### 4.1 5 大 error 类型对比

| 名词 | 定义 | 例子 |
|---|---|---|
| **Active error** | 一线人员当场犯错 | 护士开错药 / 医生开漏剂量 |
| **Latent error** ⭐ | 系统潜伏漏洞（设计 / 排班 / 流程） | EHR UI 让两个药名看起来一样；连班 24 小时疲劳 |
| **Near-miss / Close call** | 差点出事但被拦下（**没**到病人身上） | Penicillin 过敏开方了 → 护士看到 allergy → 拦下 |
| **Adverse event** | 病人**真实受到伤害**（**可能** error 引起，**也可能不是**） | 化疗副作用（**不是** error）；给错药致死（**是** error） |
| **Sentinel event** ⭐ | 死亡 / 严重伤害 / 永久功能丧失 + **意外** | Wrong-site surgery / 自杀 / 弃婴；**必须** RCA + 上报 The Joint Commission |

### 4.2 Sentinel event 强制流程

**触发 sentinel event** → 6 步：
1. 立即稳定病人
2. **保留证据**（药瓶 / 设备 / 记录）
3. 通知风险管理 + 医务部
4. 启动 **RCA**（不是 FMEA）
5. **披露 (disclose)** 给病人 / 家属（按 Ethics_Master §七）
6. 上报 The Joint Commission（30 天内）

> [!tip] Slip / Lapse / Mistake（认知层面分类，偶尔考）
> - **Slip** = 行动失误（按错按钮）
> - **Lapse** = 记忆失误（忘记一步）
> - **Mistake** = 决策失误（用错诊断方法）

### 4.3 Hazard vs Risk vs Risk Factor — 三层定义 ⭐（AMBOSS 增量 v1.2）

CK 名词配对题。

| 术语 | 定义 | 例子 |
|---|---|---|
| **Hazard** | **Source** of potential harm（源头）| Incorrect medication dosage 本身是 hazard |
| **Risk** | **Probability** of harm 发生 + 程度 | 名字相似的两种药（**amiloride vs amlodipine**）比不相似的（ramipril vs amlodipine）confusion risk 高 |
| **Risk factor** | 增加 risk probability 的**变量** | Alert fatigue / Nursing staff interruption / 排班疲劳 |

### 4.4 Adverse Event 4 类完整分类（升级 §4.1）⭐⭐

| 类型 | 定义 | 例子 |
|---|---|---|
| **Preventable adverse event** | Adverse event **due to medical error** | 给过敏药因 allergy 信息**没记录在 chart** |
| **Ameliorable adverse event** ⭐（新名词）| **Unpreventable** adverse event but severity **could've been reduced** by specific actions | IV 浸润不可防，但因 **understaffing** 没及时发现导致 harm 加重 |
| **Potential adverse event (near miss)** | Medical error 可能造成 adverse event 但被**拦下** | Nurse 发现 incorrect order 在执行前 |
| **Never event / Sentinel event** | **严重 + 完全可防 + 不该发生** | Wrong-site surgery / wrong-patient / RSO / 设施内自杀 / 用 contaminated devices / 用错药 |
| **Adverse drug event (ADE)** | 药物相关 unintended harm | Medication error 导致 harm + 非预防性 ADR / drug withdrawal |

> [!danger] 关键区分
> - "Adverse event 都是 medical error 引起" ❌ — Adverse event **可能或可能不**是 error 引起（化疗副作用不是 error）
> - "Medical error 都造成 harm" ❌ — Error 是 action/failure，**不论是否 harm**（near miss 是 error 但无 harm）
> - "Ameliorable = preventable" ❌ — Ameliorable 是**不可防但严重度可降**（因 understaffing 发现晚 = ameliorable）

### 4.5 Medical Error 4 维分类（升级 §4.1）⭐⭐⭐

CK 高频"这属于哪类 error"配对题。

| 维度 | 类型 | 定义 | 例子 |
|---|---|---|---|
| **行为方向** | **Error of omission** ⭐ | **应做未做** | 没记录 allergy 史 → 给了过敏药 |
| | **Error of commission** ⭐ | **做了不该做的 / 做错** | 不必要手术 / SC 药改 IV 给 |
| **时间层级** | **Active error** | 一线人员当场 + immediate impact | 手术错部位 / 给药错路径 |
| | **Latent error** ⭐ | 系统**潜伏漏洞**（可能引发 active error）| **同包装药相邻摆放** / **understaffing** / 新设备未培训 |
| **责任层级** | **Individual error** | 单个 HCP 失误 | 医生开错剂量 |
| | **Systems error** ⭐ | 系统设计 / 流程 / 决策 / 资源失败 | 培训不足导致急救瓶颈 |
| **行动层级** | **Execution error** | **行动**失败（计划对，执行错）| 计划给正确药但剂量**写错** |
| | **Planning error** | **决策**失败（计划本身就错）| Prescribe **错药**（即使剂量准确） |

### 4.6 Specific Medical Error Types — 6 大具体类型 ⭐⭐（AMBOSS 增量 v1.2）

| 类型 | 含义 | 高频例子 ⭐ |
|---|---|---|
| **Communication error** | HCP-病人 / HCP-HCP 沟通失败 | 字迹不清 / 缺医学翻译 / **handoff 漏 vital info（lab 结果丢、discharge 没约 follow-up）** |
| **Diagnostic error** | Diagnosis 不准 / 不及时 / 沟通不到位 | 漏 imaging / 用过时检查 / 误读 lab / 没监测 clinical sign |
| **Laboratory error** ⭐ | Lab test 任一阶段失误 | **Preanalytical 占 75% ⭐⭐⭐**（hemolysis / 量不足 / 标错样本 / postprandial 抽空腹）/ Analytical（设备故障）/ Postanalytical（transcribing / misinterpretation）|
| **Treatment error** | 治疗错误 / 延迟 | 不必要操作 / 错剂量 / 错途径 / 延迟治疗 |
| **Preventive error** | 预防失败 | 错过 prophylaxis（HAI）/ 没 follow-up / 没维护设备 |
| **Medication error** | 给药全流程失误 | Prescription / **Transcription**（mistranscribing trailing zero 是经典例子）/ Dispensation / Administration / Reconciliation |

> [!tip] CK 高频考点
> - **Lab error 75% 在 preanalytical phase** — stem 暗示"specimen contaminated / mislabeled / wrong tube" → 选 preanalytical
> - **Trailing zero**（5.0 mg 看成 50 mg）— 经典 transcription error

---

## 五、Safety Culture

### 5.1 Just Culture（公正文化）⭐

**核心三层**：
1. **Human error** → 安慰 + 系统改造（不惩罚）
2. **At-risk behavior**（走捷径但没恶意）→ 教育 + 流程改进
3. **Reckless behavior**（明知故犯）→ 惩戒

**为什么重要**：鼓励 voluntary reporting → 早发现 latent error。

> [!warning] 反 pattern
> - "护士开错药 → 立即开除" ❌ — Just culture 不惩罚 human error
> - "我们是 blame-free culture，从不惩戒" ❌ — Reckless behavior 仍要惩戒
> - "上报 error 会被记录考核" ❌ — Non-punitive reporting 才有效

#### 5.1.1 Just Culture 3 大 Behavior Categories — 决策树 + 暗号词配对 ⭐⭐⭐（v2.1 增量 — Q126013 锚定）

> [!danger] 上层§5.1 只讲总框架；本子节深化 3 categories sub-classification 决策点 — Q126013 错点正在此层

##### 3 类 Behavior 完整对照表 ⭐

| 维度 | **Human Error** | **At-risk Behavior** ⭐ | **Reckless Behavior** |
|---|---|---|---|
| **性质** | **Unintentional slip / mistake** | **Conscious shortcut / workaround** | **Conscious disregard** |
| **Behavior 触发** | 人在 following expected steps 时 slip | 知道协议但 skip — **system 压力 + 不完全 appreciate risk** | 明知违规 + **无 legitimate rationale** |
| **意图** | 无意（inadvertent）| 有意（drift from safe practice）但有"理由" | 有意 + 故意冒险 |
| **Response** | **Consoling**（reassurance + counseling）| **Coaching** ⭐ + **同时改 system conditions** | **Sanctioning**（discipline）|
| **同时做什么** | 改 system design（防再发生）| 改 system conditions（防再发生）| 个人责任为主，系统次要 |

##### 3 类 Stem 暗号词 → Response 配对 ⭐⭐⭐

| Stem 暗号 | Behavior Category | Response | 例 |
|---|---|---|---|
| "**unintentional slip**" / "**inadvertent**" / "flipping wrong switch due to poor labeling" / "following all expected steps but error" | **Human Error** | **Consoling** | 累 nurse 给 0.1 mL 误输 1 mL — slip |
| "**skips when busy**" / "**workaround**" / "shortcut" / "drift from safe practice" / "**system pressure**" / "**no prior disciplinary history**" + conscious | **At-risk Behavior** ⭐ | **Coaching** + 同时改 system ⭐ | Q126013: nurse "skips 2nd ID check when busy" + staffing shortage + 9hr no break |
| "**conscious disregard**" / "**no legitimate rationale**" / "**repeated violation despite warnings**" / "intentional risk-taking" + prior disciplinary | **Reckless Behavior** | **Sanctioning** | 反复 hand hygiene 拒做 + 被警告多次 |

##### 决策树（识别 behavior category）⭐

```
Error 发生 → 判断 behavior category：
    │
    ▼
是 unintentional slip / mistake？（人在 following expected steps 时 slip）
    │
    ├─ ✓ Yes → **Human Error** → **Consoling** + 改 system design
    │
    └─ ❌ No, 是 conscious choice
           │
           ▼
       有 legitimate rationale (system pressure / time / resource)？
           │
           ├─ ✓ Yes（system pressure + 不完全 appreciate risk + no prior disciplinary）
           │     → **At-risk Behavior** → **Coaching** ⭐ + 同时改 system conditions
           │
           └─ ❌ No legitimate rationale（明知 + 故意 + 通常 repeated pattern）
                 → **Reckless Behavior** → **Sanctioning**
```

##### Q126013 4 信号识别 At-risk Behavior（停在 coaching 不升 sanctioning）⭐

| Stem 信号 | 解读 |
|---|---|
| "states she **skips when busy**" | **Conscious choice**（不是 inadvertent slip）→ 排除 human error |
| "**covering 2 bays + staffing shortage + no break 9 hr**" | **System pressures present**（legitimate rationale）→ 排除 reckless |
| "**No prior disciplinary history**" | 不符合 reckless behavior pattern（reckless 通常 repeated）|
| "Verified med against order **BUT** 没做 second ID check" | Drift from safe practice — 知道步骤但 shortcut → At-risk |

→ 4 信号都指向 **At-risk Behavior → Coaching**

##### 反 pattern 警示 ⭐

| 误判 | 为什么错 |
|---|---|
| "Skips when busy" → Human error | ❌ Conscious shortcut ≠ inadvertent slip — slip 必须是按步骤做但 slip |
| "Skips protocol" → Reckless | ❌ 有 system pressure + no prior disciplinary → 不达 reckless（reckless 要 no legitimate rationale + 通常 repeated）|
| "Knew protocol but skipped" → Retraining | ❌ 已 know — 不是 knowledge gap；是 conscious shortcut → coaching |
| "Coaching = soft / 不问责" | ❌ Coaching ≠ no action — coaching 是 individual accountability 的低强度形式（vs 无 action）|
| "At-risk → 改 system 就够，不 coach" | ❌ 必须 **同时** coach + 改 system — 仅改 system = no-blame culture（也错）|

##### 联动 §5.4 时序原则 + §6.6 Psych Safety

- **§5.4 时序原则**：Systems first → Individual accountability。**Coaching at-risk behavior 属 individual accountability 层**（在 systems 已 reform 后）
- 但本题 stem 是 **single incident**（不是 sustained interventions 后仍 suboptimal）→ 因此**同时**改 system + coaching，不是先改 system 再 coaching
- **§6.6 Psych Safety** ✓ — Coaching 必须在 psych-safe 环境进行（reporter 不怕被罚）

##### 类比 — 开车超速

| 情景 | Category | Response |
|---|---|---|
| Slip 踩错油门（按步骤做但 slip）| Human error | Consoling + 改 system（pedal 设计 / 车道辅助）|
| 明知限速 80 但赶时间开 100（有 system pressure 如赶飞机）| **At-risk** ⭐ | **Coaching**（讨论 risk）+ 同时改 system（更好的 GPS / 公司加班政策）|
| 明知限速 80 + 无任何理由飙 150 + 之前已多次违规 | Reckless | Sanctioning（吊销驾照）|

##### 一句话锁 ⭐⭐⭐

- **"Inadvertent slip → Human error → Consoling"**
- **"Conscious shortcut + system pressure → At-risk → Coaching + 同时改 system"** ⭐
- **"Conscious disregard + no rationale → Reckless → Sanctioning"**
- **"Coaching ≠ no action；Coaching ≠ Retraining；Coaching = individual accountability 低强度形式"**

#### 5.1.2 两两区分 drill-down + 反例对照 ⭐⭐⭐⭐（v2.2 增量 — 用户看不懂边界 5-27 实战警示）

> [!danger] 用户看 §5.1.1 仍卡在"3 类边界到底怎么分"
> 上层 §5.1.1 给了 3 类对照表 + 决策树 + 暗号词配对；但实战中**两两边界**仍易混。本节做 3 对 pairwise drill-down + 反例对照，强化边界反射。

##### 5.1.2.1 Pair 1 — Human Error vs At-risk Behavior（**最难** — Q126013 错点）⭐

**关键问题**：**"她是 slip 还是 skip？"**

| 维度 | **Human Error (slip)** | **At-risk Behavior (skip)** ⭐ |
|---|---|---|
| **她当时在做什么？** | 在**按步骤做**，但某一步出错 | **跳过一步**，知道但选择不做 |
| **她事后会怎么描述？** | "我也不知道怎么回事，就**突然按错**了" | "**当时太忙了，那一步通常我会跳过**" |
| **再训练有用吗？** | ❌ 没用（slip 是 human 本能 — 训练 10 次仍会 slip）| ✅ 有用一部分（让她 appreciate risk + behavior change）|
| **是否 conscious？** | ❌ Unintentional / 无意识 | ✅ Conscious choice |
| **代表 case** | Vincristine 罐子像 Vinblastine（poor labeling）拿错 | Q126013 nurse skips 2nd ID check when busy |

###### 反例对照（同一 outcome 不同 category）

| Stem 句式 | Category |
|---|---|
| "我**其实记得**做了 2nd ID check，但**意识不清楚**点错了 patient" | **Human Error**（slip — 在按步骤做但 slip）|
| "I **skip** second ID check **when busy**"（Q126013 实际句式）| **At-risk**（conscious skip）⭐ |
| "Verified med against order **but did not perform** second ID check" + 自述 skips when busy | **At-risk** — 不是 slip 是 conscious shortcut |

###### 反射钩

> 见 nurse 自述 "**通常**会 skip / **when busy** 会 skip / **routinely** 简化某步骤" → **0.3 秒锁 At-risk**（不是 Human Error）

---

##### 5.1.2.2 Pair 2 — At-risk vs Reckless Behavior（**次难**）⭐

**关键问题**：**"她有没有 legitimate rationale？"**

| 维度 | **At-risk** ⭐ | **Reckless** |
|---|---|---|
| **System pressure?** | ✅ 有（赶 / 累 / 资源不够 / staffing shortage）| ❌ 没有 |
| **她是否觉得"应该没事吧"？** | ✅ 是（**不完全 appreciate risk**）| ❌ 明知 risk + 故意冒险 |
| **Prior disciplinary?** | 通常**无** | 通常**有**（reckless 是 **repeated pattern**）|
| **Behavior 强度** | Drift from safe practice（慢慢偏离）| Outright violation（公然违规）|
| **自述** | "I skip when busy" / "I take shortcuts to save time" | "I don't believe in this protocol" / "Alerts are annoying" |

###### Q126013 判定关键（4 信号都指 At-risk 不升 Reckless）

| 信号 | 排除 Reckless 的逻辑 |
|---|---|
| ✓ Staffing shortage + 9 hr no break + 2 bays | **System pressure 满满** → 不是 reckless（reckless 无 rationale）|
| ✓ No prior disciplinary history | **不是 repeated pattern** → 不是 reckless |
| ✓ 她说"too busy"，不是"我就是不想做" | **不是故意冒险** |
| ✓ Similar surnames + adjacent beds | **System design 差**也分担责任 |

→ 停在 **At-risk**，**不升 Reckless**

###### 反例对照（同一 nurse 同一 outcome 不同 category）

| Stem 句式 | Category |
|---|---|
| Q126013 原句式（staffing shortage + no prior history） | **At-risk** |
| "Nurse 之前已 **3 次** skip ID check 被警告 + 同事提醒 + **今天 staffing 正常** 但她仍 skip + 自述 'I don't think it's necessary'" | **Reckless** |
| "Nurse 第一次 skip + staffing 正常 + 但坚持 'I trust my visual recognition more than the protocol'" | **介于** — 倾向 Reckless（无 legitimate rationale）|

###### 反射钩

> 见 "**no prior disciplinary**" + "**system pressure 存在**"（staffing / fatigue / shortage）→ **0.3 秒判断 At-risk，不升 Reckless**

---

##### 5.1.2.3 Pair 3 — Coaching vs Retraining vs Sanctioning（3 个 response 边界）⭐

这 3 个 response **都涉及个人责任**，但**强度和性质不同**：

| Response | 何时用 | 做什么 | 用错的反 pattern |
|---|---|---|---|
| **Consoling** | Human Error | **情绪 reassurance** + 修 system design | 用在 conscious skip = no action 反 pattern |
| **Coaching** ⭐ | At-risk Behavior | **讨论 risk + behavior change**（不是单纯训练知识）+ **同时**修 system conditions | 用在 reckless = 过软；用在 human error = 过严 |
| **Retraining** | **Knowledge gap**（如新员工 / 不知道协议） | 教会**知识 / 技能** | 用在 At-risk（明知协议）= 错位 — Q126013 D 钓饵 ⚠️ |
| **Sanctioning** | Reckless Behavior | **Discipline**（warning → suspension → license review）| 用在 At-risk（有 system pressure）= 过严 — Q126013 E 钓饵 |

###### 为什么 Q126013 D (Retraining) 错 ⚠️

- Nurse **已知**协议（自述 "skip when busy" = 她**知道**该做 2nd ID check）
- Retraining 是 "**不知道**怎么做" 时的 response → **不适用于"知道但 skip"**
- 这是经典 USMLE 钓饵 — **"反复训练"**听起来"严谨"但**错位**

###### 为什么 Q126013 E (Sanctioning) 错 ⚠️

- Reckless 要求 **no legitimate rationale + 通常 repeated**
- Q126013 有 staffing shortage + 9 hr no break + no prior disciplinary → **不达 reckless 标准**
- Sanctioning at-risk → 反向 trigger fear / 藏错 → 回到 Blame Culture

###### Coaching 不是"Soft Consoling" — 关键区分 ⭐

| 维度 | Consoling | Coaching |
|---|---|---|
| **重点** | 情绪 reassurance（"你没事吧？"） | **Behavior change conversation**（"你为什么 skip？let's discuss risk + next time strategy"）|
| **有问责性？** | ❌ 无（纯安慰）| ✅ 有（individual accountability 低强度形式）|
| **要求改变？** | ❌ 不要求（system 改即可）| ✅ 要求 nurse 改变 behavior + 同时改 system |
| **何时用** | Human Error（slip 不可控）| At-risk（drift 可纠正）|

> [!warning] Coaching ≠ no action
> Coaching **是个人问责的开始** — 不是"安慰一下就过"。Just Culture 仍要求 individual accountability，只是 At-risk 的问责形式是 **conversation + behavior change**，不是 discipline。

###### 反射钩

> - 见 "nurse 知道协议但 skip" → **Coaching**（不是 Retraining）
> - 见 "system pressure + no prior history" → **Coaching**（不是 Sanctioning）
> - 见 "inadvertent slip" → **Consoling**（不是 Coaching — Coaching 暗含 conscious behavior 要改）
> - 见 "no rationale + repeated violations" → **Sanctioning**（不是 Coaching — coaching 不够）

---

##### 5.1.2.4 决策树完整走一遍 — Q126013 实战 ⭐⭐⭐

```
Q126013: Nurse gives wrong medication
    │
    ▼
Step 1: 她是 unintentional slip 吗？
    │
    问：她事后是说"我不知道怎么回事突然 slip"还是"我太忙时通常 skip"？
    │
    答：她说 "I skip second ID check when busy"
    │
    → 这是 CONSCIOUS SKIP，不是 slip
    │
    → 不是 Human Error
    │   不是 Consoling（C 钓饵）❌
    │
    ▼
Step 2: 她有 legitimate rationale 吗？
    │
    问：有 system pressure（赶 / 累 / 资源不够）吗？她是否之前已多次违规？
    │
    答：
      ✓ Covering 2 bays（staffing shortage 资源不够）
      ✓ 9 hours no break（累）
      ✓ Similar surnames + adjacent beds（system design 差）
      ✓ No prior disciplinary history（不是 repeated）
    │
    → 有 system pressure + 不是 repeated 违规
    │
    → 不是 Reckless（如果是 reckless 应该 no rationale + repeated）
    │   不是 Sanctioning（E 钓饵）❌
    │
    ▼
Step 3: 她知道协议吗？
    │
    答：知道（自述 "skip when busy" = 知道该做 2nd ID check 但选择跳过）
    │
    → 不是 knowledge gap
    │   不是 Retraining（D 钓饵）❌
    │
    ▼
Step 4: 最终判定 — At-risk Behavior ⭐
    │
    → Response: **Coaching**（A 正解）✅
    │
    → 同时改 system conditions：
        ├─ 改善 staffing（不再让她 cover 2 bays）
        ├─ 强制 break（9 hr no break 不允许）
        ├─ EHR 弹窗 "Same surname alert"
        └─ Bed 编号系统让相邻床不同色
```

##### 5.1.2.5 5 选项陷阱总结（Q126013 完整 mapping）

| 选项 | 用在哪个 category 才对？ | Q126013 钓在哪？ |
|---|---|---|
| **A. Coaching, at-risk driven by system pressures** ⭐ | At-risk Behavior | ✅ **正解** |
| B. No action, system alone responsible | **没有任何 category 应该 no action** — 任何 conscious action 都需个人责任介入 | No-blame culture 反 pattern |
| **C（我选的）. Reassuring, human error in unsafe system** | Human Error（slip）| ❌ 把 conscious skip 误当 slip — 没识别 "skips when busy" 是 conscious choice |
| D. Retraining, knowledge deficit | Knowledge gap（新员工 / 罕见病 / 不知道协议）| ❌ Nurse **已知**协议（自述）— 不是 knowledge deficit |
| E. Sanctioning, protocol violated regardless of context | Reckless Behavior（no rationale + repeated）| ❌ 有 system pressure + no prior history → 不达 reckless |

##### 5.1.2.6 最终 3 句话锁死 ⭐⭐⭐

> [!success] 最高优先一句话锁
> - **"Slip = Human Error → Consoling"** — 按步骤但 slip
> - **"Skip with reason = At-risk → Coaching + 同时改 system"** — 明知 skip + 有 system 压力 ⭐
> - **"Skip without reason = Reckless → Sanctioning"** — 明知 skip + 无理由 + 通常反复

### 5.2 Non-punitive Voluntary Reporting

- 上报系统**匿名 + 不惩罚** → 才有人报
- **Anonymous reporting** 不等于 **confidential reporting**（前者无名，后者有名但保密）
- 数据用于 **system-level improvement**，不用于个人考核

### 5.3 Patient Safety Epidemiology ⭐⭐（AMBOSS 增量 v1.2）

CK 高频背景统计（题干常用 "given that medical errors are a leading cause of death..."）：

- 全球 ~**5%** of patients experience preventable harm
- 医院 ~**10%** adverse events，**~half preventable**
- **Medical errors = 3rd leading cause of death in US ⭐⭐⭐**
- ~**250,000 deaths/yr** in US（前两位：心血管 + cancer）

> [!info] CK 用法
> 这个数据用来论证 **patient safety 的 system-level 改造紧迫性** — 题干常以此引出 "which strategy most effectively reduces medical errors?" → 答案永远是**系统改造**（forcing function / standardized protocols / safety culture / incident reporting）— **不是** "individual blame / education"。

### 5.4 Hand Hygiene Compliance Case Study + Just Culture 时序原则 ⭐⭐（v1.3.6 新增 — Q106042 锚定）

#### 反射钩

> [!info]
> Hand hygiene compliance / 类似 protocol adherence 持续 suboptimal → 反射顺序：**① 先 systems intervention**（sinks placement / training / monitoring / signage / staff input）→ **② 系统改造已 sustained + comprehensive → 仍 suboptimal → 转 individual accountability + organizational culture**（"just culture"）。
> ❌ 不能跳过 systems 直接 individual punitive（损 morale + culture of fear）。

#### Improving Hand Hygiene Compliance — 4 大 Reasons + Solutions（AMBOSS 完整表）⭐

| Reason for noncompliance | Example solution |
|---|---|
| **Ineffective placement of sinks & dispensers** | Place sinks/dispensers **outside each patient's room** |
| **Lack of accountability** ⭐ | Build hand hygiene into **provider evaluations** |
| **Lack of safety culture** | Create safety teams + provide **real-time feedback** on compliance |
| **Forgetfulness or lack of time** | Place **visual cues** (signs / red arrows) near doorways |

#### Hand Hygiene 重要性 — 必背数据

> [!tip] Hand hygiene 临床效益
> Hand hygiene = **最便宜 + 最有效**的感染控制干预（§8.4）。Reduces incidence of **preventable hospital-associated infections (HAIs) by up to 70%**。
> 但 despite evidence base，physician adherence **often remains low**（<30% in Q106042 case）。

#### Just Culture 时序原则 ⭐⭐⭐（核心 takeaway）

```
Step 1: Systems Interventions（First step + 持续 + comprehensive）⭐
    ├─ Optimizing physical environment（额外 sinks / dispensers）
    ├─ Ensuring staff knowledge + preparation（training）
    ├─ Engaging staff in organizational improvement（staff input）
    ├─ Installing transparent monitoring system（video surveillance）
    └─ Signage + visual cues
    │
    ▼ 已 sustained + comprehensive 但仍 suboptimal
    │
Step 2: Strengthen Individual Accountability + Organizational Culture ⭐
    ├─ Build compliance into provider evaluations
    ├─ Disciplinary measures for repeated transgressions
    │      （warning note → remedial training → 更进一步）
    ├─ Real-time peer feedback
    └─ 称为 "just culture"
```

> [!danger] 时序铁律
> **Step 2（individual accountability）只在 Step 1（sustained, comprehensive systems reform）之后才能启动**。直接跳到 punitive measures = **culture of fear** + 损 reporting + 损 trust。

#### 3 种医院文化 Spectrum ⭐⭐（v1.3.11 追加 — 为什么这个时序）

```
Blame Culture          Just Culture ✅          No-Blame Culture
（恐惧文化）           （平衡文化）             （无责文化）
   │                        │                        │
出错就罚人            系统 + 个人 双层管           错了也不查
   ↓                        ↓                        ↓
医护藏错不报          系统改完后再问个人责任       反复同样错误
医疗安全反而下降      患者安全持续提升              没改进动力
```

**核心理念**：错误大部分是 **system design** 的问题，少部分才是 **individual responsibility**。所以处理顺序必须**系统先 → 个人后**。

#### Just Culture 公平在 4 处（为什么叫 "Just"）⭐

| 公平在哪 | 具体表现 |
|---|---|
| **对系统公平** | 先认系统责任（修 sink / 装监控 / 培训）— 不甩锅给个人 |
| **对个人公平** | 系统都给你修好了，你还不做 = 你的责任，**这时候问责才合理** |
| **对患者公平** | 错误能被上报 + 调查 + 改进，安全持续提升 |
| **对错误态度公平** | Honest mistake（一时疏忽）≠ Reckless behavior（明知故犯）— **区别对待** |

#### 视觉 Hook — "先修路，再问司机" ⭐⭐⭐（v1.3.11 用户视觉钩）

| 角色 | 对应 |
|---|---|
| **修路** | Systems interventions（装 sink、培训、监控、signage） |
| **问司机** | Individual accountability（路修好你还违章 = 该罚） |
| **跳过修路直接罚司机** | Culture of fear ❌ |
| **路修好但永远不罚** | No-blame culture ❌ |
| **先修路 → 阶梯式问责** | **Just Culture** ✅ |

#### Q106042 4 大反 pattern 分析

| 反 pattern | 例 | 为什么错 |
|---|---|---|
| **① Cognitive bias + judgment errors** | A 选项 | Cognitive bias 是 **mental shortcuts in clinical decision-making**（如 diagnostic errors），**不**适用 simple safety action 如 handwashing |
| **② Knowledge deficiencies + organizational awareness** | C 选项 | Healthcare providers **generally aware** of hand hygiene importance；organization 已 extensive training；不是 knowledge 缺 |
| **③ Teamwork training + communication** | D 选项 | Teamwork training reduce medical errors，**但 handwashing 是 individual action**，常发生 in team members absent 时；individual accountability 才是核心 |
| **④ Individual accountability + organizational culture** ✅ 正解（B 选项）| Systems reform 已 sustained，问题在 individual physician adherence 反复 lapse → just culture 时序到位 |

#### 一句话锁

> [!success]
> 「**Hand hygiene compliance Step 1 = systems；Step 2 = individual accountability（only after sustained systems reform）**」
> 「**Just culture 不是 culture of fear — 但 systems 都做完仍 suboptimal 时，要 accountability**」

---

## 六、Communication Tools

### 6.1 SBAR — 标准化沟通框架

| 字母 | 含义 | 例子（电话给上级） |
|---|---|---|
| **S**ituation | 我是谁 + 病人是谁 + 现在发生什么 | "I'm Dr. Li, calling about Mr. Smith in Bed 5, who just developed acute chest pain." |
| **B**ackground | 相关病史 + 当前用药 + 最近事件 | "70 yo male, POD 2 from CABG, on heparin." |
| **A**ssessment | 我觉得是什么 / 担心什么 | "I'm concerned for PE vs MI." |
| **R**ecommendation | 我建议什么 / 需要什么 | "Can you come evaluate now? I'll order ECG + troponin." |

**用途**：交接班 / 紧急上报 / 跨科咨询。

### 6.2 Closed-loop Communication

**3 步循环**：
1. **Sender** 给指令 → 用病人姓名 + 具体剂量 / 操作
2. **Receiver** 复述回去（"Confirming...")
3. **Sender** 确认 / 纠正（"Correct" / "No, I said...")

**stem 触发**：复苏 / 操作室 / 紧急情境下 verbal order。

### 6.3 Time-out / Universal Protocol

详见 §3.3。WHO 推 + The Joint Commission 强制要求。

### 6.4 I-PASS — 住院医交接框架

| 字母 | 含义 |
|---|---|
| **I**llness severity | 病情严重度（stable / watcher / unstable） |
| **P**atient summary | 病人简介 + 当前问题 + 治疗 |
| **A**ction list | 接班者要做的具体事项 |
| **S**ituation awareness + contingency | 可能恶化的情景 + 应对预案 |
| **S**ynthesis by receiver | 接班者复述确认 ⭐（防漏） |

> [!tip] CK 高频
> Handoff = "最危险时刻" — 60% 医疗错误发生在 transition of care。**I-PASS 减少 handoff error 30%。**

#### 6.4.1 Reducing Errors in Patient Handoffs — 3 大优化 + 6 Best Practices ⭐⭐⭐（v1.3.9 新增 — Q21520 锚定）

Verbal handoffs (sign-outs) → adverse events 风险 ↑（especially with **many patients + high acuity**）。AMBOSS / Joint Commission 推荐 3 大优化方向：

| 优化维度 | Best practices |
|---|---|
| **Optimize information** ⭐ | ① **Discuss highest-acuity ("sickest") patients first**（Q21520 答案 ⭐）<br>② Provide extra detail on critical patients<br>③ Avoid information overload |
| **Optimize communication** | ① Follow template (eg, checklist / I-PASS / SBAR)<br>② Include **oral + written** communication<br>③ Encourage questions **throughout discussion**（不是 only at end）<br>④ Use **read-back selectively**（eg, for to-do items — closed-loop）|
| **Optimize actions** | ① Include follow-up items (to-do list)<br>② Provide **anticipatory guidance** (eg, "if/then" format — "如果 BP < 90 → 给 vasopressor") |

#### 6.4.2 Handoff 3 反 pattern（CK 高频）⭐

| 反 pattern | 例 | 为什么错 |
|---|---|---|
| **① Questions only at end** | Q21520 选项 A | 增加 rushing / forgetting 风险；应 **throughout discussion** encourage |
| **② Discourage note-taking** | Q21520 选项 C | Note-taking **应 encouraged** — emphasize + reinforce critical info |
| **③ Exhaustive details on every patient** | Q21520 选项 D | Info overload — 应 prioritize by acuity，**extra detail only on critical patients** |

#### 6.4.3 Selective Read-back vs Universal Read-back 区分 ⭐（v1.3.9 — Q19684 + Q21520 串联）

| 应用 | 场景 | 例 |
|---|---|---|
| **Selective read-back**（Q21520）| Handoff 中**只对 critical info / to-do items** 做 read-back（防 info overload）| Handoff "若 K+ < 3.5 给 oral KCl"（critical to-do）→ 接班者 read-back |
| **Universal read-back**（Q19684）| **Verbal order 每条都 read-back**（防 medication error）| "Give 20 mEq oral potassium" → 接班者 "Confirming 20 mEq oral potassium" 全条复述 |

> [!success] 一句话锁定
> **"Handoff 4 字诀：Sickest first + 减 overload + selective read-back + if/then anticipatory"** ⭐
> **"Selective read-back (handoff to-do) vs Universal read-back (verbal order) — 两者都是 closed-loop 但应用不同"** ⭐

### 6.5 Collaboration and Teamwork 框架 ⭐（AMBOSS 增量 v1.2）

**核心**：Teamwork = healthcare quality + safety 基础（被 ABMS 列入医生 evaluation 标准 — collaboration 是 "professional expectation"）。

#### 6.5.1 5 大 Domains（AMBOSS 框架）

```
1. Communication           ← §6.1-6.4（SBAR / Closed-loop / Time-out / I-PASS）
2. Teamwork & mutual support  ← §6.5.3
3. Leadership              ← §6.5.4
4. Situation monitoring    ← §3.3 Time-out 的 situational awareness
5. Conflict resolution
```

#### 6.5.2 Nonviolent Communication (NVC) — Marshall Rosenberg ⭐

**目标**：通过 empathy + awareness 改善沟通，避免 coercive / manipulative 表达。

**4 components**：
- **Observation**（陈述事实，不带评价）
- **Feelings**（表达情绪）
- **Needs**（潜在需要）
- **Requests**（具体请求）

**3 modes**：Self-empathy / Honest expression / Empathetic reception

**相关原则**：
- **Cultural humility** — 开放尊重他人文化身份
- **Active listening** — 言语 + 非言语 cue + paraphrasing 回应
- **Information sharing** — 主动确保信息完整

#### 6.5.3 Teamwork and Mutual Support

**Interprofessional vs Intraprofessional team** ⭐：
- **Interprofessional**：不同 background 协作（医生 + 护士 + 物理治疗师 / surgeon + 麻醉 + 放射）
- **Intraprofessional**：同一 background（一组物理治疗师）

**Core competencies**：
- Shared belief in teamwork（collective intelligence + synergy）
- **Psychologically safe environment** ⭐⭐ — 允许 verbalize ideas / concerns / mistakes / questions **without fear of negative consequences**
- Effective communication（SBAR / check-back）
- Optimization of team dynamics（Coordination + Cooperation + Shared decision-making）
- Reflection（debriefing post-event）

#### Features of Effective Teams in Health Care — 6 元素表 ⭐⭐⭐（v1.3.3 + v1.3.9 双锚定 — Q19739 + Q23112）

| 元素 | 核心要素 |
|---|---|
| **Safety culture** | Resource commitment to safety |
| **Collaboration** ⭐ | **Shared understanding & prioritization of goals**（Q23112 锚定）/ **Distinct roles that avoid a steep hierarchy** ⭐ |
| **Psychologic safety** ⭐ | Asking questions & voicing concerns encouraged / **Avoiding blame or retaliation** |
| **Responsiveness** | Feedback respected & promptly acted on |
| **Situational awareness** | Persistent mindfulness & safety vigilance / Cross-checking of each other's actions |
| **Transparency** | Prompt disclosure of errors & safety information |

> [!danger] Q19739 经典 stem（hierarchy + psych safety 角度）
> Senior resident pressuring junior medical student to perform unfamiliar procedure（"You've seen it done, you should be able to do one by now"）→ student 不敢拒 → 胎盘失败 + PPH。
>
> **核心 root cause = poor teamwork**（hierarchy + intimidation + lack psychological safety），**不是** cognitive bias / communication 跨职业 / didactic 缺失 / fatigue。
>
> **最有效干预 = Teamwork training + safety culture**（simulation + debriefings + rewards for identifying risks），改善 psychological safety + leader responsiveness。

> [!success] Q23112 经典 stem（shared understanding of goals 角度）⭐（v1.3.9 新增）
> ICU director 实施 interprofessional team-based rounding + 团队成员：attending physician / pharmacist / social worker / NP / case manager → most likely promote highly effective team functioning？
>
> **答案 = Shared understanding of desired goals**（**A** ✓）— Collaboration 元素的核心。
>
> **反 pattern 4 类钉死**：
> - ❌ B "Speed > safety"（team efficiency 不能 over patient safety）
> - ❌ C "Equal participation by each discipline"（roles 应 commensurate to skills，不需平等）
> - ❌ D "Reduce hierarchy + role overlap"（reduce **steep** hierarchy ✓ 但 role **overlap** ❌ — overlap 导致 harmful duplication 如多 insulin admin）
> - ✅ A "Shared understanding of goals"
>
> **Distinct roles vs overlap 关键区分**：**Distinct + unique roles ✅**（医生开药 / 护士给药 / 药师 verify — 单一 ownership）vs **Overlapping roles ❌**（多 provider 都给 insulin = potential overdose）；**Distinct + non-steep hierarchy ✅** vs **Steep hierarchy ❌**。
>
> **反射钩**：见 "interprofessional team-based rounding + effective functioning" → 0.5 秒锁 **shared understanding of goals**（不是 speed / equal participation / role overlap）

> [!info] Poor teamwork 是 sentinel events 的 leading root cause
> Improved communication reduces medical errors & improves patient/clinical outcomes — Joint Commission 数据。

**Barriers to teamwork** ⭐⭐：
- 频繁人员变动
- Physical environment 不利于团队凝聚
- **Hierarchies preventing communication ⭐⭐⭐** — 等级压制低年资发声（最重要 CK 考点）
- Inconsistent behaviors（不同 attending bedside manner 差异）

> [!danger] CK 高频 stem
> "Junior nurse 没敢说 concern → adverse outcome" → 答案是 **psychological safety / flatten hierarchy / encourage speaking up**（**不是** "blame nurse" 或 "education nurse"）

#### 6.5.4 Leadership — Soft + Hard Skills

| 类型 | 内容 |
|---|---|
| **Organizational (hard) skills** | **Coordination**：角色明确 / 目标明确 / 分配任务 / 团队结构 / 资源管理<br>**Monitoring**：调整计划 / 评估表现 / 提供 feedback |
| **Interpersonal (soft) skills** | Lead by example / 协作而非命令 / 接受来自任何 team member 的 input |

#### 6.5.5 Crisis Resource Management (CRM) ⭐

**借自航空业**的急救情境 leadership 原则。

**核心**：
- 清晰角色分配（"You bag, you compress, you record"）
- **闭环沟通**（check-back）
- 全局监控 + 资源调配
- **接受 input from 任何 team member**（不论等级）
- Debrief 复盘

**stem 触发**："code blue management" / "emergency leadership" / "team resource allocation in crisis"

#### 6.5.6 Check-Back = Closed-Loop in Health Care

衍生 §6.2 的 **closed-loop communication** 在 health care 也叫 **check-back**（AMBOSS 用语）— 同一概念。CK 两个名词都可能出现，识别为等价。

#### 6.5.7 5 大 Team Safety 工具边界表 ⭐⭐⭐（v2.1 增量 — Q106665 + Q19684 + Q106239 + Q21520 + Q107227 多锚定）

> [!danger] 5 大 team safety 工具**各有专属场景，不可互换** — 错位即失分

##### 5 大工具完整对比 ⭐

| 工具 | 何时用 | 解决什么 | Stem 触发词 | 经典锚定 |
|---|---|---|---|---|
| **Time-out** | 术前 immediately prior to incision / 高风险操作前 | **Patient ID + Procedure + Site** — wrong-site/patient/procedure 防 | "WHO Universal Protocol" / "RSO 减" / "wrong-site surgery 防" / "patient ID + side + procedure verification" | Q106239 + Q107227 |
| **Checklist** | 高风险任务执行时 | **Task completion + omission 防** | "task steps" / "high-risk procedure completion" / "surgical safety checklist" | — |
| **Handoff (I-PASS / SBAR)** | **Shift change** / patient transfer | **Information continuity — errors of omission 防** | "shift change handoff" / "I-PASS" / "SBAR" / "sickest patients first" / "structured communication during transitions" | Q21520 (sickest first) |
| **Debriefing** ⭐ | **Before / after** clinical event | **Team dynamics + hierarchy + psych safety + shared understanding** | "interprofessional debriefing" / "perioperative team safety briefing" / "address collaboration gap" / "high-reliability organization" | Q106665 (nurse co-lead) |
| **Closed-loop (Check-back)** | **Real-time** verbal order | **Accuracy of message — misinterpretation 防** | "verbal order" / "20 of K abbreviation" / "read-back" / "sound-alike drug" / "receiver repeat back" | Q19684 |

##### 互换陷阱 4 类（CK 高频钓饵）⭐⭐

| 误用 | 实际应该用 | 原因 |
|---|---|---|
| 见 "address interprofessional collaboration gap" → 选 **Handoff template** ❌ | **Debriefing** ✓ | Handoff = shift change 信息传递；不解决 intraoperative team dynamics |
| 见 "address interprofessional collaboration gap" → 选 **Checklist** ❌ | **Debriefing** ✓ | Checklist = task completion；不改 dynamics |
| 见 "verbal order miscommunication" → 选 **Sign-out / I-PASS** ❌ | **Closed-loop** ✓ | Sign-out = shift change handoff；本题是 real-time order entry |
| 见 "RSO + interruption during count" → 选 **Closed-loop** ❌ | **Time-out** ✓ | Closed-loop = verbal order accuracy；time-out 才同步注意力 + 防打断 |

##### Co-leader 选择原则（Debriefing 高频考点）⭐

| 选谁 co-lead？ | 为什么 |
|---|---|
| **Lowest-perceiving discipline**（如 nurse 评 surgeon 48 → nurse 当 co-lead） | 给 voice = 直接 address perception gap + 减 hierarchy + 增 psych safety |
| Highest-status discipline only（surgeons-only） | ❌ 反向加重 hierarchy + 不让 lowest-perceiving 有 voice |
| 随机轮值 | ❌ 不针对 perception gap source |

##### 反 pattern：Single-discipline Training ⚠️

Training **一个 discipline**（如"surgeons-only safety vigilance training" / "anesthesiologists-only Lean methods"）**不解决 interprofessional** collaboration — 必须 **interactions within team**（如 interprofessional debriefings / 联合 simulation）才行。

##### 一句话锁 ⭐⭐⭐

- **"Time-out 患者 ID / Checklist task / Handoff transition / Debriefing dynamics / Closed-loop message accuracy"** ⭐
- **"Interprofessional collaboration gap → Debriefing（不是 handoff / 不是 checklist / 不是 single-discipline training）"** ⭐
- **"Co-leader 选 lowest-perceiving discipline"** ⭐

##### 类比 — 交响乐团

- **Debriefing** = 彩排后讨论会（所有乐器都说话，减 hierarchy）⭐
- **Checklist** = 乐谱 check（task completion）
- **Handoff** = 指挥换人交接（shift change）
- **Time-out** = 演出前最后核对（patient ID + procedure + site）
- **Closed-loop** = 指挥手势确认（real-time message accuracy）

##### 6.5.7.1 Briefing vs Debriefing 边界深化 ⭐⭐⭐（v2.2 增量 — Q106665 stem 触发 "perioperative briefings AND debriefings"）

> [!warning] 笔记里 §6.5.7 把 "Debriefing" 列为单一工具；实战中 **Briefing**（事前）vs **Debriefing**（事后）必须分开识别 — Q106665 选项 B 明确包含**两者**。

###### 一句话先记 ⭐

- **Brief** = 事前**说前面**（**B**efore — B 开头对应 B 开头）
- **De-brief** = "de" 拉丁词根 = "from" → 从刚发生的事**回头看**（事后）

###### Briefing vs Debriefing 完整对照 ⭐⭐⭐

| 维度 | **Briefing**（事前简报）| **Debriefing**（事后复盘）|
|---|---|---|
| **时机** | **Before** clinical event | **After** clinical event |
| **目的** | **Anticipate**（预判 + 准备 + 对齐）| **Learn**（反思 + 改进 + system 优化）|
| **核心问句** | "We're about to do X. Are we ready?" | "We just did X. What can we learn?" |
| **典型时长** | 5-10 min | 5-15 min |
| **侧重** | 风险预测 + 角色分工 + 资源 + emergency plan | What went well + wrong + action items |
| **能改 dynamics?** | 部分（建立 shared goal）| **强**（reflect on team behavior）|
| **能减 hierarchy?** | 部分（角色分配让 junior 有 voice）| **强**（每人有 voice 讲 concerns）|

###### Briefing 典型场景

| 场景 | 内容 |
|---|---|
| **OR 术前**（pre-op briefing）| Surgeon 简述 procedure + risk + 预测出血 → nurse 报告设备 + blood → anesth 报告 patient comorbidities |
| **Shift change**（morning briefing）| Charge nurse 通报预期 admissions + 关键 patients + 资源分配 |
| **ICU rounds 前**（daily rounds briefing）| 团队对齐每个 patient 的 goals of care |
| **Code blue 前**（high-risk patient）| Crash cart 位置 + 谁压胸 + 谁 bag + 谁 record |

###### Debriefing 典型场景

| 场景 | 内容 |
|---|---|
| **OR 术后**（post-op debriefing）| 团队留 5 min — surgeon / anesth / nurse 各讲"今天哪里好 / 哪里能改"|
| **Code blue 后** | CPR 结束后立刻 — "压胸节奏太慢 / epi 给得太晚 / cart 位置远" |
| **Sentinel event 后** | 24-48 hr 内（**不是 blame meeting，是 learning meeting**）|
| **Near-miss 后** | Pharmacist intercept 错药 — 团队复盘"为什么差点出事" |

###### Briefing vs Time-out 边界（USMLE 易混）⭐

> [!danger] **Briefing ≠ Time-out**
> - **Briefing** = 事前**整体规划**讨论（5-10 min）— 在 OR 大门外 / preop holding area
> - **Time-out** = **即将开刀那一刻**的最后核对（30 秒-1 min）— **just before incision**
>
> **顺序**：**Briefing**（preop holding，整体规划）→ 进 OR → **Time-out**（刀片落下前的最后 patient/site/procedure 核对）→ 开刀

###### Debriefing vs M&M Conference 边界 ⭐

| 维度 | **Debriefing** | **M&M Conference** |
|---|---|---|
| **时机** | **Immediate**（事件后立刻 / 当天 / 24-48 hr 内）| **Delayed**（数周后月度）|
| **范围** | **Same team** 反思 single event | **跨多 case**（科室聚合）|
| **目的** | 快速 action items + behavior change | 教育性 + system improvement |
| **时长** | 5-15 min | 1-2 hr |

→ Q106665 是 **debriefing**（immediate post-op），不是 M&M

###### Q106665 为什么选 "briefings AND debriefings"

题目原文："Having nurses lead portions of the **perioperative team safety briefings AND debriefings**"

**关键**：选项里同时提到 **briefings + debriefings 两个都有** — 这是**最完整**的 team safety 工具组合：
- **Briefing**（术前）= 让 nurse 在术前就有 voice → shared goal alignment
- **Debriefing**（术后）= 让 nurse 在术后反思时有 voice → behavior change

→ **两个时点都让 nurse 有 voice** = 直接 address Q106664 暴露的 nurse 评 surgeon 48 的 perception gap

###### Stem 暗号词识别 ⭐

| Stem 暗号 | 0.5 秒识别 |
|---|---|
| "**Before** incision / event" + 结构化讨论 | **Briefing** |
| "**Anticipate** risks" / "set goals" / "team alignment" | **Briefing** |
| "**After** clinical event / surgery / code" + 结构化讨论 | **Debriefing** |
| "**Reflect on what went well / wrong**" / "learn from event" | **Debriefing** |
| "**Perioperative briefings AND debriefings**"（Q106665）| 两个**都有** — 术前 + 术后 |
| "Address **interprofessional collaboration gap** / hierarchy / psych safety" | **Debriefing 优先**（reflection 改 dynamics 更强）|

###### 类比 — 飞行员（high-reliability organization 同源）⭐

```
Briefing = 起飞前 cockpit briefing
    机长 + 副驾驶 + 乘务长 — "今天目的地天气差，预计绕飞 30 min，紧急情况谁联系塔台谁广播乘客"
    
飞行进行 ...

Debriefing = 降落后 cockpit debriefing
    "刚才 turbulence 时副驾驶 alert 我太晚 5 秒，下次注意 / 乘务长今天 boarding 比 SOP 快了 8 min，怎么做到的？"

Time-out = 起飞前最后 read-back
    塔台："Cleared for takeoff runway 27" 
    机长："Cleared takeoff runway 27, confirming"（30 秒确认）
```

###### 一句话锁 ⭐⭐⭐

- **"Brief = 事前（anticipate）；Debrief = 事后（learn）"** ⭐
- **"Perioperative briefings + debriefings 是 OR team 4 大 dynamics 改善工具"**（shared understanding / psych safety / reduce hierarchy / coordination）
- **"Time-out ≠ Briefing"** — time-out 是刀落前 30 秒最后核对，briefing 是 5-10 min 整体规划
- **"Debriefing ≠ M&M"** — debriefing immediate + same team；M&M delayed + 跨多 case

---

## 七、Disclosure of Medical Errors

> [!info] 引用 Ethics_Master §七
> 详细见 [[完整笔记/Peixuan分科笔记/Ethics_Master]] 第七节。本节只列**与 patient safety 直接相关的考点**。

| 场景 | 标准答案 |
|---|---|
| **自己犯错（即使 no harm）** | **主动告知病人 + 上报系统** — Error 是否 harm 与 disclosure 义务**无关** |
| **同事犯错** | **先和同事本人谈** → 不行再上报 |
| **病人问"是不是出错了"** | **诚实告知** |
| **掩盖了想披露** | **披露**，无论后果 |

> [!danger] 反 pattern
> - "Error 没造成 harm → 不必告诉病人" ❌
> - "告诉病人会增加 malpractice 诉讼风险 → 不告" ❌（实际上 disclosure 减少诉讼）
> - "同事犯错立刻告院长" ❌ — **先谈** 同事

---


---

### 13.10 Initial Management + Disclosure SOP + Apologize 措辞 ⭐⭐⭐

#### 13.10.1 Initial Management 5 步

发现 error → 5 步：

1. **Stabilize patient**（corrective measures）
2. **Communicate adverse event to patient**
3. **Disclose error**（见 §13.10.2）
4. **Investigate**（即使原因未明也持续 update）
5. **Promote incident reporting**

#### 13.10.2 Medical Error Disclosure SOP — 6 要素 ⭐⭐

1. **Clearly admit** error 发生
2. **State** 事件经过
3. **Explain consequences**（immediate + long-term）
4. **Describe corrective steps**
5. **Express personal regret + apologize**
6. **Allow time for questions + continued dialogue**

#### 13.10.3 Apologize 措辞 — CK 高频陷阱 ⭐⭐⭐

| 错误措辞 ❌ | 正确措辞 ✅ |
|---|---|
| "I'm sorry you **feel** that way" | "I'm sorry **this happened**" |
| "I'm sorry you **took it** that way" | "I'm sorry for the **distress caused**" |
| "I'm sorry, **BUT**..."（带 qualification） | "We have **learned** that..." |

> [!danger] 铁律
> **Apologize directly + without qualification**。任何 "but" / "feel" / "took it" 都是错答案。
>
> **Regardless of outcome, clinician must inform patient immediately + disclose nature of error.**

### 13.11 Incident Reporting Systems (IRS) ⭐

| 类型 | 含义 | 例子 |
|---|---|---|
| **Voluntary reporting** ⭐ | Confidential 个人自报 | Anonymous hotline / online portal |
| **Mandatory reporting** | State 规定 deaths / serious adverse events 上报 | The Joint Commission / 州卫生厅 |

**Advantages**：识别 systems errors（如 trailing zero label）+ aggregate sentinel events 数据 + 跨机构防错。

**Limitations** ⭐：
- **只有 ~7% errors 被报** ⭐ — voluntary 自报偏倚
- IRS 不能衡量 overall safety
- 机构间**不可比**

> [!tip] 鼓励上报策略
> Easy-to-use + confidential IRS + **learning culture（不是 blame culture）**


---

### 13.13 Simulation-Based Training (SBT) ⭐⭐（v1.3.14 — 从"次要考点"升级为"高频考点"，Q105800 锚定）

**核心**：用 simulation 训练 first-hand experience，无 patient risk。

**Advantages**：hands-on / repetition / safe / rare scenario 训练 / 跨学科练习
**Disadvantages**：贵 / artificial 环境
**Resources**：Manikin / anatomical models / actors / VR
**Examples**：技术（sutures / airway / line）/ 非技术（communication / decision-making / teamwork）/ emergency（BLS/ACLS/ATLS）

#### Unpredictable Emergency 干预选择反射钩 ⭐⭐⭐（Q105800 锚定）

> [!warning] Training 例外规则
> §三 防御层级里 training / education 通常是**最弱层**（less reliable HFE），但**对 unpredictable emergency 是例外** — training 反而是**必要 + 高效**，因为没法 engineer away。

```
题干信号：事件 unpredictable + 大比例无 risk factors（如 >50%）
    │
    ▼
① ⭐ SBT（Simulation-Based Training）— 全员 + 定期
    • Hands-on 训练 maneuvers
    • 团队协调反应
    • 跨学科 mock drill
    │
    ▼ （仅次于 SBT 的辅助）
② Team debriefings after adverse event
    • 仅 involved team 受益（reach 有限）
    • 改善沟通协调，但**不如 SBT 改善技术 skills**
    │
    ▼
③ RCA — 仅当 systematic error / preventable 时
    • Retrospective 找 root cause
    • Unpredictable emergency 大多 unpreventable → RCA 不适用
    │
    ▼
④ ❌ Risk-stratification checklist — unpredictable event 失效
    • >50% no risk factors → checklist miss the majority
    • 同 Q107152 "80% 都贴 = 失效"原理
```

#### Q105800 锚 — Shoulder Dystocia 经典 stem

| 维度 | 内容 |
|---|---|
| 事件 | Shoulder dystocia — obstetric emergency |
| Risk factors | DM / fetal weight ≥4500 g / obesity with excessive gestational weight gain |
| **关键陷阱** | **>50% 病例无 identifiable risk factors** → highly unpredictable |
| 5 大 maneuvers | McRoberts (maternal hip hyperflexion) → suprapubic pressure → posterior arm delivery → Wood's screw → Zavanelli (last resort) |
| 并发症 | Brachial plexus injury / hypoxic encephalopathy / postpartum hemorrhage |
| **预防策略** | **SBT 定期 + 全员**（不是 risk-stratification checklist 因为 unpredictable） |

#### 其他 Unpredictable Emergencies 应用 SBT 同理

| 事件 | 为什么需要 SBT |
|---|---|
| **Cardiac arrest / ACLS** | 时间紧 + 团队协调 + 罕见 |
| **OB hemorrhage** | 突发 + 大量 + 多人参与 |
| **Anaphylaxis** | 罕见 + 时间紧 + 多步骤 |
| **Pediatric resuscitation** | 罕见 + 剂量计算复杂 |
| **Difficult airway** | 罕见 + 时间紧 |

> [!tip] Memory Hook
> **"Unpredictable emergency → 训练团队 ready，不是预测谁会出事"** ⭐⭐⭐
> - Predictable risk → 筛查 + 高 risk 加干预（如术前 DVT prophylaxis）
> - **Unpredictable emergency** → SBT + 全员 ready（消防演习思路）


---

### 13.15 Abuse Identification & Mandatory Reporting ⭐⭐（v1.3.14 — Q4320 + Q13465 双锚）

> [!info] 整合来源
> Q4320（child abuse — interview patient first）+ Q13465（elder abuse — 5 信号识别）双锚定。整合 child + elder + IPV 3 类 abuse 的统一识别框架。

#### Abuse 通用流程 ⭐⭐⭐

```
怀疑 abuse（红旗信号识别）
    │
    ▼
① ⭐ 提供 safe environment（让 abuser 离开 room）
    • Child abuse: 让父母离开
    • Elder abuse: 让 family member 离开
    • IPV: 让 partner 离开
    │
    ▼
② Interview patient 直接问 abuse（physical / emotional / sexual / financial）
    • Open-ended + 年龄 / 文化适配语言
    • Document objective findings
    │
    ▼
③ 高怀疑 / confirmed → Mandatory report
    • Child abuse → CPS（Child Protective Services）
    • Elder abuse → APS（Adult Protective Services）
    • IPV → 鼓励 patient self-report，**不是** mandatory（成年 capacity decision）⭐
    │
    ▼
④ ❌ 不要先做（不能 delay 评估）：
    • Family therapy / CBT / support groups
    • Interview perpetrator alone（不能取代 patient interview）
    • Reassurance（dismissing 红旗信号）
```

> [!danger] 关键铁律
> **Assess（先评估）→ Report（后上报）** — 不能跳过 interview 直接报 CPS/APS。
> **IPV ≠ child/elder abuse**：IPV 是**成年人 autonomy** — 鼓励 self-report，不是 mandatory；child + elder 是 vulnerable population → mandatory。

#### Child Abuse 红旗信号（Q4320 锚）

| 维度 | 内容 |
|---|---|
| **Caregiver background** | Young / single parents / lower education / **substance abuse** ⭐ / depression / impulse control disorder / 自己童年被虐 |
| **Home environment** | **Unstable family situation**（divorce / conflict）/ **financial difficulties** / 缺 social support / domestic violence |
| **Children risk** | 残疾 / unplanned pregnancy / 不愿要的孩子 |
| **Clinical presentation** | Unexplained / implausible injuries / 不同 stage 愈合 injuries / malnutrition / **sudden behavioral or scholastic changes** ⭐ |
| **Management** | Document → patient interview alone → report to **CPS** if confirmed |

#### Elder Abuse 5 大信号速查（Q13465 锚）⭐⭐⭐

| 维度 | 内容 |
|---|---|
| **Risk factors** | **女性** ⭐ / **Dementia or 慢性精神病** / Functional impairments / **Shared living env** OR **Social isolation** / Poor SES |
| **Physical abuse** | Atypical 抓伤 / **异常位置 fractures**（如 orbital — not from typical fall）⭐ / 痛与 reported etiology 不符 / 多处 injuries 不同 stage |
| **Psychological abuse** | 行为 / 性格改变 / depression / anxiety |
| **Neglect** ⭐ | 营养不足 / 压疮 / **comorbid 病 deterioration**（如 T2DM 控制突然变差）|
| **Financial exploitation** ⭐ | **Medication nonadherence**（钱被占）/ 多次错过 appointments / 未付租金水电费 |
| **Management** | Document → patient interview alone → report to **APS** if confirmed |

#### 5 大经典信号集齐（Q13465 stem 范例）

```
① 异常位置 fracture（orbital - non-typical fall location）
② 多处 bruises（前臂 + 腹 - 不同位置）
③ 财务异常（"pharmacy charges too much, can't afford"）
④ Medication nonadherence + comorbid 恶化（A1c 7.2 → 9%）
⑤ Shared living environment（与 daughter + son-in-law 同住）
   ↓
= Elder Abuse（不是 dementia / depression / alcohol abuse / nutritional deficiency）
```

#### Elder Abuse vs 独居 Alcohol Abuse 区分 ⭐

| 信号 | Elder Abuse | Late-onset alcohol abuse |
|---|---|---|
| 居住 | **Shared living env**（与家人同住）⭐ | **独居** |
| Injuries | Multiple 异常位置 | Falls / 醉后伤 |
| Financial | 家人占用 fix income | 自己花在酒上 |
| Comorbid | 因 financial exploitation 恶化 | 因 alcohol 致 comorbid |

#### Memory Hook

> [!tip] Abuse 5 大反射钩
> - **"Assess 先于 Report"** — 先 interview patient，不直接 CPS/APS
> - **"父母 / 家人离开 room"** — 给 victim safe disclosure 空间
> - **"Orbital fracture in elder = 红旗"** — 非典型 fall location
> - **"5 大信号集齐 = elder abuse"**（fracture / bruise / 财务 / nonadherence / 同住）
> - **"IPV 是 self-report，不是 mandatory"** — 成年 autonomy；child + elder = vulnerable = mandatory


---

### 13.14 Navigating Stressful Situations in Residency（v1.3.1 增量）⭐

> [!info] 整合来源
> AMBOSS "Transition to Residency" 系列。重点放 CK 真考的 3 个考点（AMA / Conflict styles / Harassment），其他简短引用。

#### 13.14.1 Anger / Threatening Patient Management

**Safety First 原则**：
- 保持**安全距离**
- 站位：**自己离 door/exit 近**（不被堵住）
- 必要时叫 hospital security

**De-escalation 流程**：
1. 控制自己情绪 + 保持冷静
2. **Acknowledge** patient emotions
3. **Identify** 为什么 angry（常见 3 类）：
   - **Fatigue / pain** → 解释 evaluation + 给 timeline
   - **Delays in care** → 解释原因 + 提替代方案
   - **Medical error** → **apologize + 透明 + 解释 corrective steps**（§13.10.3 措辞）
4. 对于 aggressive demanding（要做某检查/治疗）：acknowledge 病人有权获得最佳 care + 要求 calm down 以便 provide care

**Follow-up**：debriefing with peers + 找 support system + reflection

> [!tip] 引用
> 详细 verbal de-escalation 见 [[完整笔记/专题笔记/_衍生_Ethics精简框架]] §12.12 Agitated ED Verbal De-escalation

#### 13.14.2 Leaving Against Medical Advice (DAMA / AMA) — 5 Key Components ⭐⭐

**CK 高频**：病人要求 AMA 出院 → 标准 5 步流程。

| 步 | 内容 | 关键 |
|---|---|---|
| 1 | **Assess decision-making capacity** ⭐ | Capacity 4 要素（Communicate / Understand / Appreciate / Reason）— 详见 [[完整笔记/专题笔记/_衍生_Ethics精简框架]] §二 Capacity |
| 2 | **Severity assessment** of medical condition | 离开会发生什么 risk |
| 3 | **Identify reasons** for early departure | 经济 / 家庭 / 不信任 / 误解 — 多数 可解决 |
| 4 | **Discuss alternatives** + follow-up | Outpatient / partial / 家庭支援 / 重新入院 |
| 5 | **Documentation** | Capacity 评估 / 风险告知 / 病人理解 / 替代方案 / 签字（如签）|

**关键**：**Senior resident / attending 应介入**（不只让 intern 处理 AMA）。

> [!danger] CK 经典陷阱
> - "病人 lack capacity → 让他 AMA 出院" ❌ — Capacity 不足必须 hold（按 surrogate / ED hold / 法院）
> - "AMA 病人不必给 prescription / follow-up info" ❌ — 仍要尽量提供 alternative care
> - "AMA 签字 = 医院免责" ❌ — 签字仅是证据，**不是**免责盾牌；过程必须完整

#### 13.14.3 5 Conflict Management Styles ⭐

CK 偶尔考概念配对（Thomas-Kilmann model）。

| Style | 描述 | 适用场景 |
|---|---|---|
| **Avoiding** | 不正面冲突 / 回避 | 议题不重要 / 时机不对 |
| **Accommodating** | 让步 / 满足对方 | 维系关系优先 / 自己错时 |
| **Competing** | 强势赢 / win-lose | **紧急情境**（如急救）/ 原则问题 |
| **Compromising** | 妥协 / 双方部分让步 | 时间紧 / 双方力量相当 |
| **Collaborating** ⭐ | 双方共赢 / win-win | **长期关系** / 复杂问题 / 大多数 patient care 推荐 |

**Conflict resolution 原则**：
- **不在 patient room / public** 谈
- Private setting + neutral party（**senior faculty / program director / ombuds office**）

#### 13.14.4 Workplace Harassment ⭐

**Sources**：Patients / Hospital staff（含 superiors）

**Forms（3 类）**：
- **Verbal harassment**：羞辱性 comments / 工作背景 / 外貌
- **Physical harassment**：不当触碰 / 击打 / 过近接触
- **Sexual harassment**：unwelcome 言语或身体性挑逗

**Addressing harassment from patients**：
1. 让 **nurse / 其他员工陪同** evaluate
2. 当场 set boundary："I am not comfortable with your comments. Let's keep this professional."
3. 不舒服时**excuse self** → 找 senior resident / attending 谈
4. Encounter 后找 support system

**Addressing harassment from superiors / colleagues**：
- **Ombuds office** ⭐ — 中立调解机构
- Chief residents / mentors / trusted faculty
- **Anonymous feedback**
- **Concrete written record** of incidents
- Fear of retaliation 是常见 barrier — 寻找 institution-safe reporting

#### 13.14.5 Patient Death（简短）

- Death pronouncement / documentation 详见标准临床 SOP
- 家属沟通：grief counseling / bereavement support
- 详见 [[完整笔记/专题笔记/Ethics/Ethics_EOL_Hospice与决策]] §二 End-of-life（v2.0 拆分独立文件）

#### 13.14.6 Second Victim — Personal Consequences of Medical Error ⭐

**"Second victim"** = 犯错的医生本人。常见情绪：fear / guilt / embarrassment / 失去 self-confidence。

**支持来源**：
- **Peers / senior residents / chief residents / attendings**（其他人多半也经历过）
- **Employee Assistance Program (EAP)**
- Mental health provider

**成长机会**：
- 理解 what went wrong → 避免重犯
- 识别 **system-level factors** 改进机会（不只 blame self）

> [!tip] 衍生 §13.10 联动
> Disclosure SOP（§13.10）+ M&M peer review（§13.12.5）+ Just culture（§5.1）+ Second victim support 构成完整 **post-error ecosystem**。

#### 13.14.7 Clinical Uncertainty Management ⭐（v1.3.2 增量）

**情境**：atypical symptoms + thorough workup 后仍诊断不明 → 不轻易 over-test / over-treat。

**4 大处理策略**：
1. **Basic principles + biological plausibility** 推理（没有 textbook 答案时回归生理学）
2. **Review 已做的 workup** — 避免 redundant testing
3. **Consult others** before low-evidence testing
4. **Watchful waiting** ⭐ — 短期观察后再决定是否扩展检查

**Patient communication**：
- 解释 testing 已做的 + 各自 diagnostic role
- **Shared decision-making** 下一步
- 持续症状 + 全面 workup 阴性 → 考虑 **somatic symptom disorder** 鉴别

> [!warning] CK 反 pattern
> - "Atypical symptom → 立刻全面 work-up" ❌ — 先 watchful waiting + consult
> - "病人焦虑 → 答应做不必要 imaging 安慰" ❌ — Shared decision-making + 解释 limitations
> - "拒绝病人 demand = 不 patient-centered" ❌ — 拒绝无 evidence 检查合理；用沟通而非顺从

---

## §6.6 Psychological Safety — 完整框架 + 边界表 ⭐⭐⭐（v2.0 增量 — Q106620 锚定）

> [!info] 定义
> **Psychological Safety** = team members' comfort in 必要 + appropriate safety actions（openly voice concerns / recruit help / not fear retribution）。**High Reliability Organizations (HRO)** 核心特征。Low psych safety 由 **strict hierarchy + culture of fear / blame** 引发 → 阻碍 RRT activation 等 evidence-based 安全行为。

### 6.6.1 Psych Safety 4 大特征 Hi vs Lo ⭐

| Hi Psych Safety | Lo Psych Safety |
|---|---|
| Team members openly voice concerns | Hesitate to voice opinion |
| Recruit help without shame | Fear of retribution / punishment |
| Flat communication (challenge authority OK) | Strict hierarchy / authority gradient |
| Systems thinking (blame system not person) | Culture of fear / individual blame |

### 6.6.2 Low Psych Safety 的 Stem 信号 ⭐

- 护士 / junior **hesitate** to voice concern
- 资深 / authority figure 说 **"I've been doing this X years, I know best"**
- "**Fear of being blamed / held responsible for someone else's mistake**"
- 决策被 hierarchy 压制 + 不敢 activate RRT
- High Reliability Organization (HRO) 的反面（aviation / nuclear）= 强调 psych safety

### 6.6.3 Psych Safety 改善策略

1. **Change management**（engaging front-line in designing new initiatives）
2. Increasing transparency（feedback / communication）
3. Organizational dedication to safety resources
4. Leadership endorsement of speak-up culture

### 6.6.4 Psych Safety vs Closed-loop Communication 边界表 ⭐⭐⭐

> [!danger] **题 stem 描述 "hesitate / fear" → 永远是 psych safety**（不是 closed-loop）

| 维度 | **Closed-loop Communication** | **Psychological Safety** |
|---|---|---|
| 解决什么 | **Accuracy** of verbal message（receiver 复述发送内容）| **Willingness** to communicate（是否敢/愿意说）|
| 防什么 | Miscommunication / misunderstanding | Silence / hesitation |
| Stem 信号 | "verbal order misheard" / "drug confused due to wrong readback" | "hesitate" / "fear of blame" / "hierarchy" / "20 years experience" |
| 干预 | SBAR / closed-loop verification | Change management / flat hierarchy / leadership endorsement |

### 6.6.5 Psych Safety vs Cognitive Bias 边界表 ⭐⭐⭐

> [!danger] **题 stem "fear of retribution / blame" → psych safety**（不是 bias）

| 维度 | **Cognitive Bias** | **Psychological Safety** |
|---|---|---|
| 性质 | 思维 shortcut（anchoring / availability / framing）| Emotional / cultural barrier（fear / hierarchy）|
| Stem 信号 | "fixated on initial impression" / "common dx 太 available" | "fear of being blamed" / "hesitate to challenge senior" |
| 干预 | CDSS / cognitive forcing strategies | Change management / psych safety initiatives |

#### 6.6.5.1 第 3 反 pattern — Asymmetric Ratings Between Roles = Shared Goal Mismatch ⭐⭐⭐（v2.1 增量 — Q106664 锚定 — 反射 < 1 小时未建立警示）⚠️

> [!danger] 5-27 实战警示
> 5-27 早上刚加 §6.6.5 + §6.6.7 三件套一句话锁；当天下午做 Q106664 仍被 cognitive bias 字眼吸引选错（A 而非 B）。**反射 < 1 小时未建立** — 此节为补漏。

**Q106664 Stem 模式**：OR 多职业 survey — nurse 评 surgeon 48 / surgeon 评 nurse 88（极不对称）→ 最 likely underlying factor？

**正解**：**Differences in understanding of team goals**（不是 cognitive bias）

##### 第 3 维度补全 — Shared Goal Mismatch（比 §6.6.5 中 cognitive bias / psych safety 更前置）

| 维度 | **Cognitive Bias** | **Psychological Safety** | **Shared Goal Mismatch** ⭐ NEW |
|---|---|---|---|
| **失败发生在？** | 医生大脑内部 mental shortcut | 团队互动 — 不敢说 | **团队互动 — 对 "team should function how" 定义不一致** |
| **独自工作仍发生？** | ✓ 会 | ✗ 不会 | ✗ 不会（需 ≥ 2 角色互动）|
| **Stem 暗号词** | "reviews chart prior" / "first impression" / "narrowed differential" | "fear of retribution / blame" / "hesitate to challenge" | "**asymmetric ratings between disciplines**" / "perception gap between roles" / "differences in defining collaboration" ⭐ |
| **解决方案** | Metacognition / CDSS / diagnostic timeout | Just culture / flatten hierarchy / TeamSTEPPS | **Shared goal definition + role clarification + interprofessional debriefings** |

##### Nurse-Surgeon 不对称感知机制（USMLE 经典 stem 触发）⭐

```
Surgeon 定义 collaboration = "instructions are followed promptly + accurately"
    │
    ▼
Surgeon 评 nurse 高（88）— 因为 nurse 通常 follow instructions
    │
    ▼
但 nurse 定义 collaboration = "my input is respected and acknowledged"
    │
    ▼
Nurse 评 surgeon 低（48）— 因为 surgeon 没充分 acknowledge input
    │
    ▼
不对称感知 = **不是 cognitive bias，是定义不一致 (role + goal mismatch)**
```

##### 反 pattern 钓饵：把 Cognitive Bias 误归因 Team Dynamic ⚠️

| 错误归因 | 为什么错 |
|---|---|
| "Nurses + surgeons 都有 cognitive bias" | ❌ Cognitive bias = **individual diagnostic shortcut** — 不解释 group-level perception gap |
| "Different medical knowledge / technical skills" | ❌ Technical expertise 差异不解释 collaboration **perception** 差异 |
| "Fatigue / sleep deprivation" | ❌ 若 fatigue → 跨对象一致低；本题 nurse-nurse 评分高（81）→ 不是 fatigue |
| **"Differences in understanding of team goals"** ⭐ | ✅ 正解 — 不同角色定义不一致 |

##### 反射钩（与 §6.6.7 三件套联读）

> [!success] 团队沟通完整 5 层模型（v2.1 升级 — 比早上的 4 步更细）
>
> ```
> 理想团队沟通 5 层：
>     ① "我们对 collaboration 的定义一致吗？" ← Shared Goal 解决（NEW ⭐）
>           ▼
>     ② "我敢说"                              ← Psych Safety 解决
>           ▼
>     ③ "我说出来"
>           ▼
>     ④ "你听对"                              ← Closed-loop 解决
>           ▼
>     ⑤ "你处理对"                            ← Cognitive Bias 防御
> ```
>
> **第 ① 层 Shared Goal 比 ② Psych Safety 更前置** — 即使 psych safety 满分，若 surgeon 和 nurse 对 collaboration 的定义不同，**评分仍会不对称**。
>
> **一句话锁**：**"定义不一致 = Shared Goal mismatch（debriefings + role clarification）"** ⭐

##### 反射钩（USMLE 救命）

| Stem 暗号 | 0.5 秒锁 |
|---|---|
| "**asymmetric ratings between disciplines**" / "nurse 评 surgeon 低 / surgeon 评 nurse 高" / "perception gap between roles" | **Shared Goal Mismatch / Differences in understanding** ⭐ |
| "fear of retribution / blame / hierarchy / hesitate" | Psych Safety |
| "reviews chart prior to seeing patient" / "narrowed differential" | Cognitive Bias (framing) |
| "verbal order misheard / 20 of K abbreviation" | Closed-loop |

##### 类比

餐厅评分系统 — 厨师认为"上菜快 = collaboration 好"，服务员认为"被尊重 = collaboration 好"；两人评分不对称**不是因为大脑偏差，是因为定义不同** → 解决 = **重新定义共同目标 + 各角色 voice debriefing**，不是给厨师做 cognitive bias 培训。

### 6.6.6 RRT Activation 是 Joint Management（不是 Transition of Care）

- **RRT activation** = primary team + RRT **joint patient management**（不是 handoff transition）
- Stem 干扰项 "Standardize transitions of care" → **错** — 没有 formal transition 发生
- 反 pattern：把 RRT activation 类比 sign-out / I-PASS → 错位

### 6.6.7 Memory Hook

> [!success] 三件套一句话锁（最高优先 — 信息生命周期 3 个失败层面）⭐⭐⭐
> - **"信息传不准 = Closed-loop（read-back）"** ⭐
> - **"信息不敢传 = Psych Safety（speak up / just culture）"** ⭐
> - **"信息处理偏 = Cognitive Bias（metacognition / debriefing）"** ⭐
>
> **三句联读**：**"传不准、不敢传、处理偏 — 三个层面三个解药"**
>
> ```
> 理想团队沟通 4 步：
>     ① 我敢说    ← Psych Safety 解决（信息不敢传）
>     ② 我说出来
>     ③ 你听对    ← Closed-loop 解决（信息传不准）
>     ④ 你处理对  ← Cognitive Bias 防御（信息处理偏）
> ```
>
> 任何"沟通 / 团队 / 诊断 failure"题先判**信息在哪个层面失败**，再匹配解药。

> [!success] 其他 hooks
> - **"Hesitate + fear of blame + hierarchy = Psychological Safety"** ⭐⭐⭐
> - **"Closed-loop vs Psych safety 边界：accuracy of message vs 是否敢说"** ⭐
> - **"Psych safety vs Cognitive bias 边界：emotional barrier vs mental shortcut"** ⭐
> - **"'I've been doing this 20 years' = senior 阻碍 team activation = psych safety 缺失"**
> - **"RRT activation = joint management，不是 transition of care"**

---

## §3.x Surgical Safety 三联 + Final Time-out 5 铁律 ⭐⭐⭐（v2.0 增量 — Q22186 锚定）

> [!danger] 核心铁律
> **Surgical Safety = preoperative verification + site marking + final time-out 三联。Preoperative verification 必须 involve patient/surrogate + 2 identifiers + ≥2 providers + 在 preoperative holding area。患者参与是关键 redundancy 防 wrong-site surgery。** "Brief / focused" in safety procedures = **反 pattern 警惕**。

### 3.x.1 Surgical Safety 三联完整流程

| 阶段 | 何时 | 做什么 | 谁 |
|---|---|---|---|
| **Preoperative verification** | Preoperative holding area | Patient ID + operative site + type of operation + side + 2 identifiers | **≥2 providers + 患者/surrogate** ⭐ |
| **Site marking** | Preop | Mark "YES" + initials on **operative** site only + permanent marker | Surgeon |
| **Final time-out** ⭐ | **Immediately prior to skin incision in OR** | Repeat verification of patient ID + site + side | **Entire surgical team** + addressing **all** concerns |

### 3.x.2 Final Time-out 5 铁律 ⭐

1. **位置**：OR + 紧贴 incision（不是 preop holding）
2. **时机**：immediately prior to skin incision
3. **参与者**：**entire surgical team**（不是 designated few）
4. **长度**：**不限时** — 所有 concerns / questions must be addressed
5. **范围**：再次 verify patient ID + operative site + side

### 3.x.3 "Brief / Focused" 反 Pattern 普适警示 ⭐

- Patient safety procedures 强调 **thoroughness over speed**
- 任何 "brief" / "limit length" / "focused-only" 措辞 in safety procedures → **警惕反 pattern**
- 类似反 pattern：handoff 强调"omit 不重要" = 错（标准化 sign-out 必须 cover all 维度）

### 3.x.4 Sentinel Events 风险因素

- **Wrong-side surgery** = sentinel event（patient death / irreversible harm）
- **高风险触发**：high task complexity / urgency（**schedule delays / high case volume**）/ **interchangeable surgical teams**
- 解决：加强 redundancy（不是 brief）+ 患者参与 + entire team time-out

### 3.x.5 Mark Operative Only — 反 Pattern 警示

- ❌ Mark both operative + nonoperative sites with different labels = ambiguity 反 pattern
- ✅ Mark **operative site only** + permanent marker + "YES" + initials

---

## 🔗 关联

- 🔁 **同主题错题**（聚焦 Safety 文化 + Communication）：
  - [[mistakes/uworld-mistakes_2026-05#^Q106620]] Psychological Safety vs Closed-loop vs Cognitive Bias（5-27 做对）
  - [[mistakes/uworld-mistakes_2026-05#^Q22186]] Surgical Time-out + 患者参与 site verification（5-27 错）
  - [[mistakes/uworld-mistakes_2026-05#^Q105800]] Shoulder Dystocia SBT（5-26 入库）
  - [[mistakes/uworld-mistakes_2026-05#^Q106042]] Just Culture 时序原则
  - [[mistakes/uworld-mistakes_2026-05#^Q19739]] / [[mistakes/uworld-mistakes_2026-05#^Q23112]] Features of Effective Teams 6 元素
  - [[mistakes/uworld-mistakes_2026-05#^Q4320]] / [[mistakes/uworld-mistakes_2026-05#^Q13465]] Abuse identification + mandatory reporting
  - [[mistakes/uworld-mistakes_2026-05#^Q107227]] / [[mistakes/uworld-mistakes_2026-05#^Q106239]] Time-out 3 要素
- 📚 **配套子文件**：
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_QI工具]]
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Cognitive诊断错误]]
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_HFE与药物HAC]]
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]]（主索引）
- 📚 **主笔记 / 跨学科**：
  - [[完整笔记/Peixuan分科笔记/Ethics_Master]]
  - [[完整笔记/专题笔记/Ethics/Ethics_Communication_Counseling]]
  - [[完整笔记/专题笔记/psych/psych_医患沟通对话术SOP]]（MI 框架 + Family Education + Med Counseling）
