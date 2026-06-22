---
tags:
  - USMLE-Step2
  - 肺
  - 感染
created: 2026-06-22
type: 专题笔记
---

# CAP 门诊 vs 住院 vs ICU 分层（社区获得性肺炎 community-acquired pneumonia）

> [!tip] 一句话定位
> CAP 题的真正考点 **不是背药，而是先分"门诊 vs 住院 vs ICU"**。诊断锁定后（发热 + 咳痰 + 局灶啰音 + 胸片浸润），下一步是**评严重度**——稳定门诊就口服窄谱，重症才上 IV 广谱。一旦分层做对，过度升级的干扰项自动出局。
>
> 派生自 [[NBME11_错题本#^Q076]]（24M 稳定门诊 CAP，被镰状细胞性状/哮喘/大麻标签带跑，误选 IV 氨苄西林-舒巴坦；正确 = 口服阿奇霉素）。

---

## 一、诊断 → 分层 → 选药（总决策树）

```
咳嗽 + 发热 + 局灶 crackles + 胸片浸润影
  = community-acquired pneumonia (CAP, 社区获得性肺炎)
        ↓
评严重度（先算 CURB-65 / PSI，再看 ICU 标准）
        ↓
┌─────────────┬──────────────────┬─────────────────────┐
│ 门诊 outpatient │ 住院·非 ICU ward    │ ICU                  │
│ CURB-65 0–1     │ CURB-65 ≥2          │ IDSA major 任一       │
│ PSI I–II        │ PSI III–V           │ 或 minor ≥3          │
├─────────────┼──────────────────┼─────────────────────┤
│ 口服窄谱        │ IV β-内酰胺 + 大环内酯 │ IV β-内酰胺 + 大环内酯 │
│               │ 或 呼吸氟喹诺酮单药   │ /氟喹诺酮 + 必要时     │
│               │                    │ 覆盖 MRSA / 铜绿       │
└─────────────┴──────────────────┴─────────────────────┘
```

> [!warning] 最常见的 NBME 陷阱
> **生命体征稳定（SpO₂ ≥92%、BP 正常、神志清、RR <30）的门诊 CAP，别反射上 IV 广谱。** 一堆吓人的病史标签（镰状细胞性状、童年哮喘、吸大麻）≠ 重症指征。**镰状细胞性状 (sickle cell trait) ≠ 镰状细胞病 (sickle cell disease)**——trait 通常无症状、不改 CAP 处理。

---

## 二、CURB-65（首选"是否住院"工具）⭐⭐⭐

> [!info] CURB-65 — 每项 1 分，共 5 分
>
> | 字母 | 项目 | 阈值 |
> |---|---|---|
> | **C** | Confusion（新发意识混乱）| 有 = 1 分 |
> | **U** | Urea（血尿素氮 BUN）| > 19 mg/dL（> 7 mmol/L）= 1 分 |
> | **R** | Respiratory rate（呼吸频率）| ≥ 30 /min = 1 分 |
> | **B** | Blood pressure（血压）| 收缩压 SBP (systolic BP) < 90 或舒张压 DBP (diastolic BP) ≤ 60 mmHg = 1 分 |
> | **65** | Age（年龄）| ≥ 65 岁 = 1 分 |

> [!tip] 计分 → 处置（高频）
> - **0–1 分** → **门诊 outpatient** 口服治疗（低死亡风险）
> - **2 分** → **考虑短期住院 / 观察**（中等风险）
> - **≥3 分** → **住院**，评估是否 **ICU**（高死亡风险）
>
> 简化版 **CRB-65**（不查尿素，无需抽血）→ 适合门诊/急诊快速分诊。

---

## 三、PSI / PORT score（成人肺炎严重度指数 Pneumonia Severity Index / Patient Outcomes Research Team score，更细但更繁）⭐⭐

> [!info] PSI vs CURB-65 怎么选
> - **CURB-65**：5 项、床旁秒算、NBME 默认首选 → 考试基本只考它。
> - **PSI (Pneumonia Severity Index)**：20 项（年龄/共病/查体/化验/影像），按总分分 **Risk Class I–V**，对"低危可门诊"识别更灵敏，但太繁琐。
>   - **Class I–II（≤70 分）** → 门诊
>   - **Class III（71–90）** → 短期住院 / 观察
>   - **Class IV–V（>90）** → 住院（V 常需 ICU）
>
> CK 层面记住：**PSI 更敏感地"安全地把低危人放回家"**；具体 20 项不必背。

---

## 四、ICU 入住标准（IDSA/ATS major / minor criteria）⭐⭐⭐

> [!info] 缩写
> **IDSA** = Infectious Diseases Society of America（美国感染病学会）；**ATS** = American Thoracic Society（美国胸科学会）；**ICU** = intensive care unit（重症监护室）。

> [!danger] Major criteria（满足**任一** → 直接 ICU）
> - **需要机械通气**（侵入性 invasive mechanical ventilation）
> - **感染性休克需血管升压药**（septic shock requiring vasopressors）

> [!warning] Minor criteria（满足 **≥3 项** → 考虑 ICU）
> - 呼吸频率 ≥ 30 /min
> - 氧合指数 PaO₂/FiO₂（动脉氧分压/吸入氧浓度比）≤ 250
> - 多叶浸润（multilobar infiltrates）
> - 意识混乱 / 定向障碍
> - 尿素氮 BUN ≥ 20 mg/dL
> - 白细胞减少 WBC < 4000（感染所致）
> - 血小板减少 plt < 100000
> - 体温过低 < 36℃
> - 低血压需积极液体复苏

> [!tip] 记忆钩
> **Major = 已经"上呼吸机或上升压药"**（器官支持已启动）；**Minor = 一堆"快撑不住"的预警，凑够 3 个就进 ICU。**

---

## 五、CAP 三档经验治疗（精简；完整版见反链）

> [!info] 选药速查（中英双语）
>
> | 分层 | 给药途径 | 一线方案 | 用药原则 |
> |---|---|---|---|
> | **门诊·健康无共病** | **口服 PO** | **amoxicillin** / **doxycycline** / macrolide（**azithromycin**，仅在当地耐药率低时）| 窄谱起步、只需盖典型菌；疗程最短 5 天，且退热 + 临床稳定 48–72h 后才停 |
> | **门诊·有共病**（心/肺/肝/肾病、糖尿病、酗酒、恶性肿瘤、无脾、免疫抑制）| **口服 PO** | **respiratory fluoroquinolone 单药**（levofloxacin / moxifloxacin）**或** β-lactam（amoxicillin-clavulanate / cephalosporin）+ macrolide（azithromycin）| 必须加盖非典型 + 耐药肺炎球菌；单药首选呼吸 FQ（一药全包，省事）|
> | **住院·非 ICU** | **静脉 IV**（稳定后转 PO）| **ceftriaxone + azithromycin**，或 respiratory fluoroquinolone 单药 | β-lactam 不盖非典型 → 必配大环内酯/FQ；48–72h 稳定 + 能口服 → IV→PO 序贯，早出院 |
> | **ICU** | **静脉 IV** | β-lactam（ceftriaxone / ampicillin-sulbactam）+ macrolide（azithromycin）**或** + respiratory fluoroquinolone；按风险加 MRSA / 铜绿覆盖 | 强制双药联合（不可单药）；按 major/minor 风险加挂 MRSA（vancomycin/linezolid）/铜绿（抗铜绿 β-lactam）|
>
> **核心逻辑**：所有住院方案都"典型肺炎链球菌 + 非典型菌一次覆盖"。门诊有共病也升级到能压非典型 + 耐药菌的方案。

### 5.1 每药覆盖谱速查（为什么这样配）⭐

> [!info] 一张表看懂每个 CAP 用药盖什么
> **β-内酰胺类（amoxicillin / amox-clav / ceftriaxone / amp-sulbactam）一律不盖非典型菌** → 这正是住院/ICU 方案必须再加一个大环内酯或呼吸氟喹诺酮的原因。

| 抗生素 | 典型菌（尤肺炎链球菌 *S. pneumoniae*）| 非典型菌（支原体 *Mycoplasma* / 衣原体 *Chlamydophila* / 军团菌 *Legionella*）| 额外覆盖 / 要点 |
|---|---|---|---|
| **阿莫西林 amoxicillin** | ✅ 主力 | ❌ 不盖 | + 流感嗜血杆菌 *Haemophilus influenzae*（不产酶株）；窄谱，健康门诊首选 |
| **阿莫西林-克拉维酸 amoxicillin-clavulanate** | ✅ | ❌ 不盖 | + 产 β-内酰胺酶的流感嗜血杆菌 / 卡他莫拉菌 *Moraxella catarrhalis* + 厌氧菌（误吸）|
| **头孢曲松 ceftriaxone** | ✅（含较多耐药肺炎球菌）| ❌ 不盖 | + 多数革兰阴性菌；**不盖**铜绿/MRSA/肠球菌 → 住院必配大环内酯 |
| **氨苄西林-舒巴坦 ampicillin-sulbactam** | ✅ | ❌ 不盖 | + 厌氧菌（误吸性肺炎好用）+ 产酶菌；不盖铜绿/MRSA |
| **多西环素 doxycycline** | ✅ | ✅ **都盖** | 门诊单药即可同时压典型+非典型；亦盖部分社区获得性 CA-MRSA (community-acquired MRSA) |
| **阿奇霉素 azithromycin（大环内酯）** | ⚠️ 盖但耐药率高（~25–30%）| ✅ **都盖** | 单用前提是当地肺炎球菌耐药率低 |
| **呼吸氟喹诺酮 levofloxacin / moxifloxacin** | ✅（含耐药肺炎球菌）| ✅ **都盖** | 单药全包 → 有共病/住院的省事之选；**左氧氟沙星兼盖铜绿**，莫西沙星不可靠盖铜绿但盖厌氧 |
| **万古霉素 vancomycin / 利奈唑胺 linezolid** | （加在主方案上）| — | 专补 **MRSA**；不作单药 |
| **抗铜绿 β-内酰胺**（哌拉西林-他唑巴坦 piperacillin-tazobactam / 头孢吡肟 cefepime / 头孢他啶 ceftazidime）| 部分 | ❌ | 专补 **铜绿假单胞菌**；结构性肺病/中性粒缺时加 |

> [!tip] 三条记忆主线
> 1. **β-内酰胺 = 只典型，不非典型** → 所以住院/ICU 永远"β-内酰胺 + (大环内酯 或 呼吸氟喹诺酮 FQ, fluoroquinolone)"。
> 2. **doxycycline / 大环内酯 / 呼吸氟喹诺酮 = 自带非典型覆盖** → 可作门诊单药盖全。
> 3. **vancomycin/linezolid 补 MRSA、抗铜绿 β-内酰胺补铜绿** → 都是"按风险加挂"，不是 CAP 基础方案。

> [!warning] 何时额外覆盖 MRSA / 铜绿假单胞（Pseudomonas）
> - **耐甲氧西林金黄色葡萄球菌 MRSA (methicillin-resistant *Staphylococcus aureus*)**：流感后坏死性肺炎、空洞、既往 MRSA 定植、近期住院/静脉用药史 → 加 **万古霉素 vancomycin / 利奈唑胺 linezolid**。
> - **铜绿假单胞菌 Pseudomonas (Pseudomonas aeruginosa)**：结构性肺病（支气管扩张 bronchiectasis、囊性纤维化 CF, cystic fibrosis）、近期广谱抗生素、中性粒细胞缺乏 → 抗铜绿 β-内酰胺（哌拉西林-他唑巴坦 piperacillin-tazobactam / 头孢吡肟 cefepime / 头孢他啶 ceftazidime）。
>
> ⚠️ 普通稳定门诊 CAP **不需要**抗铜绿（如头孢他啶 ceftazidime 是干扰项）。

---

## 六、初始评估后随访 + 降阶

> [!tip] 48–72 小时规则
> - 经验治疗启动后 **48–72h 评估临床反应**（退热、白细胞、氧合、症状）。
> - **临床改善 + 能口服 + 血流动力学稳定** → IV 转口服（IV-to-PO switch），可早期出院。
> - 拿到**血/痰培养** → 针对性**降阶 (de-escalation)** 到窄谱。
> - 无改善 → 重新评估：诊断错（不是 CAP？脓胸/脓肿/耐药菌/非感染）→ 复查影像 ± CT。

---

## 七、易混与高频陷阱（普适）

> [!danger] 反模式黑名单
> - ❌ "看到肺炎就上 IV 广谱"——先分层，稳定门诊一律口服。
> - ❌ 把**镰状细胞性状 / 久未发作的童年哮喘 / 吸大麻**当重症或特殊覆盖指征。
> - ❌ 给稳定门诊 CAP 开**头孢氨苄 cephalexin**（主治皮肤软组织，非 CAP 覆盖）或抗铜绿的**头孢他啶 ceftazidime**（超广谱，不需要）。
> - ❌ 把 **CURB-65 = 2** 直接当门诊——2 分应考虑住院/观察。
> - ❌ 误把 **PSI 当床旁首选**——考试默认 CURB-65。

---

## 🔗 关联

- 🔁 同主题错题：
  - [[NBME11_错题本#^Q076]] 稳定门诊 CAP → 口服阿奇霉素（被病史标签带跑误选 IV 广谱）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/pulmonary]] / [[完整笔记/专题笔记/pulmonary/pulmonary_HighYield速查总览]]（§6.1 CURB-65 + §6.2 CAP 经验用药，本笔记把分层工具展开）
- 🏥 跨学科 - 感染：
  - [[完整笔记/专题笔记/感染/感染_肺部感染病原与用药速查]]（CAP 三层经验治疗 + "看人下菜"特殊病原，选药完整版）
  - [[完整笔记/专题笔记/感染/感染_非典型肺炎鉴别与治疗]]（支原体/军团菌/衣原体——住院方案为何都含大环内酯/FQ）
  - [[完整笔记/专题笔记/感染/感染_常见病原菌总结_按部位综合征]]（下呼吸道：CAP/HAP 病原谱）
- 🌱 TODO（待生成衍生）：
  - 若后续出现 HAP (hospital-acquired pneumonia, 医院获得性肺炎) / VAP (ventilator-associated pneumonia, 呼吸机相关性肺炎) 分层选药题 → 整合 CAP vs HAP/VAP 经验治疗对照（铜绿 + MRSA 双覆盖规则）

---

## ✅ 复盘行动

- [ ] 默写 **CURB-65** 5 项 + 阈值（C/U>19/R≥30/B<90/65）
- [ ] 默写 CAP 三档一线药（门诊口服 / 住院 ceftriaxone+azithromycin / ICU 加覆盖）
- [ ] 记 **ICU major = 上呼吸机或升压药；minor ≥3**
- [ ] 记 **镰状细胞性状 ≠ 镰状细胞病**，稳定门诊别上 IV 广谱

---

## 版本记录

- **v1**（2026-06-22）：错题驱动新建（兑现 [[NBME11_错题本#^Q076]] bd TODO）。独占内容 = CURB-65 细则 + PSI 概要 + IDSA ICU major/minor criteria + 总决策树；选药做精简版并反链 [[完整笔记/专题笔记/感染/感染_肺部感染病原与用药速查]] 完整版与 [[完整笔记/专题笔记/pulmonary/pulmonary_HighYield速查总览]] §6.1-6.2。
