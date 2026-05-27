---
tags:
  - USMLE-Step2
  - 感染
created: 2026-05-26
type: 专题笔记
version: v1.0
---

# CLABSI 完整体系 — Central Line-Associated Bloodstream Infection

> [!info] 定位与边界
> 本笔记是 **CLABSI 的 ID（感染）视角主笔记** — 病原体 / 诊断 / 治疗 / 疗程 / 拔管 indication / HAC 政策。
>
> **预防 5 步 Bundle** 已在 [[完整笔记/专题笔记/USMLE/USMLE_侵入操作安全流程#5.2.3a CLABSI 预防 Bundle ⭐⭐⭐（USMLE 高频）]] 完整覆盖（含穿刺点悖论 — 感染最低 SC vs 急诊用 Femoral）→ 本笔记不复制，只链接。
>
> 与 [[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]] §13.9 HAC（CMS 不报销）+ §12.2.x Q22359（Donabedian 4 类 indicator — CLABSI 是经典 outcome / process / structural / balancing 配对题）形成 patient safety 视角互补。

---

## 一、定义 + 易混区分

### 1.1 CLABSI 定义

**CLABSI (Central Line-Associated Bloodstream Infection, 中心静脉导管相关血流感染)**：
- 患者 **central venous catheter (CVC) 留置 ≥ 48 小时**
- 发生 **primary bloodstream infection (BSI)**
- **无其他明确感染源**（不是从肺 / 尿 / 伤口扩散）

> 简单说：**导管插超过 2 天 + 血里有菌 + 找不到其他来源 = CLABSI**

### 1.2 CLABSI vs CRBSI 区分（CK 易混）⭐

| 缩写 | 全称 | 用途 | 严格度 |
|---|---|---|---|
| **CLABSI** | Central Line-**Associated** BSI | **公共卫生 / surveillance / CMS 报销** | 较宽 — 只要 CVC + BSI + 无其他源 |
| **CRBSI** | Catheter-**Related** BSI | **临床诊断 / 治疗决策** | 严格 — 需微生物证据证明 catheter 是源（DTP / 尖端培养）|

> [!tip] 边界口诀
> - **CLABSI** = surveillance 用（**CDC / CMS 视角**）
> - **CRBSI** = 临床用（**ID 视角，要求微生物证据**）
> - USMLE 多数情境用 **CLABSI**；少数 ID 题用 **CRBSI**（要求 differential time to positivity）

### 1.3 HAI / HAC 大家族中的位置

```
HAI（Hospital-Acquired Infection 院内感染）
   ├─ CLABSI ⭐  — 中心静脉导管血流感染
   ├─ CAUTI    — 导尿管尿路感染
   ├─ VAP      — 呼吸机相关肺炎
   ├─ SSI      — 手术部位感染
   └─ C. diff  — 抗生素后腹泻

HAC（Hospital-Acquired Condition CMS 不报销列表）
   ├─ 上述全部 HAI
   ├─ Falls / Pressure ulcers
   ├─ VTE post-orthopedic
   ├─ Wrong-site surgery
   └─ Foreign object retained
```

---

## 二、流行病学 + HAC 政策（高频考点）

### 2.1 数字背景

- 美国每年 **~30,000 CLABSI** 病例
- ICU 最常见 HAI 之一
- 经典预防 bundle（Pronovost / Michigan Keystone）使全美 ICU CLABSI 率 **2001-2009 下降 ~58%**

### 2.2 HAC 政策时间线 ⭐⭐⭐

| 时间 | 政策 | 影响 |
|---|---|---|
| **2008** | CMS 宣布 **HAC 不报销**（CLABSI 入列）| 医院**自掏腰包** → 推 checklist 全面普及 |
| 2011 | The Joint Commission 列 CLABSI 为 National Patient Safety Goal | 强制 surveillance + 上报 |
| 现在 | 多数医院 CLABSI 写入 quality metric / value-based reimbursement | QI / patient safety 高频考 |

> [!success] 为什么 CLABSI 是 USMLE 三重高频
> 它是 **感染 (ID) + Patient Safety / QI + Health policy** 三个 domain 的**天然交集** —
> ① ID 角度：BSI 诊治；② QI 角度：bundle / Donabedian indicator；③ Policy 角度：CMS HAC 不报销

---

## 三、病原体（CK 高频排序）

### 3.1 病原体频谱表

| 病原体 | 频率 | 来源 + 关键点 |
|---|---|---|
| **Coagulase-negative Staph (S. epidermidis)** ⭐⭐⭐ | **最常见**（~30%）| **皮肤菌群** → 经插管处进入；**biofilm 形成强**（难根除）|
| **Staphylococcus aureus** ⭐⭐ | 第二常见（~20%）| 含 **MRSA**；**致死率最高** + 转移灶风险（心内膜炎 / 骨髓炎）|
| **Enterococcus**（含 **VRE**）| 常见（~15%）| 多重耐药；常 hospital-acquired |
| **Candida**（多为 C. albicans / C. glabrata）⭐ | ICU 长留置 + **TPN** + 长 abx 后 | **真菌血症** — 必需眼科会诊（endophthalmitis）|
| Gram-negative rods（含 **Pseudomonas**, E. coli, Klebsiella）| 少（~15%）| 危重 / 免疫抑制患者 |

### 3.2 病原体反射钩 ⭐

| Stem 信号 | 0.5 秒锁 |
|---|---|
| Central line ≥ 48h + fever + 培养 **coag-neg Staph** | **CLABSI**（最常见组合）|
| ICU + **TPN** + 长 abx + fever + 血培养 **酵母 / Candida** | **Candida CLABSI** → 拔管 + 眼科 + 14d |
| 透析患者 + 长期 CVC + **MRSA** 菌血症 + 新发杂音 | CLABSI **+ 感染性心内膜炎**（转移灶）|
| 急诊 femoral line 3 天后 + Pseudomonas | CLABSI（femoral 感染率最高） |

---

## 四、临床表现 + Stem 信号

### 4.1 经典临床表现

- **发热 + 寒战**（特别是 **line flushing 后立刻发热** = 强提示）⭐
- 插管部位红肿 / 渗液 / purulence（tunnel infection）
- 严重 → sepsis / septic shock
- 持续菌血症（72h 阳培养不退）→ 提示导管未拔 + 转移灶

### 4.2 USMLE Stem 高频信号

| 信号组合 | 提示 |
|---|---|
| **CVC ≥ 48h + 新发发热 + 阳血培养** | CLABSI 直到证否 |
| **Line flush 后立刻寒战** | 经典 CLABSI bedside sign |
| **持续菌血症 > 72h despite abx** | 未拔管 / 转移灶 / endocarditis |
| **TPN + ICU 长 line + Candida** | Candida CLABSI |
| **透析 + CVC + S. aureus** | CLABSI 高致死率 + 评估 IE |

---

## 五、诊断（CK 套路）

### 5.1 诊断 Workup

1. **取双血培养**：
   - 一套从 **peripheral vein** 抽
   - 一套从 **central line** 抽（如果还在用）
2. 若拔管 → 送 **导管尖端培养**（半定量 / 定量）
3. 评估其他感染源（尿 / 痰 / 伤口）排除二次 BSI
4. 严重 / S. aureus / Candida → 评估转移灶（**TTE / TEE** 排除 endocarditis；眼底镜排除 endophthalmitis）

### 5.2 微生物诊断标准（CRBSI 严格定义）⭐

满足任一条即支持 catheter 是 BSI 源：

| 标准 | 阈值 |
|---|---|
| **Differential Time to Positivity (DTP)** ⭐⭐⭐ | Central line 培养比 peripheral **早 ≥ 2 小时阳性** |
| **Quantitative blood culture ratio** | Central line CFU ≥ 3× peripheral CFU |
| **导管尖端半定量培养** | ≥ **15 CFU/plate** |
| **导管尖端定量培养** | ≥ **10² CFU/mL** |

> [!tip] DTP 直觉
> 同时抽双血培养，central line 的菌量更多（因为是源头），所以**先长出来**。差 2 小时以上 = 几乎肯定 catheter 是源。
>
> 类比：火灾报警 — 起火房间的烟雾警报先响，远端房间的后响；时间差 = 离火源远近。

### 5.3 鉴别诊断（排除其他 BSI 源）

| 源 | 排除方法 |
|---|---|
| **Endocarditis** | TTE / TEE — 特别 S. aureus / 持续菌血症 / 新杂音 |
| **UTI / urosepsis** | UA + 尿培养 |
| **Pneumonia** | CXR + 痰培养 |
| **SSI** | 检查伤口 |
| **Abdominal source** | 体检 / CT |

---

## 六、治疗（CK 经典套路）

### 6.1 经验性抗生素（empiric） ⭐

```
Step 1: 取双血培养（抽完才开 abx）
   │
   ▼
Step 2: 经验性 abx
   │
   ├─ Vancomycin（覆盖 MRSA + coag-neg Staph + Enterococcus）⭐
   │
   ├─ + Gram(-) 覆盖（cefepime / piperacillin-tazobactam / carbapenem）
   │     ※ 严重 sepsis / 免疫抑制 / 知道有 G(-) risk 时加
   │
   └─ + Antifungal（echinocandin 首选）
         ※ 有 Candida risk（TPN / 长 line / 长 abx / ICU 久）
   │
   ▼
Step 3: 根据培养 + 药敏 narrow（48-72h 后）
```

### 6.2 拔除导管 indication ⭐⭐⭐

> [!danger] 必拔管 — "**5 大必拔条件**"
> 1. **S. aureus**（特别 MRSA）— 致死率高 + 转移灶
> 2. **Candida / 真菌**
> 3. **Pseudomonas / 难治 G(-)**
> 4. **VRE / 难治 Enterococcus**
> 5. **临床条件**：
>    - 严重 sepsis / septic shock
>    - **持续菌血症 > 72h** despite 合适 abx
>    - **Tunnel infection / port pocket abscess / exit-site purulence**

可保留 line（在 coag-neg Staph + 无并发症 + 必需 CVC 时）— 抗生素 lock therapy + 系统 abx。

### 6.3 疗程（CK 高频）

| 病原体 | 疗程 | 备注 |
|---|---|---|
| **Coagulase-negative Staph** | **5-7 天**（拔管后） | 最短 — 致病力低 |
| **Staphylococcus aureus** ⭐ | **≥ 14 天**（拔管后）| **必须 TEE 排除 IE**；阳性 IE / 转移灶 → **4-6 周** |
| **Enterococcus** | 7-14 天 | VRE 更长 |
| **Gram-negative rods** | 7-14 天 | Pseudomonas 偏长 |
| **Candida** ⭐ | **≥ 14 天**（首次阴血培养算起）+ **眼科会诊** | 排除 endophthalmitis；必须拔管 |

> [!warning] S. aureus CLABSI 必做 TEE
> S. aureus 菌血症 **transthoracic echo 灵敏度低**，必须 **TEE** 排除 IE。漏诊后果：endocarditis → embolic stroke / valve destruction → 致命。

---

## 七、预防 → 引用主笔记（不重复内容）

> [!success] 5 步 CLABSI 预防 Bundle（Pronovost / IHI / CDC 标准）
> **完整内容见** [[完整笔记/专题笔记/USMLE/USMLE_侵入操作安全流程#5.2.3a CLABSI 预防 Bundle ⭐⭐⭐（USMLE 高频）]]
>
> 简版速记：
>
> ① **手卫生** → ② **Maximal sterile barrier**（全套无菌 + 大无菌单）→ ③ **Chlorhexidine**（不用 PVI）→ ④ **首选 Subclavian**（避免 Femoral）→ ⑤ **每天 review + 早拔管**
>
> **穿刺点感染率**：**Femoral > IJV > Subclavian** ⭐⭐⭐
> **穿刺点选择悖论**：感染最低 = SC，但 SC 气胸 + 不可压迫 → 凝血障碍 / 急诊须用 IJV / Femoral

---

## 八、CK 经典 Stem 模式（5 类高频）

### 模式 1：诊断（最常见）

> 65 yo ICU 患者 + CVC 5 天 + 突发发热 + line flush 后寒战 + 无其他感染源 → next step?
>
> ✅ **取双血培养**（peripheral + central line） + 经验性 **vancomycin + G(-) 覆盖** + 评估拔管

### 模式 2：经验性 abx 选择

> CLABSI suspect → empiric abx?
>
> ✅ **Vancomycin**（覆盖 MRSA / coag-neg Staph / Enterococcus）+ 视情况加 G(-) / antifungal

### 模式 3：拔管决策

> CLABSI + 培养 **S. aureus** / **Candida** / **Pseudomonas** → 拔不拔？
>
> ✅ **必拔**（5 大必拔条件之一）

### 模式 4：QI / Patient Safety（Donabedian）

ICU CLABSI rate 持续 elevated（详见 [[完整笔记/专题笔记/USMLE/USMLE_患者安全_QI工具#12.2.x Outcome 不变诊断顺序 ⭐⭐⭐（v1.3.9 新增 — Q22359 锚定）]]）：

| Stem 表述 | Indicator 类型 |
|---|---|
| "% of central lines with daily review" | **Process** |
| "CLABSI rate per 1000 catheter-days" | **Outcome** |
| "# of ICU staff trained on bundle" | **Structural** |
| "Documentation time after bundle implementation" | **Balancing** |

### 模式 5：HAC 政策

> 医院为什么主动推 CLABSI checklist?
>
> ✅ **CMS 2008 起 HAC 不报销** → 医院自掏腰包

### 模式 6：穿刺点选择

> 危重患者紧急 CVC，感染率**最低**部位？
>
> ✅ **Subclavian**（感染最低）；但 SC 气胸最高 + 不可压迫 — 看患者条件权衡（见 [[完整笔记/专题笔记/USMLE/USMLE_侵入操作安全流程#5.2.2 CVC 选位决策树]]）

---

## 九、高频陷阱 ⭐⭐（CK 钓鱼选项）

| 陷阱 | 为什么错 |
|---|---|
| **Femoral vein 感染最低** | ❌ 反了 — **Femoral 最高，SC 最低**（"会阴 / 不易固定 / 易污染"）|
| **Povidone-iodine 优于 chlorhexidine** | ❌ 反了 — **Chlorhexidine > PVI**（CDC 标准）|
| **S. aureus CLABSI 用 TTE 就够** | ❌ **必须 TEE**（TTE 灵敏度低）|
| **Coag-neg Staph 必拔管** | ❌ **可保留** + 抗生素 lock；**S. aureus / Candida / Pseudomonas / VRE 才必拔** |
| **Candida CLABSI 不用眼科会诊** | ❌ **必做** — 排除 endophthalmitis |
| **S. aureus CLABSI 7 天疗程** | ❌ **≥ 14 天**（拔管后算起），有 IE → 4-6 周 |
| **CLABSI checklist 实施后率不变 → patient factors** | ❌ Patient factors 不 systematically alter — 先查 **Process compliance**（详见 [[完整笔记/专题笔记/USMLE/USMLE_患者安全_QI工具#12.2.x Outcome 不变诊断顺序 ⭐⭐⭐（v1.3.9 新增 — Q22359 锚定）]]）|

---

## 十、Memory Hooks（一句话锁定）

- **"CLABSI = 中心导管 ≥ 48h + 血流感染 + 找不到其他来源"** ⭐
- **"CLABSI = surveillance（CDC/CMS）；CRBSI = 临床（要求 DTP / 尖端培养）"** ⭐
- **"最常见菌 = Coag-neg Staph（皮肤）；最致命菌 = S. aureus（必 TEE / ≥14d）"** ⭐⭐⭐
- **"5 必拔：S. aureus / Candida / Pseudomonas / VRE / 严重 sepsis 或持续菌血症 > 72h"** ⭐⭐⭐
- **"Candida 血症 → 拔管 + 眼科会诊 + ≥ 14 天"** ⭐
- **"DTP ≥ 2h（CL 比 peripheral 先长）= catheter 是源"** ⭐
- **"Femoral 最脏；Subclavian 最干净"**（感染率角度）⭐
- **"Chlorhexidine > Povidone-iodine（CDC 标准）"**
- **"5 步 bundle：手 + 全套无菌 + 氯己定 + SC（避 Femoral）+ 每天 review"** — 详见 [[完整笔记/专题笔记/USMLE/USMLE_侵入操作安全流程#5.2.3a CLABSI 预防 Bundle ⭐⭐⭐（USMLE 高频）]]
- **"HAC = CMS 2008 起不报销 → 医院自掏腰包推 checklist"** ⭐
- **"S. aureus CLABSI 必做 TEE — TTE 灵敏度低，漏诊 IE 致命"** ⭐

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes#^Q3504]] CVC 置入后必做 CXR（CLABSI 不是直接锚但同 CVC 主题）
  - 暂无直接 CLABSI 诊治错题（待 UW 出现后回填）
- 📚 主笔记：
  - [[完整笔记/Peixuan分科笔记/感染]]（学科主笔记 — ID 整体视角）
  - [[完整笔记/Peixuan分科笔记/外科]]（CVC 维护 + bundle 简版）
- 🏥 跨学科：
  - [[完整笔记/专题笔记/USMLE/USMLE_侵入操作安全流程]] §5.2.3a — **预防 Bundle 完整内容在此**（不重复）
  - [[完整笔记/专题笔记/USMLE/USMLE_患者安全与质量改进工具]] §13.9 HAC（CMS 不报销）+ §12.2.x（Q22359 Donabedian 4 indicator CLABSI 经典 stem）
  - [[完整笔记/专题笔记/感染/感染_感染性心内膜炎完整体系]] — S. aureus CLABSI 必排除 IE（TEE）
  - [[完整笔记/专题笔记/感染/感染_抗生素高频20场景秒杀]] — 经验性 vanco + G(-) 覆盖
  - [[完整笔记/Peixuan分科笔记/心内]] — S. aureus 菌血症 + 新杂音 → IE
- 🌱 TODO：
  - 累积 3+ 道 CLABSI 实题（诊断 / 经验 abx / 拔管 indication / 疗程）后回填具体 Q 锚
  - 累积 HAI 家族错题（CAUTI / VAP / SSI / C. diff）→ 考虑独立 `感染_HAI家族大全` 整合 5 大 HAI 速查
  - S. aureus 菌血症完整 workup（含 TEE + 转移灶 + 疗程）→ 考虑独立 `感染_S_aureus菌血症完整SOP`

---

## ✅ 学习清单（建议顺序）

1. 背 CLABSI 定义 + 与 CRBSI 区分（surveillance vs 临床）
2. 背病原体频谱（**Coag-neg Staph 最常见 / S. aureus 最致命 / Candida 必眼科**）
3. **5 必拔条件**（S. aureus / Candida / Pseudomonas / VRE / 严重临床）⭐⭐⭐
4. 疗程（coag-neg 7d / S. aureus 14d + TEE / Candida 14d + 眼科）
5. DTP 诊断标准（≥ 2h 差）
6. 预防 5 步 bundle 跳转到 [[完整笔记/专题笔记/USMLE/USMLE_侵入操作安全流程#5.2.3a CLABSI 预防 Bundle ⭐⭐⭐（USMLE 高频）]] 复习
7. HAC 政策（CMS 2008 不报销）+ Donabedian 4 indicator 配对（跳转 §12.2.x）
8. 6 类 CK stem 模式 + 高频陷阱默写
9. Memory Hooks 滚动复习
