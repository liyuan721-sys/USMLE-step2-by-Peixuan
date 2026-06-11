---
tags:
  - USMLE-Step2
  - 心血管
created: 2026-06-11
type: 专题笔记
---

# QT 间期长短与 TdP（QT interval — long / short & Torsades）

> [!info] 用途
> QT 的**双向**地图：正常值 → 怎么测（Bazett / 目测）→ **延长**（药物 / 电解质 / 先天 LQTS / TdP 处置）→ **缩短**（高钙 / 高钾 / digoxin / 先天 SQTS）。
> 电解质→ECG 全景图见 [[完整笔记/专题笔记/心内/心内_代谢性ECG改变]]；本笔记是 QT 这一条的纵深版。

---

## §零 正常值速查 ⭐

> [!info] 地基：QRS 看钠、QT 看钾钙（动作电位映射）⭐
> 一切规律的总根 —— ECG 段对应哪个离子：
>
> | ECG 段 | 动作电位 | 主导离子 | 意义 |
> |---|---|---|---|
> | **QRS** | phase 0 | **Na⁺ 内流** | 心室去极化（传导速度）|
> | **QT** | phase 0 → 3 全程 | **K⁺ 为主 + Ca²⁺（平台）** | 去极化 + 复极总时长 |
>
> **一句话**：QRS 宽窄 = Na⁺ 通道功能（堵钠 → QRS 宽）；QT 长短 = 复极 K⁺ + 平台 Ca²⁺。
> **高钾很特殊，两头都碰**：IKr↑ → short QT（复极端）；重度抑制传导 → 宽 QRS → 故它在本卡(QT)和 [[完整笔记/专题笔记/心内/心内_宽QRS鉴别与解毒]] 都出现。

> [!info]- 动作电位 5 相图（想看离子细节再展开）
> ```
> 电位
>  +20 │      ___________
>      │    1/        2  \        ← phase 2 平台：Ca²⁺ 内流 ⇄ K⁺ 外流
>    0 │   0│              \3
>      │   /│               \
>  -90 │__/ │________________\___4__ ← phase 4 静息
>      └────┼────────────────┼─────
>         phase 0          phase 3
>         Na⁺ 内流         K⁺ 外流
>
> phase 0 = Na⁺ 内流（快钠通道）→ 去极化 → QRS
> phase 1 = 短暂 K⁺ 外流（Ito）
> phase 2 = Ca²⁺ 内流 ⇄ K⁺ 外流（平台）→ QT 平台端
> phase 3 = K⁺ 外流（IKr/IKs）→ 复极 → QT 复极端
> phase 4 = 静息（Na/K-ATP 酶）
> ```
>
> | 现象 | 离子机制 | 落在 |
> |---|---|---|
> | TCA / 高钾 → 宽 QRS | Na⁺ 通道抑制 → phase 0 慢 | QRS |
> | 低钾 / 低镁 / 药物 → 长 QT | K⁺ 外流↓ → phase 3 慢 | QT 复极端 |
> | 低钙 → 长 QT | Ca²⁺ → phase 2 平台延长 | QT 平台端 |
> | 高钙 → 短 QT | Ca²⁺ → phase 2 平台缩短 | QT 平台端 |
> | 高钾 → 短 QT | K⁺↑ → IKr↑ → phase 3 加快 | QT 复极端 |

### 0.1 QTc（校正后 QT — 临床实际用这个）

| 分类 | 男 Male | 女 Female |
|---|---|---|
| **正常 Normal** | ≤440 ms | ≤450 ms |
| **临界 Borderline** | 440–460 ms | 450–470 ms |
| **延长 Prolonged** | >450 ms | >460–470 ms |

> [!tip] 考试只需锁 2 个数
> - **QTc >500 ms = 高危**，显著增加 **TdP（尖端扭转型室速）**风险 ← 最常考阈值
> - **QTc <340 ms = 异常短** → 想高钙 / 高钾 / digoxin / 先天 SQTS

### 0.2 怎么测

```
Bazett 公式：QTc = QT / √(RR)        （RR 单位 = 秒）
  心率快 → QT 自然缩短；心率慢 → QT 自然延长 → 必须校正

目测法则：正常 QT 应 < 一半 RR 间期（心率正常时）
```

---

## §一 QT 延长（Long QT）

### 1.1 三大类病因

| 类别 | 具体 | 钥匙 |
|---|---|---|
| **电解质"三低"** | **低钾 / 低镁 / 低钙** | 利尿剂、呕吐腹泻、CKD、胰腺炎、TLS |
| **药物** | 见 1.2 清单 | ICU / 多药老人 |
| **先天 LQTS** | LQT1/2/3（见 1.3）| 年轻人晕厥 / 猝死家族史 |
| **其他** | ICH/SAH 神经源性、低温、心动过缓、甲减 | — |

