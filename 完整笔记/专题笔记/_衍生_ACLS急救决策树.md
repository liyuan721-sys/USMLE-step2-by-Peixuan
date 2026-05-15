---
tags:
  - USMLE-Step2
  - 心血管
  - 急诊
  - 专题笔记
created: 2026-05-14
type: 专题笔记
parent_topic: ACLS 心脏骤停急救决策树 + 4 节律 + 5H5T + 三种电击
source_错题: Q4725
---

# _衍生_ACLS 急救决策树（Advanced Cardiac Life Support）

> [!info] 本笔记定位
> **心脏骤停 + 不稳定心律失常的急救决策枢纽**。
> - USMLE Step 2 CK 急救场景高频考点
> - 核心思维：**"先看脉搏，后看节律"** — 脉搏决定治疗，节律决定诊断
> - 与 [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] 互补：本笔记讲**急救流程**，Vaughan 讲**药物对照**
> 
> **来源**：错题 Q4725（PEA 房颤）+ 后续 VF / Asystole / 不稳定心律失常 / ROSC 题积累

---

## Part 0. 核心方法论

### 0.1 "V 除颤，P/A 按压" 二分铁律 ⭐⭐⭐

> [!success] 4 字诀
> **"V 除颤（VF + 无脉 VT），P/A 按压（PEA + Asystole）"**
> - V = **V**entricular（VF + 无脉 VT）→ 电击有效
> - P/A = **P**ulseless / **A**systole → 电击无用，按压 + Epi + 找原因

### 0.2 "先脉搏，后节律" ⭐⭐⭐

> [!danger] 关键反陷阱
> 看到 stem 给节律（房颤 / 窦律 / 缓慢律），**先停下来**问：**有脉吗？**
> - **节律决定诊断**（VF / PEA / Asystole）
> - **脉搏决定治疗**（电击 vs CPR + Epi）

### 0.3 PEA 经典比喻

> [!tip] PEA = 电话有铃声但没人接
> - 监护仪显示节律 = 铃声
> - 心肌不收缩 = 没人接
> - **电击没用**（电铃声的电话没意义）
> - 治疗 = 找"为什么没人接"（5H5T）+ 持续敲门（CPR）+ 唤醒剂（Epi）

---

## Part 1. 心脏骤停 4 种节律对照表 ⭐⭐⭐

### 1.1 完整对比

| 节律 | ECG 特征 | 脉搏 | 处理 | 是否除颤？|
|---|---|---|---|---|
| **VF**（Ventricular Fibrillation 室颤）| 完全混乱波形，**无 QRS** | 无 | CPR + **除颤** + Epi | ✓ **是** |
| **Pulseless VT**（无脉室速）| 宽 QRS 规整 / 多形 | 无 | CPR + **除颤** + Epi | ✓ **是** |
| **PEA**（Pulseless Electrical Activity）| **任何有形节律**（窦律 / 房颤 / 缓慢 / etc）| **无** ★ | CPR + Epi + 5H5T | ❌ **否** |
| **Asystole**（停搏）| **直线**（必须确认 2 导联避免误判）| 无 | CPR + Epi + 5H5T | ❌ **否** |

### 1.2 ECG 识别细节

> [!info] Asystole 确认要点
> 真 asystole **必须 2 导联确认** — 单导联直线可能是导联脱落 / 电极接触不良 / fine VF 被误判。

> [!info] PEA 范围
> PEA = "电活动 + 无脉" 的统称，**包括所有非 VF / 非 VT 的节律**：窦律 / 房颤 / 房扑 / 缓慢律 / 不规则律 / agonal rhythm 全算。

---

## Part 2. 完整 ACLS 算法

**UWorld 官方流程图**（本地截屏）：

![[{D20DE2F4-B2B2-475A-8530-4F4B105CE8BD}.png]]

