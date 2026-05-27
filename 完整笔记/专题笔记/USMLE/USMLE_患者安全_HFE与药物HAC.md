---
tags:
  - USMLE-Step2
  - Ethics
  - HFE
  - 药理
created: 2026-05-27
type: 专题笔记
---

# USMLE_患者安全_HFE 与药物 HAC

> [!info] 本笔记定位
> 从 [[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]] (原 v1.3.15 大文件) 拆出，专注 **Human Factors Engineering + Tall Man Lettering + Medication Reconciliation + Hospital-Acquired Conditions + Procedural Iatrogenic Harm + Risk Factors for Medical Errors**（含 Q19788 Patient-Centered Counseling + Q22186 Surgical Safety + Q107154/Q107171 Falls 二级预防 待加 B 增量）。
> 4 子文件之一（另 3：[[完整笔记/专题笔记/USMLE/USMLE_患者安全_QI工具]] / [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Safety文化与沟通]] / [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Cognitive诊断错误]]）。
> 主索引：[[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]]。

## §0 本文件目录

- §八 杂项必考（每条 1-2 行）
- **§8.6 CPOE + CDSS 完整框架** ⭐⭐⭐（v2.0 拓展 — input 端 vs decision 端 / 5 联问题 / CK 反射钩 / 反 pattern / 局限性）
- §13.1 Specific Error Types 续（5 类补充）
- §13.2 Procedural Iatrogenic Harm — 速查表
- §13.3 Risk Factors for Medical Errors — 3 大类
- §13.6 Human Factors Engineering (HFE) — 3 档 Reliability 分级
- **§13.6.x HFE 3 机制 + Point of Care + Adherence 效力排序**（v2.0 — Q106819）
- §13.6.1 Clinical Decision Support Systems (CDSS) 完整框架（Q18754 锚 — medication error detect vs 不能 detect 4 类）
- §13.7 Tall Man Lettering + "Do Not Use" Abbreviations
- §13.8 Medication Reconciliation + Teach-Back + Prescribing Cascade
- **§13.8.x Patient-Centered Counseling 4 法 + sound-alike trap + ADE 3 维**（v2.0 — Q19788）
- §13.9 Hospital-Acquired Conditions (HACs)
- **§3.x Surgical Safety 三联 + Final time-out 5 铁律 + Brief 反 pattern**（v2.0 — Q22186，加在 Safety文化与沟通子文件 §三 — [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Safety文化与沟通#§3.x Surgical Safety 三联 + Final Time-out 5 铁律 ⭐⭐⭐（v2.0 增量 — Q22186 锚定）|跳转]]）
- **§13.9.x Fall Secondary Prevention + multifactorial 7 维**（v2.0 — Q107154/Q107171 — 与 [[完整笔记/专题笔记/USMLE/USMLE_老年Fall3层防护]] 互补）

---

## 八、杂项必考（每条 1-2 行）

### 8.1 Medication Reconciliation（药物核对）
- 入院 / 出院 / 转科 / 转 ICU 时，**重新核对全部药物清单**
- 防 medication error + duplicate prescribing + omitted med

### 8.2 Two-patient Identifiers（双重身份核对）
- 给药 / 抽血 / 操作前用 **2 个 identifier** 核对
- ✅ 姓名 + DOB / 姓名 + MRN
- ❌ 床号（病人可能换床）/ 房间号

### 8.3 Surgical Site Marking（手术部位标记）
- 病人**清醒 + 自己确认**时标记（非麻醉后）
- 由主刀外科医生标
- 标在**会出现在手术野**的位置

### 8.4 Hand Hygiene（手卫生）
- **最便宜 + 最有效**的感染控制干预
- 5 个时机（WHO）：① 接触病人前 ② 操作前 ③ 接触体液后 ④ 接触病人后 ⑤ 接触病人环境后

### 8.5 Bar-code Medication Administration（BCMA）
- 给药前**扫病人腕带 + 药品条码** → 系统验证 5 R（right patient / drug / dose / route / time）
- 属于 **automation** 层防御（§3 梯队第 ②）

### 8.6 Computerized Provider Order Entry (CPOE) + Clinical Decision Support

> [!info] **CPOE = 录入系统；CDSS = 录入时的智能层**
> CPOE 解决 input 端（handwriting / verbal / transcription / abbreviation）；CDSS 解决 decision 端（drug-drug / allergy / dose / pathway）。**联用 = medication safety 黄金组合**（USMLE 高频说法），单独使用都不够。

#### 8.6.1 CPOE 定义 + 解决的核心问题 ⭐⭐⭐

**CPOE** = **Computerized Provider Order Entry（计算机化医嘱录入系统）** — 医生**直接在电脑录入医嘱**（处方 / 检验 / 影像 / 会诊），替代手写 Rx + verbal order。

**CPOE 解决 5 联 input 端问题** ⭐：

| 传统手写 / verbal order 的问题 | CPOE 怎么解决 |
|---|---|
| **Illegible handwriting** ⭐ | 电子录入 = 字迹清晰 |
| **Verbal order miscommunication**（sound-alike 听错 / 错读）| 直接录入 = 无 verbal 链 |
| **Vague Rx**（剂量 / 频率 / 给药途径不全）| CPOE 强制 fill required fields |
| **Transcription error**（药房 / 护士抄错）| 录入直接传到药房 / 护士站 = 无中间 transcription |
| **"Do Not Use" Abbreviations**（U / IU / qd / qod / MgSO4）| CPOE 禁用 abbreviation drop-down |

#### 8.6.2 CPOE vs CDSS 关系对照 ⭐⭐⭐

| | **CPOE** | **CDSS** |
|---|---|---|
| 是什么 | **录入系统**（input 工具）| **智能层**（提醒 / 警示 / 推荐）|
| 解决什么 | Handwriting / verbal / transcription / abbreviation / vague Rx | Drug-drug interaction / allergy / dose / algorithm / order set |
| 类比 | Word 软件本身 | Word 的"语法检查 + 自动建议" |
| 减 error 类型 | Communication / writing / transcription 端 error | Clinical decision 端 error |

→ **CPOE + CDS 联用** = 录入瞬间 alert（drug-drug / allergy / dose / pathway）；单独 CPOE = 字迹清晰但不能 detect interactions；单独 CDSS = 没 CPOE 录入入口就没机会触发。

#### 8.6.3 CPOE CK 高频反射钩 ⭐⭐⭐

```
Stem 关键词 → 0.3 秒锁
─────────────────────────────────────────────
"Illegible handwriting" + medication error             → CPOE
"Verbal order" + sound-alike / 错读                   → CPOE（消除 verbal 链）+ closed-loop verification（如果必须 verbal）
"Transcription error"（药房 / 护士抄错）              → CPOE（直接电子传输）
"Do not use" abbreviations 错读（U → 0 / IU → IV）   → CPOE（禁 abbreviation drop-down）
Drug-drug interaction / allergy / dose                → CPOE + CDSS
复杂医嘱 bundle（sepsis / DKA / stroke order set）   → CPOE + CDSS order sets
```

#### 8.6.4 CPOE 局限性 — 不能解决什么 ⭐

> [!warning] CPOE 不是万能 — 反 pattern 警示

| CPOE 不能解决 | 应选 |
|---|---|
| Clinical judgment error（开错适应症）| CDSS algorithm / training |
| Cognitive bias / overload（漏 dx）| **CDSS reminders + cognitive forcing**（见 [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Cognitive诊断错误#§13.5.x Diagnostic Error 干预匹配表 + CDSS 3 大机制 ⭐⭐⭐（v2.0 增量 — Q106049 锚定 — Linked vignette Item 2 of Q106048）|§13.5.x CDSS 7 联临床形式]]）|
| Communication gap（hesitate to question senior）| **Psych safety**（见 [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Safety文化与沟通#§6.6 Psychological Safety — 完整框架 + 边界表 ⭐⭐⭐（v2.0 增量 — Q106620 锚定）|Safety文化 §6.6]]）|

#### 8.6.5 CPOE 本身可引入的新 error ⭐

> [!danger] CPOE 自身风险（CK 偶考）
> - **Drop-down 选错**（drug name 列表相邻 → 选成 sound-alike）→ **Tall Man Lettering** 缓解（见 §13.7）
> - **Copy-paste error**（旧 note 复制 → propagation of outdated info）
> - **Alert fatigue**（过多 pop-up → 医生 ignore）→ tailored alerts > universal
> - **CPOE override**（医生 ignore alert）→ 失去保护层 → 解决 = leadership endorsement + audit

#### 8.6.6 减 error 量化数据（CK 偶考）

- CPOE 实施减 **medication prescription error ~50%+**
- CPOE + CDSS 联用减 **serious medication error ~80%**（高峰）

#### 8.6.7 Memory Hook

> [!success]
> - **"CPOE = 录入系统；CDSS = 智能层；两者联用 = medication safety 黄金组合"** ⭐⭐⭐
> - **"CPOE 解决 input 端：handwriting / verbal / transcription / abbreviation / vague Rx"**
> - **"CDSS 解决 decision 端：drug-drug / allergy / dose / algorithm / order set"**
> - **"Illegible / verbal / abbreviation → CPOE"**；**"interaction / allergy / dose / pathway → CPOE + CDSS"**
> - **"CPOE 不解决：clinical judgment / cognitive bias / communication / psych safety"**

---

### 13.1 Specific Error Types 续 — 5 类补充（衍生 §4.6 扩展）⭐

### 13.1 Specific Error Types 续 — 5 类补充（衍生 §4.6 扩展）⭐

| 类型 | 含义 | 高频例子 |
|---|---|---|
| **Patient identification errors** ⭐ | 病人辨识失误 | **Mislabeling**（wrong wristband → transfusion error）/ Lack of dual validation（无 verbal verification） |
| **Device errors** | 设备使用失误 | **User-associated**: improper training, unergonomic<br>**Device-associated**: malfunction, outdated |
| **Monitoring errors** ⭐ | 监测设备 / 药物失误 | Cardiac telemetry（disconnected wires / 错设置 / **device-patient interface failure 最常见**）/ Drug monitoring（**warfarin 无 INR / vancomycin 无 trough**）/ **Alert fatigue** |
| **Documentation errors** ⭐ | 文档失误 | 不完整 / 字迹不清 / 错 patient chart / **Note bloat**（copy-paste 长 note 掩埋关键信息）/ **Propagation of outdated info**（旧 vital signs / 旧 drug doses） |
| **Procedural errors** ⭐⭐ | 操作失误 | Universal protocol 违反（wrong patient/site/procedure）/ Retained foreign bodies / Iatrogenic harm（见 §13.2） |

### 13.2 Procedural Iatrogenic Harm — 速查表 ⭐⭐⭐

CK 高频"哪个 procedure → 哪个并发症"配对题。

| Procedure | 经典 iatrogenic harm |
|---|---|
| **Paracentesis** | **Bowel perforation** |
| **Central venous / arterial line** | Arterial puncture / bleeding / **venous thrombosis** |
| **Thoracentesis** | **Pneumothorax** ⭐ |
| **Lumbar puncture** | Bleeding / **paralysis** |
| **Anesthesia** | 错剂量 / 错 agent / wrong patient |

### 13.3 Risk Factors for Medical Errors — 3 大类 ⭐⭐⭐

医疗 = complex system，error 来自**多因素交互**，不是单一个人。

#### 13.3.1 Workplace Risk Factors

| 类别 | 具体 |
|---|---|
| **Environment** | High noise / poor lighting / improper temp / severe weather / bad air / poor workspace design |
| **Technology & tools** | Ineffective comm tech / malfunctioning IT / limited tools availability |
| **Human resources / organizational** ⭐ | **Understaffing** / Scheduling errors / **Excessive workload (mismatched HCP-to-patient ratio)** |

#### 13.3.2 HCP-Associated Risk Factors ⭐⭐⭐

| 因素 | 含义 / CK stem |
|---|---|
| **Inexperienced clinician** | 经验不足 → diagnostic / judgment errors |
| **Overcommitment** | 投入过多时间精力 → **burnout** |
| **Fatigue** (sleep deprivation) | Impaired cognition → 错误判断 |
| **Alert fatigue** ⭐⭐⭐ | CDSS / 设备 alert 过多 → desensitization → ignore alerts |
| **Burnout syndrome** | 慢性 stress → 工作不满 / 错误增加 |
| **Compassion fatigue** | 长期 patient distress 暴露 → 烦躁 + 满意度下降 |

> [!warning] Alert Fatigue 解决策略 ⭐
> - 减少 clinically irrelevant alerts
> - **分级 alert severity**（不是所有 alert 都一样紧急）
> - **Forcing function 保留给 high-harm 行为**，避免过度使用（过多 = override 习惯）

#### 13.3.3 Patient-Associated Risk Factors（含 SDOH）⭐⭐

- **Extremes of age**（婴幼儿 / 老年）
- Multiple comorbidities
- Prolonged hospital stay
- Cultural factors（religious rules / gender restrictions）
- **Social Determinants of Health (SDOH)**：
  - **Low health literacy** ⭐⭐（常伴 low SES）
  - **Non-White race**
  - **Limited English proficiency**
  - **Medicaid insurance**

> [!info] CK 高频 stem
> "Older / female / non-White 病人 diagnostic error 率更高" → 答案常涉及 **implicit bias / deliberate reflection / health disparity 干预**（不是 "blame patient"）

> [!tip] SDOH 完整框架 → 跳转
> 本节只列 SDOH 作为 medical error 的 patient-side risk factor（简版）。**SDOH 5 大 Domain 完整框架 + 4 种 CK stem 模式 + 高频干预答案库 + LEP / interpreter 铁律 + Cross-cultural care 3 大支柱 + Cultural humility vs Competency** 见独立专题 → [[完整笔记/专题笔记/USMLE/USMLE_SDOH_Health_Equity]]


---

### 13.6 Human Factors Engineering (HFE) — 3 档 Reliability 分级表 ⭐⭐⭐（v1.3.3 升级 — Q19718 锚定）

**核心哲学**："Medical errors 不是 individual actions 主要造成，而是 **risk factors 间交互**的结果" — Person-focused（education）**弱于** system-focused（forcing function）。

#### HFE Reliability 3 档完整表 ⭐⭐⭐

| Reliability | Strategy | 描述 + 例子 |
|---|---|---|
| **Highest** | **Forcing functions** ⭐ | Hard stops in design / process to eliminate risk for incorrect use<br>例：anesthesia gas 各自 fit 一个 compatible socket，不可互换 |
| | **Computerized automation** | Automated processes remove human effort + variations causing error<br>例：automated vital signs monitoring；**CDSS** 见 §13.6.1 详细 |
| | **Environment & physical layout** ⭐⭐（Q19718 答案）| Workspace design facilitates correct action + minimizes error<br>例：**look-alike drugs stocked in different locations**（heparin 10 vs 1000 u/mL 分开抽屉）|
| **High** | **Standardization & simplification** | Uniform processes minimize variation / complexity / learning curve<br>例：every unit follows same heparin administration process |
| | **Human-machine redundancy** | Repetitive step to confirm correct action in error-prone process<br>例：barcode scanning + visual inspection |
| **Medium** | **Reminders, alerts & double-checks** | Processes prompting providers to check actions<br>例：drug-drug interaction alerts / time-out before procedures |
| **Less reliable**（最弱） | Training / policy changes / education | — |

> [!danger] Q19718 经典 stem — Look-alike vial 弄错浓度
> Anesthesiologist 用错 heparin vial（10 units/mL 而非 1000 units/mL）→ inadequate anticoagulation → thromboembolic stroke risk。
>
> **最有效干预 = Environmental design（B 答案）** — look-alike vials 存不同位置防 confusion。
> ❌ Device automation（A）：dynamic bolus 不像 continuous infusion 适合自动化；需 human 实时反应
> ❌ Mathematical skills（C）：本题计算实际正确（5 mL × 1000 u/mL = 5000 units）；问题在选错 vial 不在算错
> ❌ Psychological safety / Team communication（D/E）：本题是 workflow + environment 问题，不是 fear / 沟通断裂

> [!tip] 与 §三 防御金字塔的关系
> §三 是 patient safety 通用 9 层防御梯队；本表是 HFE 特定的 3 档分级 — **两者顶端等价**（forcing function = 最强）。HFE 表更细化"系统设计学派"如何分级。

> [!info] Q19718 同主题加 §13.7 "Do Not Use" 列表联动
> Look-alike / sound-alike 药 → 不仅环境分开存放（本节）也用 **Tall man lettering**（§13.7）— 两层 HFE 防御叠加最有效。

#### 13.6.1 Clinical Decision Support Systems (CDSS) 完整框架 ⭐⭐（v1.3.5 新增 — Q18754 锚定）

> [!info] 与 Cognitive诊断错误子文件 §13.5.x 互补关系
> 本节聚焦 **CDSS 在 medication error detect vs 不能 detect 的 4 类深度框架**（Q18754 锚）。
> CDSS 在 **Diagnostic Error / Cognitive Overload 干预** 中的角色 — **7 联临床形式 + 反 pattern + Alert Fatigue + HFE Tier 2-3 跨度** 见 [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Cognitive诊断错误#§13.5.x Diagnostic Error 干预匹配表 + CDSS 3 大机制 ⭐⭐⭐（v2.0 增量 — Q106049 锚定 — Linked vignette Item 2 of Q106048）|Cognitive诊断错误 §13.5.x]]。

**CDSS** = computerized tools integrated into EHR / CPOE → 在 point-of-care **prompt providers** based on patient data → reduce medical errors。

##### CDSS 完整框架 ⭐

| 维度 | 内容 |
|---|---|
| **Purpose** | • Assist providers in making clinical decisions based on patient data（lab / dx）<br>• Usually integrated into **computerized provider order entry (CPOE) systems**<br>• Recommend actions to providers based on patient clinical information |
| **Potential benefits** | • Increase **reliability** of medical decision-making（limiting harmful variations of care）<br>• Detect + intervene in cases of **human error**（entering incorrect drug dose）<br>• Reduce **medication prescription errors** |
| **Examples** | • Tool suggesting default drug dose + frequency based on **patient weight**<br>• Prompt recommending **DVT prophylaxis** in post-op high-risk surgery patient<br>• Prompt recommending **diagnostic tests for suspected PE** |

##### CDSS 能 detect vs 不能 detect — 4 类 medication error 对照 ⭐⭐⭐（Q18754 核心）

| Medication error 子类型 | CDSS 能 detect？ | 为什么 |
|---|---|---|
| **Mathematical error** ⭐（drug dose conversion / calculation 错）| ✅ **能**（Q18754 答案）| CDSS 内置 dose equivalency tables + alert 异常剂量；如 morphine 1 mg IV ≈ hydromorphone 0.25 mg IV → CDSS 知道 hydromorphone 1 mg = ~4 mg morphine，warn high dose |
| **Drug monitoring error** | 部分能 | CDSS 可 prompt INR check for warfarin，但**实际 reconciling labs / acting on results** 不在 CDSS 范围（需 provider action）|
| **Patient identification error** | ❌ **不能** | Patient ID error（wrong-patient surgery）= mislabeling / wristband 问题 → 用 **dual identifiers + barcode**（§13.1）防，不是 CDSS |
| **Mislabeling / specimen error** | ❌ **不能** | Lab specimen mislabel = preanalytical phase error → 用 **barcode + dual ID + visual inspection** 防，不是 CDSS |

##### CDSS = HFE Highest 档 Automation（§13.6 内嵌）

CDSS 属于 **Computerized automation**（HFE Highest 档第 2 个）— 减少 human effort + 自动检查 + alert pre-emptive errors。

##### CDSS 使用限制（USMLE 反 pattern 警示）⭐

> [!warning] CDSS 不是万能
> - **Alert fatigue** — 过多 alert → provider override；CDSS 设计需 prioritize high-severity alerts（§13.3.2 解决方案）
> - **不能替代 clinical judgment** — CDSS 是 decision **support** 不是 decision **maker**
> - **不能 detect physical / workflow errors**（如 wrong site surgery / specimen mislabel）— 这些需 forcing function / time-out / 2 identifiers
> - **依赖正确数据 input** — garbage in, garbage out（错的患者体重 → CDSS 给错剂量推荐）

##### Q18754 钓饵分析

| 选项 | 为什么 |
|---|---|
| **A. Drug monitoring error** ❌ | CDSS 可 prompt 查 INR / vanco trough，但**重点是 prompt，不是 detect 已发生的 monitoring lapse**；本题 stem 是 conversion error（mathematical），不是 monitoring |
| **B. Mathematical error** ✅ 正解 | CDSS 内置 morphine→hydromorphone 4:1 equivalency → alert 高剂量；本 case 完美 fit |
| **C. Mislabeling error** ❌ | Mislabeling 是 specimen / wristband 错 → 需 **dual identifiers + barcode**，不是 CDSS 范围 |
| **D. Patient identification error** ❌ | 同上 — patient ID 错需 dual ID + barcode；CDSS 是基于 patient data 推荐，不验证 patient identity |

##### 一句话锁

> [!success]
> 「**CDSS = HFE Automation 档；最擅长 detect mathematical / drug dose error；不能 detect patient ID / mislabeling**」
> 「**CDSS 配 CPOE 用 — Computerized Provider Order Entry 提供平台**」
> 「**Q18754 stem morphine→hydromorphone 4:1 conversion → CDSS 在 prompt alert mathematical conversion error**」

### 13.7 Tall Man Lettering + "Do Not Use" Abbreviations ⭐⭐⭐

#### Tall Man Lettering
**目的**：让 look-alike / sound-alike 药名视觉区分（大写关键不同字母）。

经典例子：
- **DOBUTamine vs DOPamine** ⭐⭐
- **amILOride vs amLODipine**

#### "Do Not Use" Abbreviations List（The Joint Commission）⭐⭐⭐

| 缩写 | 问题 | 替代 |
|---|---|---|
| **U / IU** | 看成 "0" 或 "IV"（10U → 100 / 10IV）| 写 "units" |
| **QD / QOD** | 互相混淆（每天 → 隔天 / 每天 4 次）| 写 "daily" / "every other day" |
| **MS / MSO4** | morphine vs MgSO4 混淆 | 写全名 |
| **MgSO4** | 看成 morphine sulfate | 写 "magnesium sulfate" |
| **Trailing zero** (1.0 mg) ⭐⭐ | 看成 "10 mg" → **10 倍剂量** | 写 "1 mg" |
| **Lack of leading zero** (.1 mg) ⭐⭐ | 看成 "1 mg" → **10 倍剂量** | 写 "0.1 mg" |

> [!danger] CK 经典 stem
> Trailing zero / lack of leading zero → **transcription error** → **10 倍剂量错误**（high-yield 题型）

### 13.8 Medication Reconciliation + Teach-Back + Prescribing Cascade

#### 13.8.1 Medication Reconciliation 升级（衍生 §8.1）⭐

**Transition of care**（admission / transfer / discharge）必做。

**4 步**：
1. Identify previous medications（**入院问"上次什么时候吃药"** → 正确 timing 下新 order）
2. Compare 新旧 list → identify discrepancies
3. 评估每个 med：continue / discontinue / dose-adjust / restart
4. 创建新 list + 文档化 reasons

> [!warning] 陷阱
> Transfer / discharge 时**回头核对 home med list**（入院时记录的）— 否则**家用药漏掉**。

#### 13.8.2 Teach-Back Method ⭐⭐

**核心**：让病人**复述**理解 — **不是**问 "Do you understand?"。

- Limited health literacy → 高 med error risk
- Simple language + ask to summarize → 纠错
- 提供 **dose aids**（pill box / blister pack）
- **黄金问法**："**What questions do you have for me?**"（而非 "Do you have any questions?"）

#### 13.8.3 Prescribing Cascade ⭐⭐

**定义**：药物副作用**误认为新疾病** → 加新药 → 新副作用 → 又加新药 → 循环。

**经典 cascade 3 例**：
- **NSAIDs → hypertension → antihypertensive treatment** ⭐
- **Thiazide diuretics → hyperuricemia → gout treatment**
- **Antipsychotics → parkinsonism → antiparkinson medication**

**Prevention**：保守 prescribing / **brown bag review**（让病人带所有药来）/ 出现新症状先问 "是新药副作用吗" / 识别 ADE → 停 / 换药，不加新药。

### 13.9 Hospital-Acquired Conditions (HACs) ⭐

**定义**：住院期间新发、入院时不存在的状况；多数 preventable。**2008 起 CMS 不报销 HACs** → 强制 evidence-based 预防。

| HAC | 核心预防 |
|---|---|
| **CAUTI** | 减少不必要 catheter + 早拔 |
| **CLABSI** ⭐ | Sterile insertion bundle + 早拔；**ID 完整体系**（病原体 / 诊断 DTP / 5 必拔 / 疗程 / HAC 政策）→ [[完整笔记/专题笔记/感染/感染_CLABSI完整体系]]；**预防 bundle 详解** → [[完整笔记/专题笔记/USMLE/USMLE_侵入操作安全流程#5.2.3a CLABSI 预防 Bundle ⭐⭐⭐（USMLE 高频）]] |
| **VAP** | Head-of-bed 30° + 口腔护理 + 早脱机 |
| **SSI** | Pre-op abx + skin prep + normothermia |
| **C. difficile** | 谨慎 abx + isolation + **手卫生用 soap+water**（alcohol gel 无效） |
| **Decubitus ulcers** | 翻身 / 减压 / 营养 |
| **VTE** | Risk-based prophylaxis |
| **Falls** | Tailored individual risk factors → 干预 menu；**首选 direct supervision**（1:1 sitter / 视线内 room）；❌ **反 pattern**：bed alarms（alert fatigue）+ 4-side bed rails（climb over）+ physical restraints（resist 摔重）+ 夜间 bright lighting（worsens delirium）— **详见 §13.9.1**|
| **OB adverse events** | Standardized HTN / hemorrhage protocols + safe oxytocin/MgSO4 + C/S **time-out** |

#### 13.9.1 Inpatient Falls Prevention Deep Dive ⭐⭐⭐（v1.3.13 — Q107149 + Q107152 + Q107151 三连）

> [!info] 为什么单独开节
> §13.9 表里 Falls 一行原本简化为"床栏 + 灯光" — **直接错**：4-side rails + bright nighttime lighting 实际都是 anti-patterns。需要单独详解。

##### Inpatient Falls Prevention Hierarchy ⭐（高 risk + delirium）

```
优先级排序：
1. ⭐ Close direct supervision（人 > 机器）
   ├─ 1:1 sitter（dedicated sitter / family at bedside）
   ├─ 视线内 room（nursing station 对面 / 房门开）
   └─ 频繁 nursing checks（每 15 min）
2. Frequent supervised toileting（hourly）
   └─ ❌ 不让 high-risk 独用 bedside commode
3. Optimize room environment
   ├─ Low bed（地板式 / 床矮）
   ├─ Minimize furniture（清通道）
   └─ Lighting: day bright, night dim ⭐（delirium 夜亮扰 sleep-wake）
4. ❌ AVOID 反 pattern
   ├─ Bed alarms（alert fatigue + 响时已摔）
   ├─ Physical restraints（wrist / vest — resist 摔更重）
   └─ Bed rails 4 侧（climb over → 摔更高）
```

##### 3 大反 pattern + 反 evidence 理由（CK 高频钓饵）⭐⭐⭐

| 反 pattern | 看起来合理 | 实际 evidence | Q 锚定 |
|---|---|---|---|
| **Bed alarm** | "Early warning system" | **无 evidence reduce falls**：alert fatigue（太多假警报）+ 响时已摔（反应慢于跌倒）| Q107149 + Q107152 双锚 |
| **Bed rails 4-side** | "防止患者下床" | Patients **climb over** → 摔得更高更重；只用辅助 reposition（最多 2 侧）| Q107149 |
| **Physical restraints** | "限制活动 = 安全" | Patients **挣扎抵抗** → fall + injury 反而 ↑；仅用于明确危险（暴力 / 拔管）| Q107149 |
| **Bright lighting at night**（delirium）| "看清楚 = 安全" | 扰乱 sleep-wake cycle + 加重 agitation → 间接增 fall | Q107149 |

##### Tailored vs Standardized 策略（Q107152 锚定）⭐⭐⭐

| 维度 | One-size-fits-all（错）| Tailored / 个体化（对）|
|---|---|---|
| **触发** | 单一 quantitative score → 同一套干预 | 多维 risk assessment → menu 选 intervention |
| **High prev 群表现** | 80% 都 high-risk → 同一套 = 资源稀释 + 无 discriminate | 同 80% 但每人不同 risk → 不同 intervention |
| **Visual cues / wristbands** | 80% 都贴 = 失效 | 只贴 true high-risk = 有效 |
| **Evidence** | Quantitative score 在 high prev 群 PPV 低 | Multidisciplinary qualitative assessment 优 |

##### Q107151 连锁：Screening Tool 在 High Prev 群的局限

**为什么 quantitative fall risk score 在 geriatric 大量人群里效用低**：

```
High pretest probability（geriatric population fall prevalence 高）
   │
   ▼
Quantitative score（"高/低"二分）→ 80% classify 阳性
   │
   ▼
PPV 低（high-risk 群里真摔的比例不高 ≈ 11.5/1000）
+ Specificity 低（high false-positive）
   │
   ▼
后果：① alert fatigue（staff 不当真）② resource dilution（资源平摊到 80% 人）
   │
   ▼
Solution（Q107152）：tailored multidisciplinary qualitative assessment > quantitative score
```

##### AMBOSS Falls in Older Adults 速查表（背）

| 维度 | 内容 |
|---|---|
| **Overview** | Leading cause of injury / morbidity / mortality in elderly |
| **Risk factors** | History of fall / sensory + cognitive disturbance / chronic disease (T2DM/arthritis/CVD) / medications (neuroleptics/antidepressants/vasodilators) |
| **Outpatient prevention** | Screen: "**Get up & go**" test ⭐ + vision + hearing + bone density + orthostasis；medication review；vit D 补充；supervised exercise |
| **Inpatient prevention** | Assess fall risk + **tailor** strategies；optimize environment；frequent checks high-risk；**避免 restraints + alarm over-reliance** |

##### Memory Hook

> [!tip] Falls 反射钩
> - **"摔倒预防 = 人看着 > 机器叫"** ⭐⭐⭐ — Direct supervision > bed alarm（alert fatigue + 太晚）
> - **"3 不要"**：不要 bed alarm / 不要 4-side rails / 不要 restraints — 看着合理实际增加 falls
> - **Delirium 灯光**："Day bright, night dim" — 夜亮反加重 agitation
> - **High prev 群 + quantitative score = 低 PPV** → tailored 个体化优于一刀切
> - **"80% 都贴 = 失效"** — visual cues / wristbands 需要 minority 才有 discrimination value

---

## §13.6.x Human Factors Engineering — 3 机制 + Point of Care + Adherence 效力排序 ⭐⭐⭐（v2.0 增量 — Q106819 锚定）

> [!danger] 核心铁律
> **HFE = process design minimize human effort for correct action。Visual aids at point of care（brightly colored signs outside patient rooms）通过 ① optimize environmental design + ② reduce reliance on memory + ③ increase attention via alerts 改善 adherence — 比 passive training / 比 patient-driven advocacy / 比 supply at central location 更 effective。**

### 13.6.x.1 HFE 3 大机制

1. **Optimize environmental design** — sign at room door = relevant info immediately prior to patient contact
2. **Reduce reliance on memory** — sign specifies protocol details（不靠脑记）
3. **Increase attention via alerts** — brightly colored + strategically placed

### 13.6.x.2 Point of Care 原则 ⭐

> [!warning] 所有 infection control 资源应**就近 patient room**
> 反 pattern：放 central workstation / single location / break room → 离 use point 远 → adherence 差

### 13.6.x.3 Adherence Strategies 效力排序 ⭐⭐⭐

| 策略 | 主动/被动 | 效力 |
|---|---|---|
| **Visual aids at point of care** ⭐ | 主动 + environmental | 最强 |
| Equipment at point of care（hand sanitizer outside each room）| 主动 + environmental | 强 |
| Patient advocacy / asking providers | 被动（依赖 patient capacity）| 弱 |
| Repeated mandatory training | **被动 + add burden** | 弱 |
| Equipment at central workstation | 错位置 | 反向 |

### 13.6.x.4 Environmental Design > Training when Guidelines Exist 铁律 ⭐

- **Education / training** = passive；只在 knowledge deficiency 时有效
- **Environmental design** = active；改变行为 default
- 当 stem "guidelines 已 established 但 adherence 差" → 不是 knowledge 问题，是 design 问题 → **选 environmental，不选 training**

### 13.6.x.5 Isolation Precautions 4 类速查（HFE 配套 — 视觉提示内容）

| Type | Pathogens | Key Requirements |
|---|---|---|
| **Airborne** | TB / primary VZV / disseminated VZV / VZV in immunocompromised / COVID-19 / measles | **Negative pressure room + N95** |
| **Contact** | MDR (MRSA / VRE / ESBL) / C diff / E coli O157:H7 / RSV / VZV | Gloves + gowns + single-use equipment |
| **Droplet** | Neisseria meningitidis / Hib / Mycoplasma / influenza / adenovirus | Mask within 1-2 m (3-6 ft) |
| **Standard** | All patients regardless of infection | Hand hygiene + appropriate PPE when needed |

---

## §13.8.x Patient-Centered Medication Counseling — 4 法 + Sound-alike Trap + ADE 3 维 ⭐⭐⭐（v2.0 增量 — Q19788 锚定）

> [!danger] 核心铁律
> **Teach-back（让患者用自己话 describe changes）是最强工具 → 直接 detect miscomprehension，特别防 sound-alike drugs（Glucovance/Glucophage 经典 trap）。** "Ask if questions" 是被动反 pattern。

### 13.8.x.1 Patient-Centered Counseling 4 法（效力排序）⭐

| 方法 | 主动 vs 被动 | 效力 |
|---|---|---|
| **Teach-back** ⭐⭐⭐ | 主动 | 最强 — 患者用自己话 describe 理解 → detect miscomprehension |
| **Plain-language**（drug names / indication / dose / frequency）| 主动 | 强 |
| **Medication reconciliation**（multi-provider checkpoints）| 主动 | 强 — 防 omission |
| "Ask if any questions" | **被动** | 弱 — 患者不知该问什么；通常答 "no" |

### 13.8.x.2 ADE Risk Factors 3 大维度 ⭐

| 维度 | Risk Factors | Corrective Strategies |
|---|---|---|
| **Patient** | Polypharmacy / Low health literacy / Very young or advanced age / Communication barriers / Nonadherence | Increased checkpoints in med reconciliation + plain-language counseling + teach-back |
| **Provider** | Vague Rx / Incorrect med reconciliation / Absence of counseling / Illegible handwriting | Standardize Rx + e-prescribing + counseling |
| **Medication** ⭐ | **Look-/sound-alike drugs**（Glucovance/Glucophage / prednisone-prednisolone / hydroxyzine-hydralazine）| Plain-language counseling + teach-back + tall-man lettering |

### 13.8.x.3 Sound-alike Drug Trap 高频对 ⭐

| Pair | 关键区别 | Risk |
|---|---|---|
| **Glucovance vs Glucophage** ⭐ | Glucovance 含 sulfonylurea → 致 hypo；Glucophage = metformin only | 老人 advanced age + low health literacy 高 hypo 风险 |
| **Prednisone vs Prednisolone** | Prodrug vs 活性形式（经肝转换）| 处方混淆 |
| **Hydroxyzine vs Hydralazine** | 抗组胺 vs vasodilator | 完全不同适应症 |

### 13.8.x.4 Teach-back 强制场景（反射触发）

```
Stem 出现 → 0.3 秒锁 teach-back
─────────────────────────────────────────────
出院 + medication change + 老人              → teach-back
Sound-alike drug                             → teach-back
低 health literacy + 复杂新治疗方案          → teach-back
住院 → 门诊 transition + polypharmacy        → teach-back
```

### 13.8.x.5 "Cognitively Intact → Direct Engagement" 原则 ⭐

- **Cognitively intact + 独立**患者 → **direct engagement 优先**
- Family member 介入条件 = patient cognition / functional status impaired
- 反 pattern：cognitively intact 患者 family 主导 counseling → 错位

### 13.8.x.6 反 Pattern 速排

| 选项 | 为什么错 |
|---|---|
| "Ask if questions at end" | 被动 — 患者不知该问 |
| "Avoid combination drugs" | 错 — combination 增 adherence + convenience，不应一概避免 |
| "Family member present"（in cognitively intact patient）| direct engagement 优先 |
| "Printed copy of discharge summary" | 被动 — 患者可能不读 / 不理解 |

---

## §13.9.x Fall Secondary Prevention + Multifactorial 7 维（v2.0 增量 — Q107154 + Q107171 锚定）⭐⭐⭐

> [!info] 完整版见 [[完整笔记/专题笔记/USMLE/USMLE_老年Fall3层防护]]
> 本节是 §13.9 HAC Falls 的拓展 — Fall 4 题成体系（Q107151/Q107152/Q107154/Q107171）已建独立衍生 [[完整笔记/专题笔记/USMLE/USMLE_老年Fall3层防护]]。本节保留 §13.9 视角速查 + Patient Safety 框架挂钩点。

### 13.9.x.1 老年 Fall 3 层防御 ⭐⭐⭐

| 层级 | 目标 | 关键干预 |
|---|---|---|
| **Primary**（防 fall 发生）| 减 fall 频率 | Exercise + home safety + medication review + vision-hearing + vitamin D |
| **Secondary**（减 fall 后 serious injury）⭐ | 减 hip fracture | **FRAX → DEXA → bisphosphonate**（10-yr fracture risk >2.5%）|
| Tertiary（fall 后 recovery）| 恢复功能 | PT / OT rehab |

> [!info] **PT vs OT 缩写**（Fall 防护中角色）
> - **PT = Physical Therapy（物理治疗）** — gait / balance / strength → Fall 防护中负责 balance training + supervised exercise + cane-walker 训练
> - **OT = Occupational Therapy（作业治疗）** — ADL（穿衣/洗澡/做饭/上厕所）+ **home safety assessment** ⭐ + adaptive equipment
> - **Primary**：OT 主导 home safety；**Tertiary**：PT + OT 联合 rehab
> - 详见 [[完整笔记/专题笔记/USMLE/USMLE_老年Fall3层防护]] §2.1 PT vs OT 完整对照表

### 13.9.x.2 Multifactorial Risk Assessment 7 维矩阵 ⭐

| 维度 | 评估 | 干预 |
|---|---|---|
| **Vision** ⭐ | Visual acuity + dilated eye exam | Corrective eyewear + cataract surgery |
| Hearing | Audiometry | Hearing aids |
| Proprioception / Balance | Get-up-and-go test | PT balance training |
| Strength | Manual muscle testing | Supervised exercise + PT |
| Medication review | Polypharmacy + 高 risk drugs | Deprescribe |
| Home safety | OT 评估 | 修缮 |
| **Bone density** ⭐ | FRAX → DEXA | Bisphosphonate（secondary injury prevention）|

### 13.9.x.3 反 Pattern 4 联 ⭐⭐⭐

| 反 pattern | 为什么无效 |
|---|---|
| **Call alarm / bed alarm**（universal）| 严重 fall injuries（LOC / fracture）患者**无法激活** + 80% 都贴 = 失效（Q107152 + Q107154 同源 2 次踩 → 🔴）|
| **Wearable hip protector** | 依从性极差 → multiple studies 无 fracture risk 减少 |
| **Discontinue anticoagulation 防 SDH** | AF stroke 风险 ≫ fall-related SDH 风险 — 不停 |
| **Cane / walker for fear of fall** | 反而 higher fall risk（被 device 绊倒）— 除非 PT 训练后 |

### 13.9.x.4 关键铁律

- **"Reduce SERIOUS fall-related injury" = reduce hip fracture = optimize bone density**（永远）
- **AF + fall = 不停抗凝**（stroke ≫ SDH）
- **Orthostasis 定义** = sitting → standing BP 差 **≥20/10 mmHg**（142/87 → 141/79 = 不算 → 不停 ACE）
- **保 Independence 原则**：先 screen correctable，最后才 facility / assisted living
- **"Primary 已做 → 切 secondary"思维模型**（不要重复选 primary 项）

### 13.9.x.5 Vision = Fall 关键 Contributor 机制

```
Age-related decline
  ├─ Proprioception ↓
  └─ Balance ↓
       ↓
依赖 visual input ↑
       ↓
若 visual acuity ↓（cataract / macular degen）
       ↓
Fall risk substantially elevated（尤其暗处 / 夜起厕所）
```

---

## 🔗 关联

- 🔁 **同主题错题**（聚焦 HFE + 药物 + HAC）：
  - [[mistakes/uworld-mistakes#^Q19788]] Patient-Centered Counseling + Glucovance/Glucophage sound-alike + teach-back（5-27 做对）
  - [[mistakes/uworld-mistakes#^Q106819]] Human Factors Engineering + 视觉提示（5-27 做对）
  - [[mistakes/uworld-mistakes#^Q22186]] Surgical Safety + 患者参与 site verification（5-27 错）
  - [[mistakes/uworld-mistakes#^Q107151]] Fall screening tool low PPV（5-26 做对）
  - [[mistakes/uworld-mistakes#^Q107152]] Tailored fall prevention + bed alarm 反 pattern（5-26 错）
  - [[mistakes/uworld-mistakes#^Q107154]] Fall secondary prevention + bone density + call alarm 反 pattern（5-27 错 🔴）
  - [[mistakes/uworld-mistakes#^Q107171]] Fall + visual acuity + multifactorial 7 维（5-27 做对）
  - [[mistakes/uworld-mistakes#^Q19718]] HFE 5 methods 3 档分级 + Q105825 standardization 锚
  - [[mistakes/uworld-mistakes#^Q20431]] Prescribing Cascade + home health care
- 📚 **配套子文件**：
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_QI工具]]
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Safety文化与沟通]]
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全_Cognitive诊断错误]]
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]]（主索引）
- 📚 **主笔记 / 跨学科**：
  - [[完整笔记/Peixuan分科笔记/Ethics_Master]]
  - [[完整笔记/专题笔记/USMLE/USMLE_老年Fall3层防护]]（Fall 4 题成体系完整版 — 与本 §13.9 互补）
  - [[完整笔记/专题笔记/USMLE/USMLE_易混药物对照]] §2（sound-alike drugs — 与 §13.7 Tall Man 互补）
  - [[完整笔记/专题笔记/psych/psych_医患沟通对话术SOP]] Part 9（Medication Counseling 4 法 — 与 §13.8 Teach-back 互补）
  - [[完整笔记/Peixuan分科笔记/感染]] / [[完整笔记/专题笔记/感染/感染_CLABSI完整体系]]（§13.9 HAC 互补）