### 1.2 延长 QT 的高频药物清单 ⭐

```
抗心律失常   : Sotalol, Amiodarone, Quinidine, Procainamide, Dofetilide (IA/III 类)
抗生素       : 大环内酯 Macrolides (azithromycin), 氟喹诺酮 Fluoroquinolones
抗精神病     : Ziprasidone, Haloperidol, Quetiapine
抗抑郁       : TCA (三环类), Citalopram (SSRI 中剂量依赖)
止吐         : Ondansetron (昂丹司琼)
其他         : Methadone (美沙酮), 抗真菌唑类
```

> [!warning] Stem 反射
> **ICU / 老人 + 新发长 QT** → 先扫**药物清单**（azithromycin / 氟喹诺酮 / haloperidol / methadone / ondansetron）+ **查电解质**（K/Mg/Ca）。多药叠加是最常见诱因。

### 1.3 先天性 LQTS 三亚型 + 触发 ⭐

| 亚型 | 通道 | 典型触发 trigger | Memory Hook |
|---|---|---|---|
| **LQT1** | K⁺ (IKs)↓ | 运动，尤其**游泳 swimming** | 游泳 = 1 |
| **LQT2** | K⁺ (IKr)↓ | **情绪 / 突发声响**（闹钟、电话铃）| 声音 = 2 |
| **LQT3** | Na⁺↑ | **睡眠 / 休息中 sleep** | 睡觉 = 3 |

> [!tip] Stem 模式
> "游泳时晕厥/溺水" → LQT1｜"闹钟惊醒后倒下" → LQT2｜"睡眠中猝死家族史" → LQT3

**两个综合征名（考遗传模式）：**

| 综合征 | 遗传 | 特征 |
|---|---|---|
| **Romano-Ward** | 常显 AD | 纯心脏，**听力正常** |
| **Jervell-Lange-Nielsen** | 常隐 AR | 长 QT + **先天性感音性耳聋** sensorineural deafness |

### 1.4 慢性管理

```
首选     : β-blocker (β受体阻滞剂)   ← LQT1/LQT2 最有效
生活      : 避免竞技运动（尤其 LQT1 避游泳）+ 避开延长 QT 药物
高危→ICD : QTc>500 / 反复晕厥 / 心脏骤停史
家系      : 筛查一级亲属（AD 遗传）
```

---

## §二 Torsades de Pointes（TdP）处置 ⭐⭐

```
TdP 发作
  │
  ├─ 不稳定 / 无脉 (unstable / pulseless) → 立即 电除颤 defibrillation
  │
  └─ 稳定 stable
        ├─ ① IV Magnesium sulfate (硫酸镁)  ← 一线，即使血镁正常也给
        ├─ ② 纠正诱因：补 K 至高限、停致病药
        └─ ③ 反复 → Overdrive pacing (超速起搏) 或 Isoproterenol（加快心率→缩短 QT）
```

> [!danger] 单个最高频考点
> **稳定 TdP → IV 硫酸镁 (magnesium)**，不是抗心律失常药！多数抗心律失常药反而延长 QT，会加重。
> 对照陷阱：**低体温 + 长 QT → 复温**（不是镁）见 [[完整笔记/专题笔记/外科/外科_低体温分级与复温]]。

---

## §三 QT 缩短（Short QT）

### 3.1 四大病因 + 机制 ⭐

| 病因 | 机制（缩在哪个 phase）| USMLE 怎么考 |
|---|---|---|
| **高钙 hypercalcemia** | Ca²⁺ 缩短动作电位**平台期 phase 2** | 直接考 "short QT"（最干净）|
| **高钾 hyperkalemia** | 细胞外 K⁺↑ → IKr↑ → **phase 3 复极加快** | 主考"**高尖窄底 T 波**"，short QT 是伴随征 |
| **Digoxin（地高辛）** | 缩短复极 | 考"**盆状 scooped ST 下垂**（digitalis effect）"+ short QT |
| **先天 SQTS** | K⁺ 通道功能获得 gain-of-function | 房颤 + 室颤 + 猝死 |

> [!warning] 关键澄清（我曾把这条简化错）
> "钙管平台期、高钙缩短"**没错**，但 short QT **不只是高钙** —— **高钾也缩短 QT**，只是走另一条通路：
> - **高钙** → 缩短 **phase 2 平台期**
> - **高钾** → 加速 **phase 3 复极**
> 两条路都通向 short QT。别把 short QT 直接等号 = 高钙。