> [!info] 图示读法
> - **左路 VF / 无脉 VT**：CPR → **除颤** → 继续 CPR + IV/IO + Epi q3-5 min → rhythm check → 仍 shockable → 再除颤（第 3 次后加 **Amiodarone**）→ ROSC
> - **右路 PEA / Asystole**：CPR → 不除颤 → IV/IO + Epi q3-5 min + **找 5H5T** → rhythm check → 若变 shockable rhythm → 走左路
> - **两路汇合**：每 2 min check pulse & rhythm + treat reversible causes → 直到 ROSC
> - **★ Amiodarone 注脚**：仅在 **第 3 次除颤后** 给（300 mg → 150 mg）
> 
> 🔗 详见 [[mistakes/uworld-mistakes#^Q4725]]

### 2.1 文字版总流程

```
心脏骤停（无意识 + 无脉 + 无呼吸 / agonal）
        │
        ▼
   立即 CPR + 给氧 + 连监护
   30:2（按压 : 通气）
   100-120 次/分，深度 5-6 cm
        │
        ▼
   评估节律（每 2 min）
        │
   ┌────┴────────────────────┐
   ▼                          ▼
可除颤 (VF / pulseless VT)  不可除颤 (PEA / Asystole)
   │                          │
   ▼                          ▼
1. Defibrillation 200J 双相  1. CPR x 2 min
2. CPR x 2 min                2. IV / IO access
3. IV / IO access             3. **Epi 1 mg q3-5 min**
4. **Epi 1 mg q3-5 min**      4. Treat reversible (5H5T)
   │                          │
   ▼                          ▼
重新评估节律                重新评估节律
   │                       （ROSC? 或继续 CPR？）
   ▼
仍 VF? → 再除颤
+ Amiodarone 300 mg（第 3 次除颤后）
+ Lidocaine（替代）
   │
   ▼
ROSC → 复苏后管理（targeted temp / 心导管 / ICU）
```

### 2.2 高质量 CPR 关键参数

| 参数 | 标准 |
|---|---|
| **按压频率** | 100-120 次 / min |
| **按压深度** | 5-6 cm（成人）|
| **按压：通气** | **30 : 2**（未插管）;  插管后持续按压，10 次/min 通气 |
| **rhythm check 频率** | **每 2 min** 一次（不超过 10 秒）|
| **switch compressor** | 每 2 min 换人（避免疲劳） |
| **ETCO2 监测** | > 10 mmHg 提示有效；ROSC 时突增 |

### 2.3 "见骤停先做什么"决策序列

```
1. 确认无反应 → 喊救命 + 启动 code blue
2. 检查 pulse + breathing（≤ 10 秒）
3. 启动 CPR（30:2）
4. 接 AED / 监护仪 → 评估节律
5. 评估节律后按 2.1 流程
```

---

## Part 3. 5H5T 可逆因（PEA / Asystole 必找） ⭐⭐⭐

### 3.1 完整清单

| H（5 个）| T（5 个）|
|---|---|
| **H**ypovolemia 低血容量 | **T**ension pneumothorax 张力气胸 |
| **H**ypoxia 低氧 | **T**amponade (cardiac) 心包填塞 |
| **H**ydrogen ion 酸中毒 | **T**oxins 毒物（CCB / β-B / TCA / 阿片 / 可卡因）|
| **H**ypo / Hyperkalemia 钾异常 | **T**hrombosis (Pulmonary) 肺栓塞 |
| **H**ypothermia 低温 | **T**hrombosis (Coronary) 冠脉栓塞（MI）|

### 3.2 每个可逆因的针对性处理

| 可逆因 | 识别 stem 关键词 | 处理 |
|---|---|---|
| **Hypovolemia** | 出血史 / 烧伤 / 严重脱水 / 低 CVP | **IV 补液**（晶体 + 血制品如失血）|
| **Hypoxia** | COPD / 哮喘急性 / 窒息 / 溺水 | 高流量氧 + 气道管理 |
| **H+ 酸中毒** | DKA / 肾衰 / 严重休克 / pH < 7.1 | **NaHCO3** + 治原因 |
| **高 K** | 透析患者 / CKD / 横纹肌溶解 / TLS | **Ca + insulin + glucose + Kayexalate + 透析** |
| **低 K** | 利尿剂 / 呕吐腹泻 | 补 K + Mg |
| **Hypothermia** | 暴露史 / 溺水 / 老人 | **复温**（"不死直到温暖死"）|
| **Tension pneumo** | 创伤 / 机械通气 / 气管偏 | **针刺减压** 2-3 IS midclavicular |
| **Tamponade** | 尿毒症 / 创伤 / 抗凝 / 主动脉夹层 | **心包穿刺** subxiphoid |
| **Toxins** | 中毒史 / 用药史 | 解毒剂（Naloxone / Flumazenil / Glucagon / NaHCO3 for TCA / Insulin for CCB）|
| **PE** | DVT / 长期卧床 / 高凝 | **tPA 溶栓** |
| **MI** | 胸痛先发 / CAD 史 | **心导管 / PCI** |

### 3.3 高频考点：哪些可逆因有特异治疗

> [!success] 4 个"想到立刻做"特异处理
> - **张力气胸** → 针刺减压（不等 CXR）
> - **心包填塞** → 床旁 echo → 心包穿刺
> - **PE 不稳** → 床旁 TTE → tPA
> - **高 K** → Ca + insulin + glucose

---

## Part 4. ACLS 用药速查 ⭐⭐⭐

### 4.1 主要用药

| 药 | 剂量 | 用途 | 时机 |
|---|---|---|---|
| **Epinephrine** | **1 mg IV / IO q3-5 min** | **所有 4 种骤停节律** ⭐ | 越早越好（不可除颤节律立即给；可除颤节律首次除颤后给）|
| **Amiodarone** | 300 mg IV bolus → 150 mg | VF / 无脉 VT | **第 3 次除颤后** |
| **Lidocaine** | 1-1.5 mg/kg | VF / 无脉 VT 替代 | Amio 替代（资源 / 过敏）|
| **Magnesium** | 1-2 g | **Torsades de Pointes** | 任何时间，不论血 Mg |
| **Atropine** | 1 mg q3-5 min（max 3 mg）| **症状性窦缓 / AV 阻滞**（**有脉**）| ❌ **不用于 asystole**（2010 AHA 移除） |
| **NaHCO3** | 1 mEq/kg | 严重酸中毒 / 高 K / TCA 中毒 | 选择性，不常规 |
| **Calcium** | 1 g IV | 高 K / CCB 中毒 / 低 Ca | 选择性 |

### 4.2 复苏后管理用药（ROSC 后）

| 药 | 用途 |
|---|---|
| **Norepinephrine / Epi 输注** | 维持 MAP ≥ 65 mmHg |
| **Amiodarone 维持** | 预防 VF 复发 |
| **Targeted Temperature Management** | 32-36°C × 24h（昏迷患者，防神经损伤）|

### 4.3 反陷阱：什么药 USMLE 不要选

> [!danger] ACLS 常见错误选项
> - ❌ **Atropine for asystole**（2010 移除）
> - ❌ **Lidocaine for PEA**（Lidocaine 只用于 VF / 无脉 VT）
> - ❌ **NaHCO3 常规**（除非证据明确：高 K / 严重酸 / TCA）
> - ❌ **Amio 第一次除颤就给**（必须第 3 次除颤后）
> - ❌ **Procainamide 急性 VF**（IA 类，复苏中不用）

---

## Part 5. 三种"电击方式"对比 ⭐⭐⭐

> [!warning] USMLE 最易混
> Defibrillation / Synchronized Cardioversion / Pacing 完全不同，混了 = 致命。

| 维度 | **Defibrillation**（除颤）| **Synchronized Cardioversion**（同步复律）| **Pacing**（起搏）|
|---|---|---|---|
| 同步 R 波？| **否** | **是** | — |
| 能量 | 高（200J 双相 / 360J 单相）| 低（50-200J 递增）| 低脉冲 |
| **脉搏要求** | 必须**无脉** | 必须**有脉** | 有脉（缓慢）|
| **意识** | 无 | 通常需镇静 | 清醒 |
| **适应症** | **VF / 无脉 VT** | **有脉**的不稳定 SVT / 房颤 / 房扑 / 单形 VT | 症状性窦缓 / 高度 AV 阻滞 |
| 危险性 | 必须，不电就死 | 不同步 + 有脉 → 误击在 T 波 → **VF** | 一般安全 |

### 5.1 "同步"的意义

> [!info] 为什么同步那么重要？
> 心动周期里有个**易损期**（T 波）— 电击落在这里会诱发 VF。
> - **VF / 无脉 VT 已经没节律可同步** → 直接除颤
> - **有脉患者**有节律 → 必须同步到 R 波避开 T 波 → 用 Synchronized Cardioversion

### 5.2 起搏（Pacing）适应症

| 类型 | 适应症 |
|---|---|
| **Transcutaneous Pacing (TCP)** | 急救：症状性窦缓 / Mobitz II / 完全 AVB / Atropine 失败 |
| **Transvenous Pacing (TVP)** | 短期过渡：TCP 后维持，等永久起搏器 |
| **Permanent Pacemaker (PPM)** | 永久：症状性窦缓 / 完全 AVB / 双束支 + 晕厥 |

---

## Part 6. 心律失常急救三分类决策树

```
Step 1: 患者有脉吗？
   │
   ┌────┴────┐
   无脉      有脉
   │         │
   ▼         ▼
Step 2a:   Step 2b: 血流动力学稳定？
评估节律     │
   │      ┌──┴──┐
   ▼     稳定   不稳定
┌──┴──┐   │       │
VF/VT  PEA/  ▼       ▼
除颤   Asys 抗心律失常  Synchronized
       CPR  药         Cardioversion
            (按节律类型)  （任何不稳的房颤 / SVT /
                          单形 VT 都用同步）
```

### 6.1 "稳定 / 不稳定"判定（高频）

> [!warning] 任 1 条即"不稳定"
> - **SBP < 90** 或灌注差
> - **意识改变**
> - **持续胸痛 / 缺血表现**
> - **急性心衰**
> - 任 1 条满足 → **不稳定** → 立即同步复律（不再药物）

### 6.2 稳定患者的抗心律失常药选择

| 节律 | 一线 |
|---|---|
| SVT（窄 QRS 规整）| Vagal → **Adenosine IV push** |
| 房颤 / 房扑 控率 | β-blocker / Diltiazem |
| 房颤 / 房扑 律转 | **Amiodarone** / 电复律（择期） |
| 单形 VT 稳定 | **Amiodarone** / Lidocaine |
| 多形 VT（TdP）| **Magnesium** |
| WPW + AFib | **Procainamide / Ibutilide**（**禁** AV 结阻滞剂）|

---

## Part 7. "看到房颤" 答题决策树 ⭐⭐⭐

```
看到 stem 提到房颤 → 必须先问：

1. 有脉吗？
   - 无脉 → PEA → CPR + Epi（不电击！）★ Q4725 陷阱
   - 有脉 → 继续

2. 血流动力学稳定吗？
   - 不稳定（低 BP / 意识 / 胸痛 / 心衰）→ Synchronized Cardioversion
   - 稳定 → 继续

3. WPW 患者？
   - 是 → Procainamide / Ibutilide / 电复律
       **禁用 AV 结阻滞剂**（β / CCB / Adenosine / Digoxin → VF）
   - 否 → 率控（β / Diltiazem）或律转（amiodarone / 择期 cardio）

4. 长期管理：
   - CHA2DS2-VASc 评分 → 抗凝（Apixaban / Warfarin 机械瓣）
```

---

## Part 8. ROSC 后管理（Post-Cardiac Arrest Care）

### 8.1 立即处理 4 步

```
1. 优化氧合 + 通气
   - SpO2 目标 92-98%（避免高氧 → 神经损伤）
   - ETCO2 目标 35-45 mmHg

2. 血流动力学支持
   - MAP ≥ 65 mmHg
   - IV fluid + Norepinephrine / Epi 输注

3. 找诱因 + 治原因
   - 12 导联 ECG（找 STEMI → 心导管）
   - 5H5T 评估
   - 实验室全套 + ABG

4. 神经保护
   - Targeted Temperature Management (TTM)
     32-36°C × 24h（昏迷患者）
   - 控癫痫（EEG 监测）
   - 神经预后评估 ≥ 72h 后
```

### 8.2 复苏后心导管指征

> [!success] 复苏后立即做心导管的指征
> - **STEMI 表现** → 立即去 cath lab（< 90 min）
> - **不稳定 + 怀疑 ACS** → 紧急
> - **VF / 无脉 VT 骤停** + 高度怀疑 ACS → 即使无明显 STEMI，也考虑早期心导管

---

## Part 9. PALS 速查（儿童 ACLS 简短对比）

| 项 | 成人 ACLS | 儿童 PALS |
|---|---|---|
| **CPR 按压：通气** | 30 : 2（单人）| 30 : 2（单人）/ **15 : 2**（双人 + 儿童）|
| **按压深度** | 5-6 cm | **胸廓深度 1/3** |
| **按压频率** | 100-120 / min | 同 |
| **Epi 剂量** | 1 mg | **0.01 mg/kg** |
| **除颤能量** | 200J | **2 J/kg**（首次）→ 4 J/kg |
| **可逆因** | 5H5T | 同 |

---

## Part 10. Memory Hook 集合

### 10.1 核心口诀

> [!success] 5 个核心口诀
> 1. **"V 除颤（VF + 无脉 VT），P/A 按压（PEA + Asystole）"**
> 2. **"先看脉搏，后看节律"** — 脉搏决定治疗，节律决定诊断
> 3. **"PEA = 电话有铃声但没人接"** — 节律 ≠ 循环
> 4. **"V 字开头要除颤；P/A 开头要按压"**
> 5. **"flatline shock 是电视剧；真临床绝不电 asystole"**

### 10.2 时间窗 3 个数字

> [!tip] ACLS 三个时间数字
> - **30 : 2** = CPR 按压 : 通气比
> - **2 min** = 每周期 + rhythm check
> - **3-5 min** = Epi 间隔

### 10.3 5H5T 速记

> H = "**5 个 Hypo-**"（Hypovolemia / Hypoxia / Hypothermia / Hypo-Hyperkalemia）+ **H 离子**（酸）
> T = "**5 个 T**"（Tension pneumo / Tamponade / Toxins / Thrombosis × 2: **P**E + **M**I）

### 10.4 用药记忆

> [!tip] Epi vs Amio 记忆
> - **Epinephrine** = "**E**arly + **E**veryone" — 越早越好 + 4 种节律都用
> - **Amiodarone** = "**A**fter 3rd shock" — 第 3 次除颤后才给

### 10.5 三种"电"方式速记

> **"无脉无 R = Defib，有脉同 R = Sync，缓慢起搏 = Pacing"**

---

## Part 11. 跨学科陷阱

| 学科 | 陷阱 | 关键点 |
|---|---|---|
| **外科** | 创伤性心包填塞 → PEA | 5T 之 Tamponade，**穿刺急救** |
| **外科** | 张力气胸 → PEA | 5T 之 Tension pneumo，**针刺减压不等 CXR** |
| **肺** | 大块 PE → 不稳定 → PEA | 5T 之 PE，**tPA 溶栓** |
| **感染** | 脓毒症 → 持续低血容量 → PEA | 5H 之 Hypovolemia，**大量补液 + 升压药** |
| **内分泌** | DKA / Adrenal crisis → PEA | 5H 之 Hypovolemia + H+ 酸中毒 |
| **肾 / Heme** | 高 K（CKD / TLS / 溶血）→ VF | 5H 之 Hyperkalemia，**Ca + insulin** |
| **中毒** | TCA → VT/VF；β-B/CCB → bradycardia → PEA | 5T 之 Toxins，**特异解毒**（NaHCO3 / Glucagon / Insulin）|
| **低温**（户外 / 老人）| Hypothermia → VF | 5H 之 Hypothermia，**复温**（"不死直到温暖死"）|
| **儿科** | 溺水 → Hypoxia → 骤停 | PALS 流程 + 5H 之 Hypoxia |
| **神经** | 重型卒中 → herniation → 骤停 | 不可逆，但仍按 ACLS 跑 |

---

## Part 12. 高频陷阱总结

| 陷阱 | 正确认知 |
|---|---|
| ❌ 看到房颤 = 复律 | ✓ 必须先看脉搏；**无脉房颤 = PEA = 不电击** |
| ❌ PEA 可以除颤 | ✓ 错！PEA = 电活动正常但心肌不收缩，电击对"机械停跳"无效 |
| ❌ Asystole 给 atropine | ✓ 错！2010 AHA 已移除；asystole = CPR + Epi |
| ❌ "有节律 = 有循环" | ✓ 错！PEA 关键就是节律和循环脱钩 |
| ❌ 见骤停先评估 ABG / 实验室 | ✓ 错！先 CPR；评估同步做 |
| ❌ 第一次除颤就给 amiodarone | ✓ 错！第 3 次除颤后才给 |
| ❌ Defibrillation 和 Cardioversion 一样 | ✓ 错！同步与否 + 脉搏要求完全不同 |
| ❌ Lidocaine 是 PEA 一线药 | ✓ 错！Lidocaine 仅用于 VF / 无脉 VT |
| ❌ "flatline shock" | ✓ 电视剧才有；真临床绝不电击 asystole |
| ❌ PEA 不需要找原因 | ✓ 错！**5H5T 必找**；不像 VF 单纯电击就行 |
| ❌ ROSC 后高流量氧最好 | ✓ 错！避免高氧（神经损伤）→ SpO2 92-98% |
| ❌ ROSC 后立即唤醒患者 | ✓ 错！昏迷患者需 TTM 32-36°C × 24h |

---

## 🔗 关联

- 🔁 **同主题错题**：
  - [[mistakes/uworld-mistakes#^Q4725]] PEA 房颤陷阱（首张 ACLS 卡）
  - 等后续 VF / Asystole / 同步复律 / 5H5T 各因 / ROSC 后管理题积累
- 📚 **主笔记**：
  - [[完整笔记/Peixuan分科笔记/心内]]（ACLS + 心律失常急救）
  - [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] ⭐（**姊妹笔记** — Vaughan 讲药物对照，本笔记讲急救流程；两者互补）
- 🏥 **跨学科**：
  - [[完整笔记/Peixuan分科笔记/外科]]（创伤性心包填塞 / 张力气胸 → PEA → 特异处理）
  - [[完整笔记/Peixuan分科笔记/pulmonary]]（大块 PE → 不稳 → PEA → tPA）
  - [[完整笔记/Peixuan分科笔记/感染]]（脓毒症休克 → 持续低血容量 → PEA）
  - [[完整笔记/Peixuan分科笔记/endocrine]]（Adrenal crisis / DKA → PEA）
  - [[完整笔记/专题笔记/_衍生_主动脉急症决策树]]（心包填塞共享 + 难治性休克 / PEA 系列）
  - [[完整笔记/专题笔记/_衍生_肾上腺皮质功能不全决策树]]（Adrenal crisis → 持续低 BP → PEA 病因）
  - [[完整笔记/专题笔记/_衍生_读题策略_临床决策与题型识别]]（"看到节律就电"反射 = 模式识别错位）
- 🌱 **TODO（持续扩充）**：
  - 累计 3+ 道 PEA 病因题（5H5T 各场景）→ 拆出 [[完整笔记/专题笔记/_衍生_PEA可逆因鉴别]]
  - 累计 3+ 道 ROSC 后管理题（TTM / 心导管时机 / 神经预后）→ 补 Part 8
  - 累计 3+ 道 PALS 儿童急救题 → 扩 Part 9
  - 累计 3+ 道"同步 vs 不同步电复律"陷阱题 → 补 Part 5

---

## 📋 文件元信息

- **建立**：2026-05-14（由 Q4725 PEA 房颤陷阱触发）
- **状态**：v1 完整版（12 个 Part：方法论 + 4 节律 + ACLS 算法 + 5H5T + 用药 + 三种电击 + 急救分类决策 + 房颤决策 + ROSC + PALS + Memory Hook + 跨学科陷阱）
- **应试目标**：USMLE Step 2 CK 急救 + ICU + 围手术期 ACLS 模块
- **复习节奏**：
  - 考前每周扫 Part 0 + Part 10（Memory Hook）+ Part 12（陷阱）
  - 考前 1 月精读 Part 1-7（4 节律 / ACLS 算法 / 5H5T / 用药 / 三种电击 / 急救分类 / 房颤决策）
- **5 天 ACLS 巩固计划**（Peixuan 推荐）：
  - Day 1：4 节律对照（Part 1） + "V 除颤 P/A 按压"
  - Day 2：5H5T + 针对处理（Part 3）
  - Day 3：用药速查（Part 4）+ Epi q3-5 / Amio 第 3 次
  - Day 4：三种"电"方式（Part 5） + 房颤决策（Part 7）
  - Day 5：全套默写 + ROSC 管理（Part 8）

**Last updated**: 2026-05-14 v1
