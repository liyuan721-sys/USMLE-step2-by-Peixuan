# 高频评分 & 临床公式速查

> 派生自所有笔记 + 公开教科书概念。日期: 2026-05-10
> 用法：vignette 给数据让你算评分/做决策时，直接查这里。
> 版权说明：所有分值表基于公开医学教科书（Harrison's, UpToDate 公开摘要, ACC/AHA / WHO / ADA 指南条目）重新整理，未复制 UWorld 题干/解析。

## 📋 目录

> [!tip]- 点击跳转专科（12 节 — 按系统 + 通用）
>
> ### 临床专科评分
> - [[#Cardiovascular 心血管]]（CHADS2 / HAS-BLED / TIMI / Killip 等）
> - [[#Pulmonary / PE 肺与肺栓塞]]（Wells / PERC / CURB-65 等）
> - [[#Hepatology 肝]]（Child-Pugh / MELD / Maddrey 等）
> - [[#Renal & Electrolyte 肾与电解质]]（GFR / FENa / 透析急诊等）
> - [[#Neurology 神经]]（NIHSS / GCS / Hunt-Hess 等）
> - [[#Endocrine 内分泌]]（DKA criteria / HbA1c / etc.）
> - [[#Sepsis / ICU 急症]]（qSOFA / SIRS / APACHE 等）
> - [[#Psych 精神]]（PHQ-9 / GAD-7 等）
> - [[#OB/GYN 妇产]]（Bishop / APGAR 等）
> - [[#Pediatrics 儿科]]（APGAR / Tanner 等）
>
> ### 通用 + 易混
> - [[#通用公式 General Formulas]]
> - [[#⚠️ 易混评分对照]]

---

## Cardiovascular 心血管

### CHADS2

**用途**：早期版本的房颤血栓栓塞风险评估，已逐步被 CHA2DS2-VASc 取代；CK 仍可能考"两个评分谁更敏感"对照题。

**计算**：

| 字母 | 含义 | 分值 |
|:---|:---|:---|
| C | Congestive heart failure | 1 |
| H | Hypertension | 1 |
| A | Age ≥ 75 | 1 |
| D | Diabetes | 1 |
| S2 | Stroke / TIA 既往 | 2 |

**Cutoff 解读**：
- 0 → 低危，可不抗凝
- 1 → 中危，可考虑抗凝或抗血小板
- ≥ 2 → 高危，必须口服抗凝

**CK 高频考法**：考"为什么现在不再首选 CHADS2"，答案是它漏掉了女性、血管病变、年龄 65–74 三类中危人群。

**笔记出处**：心内.md（与 CHA2DS2-VASc 对照提及）。

---

### CHA2DS2-VASc

**用途**：非瓣膜性房颤患者的卒中/系统栓塞风险分层，决定是否长期口服抗凝（DOAC 优先，机械瓣/中重度二尖瓣狭窄改 warfarin）。

**计算**：

| 字母 | 含义 | 分值 |
|:---|:---|:---|
| C | Congestive heart failure / LV dysfunction | 1 |
| H | Hypertension | 1 |
| A2 | Age ≥ 75 | 2 |
| D | Diabetes | 1 |
| S2 | Stroke / TIA / 系统血栓栓塞既往 | 2 |
| V | Vascular disease（旧 MI、PAD、主动脉斑块） | 1 |
| A | Age 65–74 | 1 |
| Sc | Sex category = 女性 | 1 |

**Cutoff 解读**（三档决策）：
- 男 0 / 女 1（仅性别）→ **不抗凝**（明确）
- 男 1 / 女 2 → **Shared decision-making**（必须和患者讨论）⚠️ **灰区**（USMLE 沟通伦理考点）
- 男 ≥ 2 / 女 ≥ 3 → **启动 DOAC**（apixaban、rivaroxaban、dabigatran、edoxaban）
- 中重度二尖瓣狭窄或机械瓣 / APS → 跳过评分，直接 warfarin（INR 目标 2–3 或 2.5–3.5）

**Trigger vs Substrate**：AF 抗凝针对的是慢性 **substrate**（心房纤维化、扩大），不是 AF 本身。年轻、可逆诱因（binge drinking / 甲亢 / 急性病）+ normal echo + 无 HTN/HF/DM/卒中 → 评分低 → 不抗凝。

**CK 高频考法**：
- vignette 给 70 岁女性新发房颤 + DM + HTN（= 1+1+1+1 = 4 分）→ 答 DOAC，不要选 aspirin。
- 陷阱 1：女性 0 个其他危险因素时性别分不计入治疗决策。
- 陷阱 2：**DAPT（ASA + clopidogrel）≠ "温和抗凝"** — 出血 ≈ 抗凝、获益 ≪ 抗凝，AF 指南已淘汰。
- 陷阱 3：**ASA 单药**用于 AF 卒中预防基本无效，不推荐。
- 关联错题：[[mistakes/uworld-mistakes_2026-05#^Q4469]] AF + 可逆诱因 + 评分 0 → 不抗凝。

**笔记出处**：心内.md（含完整字母表 + 性别陷阱）。

---

### HAS-BLED

**用途**：评估房颤患者抗凝时的大出血风险，用于"识别和纠正可调整危险因素"，不是用来阻止抗凝。

**计算**：

| 字母 | 含义 | 分值 |
|:---|:---|:---|
| H | Hypertension（SBP > 160） | 1 |
| A | Abnormal renal/liver function（每项 1） | 1–2 |
| S | Stroke 既往 | 1 |
| B | Bleeding 既往或倾向 | 1 |
| L | Labile INR | 1 |
| E | Elderly（> 65） | 1 |
| D | Drugs（NSAID/抗血小板）/酒精（每项 1） | 1–2 |

**Cutoff 解读**：
- ≥ 3 → 高出血风险，密切随访 + 纠正可调因素（控压、停 NSAID、戒酒、稳定 INR）
- 不是抗凝绝对禁忌

**CK 高频考法**：vignette 给一个老人 HAS-BLED = 4 + CHA2DS2-VASc = 5，问下一步。答仍抗凝 + 修正可调危险因素。

**笔记出处**：⚠️ 笔记中未检索到完整字母表，以下基于公开教科书概念整理。

---

### TIMI Risk Score（NSTEMI / UA）

**用途**：NSTEMI/UA 患者 14 天内复合终点（死亡 + 新 MI + 紧急血运重建）风险分层，决定早期侵入策略。

**计算**：

| 项目 | 分值 |
|:---|:---|
| 年龄 ≥ 65 | 1 |
| ≥ 3 个 CAD 危险因素（HTN/DM/家族史/吸烟/高脂） | 1 |
| 已知 CAD（既往 ≥ 50% 狭窄） | 1 |
| 24 h 内服用 ASA | 1 |
| 24 h 内 ≥ 2 次 angina | 1 |
| ST 段偏移 ≥ 0.5 mm | 1 |
| 心肌标志物升高（troponin） | 1 |

**Cutoff 解读**：
- 0–2 → 低危，先 stress test
- 3–4 → 中危
- 5–7 → 高危 → 早期侵入（24 h 内造影 ± PCI）

**CK 高频考法**：稳定 NSTEMI vignette 给 troponin↑、动态 ST 改变、≥ 65 岁 → 高 TIMI → 选"早期冠脉造影"，不要选保守。

**笔记出处**：心内.md（"NSTEMI/UA：TIMI ≥ 3 或 GRACE > 140 → 24h 早期造影"）。

---

### GRACE Score

**用途**：ACS 患者住院期 + 6 个月内死亡风险预测；比 TIMI 更精细，CK 主要识别"GRACE > 140 → 24 h 内造影"这一阈值。

**计算**（关键变量）：

| 变量 | 方向 |
|:---|:---|
| 年龄 | 越大越高 |
| 心率 | 越快越高 |
| 收缩压 | 越低越高 |
| Killip class | 越高越高 |
| 血清肌酐 | 越高越高 |
| 心搏骤停（入院时） | 加分 |
| ST 段偏移 | 加分 |
| 心肌标志物升高 | 加分 |

**Cutoff 解读**：
- < 109 → 低危
- 109–140 → 中危
- \> 140 → 高危 → 24 h 内造影

**CK 高频考法**：vignette 给入院 HR 110、SBP 100、Cr 1.8、troponin 升高 → GRACE 高 → 早期侵入。

**笔记出处**：心内.md（"GRACE > 140 → 24 h 早期造影"，与 TIMI 并列出现）。

---

### NYHA 功能分级

**用途**：心衰症状严重度分级，决定 CRT/ICD/移植资格，是预后指标。

**计算**：

| 级别 | 描述 |
|:---|:---|
| I | 体力活动不受限，常规活动不引发症状 |
| II | 轻度受限，常规活动引发症状（爬两层楼气短） |
| III | 明显受限，少于常规活动即症状（短距步行气短） |
| IV | 任何活动均不适，或静息时即有症状 |

**Cutoff 解读**：
- NYHA II–III + LVEF ≤ 35% + LBBB QRS > 150 ms → CRT 适应证
- NYHA II–III + LVEF ≤ 35% → ICD 一级预防
- NYHA IV 持续 → 评估移植 / LVAD

**CK 高频考法**：vignette 给"轻度活动即气短，但休息时无症状"→ NYHA III → 上 CRT/ICD 决策树。

**笔记出处**：心内.md（CRT/ICD 适应证段）。

---

### Killip 分级（急性 MI）

**用途**：急性 MI 床旁查体快速预后分级，与 30 天死亡率正相关。

**计算**：

| 级别 | 体征 | 估计 30 天死亡率 |
|:---|:---|:---|
| I | 无心衰体征 | ~5% |
| II | 肺底湿啰音 / S3 / 颈静脉怒张 | ~15% |
| III | 急性肺水肿 | ~30% |
| IV | 心源性休克（SBP < 90，组织灌注不足） | ~60–80% |

**Cutoff 解读**：
- 越高死亡率越高
- Killip IV 即心源性休克 → 立即冠脉造影 + 机械支持（IABP / Impella）

**CK 高频考法**：vignette 给 STEMI + 双肺湿罗音满肺 → Killip III → 直接 PCI + IV 利尿。

**笔记出处**：⚠️ 笔记未单独列分级表，以下基于公开教科书概念整理。

---

## Pulmonary / PE 肺与肺栓塞

### Wells Score（PE）

**用途**：评估急诊胸痛/呼吸困难患者 PE 临床概率，决定下一步检查（D-dimer vs CTPA）。

**计算**：

| 项目 | 分值 |
|:---|:---|
| DVT 临床体征 | 3 |
| PE 比其他诊断更可能 | 3 |
| HR > 100 | 1.5 |
| 4 周内制动或手术 | 1.5 |
| 既往 DVT/PE | 1.5 |
| 咯血 | 1 |
| 恶性肿瘤（active 或 6 个月内治疗） | 1 |

**Cutoff 解读**（两层法，最常用）：
- ≤ 4 → "PE unlikely" → 测 D-dimer；阴性排除，阳性 → CTPA
- \> 4 → "PE likely" → 直接 CTPA（肾差/孕妇用 V/Q）

**CK 高频考法**：vignette 给单侧腿肿 + HR 110 + 近期手术（3+1.5+1.5 = 6）→ Wells > 4 → 跳过 D-dimer 直接 CTPA。

**笔记出处**：⚠️ 笔记中未检索到完整 Wells PE 表，以下基于公开教科书概念整理。

---

### Wells Score（DVT）

**用途**：下肢肿胀/疼痛患者 DVT 临床概率，决定下一步是 D-dimer 还是直接超声。

**计算**：

| 项目 | 分值 |
|:---|:---|
| 活动性肿瘤 | 1 |
| 瘫痪/制动 | 1 |
| 卧床 ≥ 3 天或大手术 4 周内 | 1 |
| 沿深静脉走行压痛 | 1 |
| 整条腿肿 | 1 |
| 小腿周径差 > 3 cm | 1 |
| 凹陷性水肿（症状腿更重） | 1 |
| 侧支表浅静脉（非曲张） | 1 |
| 既往 DVT | 1 |
| 替代诊断同样可能 | -2 |

**Cutoff 解读**：
- ≤ 0 → 低概率 → D-dimer；阴性排除
- 1–2 → 中概率 → D-dimer 或超声
- ≥ 3 → 高概率 → 直接压迫超声

**CK 高频考法**：vignette 给恶性肿瘤患者新发单侧腿肿 → 高 Wells → 直接超声，不浪费时间测 D-dimer。

**笔记出处**：⚠️ 笔记中未检索到完整 Wells DVT 表，以下基于公开教科书概念整理。

---

### PERC（Pulmonary Embolism Rule-out Criteria）

**用途**：低概率 PE 患者全部 8 条阴性时，可直接排除 PE 而不必测 D-dimer。

**计算**（全 8 条都必须为"否"才能排除）：

| 项目 | 满足条件 |
|:---|:---|
| 年龄 < 50 | 是 |
| HR < 100 | 是 |
| SpO2 ≥ 95% RA | 是 |
| 无单侧腿肿 | 是 |
| 无咯血 | 是 |
| 4 周内无手术/创伤 | 是 |
| 既往无 DVT/PE | 是 |
| 无外源性雌激素使用 | 是 |

**Cutoff 解读**：
- 全 8 条满足 + 临床低概率 → 排除 PE，停止检查
- 任一条不满足 → 测 D-dimer 或 CTPA

**CK 高频考法**：年轻健康人有焦虑发作 + 胸痛 + RA 100% + HR 80 → PERC 全阴性 → 不需要 D-dimer。

**笔记出处**：⚠️ 笔记中未检索到 PERC，以下基于公开教科书概念整理。

---

### CURB-65

**用途**：CAP 严重度床旁评估，决定门诊 vs 住院 vs ICU。

**计算**：

| 字母 | 含义 | 分值 |
|:---|:---|:---|
| C | Confusion（新发） | 1 |
| U | Urea > 19 mg/dL（BUN > 19） | 1 |
| R | Respiratory rate ≥ 30 | 1 |
| B | BP（SBP < 90 或 DBP ≤ 60） | 1 |
| 65 | Age ≥ 65 | 1 |

**Cutoff 解读**：
- 0–1 → 门诊
- 2 → 住院普通病房
- ≥ 3 → 考虑 ICU

**CK 高频考法**：vignette 给老年 CAP + BUN 升高 + RR 32 + 神志改变 → ≥ 3 → ICU。

**笔记出处**：pulmonary.md（CURB65 五条 + 住院抗生素选择）。

---

### PSI（Pneumonia Severity Index, 简版关键变量）

**用途**：CAP 30 天死亡率分层，比 CURB-65 更精细但变量多，CK 仅识别 5 类分层概念。

**计算**（关键变量）：

| 变量 | 方向 |
|:---|:---|
| 年龄（男岁数 / 女岁数 - 10） | 越大越高 |
| 养老院居住 | +10 |
| 合并症（肿瘤/CHF/CKD/肝/CVA） | 加分 |
| 神志改变、HR ≥ 125、RR ≥ 30、SBP < 90、Temp < 35 或 ≥ 40 | 加分 |
| 实验室：pH < 7.35、BUN ≥ 30、Na < 130、Glc ≥ 250、Hct < 30、PaO2 < 60、胸腔积液 | 加分 |

**Cutoff 解读**：
- Class I–II → 门诊
- Class III → 短期观察
- Class IV–V → 住院 / ICU

**CK 高频考法**：CK 较少直接算 PSI，主要识别"PSI 比 CURB-65 更全面，住院判定更准"。

**笔记出处**：⚠️ 笔记未提及 PSI 简版，以下基于公开教科书概念整理。

---

## Hepatology 肝

### MELD（简版）

**用途**：肝硬化患者 90 天死亡率预测，肝移植排序的核心指标。

**计算**（关键变量，logarithmic）：

| 变量 | 方向 |
|:---|:---|
| Bilirubin | 越高越高 |
| INR | 越高越高 |
| Creatinine | 越高越高（透析者按 4.0 算） |
| Sodium（MELD-Na 加入） | 越低越高 |

**Cutoff 解读**：
- < 9 → 90 天死亡率约 2%
- 10–19 → 约 6–20%
- 20–29 → 约 20–55%
- ≥ 30 → > 50%
- 移植上线常需 MELD ≥ 15

**CK 高频考法**：vignette 给晚期肝硬化患者讨论移植资格 → 答 MELD-Na 决定排序。

**笔记出处**：⚠️ 笔记未单独建表，以下基于公开教科书概念整理。

---

### Child-Pugh

**用途**：肝硬化代偿/失代偿分级，预测手术风险与 1–2 年生存率，临床决策（如 NSBB、TIPS）。

**计算**：

| 项目 | 1 分 | 2 分 | 3 分 |
|:---|:---|:---|:---|
| Bilirubin (mg/dL) | < 2 | 2–3 | > 3 |
| Albumin (g/dL) | > 3.5 | 2.8–3.5 | < 2.8 |
| INR | < 1.7 | 1.7–2.3 | > 2.3 |
| Ascites | 无 | 轻 | 中重 |
| Encephalopathy | 无 | I–II | III–IV |

**Cutoff 解读**：
- A（5–6 分）→ 代偿，1 年生存 ~100%
- B（7–9 分）→ 代偿性失代偿，1 年 ~80%
- C（10–15 分）→ 失代偿，1 年 ~45%
- Child C 静脉曲张可启动 NSBB；Child C 一般不耐受大手术

**CK 高频考法**：vignette 给肝硬化 + 腹水中量 + 低 albumin + INR 升高 → 算 B/C → 决定胃镜/NSBB 时机。

**笔记出处**：消化腺.md（"Child-Pugh C 级建议使用 NSBB"等条目，未列完整 5 项表）。

---

### Maddrey Discriminant Function (DF)（酒精性肝炎）

**用途**：判断重症酒精性肝炎是否启动 prednisolone 治疗。

**计算**：

| 公式 |
|:---|
| DF = 4.6 × (PT 患者 - PT 对照) + Total bilirubin (mg/dL) |

**Cutoff 解读**：
- DF ≥ 32 → 重症 → 启动 prednisolone 28 天（GI 出血/感染/肾衰是相对禁忌；胰腺炎也避免）
- 7 天后 Lille 评分 ≥ 0.45 → 治疗失败，停药

**CK 高频考法**：vignette 给酗酒+黄疸+发热+白细胞↑+PT 延长 16 s + Bili 12 → 算 DF ≈ 4.6×16 + 12 ≈ 86 → 上糖皮质激素（先排除感染/GIB）。

**笔记出处**：⚠️ 笔记未提及 Maddrey，以下基于公开教科书概念整理。

---

## Renal & Electrolyte 肾与电解质

### eGFR（Cockcroft-Gault）

**用途**：估算肌酐清除率，主要用于药物剂量调整（不再用于 CKD 分期，CKD 分期用 CKD-EPI）。

**计算**：

| 公式 |
|:---|
| CrCl = [(140 - 年龄) × 体重 (kg)] / [72 × Cr (mg/dL)] × (女性 × 0.85) |

**Cutoff 解读**（CKD 分期用 CKD-EPI eGFR，单位 mL/min/1.73 m²）：
- ≥ 90 → G1（伴蛋白尿/影像异常才算 CKD）
- 60–89 → G2
- 45–59 → G3a
- 30–44 → G3b
- 15–29 → G4
- < 15 → G5（透析准备）

**CK 高频考法**：老年瘦弱女性 Cr 1.0 但 CrCl 实际只有 30 → 减药（如 enoxaparin、阿昔洛韦、二甲双胍）。陷阱：肌酐"正常"≠ 肾功能正常。

**笔记出处**：肾脏.md（多处 "AKI / eGFR 低"条目）。

---

### Anion Gap

**用途**：代谢性酸中毒分类（高 AG vs 正常 AG）。

**计算**：

| 公式 |
|:---|
| AG = Na - (Cl + HCO3) |
| 校正 AG = AG + 2.5 × (4 - albumin) |

**Cutoff 解读**：
- 正常 AG ≈ 8–12
- AG > 12 → 高 AG 代谢性酸中毒（MUDPILES：Methanol、Uremia、DKA、Propylene glycol、Iron/INH、Lactic、Ethylene glycol、Salicylates）
- 正常 AG → HARDASS：腹泻、Renal tubular acidosis、Acetazolamide、Spironolactone、Saline

**CK 高频考法**：低白蛋白患者 AG"看似正常"实则升高 → 必须校正。

**笔记出处**：⚠️ 笔记未单独列公式，以下基于公开教科书概念整理。

---

### FeNa（Fractional Excretion of Sodium）

**用途**：少尿型 AKI 鉴别 prerenal vs intrinsic（ATN）。利尿剂使用时改用 FeUrea。

**计算**：

| 公式 |
|:---|
| FeNa% = (Urine Na × Plasma Cr) / (Plasma Na × Urine Cr) × 100 |
| FeUrea% = (Urine BUN × Plasma Cr) / (Plasma BUN × Urine Cr) × 100 |

**Cutoff 解读**：
- FeNa < 1% → Prerenal（容量不足、心衰、肝肾综合征）；BUN/Cr > 20:1
- FeNa > 2% → ATN/intrinsic；BUN/Cr < 20:1
- FeNa 1–2% → 不确定
- 利尿剂下：FeUrea < 35% → prerenal

**CK 高频考法**：vignette 给少尿 + 大手术失血 + BUN 60 / Cr 2.0（比 30:1）+ FeNa 0.5% → prerenal → 补液。

**笔记出处**：肾脏.md（"BUN:Cr > 20:1 + FeNa < 1% + Urine Na < 20"经典 prerenal 三联表）。

---

### Corrected Calcium（校正钙）

**用途**：低白蛋白时血清总钙看似低，需校正以判断真正的钙离子水平。

**计算**：

| 公式 |
|:---|
| Corrected Ca = 测量 Ca + 0.8 × (4.0 - albumin g/dL) |

**Cutoff 解读**：
- 正常校正钙 8.5–10.5 mg/dL
- 危急：校正钙 < 7 或 > 14 → 立即处理
- 也可直接测 ionized Ca 取代校正

**CK 高频考法**：肾病综合征/肝硬化患者 albumin 2.0、Ca 7.5 → 校正 = 7.5 + 0.8×2 = 9.1 → 实际正常，不必补钙。

**笔记出处**：⚠️ 笔记未单独列公式，以下基于公开教科书概念整理。

---

### Creatinine Clearance（24 h 尿）

**用途**：金标准评估 GFR，但实操少用，主要用于 Cockcroft-Gault 不准的人群（极胖、极瘦、肌肉萎缩）。

**计算**：

| 公式 |
|:---|
| CrCl = (Urine Cr × Urine volume) / (Plasma Cr × time in min) |

**Cutoff 解读**：
- < 60 → CKD 倾向（需要慢性 + 影像/蛋白尿才算 CKD）
- 留尿不全的标志：24 h 尿肌酐量过低（男 ~20 mg/kg、女 ~15 mg/kg）

**CK 高频考法**：质疑"为什么这个肌肉萎缩老人 Cr 0.7 但需要减药"→ 真实 CrCl 已经很低。

**笔记出处**：⚠️ 笔记未单独列公式，以下基于公开教科书概念整理。

---

## Neurology 神经

### NIHSS（NIH Stroke Scale）

**用途**：急性卒中严重度评估，决定 tPA / 血管内取栓资格、预后预测。

**计算**（11 大项 0–42 分，简版关键域）：

| 域 | 分值范围 |
|:---|:---|
| 意识水平 | 0–3 |
| 凝视 | 0–2 |
| 视野 | 0–3 |
| 面瘫 | 0–3 |
| 上肢运动（左/右） | 0–4 each |
| 下肢运动（左/右） | 0–4 each |
| 共济失调 | 0–2 |
| 感觉 | 0–2 |
| 语言 | 0–3 |
| 构音 | 0–2 |
| 忽略 | 0–2 |

**Cutoff 解读**：
- 0 → 无症状
- 1–4 → 轻
- 5–15 → 中
- 16–20 → 中重
- 21–42 → 重
- NIHSS ≥ 6 + 大血管闭塞（ICA/M1）+ 24 h 内 → 评估机械取栓
- NIHSS > 25 → tPA 相对禁忌（出血风险）

**CK 高频考法**：vignette 给醒后偏瘫 NIHSS 18 + LKW 5 h → 取栓窗口（6–24 h，配合灌注影像）。

**笔记出处**：⚠️ 笔记未单独建 NIHSS 表，以下基于公开教科书概念整理。

---

### GCS（Glasgow Coma Scale）

**用途**：意识水平床旁分级；TBI、内科昏迷、ICU 监测均用。总分 3–15。

**计算**：

| 域 | 分值 | 描述 |
|:---|:---|:---|
| 睁眼 E | 4 | 自发 |
|  | 3 | 呼之 |
|  | 2 | 疼痛刺激 |
|  | 1 | 无反应 |
| 言语 V | 5 | 切题 |
|  | 4 | 错乱 |
|  | 3 | 不当词 |
|  | 2 | 难以理解的声音 |
|  | 1 | 无 |
| 运动 M | 6 | 听指令 |
|  | 5 | 定位疼痛 |
|  | 4 | 屈曲回避 |
|  | 3 | 异常屈曲（去皮层） |
|  | 2 | 异常伸直（去大脑） |
|  | 1 | 无 |

**Cutoff 解读**：
- 13–15 → 轻度脑损伤
- 9–12 → 中度
- ≤ 8 → 重度 → 气管插管保护气道
- GCS 3 = 最低（不能为 0）

**CK 高频考法**：TBI vignette + GCS 7 → 立即插管。

**笔记出处**：⚠️ 笔记未单独建表，以下基于公开教科书概念整理。

---

### Hunt-Hess Scale（SAH）

**用途**：动脉瘤性蛛网膜下腔出血严重度分级，预测预后与手术时机。

**计算**：

| 级别 | 描述 |
|:---|:---|
| I | 无症状或轻微头痛 + 轻度颈强 |
| II | 中重度头痛 + 颈强 ± 颅神经麻痹（无其他神经缺损） |
| III | 嗜睡 + 轻局灶缺损 |
| IV | 昏迷 + 中重度偏瘫 + 早期去脑 |
| V | 深昏迷 + 去大脑 + 濒死 |

**Cutoff 解读**：
- I–III → 较好预后，可早期开颅或介入
- IV–V → 预后差，先稳定再决策

**CK 高频考法**：vignette "the worst headache of my life" + 颈强 + 嗜睡 → Hunt-Hess III → 立即 CT 头颅，阴性 → LP 找黄变。

**笔记出处**：⚠️ 笔记未单独列分级表，以下基于公开教科书概念整理。

---

### ABCD2（TIA 后卒中风险）

**用途**：TIA 患者 2/7/90 天卒中风险预测，决定门诊 vs 住院评估。

**计算**：

| 字母 | 含义 | 分值 |
|:---|:---|:---|
| A | Age ≥ 60 | 1 |
| B | BP ≥ 140/90 | 1 |
| C | Clinical：单侧无力 = 2；言语障碍无力 = 1 | 0–2 |
| D | Duration：≥ 60 min = 2；10–59 min = 1 | 0–2 |
| D | Diabetes | 1 |

**Cutoff 解读**：
- 0–3 → 低危
- 4–5 → 中危
- 6–7 → 高危 → 住院/快速评估
- 当代趋势：所有 TIA 都建议 24–48 h 内全面影像 + 病因评估，分数仅作辅助

**CK 高频考法**：vignette 给 70 岁 + HTN + 单侧无力 90 min → ABCD2 = 1+1+2+2 = 6 → 住院。

**笔记出处**：⚠️ 笔记未单独列 ABCD2，以下基于公开教科书概念整理。

---

## Endocrine 内分泌

### Diabetes Diagnostic Criteria（成人 T2DM）

**用途**：诊断 DM；任一标准满足且确认（无症状者第二次）即可。

**计算**：

| 项目 | 阈值 |
|:---|:---|
| HbA1c | ≥ 6.5% |
| FPG（≥ 8 h 空腹） | ≥ 126 mg/dL |
| OGTT 2 h（75 g） | ≥ 200 mg/dL |
| 随机血糖 + 高血糖症状 | ≥ 200 mg/dL（单次即可） |

**Prediabetes**：
- A1c 5.7–6.4%
- FPG 100–125
- OGTT 2 h 140–199

**Cutoff 解读**：
- 任一阳性 + 第二次确认（不同日或不同方法）→ 诊断 DM
- 单次随机 ≥ 200 + 典型症状（多饮多尿体重↓）→ 单次即诊断

**CK 高频考法**：vignette 给 PCOS / HTN 患者初查 → 选 FPG 或 A1c 筛查（35–70 岁 + BMI ≥ 25 普筛）。

**笔记出处**：endocrine.md（"Random > 200 with symptoms / A1c > 6.5% / FPG ≥ 126"等条目）。

---

### DKA Diagnostic Criteria

**用途**：诊断糖尿病酮症酸中毒，决定 IVF + 胰岛素 + 钾路径。

**计算**：

| 项目 | 阈值 |
|:---|:---|
| 血糖 | > 250 mg/dL（妊娠或 SGLT2 可正常） |
| pH | < 7.30 |
| HCO3 | < 18 |
| Ketones（β-OHB 或尿酮） | 阳性 |
| Anion gap | > 10–12 |
| 神志 | 警觉或轻度改变 |

**严重度**：
- 轻：pH 7.25–7.30
- 中：pH 7.00–7.24
- 重：pH < 7.00

**CK 高频考法**：vignette 给 T1DM 青年 + 腹痛呕吐 + 血糖 450 + AG 28 + pH 7.15 → 中重 DKA → IVF 优先 → 钾正常或低 → 先补钾再上 insulin（K < 3.3 时禁用 insulin）。

**笔记出处**：endocrine.md（DKA / HHS 对比条目）。

---

### HHS Diagnostic Criteria

**用途**：诊断高渗性高血糖状态（多见老年 T2DM），治疗以补液为主。

**计算**：

| 项目 | 阈值 |
|:---|:---|
| 血糖 | > 600 mg/dL |
| 血浆渗透压 | > 320 mOsm/kg |
| pH | > 7.30 |
| HCO3 | > 18 |
| Ketones | 阴性或微量 |
| Anion gap | 正常 |
| 神志 | 明显改变（昏睡至昏迷） |

**Cutoff 解读**：
- 治疗顺序：先大量补液（NS 1–1.5 L/h × 2 h）→ 纠 K → 再上 insulin
- 死亡率高于 DKA（10–20% vs 2–5%）

**CK 高频考法**：vignette 给 75 岁 T2DM + 神志改变 + 血糖 800 + 渗透压 340 + 无酮 → HHS → 立即查 chemistry + 大量补液。

**笔记出处**：endocrine.md（"HHS：老年 T2DM，血糖 > 600，渗透压 > 320，无酮，神志改变"）。

---

### 儿童 DM 诊断

**用途**：儿童糖尿病诊断阈值与成人相同；T1DM 占儿童多数，但肥胖儿童 T2DM 增多。

**计算**：

| 项目 | 阈值（同成人） |
|:---|:---|
| HbA1c | ≥ 6.5% |
| FPG | ≥ 126 |
| OGTT 2 h | ≥ 200 |
| 随机 + 症状 | ≥ 200 |

**Cutoff 解读**：
- T1DM 起病常急（多尿多饮 + 消瘦数周 + 经常以 DKA 首发）→ 立即胰岛素，不等 OGTT
- T2DM 儿童肥胖 + 黑棘皮 → 同成人阈值，但首选 metformin（如肾不耐 + A1c < 9 + 无 DKA）

**CK 高频考法**：vignette 给 12 岁瘦弱儿童突发多尿 + Glucose 500 + 酮体 + AG 高 → T1DM + DKA → 直接收住院。

**笔记出处**：⚠️ 笔记未单独建儿童糖尿病诊断表，以下基于公开教科书概念整理。

---

## Sepsis / ICU 急症

### qSOFA

**用途**：床旁快速筛查 sepsis 高死亡风险（不需实验室）。

**计算**：

| 项目 | 阈值 | 分值 |
|:---|:---|:---|
| Respiratory rate | ≥ 22 | 1 |
| Altered mentation | GCS < 15 | 1 |
| Systolic BP | ≤ 100 | 1 |

**Cutoff 解读**：
- ≥ 2 → 高死亡风险，进入 sepsis 评估通路
- 不再用作 sepsis 诊断标准（2021 SSC 已退化为筛查）

**CK 高频考法**：vignette 给老人发热 + RR 24 + SBP 90 + 淡漠 → qSOFA = 3 → 启动 sepsis bundle。

**笔记出处**：⚠️ 笔记未单独列 qSOFA，以下基于公开教科书概念整理。

---

### SOFA（简版）

**用途**：ICU sepsis 器官功能障碍量化；Sepsis 当前定义 = 感染 + SOFA 升高 ≥ 2。

**计算**（6 系统 0–4 分各，总 0–24）：

| 系统 | 关键变量 |
|:---|:---|
| Respiratory | PaO2/FiO2 |
| Coagulation | Platelet 计数 |
| Liver | Bilirubin |
| Cardiovascular | MAP / 升压药剂量 |
| CNS | GCS |
| Renal | Cr 或尿量 |

**Cutoff 解读**：
- ≥ 2 分增加（基于基线）→ Sepsis（在感染语境下）
- Septic shock = 充分补液后仍需升压药维持 MAP ≥ 65 + 乳酸 > 2

**CK 高频考法**：识别 sepsis 现代定义"感染 + SOFA ≥ 2"。

**笔记出处**：⚠️ 笔记未单独建 SOFA 表，以下基于公开教科书概念整理。

---

### SIRS（旧标准，仍 CK 出题）

**用途**：早期非特异性筛查；当前已被 Sepsis-3 取代，但仍是 CK 经典考点。

**计算**：

| 项目 | 阈值 |
|:---|:---|
| Temp | > 38 或 < 36 |
| HR | > 90 |
| RR | > 20 或 PaCO2 < 32 |
| WBC | > 12 或 < 4 或 > 10% bands |

**Cutoff 解读**：
- ≥ 2 项 → SIRS
- SIRS + 感染源 = 旧定义 sepsis（已淘汰但 CK 仍考）
- SIRS + 器官衰竭 = 旧定义 severe sepsis

**CK 高频考法**：vignette 给 T 39 + HR 110 + RR 24 + WBC 18 → 满足 SIRS → 找感染源。

**笔记出处**：⚠️ 笔记未单独列 SIRS，以下基于公开教科书概念整理。

---

## Psych 精神

### PHQ-9 / PHQ-2

**用途**：抑郁筛查（PHQ-2）+ 严重度量化（PHQ-9）。

**计算**：

PHQ-2（两题）：

| 项目 | 描述 |
|:---|:---|
| 1 | 过去 2 周兴趣丧失 |
| 2 | 过去 2 周情绪低落 |

每题 0–3，总 0–6。

PHQ-9（九题）：在 PHQ-2 基础上加 7 题（睡眠、能量、食欲、自责、注意力、精神运动、自杀意念）。每题 0–3，总 0–27。

**Cutoff 解读**：
- PHQ-2 ≥ 3 → 进 PHQ-9
- PHQ-9：5–9 轻、10–14 中、15–19 中重、20–27 重
- ≥ 10 → 启动治疗（SSRI ± CBT）
- 任何"自杀意念"题阳性 → 立即评估安全

**CK 高频考法**：成人初筛抑郁选 PHQ-2/PHQ-9。任何分值搭配自杀意念阳性 → 安全评估优先。

**笔记出处**：_衍生_鉴别诊断速查.md（PHQ-9 用于 depression workflow）。

---

### GAD-7

**用途**：广泛性焦虑筛查与严重度。

**计算**：

| 7 项内容 |
|:---|
| 紧张/不安 |
| 难控制担忧 |
| 担心多事 |
| 难放松 |
| 坐立不安 |
| 易激惹 |
| 害怕"坏事将发生" |

每项 0–3，总 0–21。

**Cutoff 解读**：
- 5–9 → 轻度
- 10–14 → 中度
- 15–21 → 重度
- ≥ 10 → 进一步评估，启动 SSRI/SNRI ± CBT

**CK 高频考法**：成人焦虑筛查首选 GAD-7。

**笔记出处**：⚠️ 笔记未提及，以下基于公开教科书概念整理。

---

### MMSE（Mini-Mental State Exam）

**用途**：认知障碍/痴呆床旁筛查（受教育程度有限时使用）。

**计算**：

| 域 | 分值 |
|:---|:---|
| 定向（时间 + 地点） | 10 |
| 注册（3 词） | 3 |
| 注意/计算（serial 7 或 spell WORLD 倒序） | 5 |
| 回忆（3 词） | 3 |
| 命名 + 复述 + 阅读 + 书写 + 三步指令 + 抄绘 | 9 |

总 0–30。

**Cutoff 解读**：
- ≥ 24 → 正常（受教育影响）
- 19–23 → 轻度
- 10–18 → 中度
- < 10 → 重度
- 受教育程度低 → 假阳性
- MoCA 对轻度认知障碍更敏感

**CK 高频考法**：老人记忆减退筛查首选 MMSE 或 MoCA；筛阳后 → 排除可逆原因（B12、TSH、neurosyphilis、NPH）。

**笔记出处**：⚠️ 笔记未单独建 MMSE 表，以下基于公开教科书概念整理。

---

### MoCA（Montreal Cognitive Assessment）

**用途**：MCI（轻度认知障碍）筛查，较 MMSE 更敏感于早期。

**计算**：

| 域 |
|:---|
| 视觉空间/执行（连线 + 立方体 + 钟表） |
| 命名（动物） |
| 注意（数字 + 字母 + serial 7） |
| 语言（重复 + 流畅性） |
| 抽象 |
| 延迟回忆 |
| 定向 |

总 0–30，受教育 ≤ 12 年加 1 分。

**Cutoff 解读**：
- ≥ 26 → 正常
- < 26 → 异常 → 进一步评估

**CK 高频考法**：vignette 给"早期记忆/找词困难但日常生活独立"→ MoCA 比 MMSE 更敏感。

**笔记出处**：⚠️ 笔记未提及，以下基于公开教科书概念整理。

---

### AUDIT-C / CAGE

**用途**：酒精使用障碍筛查。AUDIT-C 是 USPSTF 推荐的初筛；CAGE 历史经典。

**计算**：

AUDIT-C（3 项 0–4 分）：

| 项目 |
|:---|
| 频率（多久喝一次） |
| 量（典型一次几杯） |
| 暴饮（多久 ≥ 6 杯一次） |

总 0–12。

CAGE（4 项 yes/no）：

| 字母 | 问题 |
|:---|:---|
| C | 想 Cut down？ |
| A | 别人 Annoyed 你的喝法？ |
| G | 喝酒让你 Guilty？ |
| E | 早起 Eye-opener（晨饮）？ |

**Cutoff 解读**：
- AUDIT-C：男 ≥ 4，女 ≥ 3 → 阳性 → 简短咨询/进一步评估
- CAGE：≥ 2 → 阳性 → 进一步评估
- 两者均为筛查，确诊用 DSM-5 AUD 标准

**CK 高频考法**：成人初查酒精问题 → AUDIT-C；CAGE ≥ 2 + 否认 → 表现型 enabler/家庭。

**笔记出处**：⚠️ 笔记未单独列，以下基于公开教科书概念整理。

---

### CIWA-Ar（Alcohol Withdrawal）

**用途**：酒精戒断严重度量化，指导 benzodiazepine 剂量。

**计算**（10 项各 0–7，恶心/震颤/出汗/焦虑/激越/触觉/听觉/视觉/头痛/定向）：

| 总分 | 严重度 |
|:---|:---|
| < 10 | 轻 |
| 10–18 | 中 |
| ≥ 19 | 重，谵妄震颤风险高 |

**Cutoff 解读**：
- < 10 → 监测
- ≥ 10 → benzodiazepine（lorazepam 肝差选；diazepam/chlordiazepoxide 肝功好用）
- 谵妄震颤（DT）= 戒断 48–96 h + 自主神经亢进 + 幻觉 + 定向障碍 → 死亡率 ~5%，需 ICU

**CK 高频考法**：住院 48 h 戒酒老人发热 + 心动过速 + 震颤 + 幻视 → DT → IV BZD + 监护。

**笔记出处**：⚠️ 笔记未提及，以下基于公开教科书概念整理。

---

## OB/GYN 妇产

### Bishop Score

**用途**：评估宫颈成熟度，判断引产成功概率与方法。

**计算**：

| 项目 | 0 | 1 | 2 | 3 |
|:---|:---|:---|:---|:---|
| Dilation (cm) | 关闭 | 1–2 | 3–4 | ≥ 5 |
| Effacement (%) | 0–30 | 40–50 | 60–70 | ≥ 80 |
| Station | -3 | -2 | -1/0 | +1/+2 |
| Consistency | 硬 | 中 | 软 | — |
| Position | 后 | 中 | 前 | — |

**Cutoff 解读**：
- ≥ 8 → 宫颈成熟，引产成功率高（直接 oxytocin/AROM）
- ≤ 6 → 不成熟 → 先催熟（misoprostol、dinoprostone、Foley）
- 7 → 中间区

**CK 高频考法**：vignette 给孕妇 41 周 + Bishop 4 → 先 prostaglandin 催熟。

**笔记出处**：⚠️ 笔记未单独建 Bishop 表，以下基于公开教科书概念整理。

---

### Apgar Score

**用途**：新生儿生后 1 min / 5 min（必要时 10 min）即时评估。

**计算**：

| 项目 | 0 | 1 | 2 |
|:---|:---|:---|:---|
| Appearance（肤色） | 全身青紫/苍白 | 躯干红末端青 | 全身红 |
| Pulse | 无 | < 100 | ≥ 100 |
| Grimace（反射激惹） | 无 | 皱眉 | 哭 |
| Activity（肌张力） | 软 | 屈曲减少 | 主动屈 |
| Respiration | 无 | 慢/不规则 | 强哭 |

**Cutoff 解读**：
- 7–10 → 正常
- 4–6 → 中度抑制 → 复苏
- 0–3 → 重度抑制 → 立即复苏
- 不用于决定是否复苏（复苏看呼吸/HR/张力 NRP）；用于反映复苏效果

**CK 高频考法**：5 min Apgar < 7 → 继续每 5 min 评估至 20 min；< 5 → 高风险脑损伤。

**笔记出处**：⚠️ 笔记未单独列 Apgar 表，以下基于公开教科书概念整理。

---

### Modified Biophysical Profile（BPP）

**用途**：胎儿宫内健康综合评估，5 项 ×2 分（满分 10）；Modified BPP = NST + AFI。

**计算**（完整 BPP 5 项）：

| 项目 | 2 分标准 |
|:---|:---|
| NST（胎心反应） | reactive |
| 胎儿呼吸运动 | ≥ 30 sec 持续 / 30 min |
| 胎动 | ≥ 3 次身体或肢体动作 / 30 min |
| 张力 | ≥ 1 次屈伸 |
| AFI | 单最大囊袋 ≥ 2 cm 或 AFI > 5 |

**Cutoff 解读**：
- 8–10 → 正常
- 6 → 可疑，重复
- ≤ 4 → 异常，考虑分娩
- Modified BPP 阴性 + AFI 正常 → 可不做完整 BPP

**CK 高频考法**：高危妊娠产前监护 → 先 NST，再 BPP；BPP 4 分 + 足月 → 立即分娩。

**笔记出处**：⚠️ 笔记未单独建 BPP 表，以下基于公开教科书概念整理。

---

### Naegele 规则（EDD 计算）

**用途**：根据 LMP 计算预产期。

**计算**：

| 公式 |
|:---|
| EDD = LMP + 1 年 - 3 月 + 7 天 |
| 等价：LMP + 280 天 |

**Cutoff 解读**：
- 按 28 天月经周期推；周期长则 EDD 后移
- 早孕期 US（CRL，<13+6 周）若与 LMP 差 > 7 天，以 US 为准
- Term 38 0/7–41 6/7 周；41 周 → 引产或加强监护

**CK 高频考法**：LMP 与首次 US 不一致 vignette → 早孕 US 优先确定 EDD。

**笔记出处**：⚠️ 笔记未单独提 Naegele，以下基于公开教科书概念整理。

---

## Pediatrics 儿科

### Apgar（cross-ref）

见 OB/GYN 章节。儿科常考"5 min Apgar 为何更重要"——预后相关性更高。

---

### Centor / Modified McIsaac（GAS 咽炎）

**用途**：成人/儿童咽炎判断 GAS 概率，决定是否做 RADT/培养。

**计算**：

| 项目 | 分值 |
|:---|:---|
| 体温 > 38 | 1 |
| 无咳嗽 | 1 |
| 颈前淋巴结肿大压痛 | 1 |
| 扁桃体渗出/肿大 | 1 |
| Modified（McIsaac）：年龄 3–14 | +1 |
| Modified：年龄 15–44 | 0 |
| Modified：年龄 ≥ 45 | -1 |

**Cutoff 解读**：
- 0–1 → 不查不治
- 2–3 → RADT；阳性 → 治；阴性（儿童）→ 培养
- 4–5 → RADT；治疗大概率开始（部分指南）
- 治疗：penicillin V 或 amoxicillin（青霉素过敏 → cephalexin/macrolide）

**CK 高频考法**：vignette 给 8 岁儿童发热咽痛颈淋巴结肿大无咳嗽 → Centor 4 → RADT；阴性补培养（儿童特别强调）。

**笔记出处**：⚠️ 笔记未单独建 Centor 表，以下基于公开教科书概念整理。

---

### 儿童 BMI 百分位解读

**用途**：儿童 ≥ 2 岁体重分类（成人 BMI 阈值不适用，因发育阶段）。

**计算**：

| 百分位 | 分类 |
|:---|:---|
| < 5th | 偏瘦 |
| 5th–84th | 正常 |
| 85th–94th | 超重 |
| ≥ 95th | 肥胖 |
| ≥ 99th | 重度肥胖 |

**Cutoff 解读**：
- ≥ 95th → 评估合并症（HTN、T2DM、NAFLD、OSA、PCOS）
- 85th–94th + 合并症 → 同 95th 处理

**CK 高频考法**：12 岁 BMI 32 → 95th 以上 → 筛 A1c、ALT、lipid。

**笔记出处**：⚠️ 笔记未提及，以下基于公开教科书概念整理。

---

## 通用公式 General Formulas

### BMI 分类（成人）

**用途**：成人体重分类，决定肥胖治疗与并发症筛查。

**计算**：

| 公式 |
|:---|
| BMI = 体重 (kg) / 身高² (m²) |
| BMI = 体重 (lb) × 703 / 身高² (in²) |

**Cutoff 解读**：

| BMI | 分类 |
|:---|:---|
| < 18.5 | 偏瘦 |
| 18.5–24.9 | 正常 |
| 25.0–29.9 | 超重 |
| 30.0–34.9 | 一级肥胖 |
| 35.0–39.9 | 二级肥胖 |
| ≥ 40 | 三级（severe/morbid） |

**CK 高频考法**：BMI ≥ 35 + 合并症 或 BMI ≥ 40 → 减重手术指征；BMI ≥ 30（或 ≥ 27 + 合并症）→ 药物（liraglutide、semaglutide、phentermine-topiramate）。

**笔记出处**：endocrine.md（"35–70 岁 + BMI ≥ 25 普筛糖尿病"）。

---

### Mean Arterial Pressure (MAP)

**用途**：组织灌注压估算，sepsis/休克目标 ≥ 65 mmHg。

**计算**：

| 公式 |
|:---|
| MAP ≈ DBP + 1/3 (SBP - DBP) |
| 或 MAP = (SBP + 2×DBP) / 3 |

**Cutoff 解读**：
- 正常 70–100
- < 60 → 器官灌注不足
- Sepsis 目标 ≥ 65（充分补液后用 norepinephrine）
- 急性脑出血降压目标 SBP 130–140，注意维持 CPP（CPP = MAP - ICP）

**CK 高频考法**：sepsis vignette 给 BP 85/50 → MAP ≈ 62 → 升压药；不做"等会儿再说"。

**笔记出处**：⚠️ 笔记未单独建公式，以下基于公开教科书概念整理。

---

### A-a Gradient（肺泡-动脉氧分压差）

**用途**：低氧血症机制鉴别（V/Q 失调、shunt vs 通气不足/高海拔）。

**计算**：

| 公式 |
|:---|
| PAO2 = FiO2 × (Patm - PH2O) - PaCO2/0.8 |
| 海平面 RA：PAO2 ≈ 150 - PaCO2/0.8 |
| A-a = PAO2 - PaO2 |

**Cutoff 解读**：
- 正常 ≈ 年龄/4 + 4（青壮年 < 15）
- A-a 增大 → V/Q 失调（COPD、PE、肺炎）、shunt（ARDS、肺水肿、心内分流，吸氧不纠正）、弥散障碍（肺纤维化）
- A-a 正常 + 低氧 → 通气不足（药物/CNS）或高海拔（FiO2 低）

**CK 高频考法**：vignette 给阿片中毒患者 PaO2 60 + PaCO2 60 → A-a 正常 → 通气不足 → naloxone；ARDS PaO2 60 on 100% FiO2 → A-a 大且吸氧不改善 → shunt。

**笔记出处**：⚠️ 笔记未单独建公式，以下基于公开教科书概念整理。

---

### Winters Formula（代谢性酸中毒预测 PCO2）

**用途**：判断代谢性酸中毒患者呼吸代偿是否充分（混合酸碱）。

**计算**：

| 公式 |
|:---|
| 预期 PaCO2 = 1.5 × HCO3 + 8 ± 2 |

**Cutoff 解读**：
- 实际 PaCO2 ≈ 预期 → 单纯代谢酸 + 适当呼吸代偿
- 实际 PaCO2 > 预期 → 合并呼吸性酸中毒
- 实际 PaCO2 < 预期 → 合并呼吸性碱中毒

**CK 高频考法**：DKA 患者 HCO3 10 → 预期 PaCO2 ≈ 23 ± 2；若实际 PaCO2 35 → 合并呼吸酸（疲劳/插管前兆）。Salicylate 中毒：HCO3 14 + 预期 PaCO2 ≈ 29，但实际 22 → 合并呼吸碱（典型 mixed picture）。

**笔记出处**：⚠️ 笔记未单独建公式，以下基于公开教科书概念整理。

---

## ⚠️ 易混评分对照

### CHADS2 vs CHA2DS2-VASc

| 维度 | CHADS2 | CHA2DS2-VASc |
|:---|:---|:---|
| 项目数 | 5 | 8 |
| 包含女性 | 否 | 是（1 分） |
| 包含血管病 | 否 | 是（1 分） |
| 年龄分层 | 仅 ≥ 75（1 分） | 65–74（1 分），≥ 75（2 分） |
| 抗凝阈值 | ≥ 2 | 男 ≥ 2 / 女 ≥ 3 |
| 现行使用 | 已淘汰 | 现行金标准 |

**何时用哪个**：现在临床和 USMLE 都默认用 CHA2DS2-VASc（更敏感，涵盖女性/血管病史/年龄分层）。CHADS2 只在历史题目或对照题中出现。

---

### Wells PE vs Wells DVT

| 维度 | Wells PE | Wells DVT |
|:---|:---|:---|
| 临床场景 | 胸痛/呼吸困难疑 PE | 单侧腿肿/痛疑 DVT |
| 关键变量 | "PE 比其他诊断更可能"（3 分） + 既往 PE/DVT | 沿深静脉走行压痛 + 整条腿肿 + 周径差 |
| Cutoff（两层法） | ≤ 4 unlikely / > 4 likely | ≤ 0 低 / 1–2 中 / ≥ 3 高 |
| Unlikely 下一步 | D-dimer | D-dimer |
| Likely 下一步 | CTPA（孕/肾差选 V/Q） | 压迫超声 |

**何时用哪个**：症状决定。腿肿先 Wells DVT，胸痛先 Wells PE；不要混用变量。

---

### TIMI vs GRACE

| 维度 | TIMI | GRACE |
|:---|:---|:---|
| 终点 | 14 天死亡 + 新 MI + 紧急血运重建 | 院内 + 6 个月死亡 |
| 变量数 | 7 | 8（含连续变量） |
| 计算方式 | 简单加分 | 加权（需在线计算器） |
| 阈值 | ≥ 3 中高危 | > 140 高危 |
| 优势 | 床旁速算 | 更精准 |

**何时用哪个**：CK 题干通常给两个评分名互换列出。同时给 troponin↑、动态 ST 改变 → 两者都中高危 → 24 h 内造影。

---

### qSOFA vs SOFA vs SIRS

| 维度 | SIRS | qSOFA | SOFA |
|:---|:---|:---|:---|
| 用途 | 旧 sepsis 定义筛查 | 床旁现代筛查 | sepsis 现代诊断（器官衰竭） |
| 实验室需要 | 是（WBC） | 否 | 是（PaO2/FiO2、Plt、Bili、Cr） |
| 项目数 | 4（T、HR、RR、WBC） | 3（RR、神志、SBP） | 6 系统 |
| 阈值 | ≥ 2 项 | ≥ 2 分 | ≥ 2 分增加 |
| 当前地位 | 历史，CK 仍考 | 床旁筛查 | 诊断核心（Sepsis-3） |

**何时用哪个**：CK 现代答 qSOFA 床旁/SOFA 诊断；遇到经典老题用 SIRS + 感染源 = sepsis。

---

### MELD vs Child-Pugh

| 维度 | MELD（-Na） | Child-Pugh |
|:---|:---|:---|
| 用途 | 移植排序、短期死亡率 | 长期生存 + 手术风险 |
| 变量 | Bilirubin + INR + Cr (+Na) | Bili + Albumin + INR + 腹水 + 脑病 |
| 是否含主观 | 全客观 | 含主观（腹水/脑病分级） |
| 计算 | 复杂对数 | 简单 5 项加分 |
| 阈值 | ≥ 15 移植上线 | A/B/C 三级 |

**何时用哪个**：移植决策 → MELD；腹水/曲张/手术耐受 → Child-Pugh。CK 题干给 albumin + 腹水 + 脑病 → Child-Pugh；给 Cr + INR + Bili 三件套 → MELD。

---

### PHQ-9 vs GAD-7

| 维度 | PHQ-9 | GAD-7 |
|:---|:---|:---|
| 病种 | 抑郁 | 广泛性焦虑 |
| 项目 | 9 | 7 |
| 总分 | 0–27 | 0–21 |
| 治疗阈值 | ≥ 10 | ≥ 10 |
| 含自杀题 | 是（9 题） | 否 |

**何时用哪个**：情绪低落兴趣丧失 → PHQ；过度担忧紧张 → GAD-7。两个都阳性常见，按主诉先治。

---

### MMSE vs MoCA

| 维度         | MMSE     | MoCA    |
| :--------- | :------- | :------ |
| 总分         | 30       | 30      |
| 时长         | 5–10 min | 10 min  |
| 对早期 MCI 敏感 | 较低       | 较高      |
| 受教育影响      | 较大       | 加 1 分校正 |
| 异常阈值       | < 24     | < 26    |

**何时用哪个**：怀疑早期 MCI 或受教育程度高的患者 → MoCA；社区快速筛查 → MMSE。

---

### CIWA-Ar vs DT 诊断

| 维度 | CIWA-Ar | 谵妄震颤（DT） |
|:---|:---|:---|
| 性质 | 戒断量化量表 | 临床综合征 |
| 触发治疗 | ≥ 10 → BZD | 已发生 → ICU + IV BZD |
| 时间窗 | 戒酒 6–48 h | 48–96 h |
| 死亡率 | — | ~5% |

**何时用哪个**：评估 → CIWA-Ar；诊断危急状态 → DT 临床定义（自主神经亢进 + 幻觉 + 定向障碍）。

---

### AUDIT-C vs CAGE

| 维度 | AUDIT-C | CAGE |
|:---|:---|:---|
| 项目 | 3（频率/量/暴饮） | 4（C/A/G/E） |
| 评分 | 0–12 连续 | 4 个 yes/no |
| 阈值 | 男 ≥ 4 / 女 ≥ 3 | ≥ 2 |
| 优势 | 量化使用模式 | 抓"问题饮酒"心理学线索 |
| 当前推荐 | USPSTF 首选 | 历史经典 |

**何时用哪个**：现代成人筛查 → AUDIT-C；CK 经典 vignette + 否认问题但 CAGE 阳性 → 仍干预。

---

### 糖尿病：DKA vs HHS

| 维度 | DKA | HHS |
|:---|:---|:---|
| 人群 | T1DM 多 | 老年 T2DM |
| Glucose | > 250 | > 600 |
| pH | < 7.30 | > 7.30 |
| HCO3 | < 18 | > 18 |
| Ketones | 阳性 | 阴/微 |
| Anion gap | 大 | 正常 |
| Osm | 中等升高 | > 320 |
| 神志 | 警觉到轻度改变 | 显著改变到昏迷 |
| 治疗顺序 | IVF → K → insulin（K < 3.3 暂停 insulin） | IVF（更激进）→ K → insulin |
| 死亡率 | 2–5% | 10–20% |

**何时用哪个**：青年急性 + 酮 + 大 AG → DKA；老年慢病 + 神志差 + 极高糖 + 无酮 → HHS。

---

### Apgar 1 min vs 5 min

| 维度 | 1 min Apgar | 5 min Apgar |
|:---|:---|:---|
| 反映什么 | 出生时即时状态 | 复苏效果 + 预后 |
| 决定复苏 | 否（NRP 看呼吸/HR/张力） | 否 |
| 预后相关性 | 弱 | 强（< 7 → 持续每 5 min 评估） |

**何时用哪个**：CK 强调"5 min Apgar 决定预后跟进，1 min 是历史快照"。

---

### CURB-65 vs PSI

| 维度 | CURB-65 | PSI |
|:---|:---|:---|
| 变量数 | 5 | 20+ |
| 床旁可算 | 是 | 否（需在线） |
| 准确度 | 低 | 高 |
| 临床偏好 | 急诊/床旁 | 复杂病例/研究 |

**何时用哪个**：CK 默认 CURB-65；问"哪个更精确"答 PSI。

---

### Wells（DVT/PE）vs PERC

| 维度 | Wells | PERC |
|:---|:---|:---|
| 用途 | 概率分层 | 排除（rule-out） |
| 何时用 | 中-高概率患者 | 仅低概率患者 |
| 阴性意义 | 仍需检查 | 全 8 阴性 + 低概率 → 直接排除 |

**何时用哪个**：先用 Wells；低概率 + PERC 全阴性 → 不必测 D-dimer。

---

> **复习提示**：USMLE Step 2 CK vignette 80% 不直接给评分名，要从临床描述识别"该用哪个评分"。先把"触发场景 → 评分"对应关系背熟，分值表和阈值再补。