### 3.2 同样 short QT，看伴随征区分

| short QT 伴随 | 指向 | 找什么背景 |
|---|---|---|
| **高尖窄底 T + QRS 增宽** | **高钾** | CKD / 透析漏做 / ACEI / 挤压伤 |
| **stones bones groans + 多尿烦渴** | **高钙** | 恶性肿瘤 / 甲旁亢 |
| **盆状 ST + 恶心 / 黄绿视** | **Digoxin** | 老人 + 利尿剂 + 房颤治疗 |

---

## §四 一张图记牢"钙钾与 QT/T"

```
            QT 延长 (long)              QT 缩短 (short)
钙 Ca   :   低钙 ──────────────►        高钙 ──────────► (phase 2 平台期)
钾 K    :   低钾 → T平+U波            高钾 → T高尖 (phase 3 复极)
镁 Mg   :   低镁 ──► TdP               —
           （三低 = 低K/低Mg/低Ca → TdP）
```

> [!success] Memory Hook
> **"高短低长"看钙**（高钙短 QT / 低钙长 QT）；**钾走两头**（低钾 T 平 + U 波 / 高钾 T 高尖 + short QT）；**长 QT 三低记 K-Mg-Ca，治 TdP 认硫酸镁。**

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes_2026-06#^Q11417]] 低体温 + 长 QT → 复温（≠镁，TdP 才用镁）
  - [[mistakes/uworld-mistakes_2026-05#^Q19929]] 高钾 ECG（short QT / T 高尖同源）
  - [[mistakes/uworld-mistakes_2026-05#^Q4454]] Digoxin 效应（scooped ST + short QT）
  - （等积累 TdP / LQTS / 低钙长 QT 各 1-2 道补锚点）
- 📚 主笔记：
  - [[完整笔记/Peixuan分科笔记/心内]]（心律失常 / ECG）
  - [[完整笔记/Peixuan分科笔记/肾脏]]（电解质 → QT）
- 🏥 跨学科：
  - [[完整笔记/专题笔记/心内/心内_代谢性ECG改变]]（电解质/中毒 ECG 全景，QT 是其中一行）
  - [[完整笔记/专题笔记/心内/心内_Vaughan_Williams抗心律失常药]](IA/III 类延长 QT)
  - [[完整笔记/专题笔记/心内/心内_晕厥鉴别决策树]](LQTS 致晕厥/猝死)
  - [[完整笔记/专题笔记/外科/外科_低体温分级与复温]](低温长 QT → 复温的对照陷阱)
  - [[完整笔记/专题笔记/肾脏/肾脏_电解质急症速查]](K/Ca/Mg 细节)
- 🌱 TODO：
  - 等收齐 **低钙长 QT（甲旁减/CKD/胰腺炎）** 错题 → §一 1.1 补题号锚点
  - 等收齐 **先天 LQTS / 游泳晕厥** 错题 → §1.3 补锚点

## ✅ 复盘行动

- [ ] 默写 QTc 正常值（男 ≤440 / 女 ≤450；>500 高危）
- [ ] 默写延长 QT 药物清单（抗心律失常 IA/III + 大环内酯/氟喹诺酮 + haloperidol + methadone + ondansetron）
- [ ] 默写 LQT1/2/3 触发（游泳 / 声音 / 睡眠）+ Romano-Ward vs Jervell-Lange-Nielsen
- [ ] 默写稳定 TdP → IV 硫酸镁（低温长 QT → 复温的对照）
- [ ] 默写 short QT 四病因 + 高钙(phase2) vs 高钾(phase3) 机制差异
- [ ] 默写"高短低长看钙、钾走两头"

---

## 版本记录

- **v1**（2026-06-11）：兑现 [[完整笔记/专题笔记/心内/心内_代谢性ECG改变]] 第 245 行 TODO。QT 双向纵深：正常值 + Bazett/目测 + 长 QT（药物清单/三低/LQTS 1-3/Romano-Ward/JLN/TdP 处置）+ 短 QT（高钙 phase2 / 高钾 phase3 / digoxin / SQTS）+ 钙钾对账图。起因：用户指出"short QT 不止高钙、高钾也缩短"的一致性漏洞。
- **v1.1**（2026-06-11）：§零开头加"地基块" —— 动作电位 5 相 → QRS(Na)/QT(K·Ca) 总映射表 + 5 相 ASCII 图（折叠）+ 现象反推表，作为本卡与宽 QRS 卡的共同地基。
