---
tags:
  - USMLE-Step2
  - 肺
created: 2026-06-12
type: 专题笔记
---

# 机械通气：操作流程与调参 (Mechanical Ventilation — Workflow & Adjustment)

> [!info] 全流程速览（按临床实际发生顺序）
> 本篇按**真实床旁顺序**排成 5 步操作主干；每步的"为什么"都收进可折叠 `原理` callout，想深究再点开。
> **第0步 上机决策**（无创 vs 插管）→ **第1步 初始设置**（四个旋钮）→ **第2步 评估**（测压力 + 查 ABG）→ **第3步 判读异常 → 调哪个钮** → **第4步 特殊情景的调参约束**（ARDS / COPD / 低血压 / 撤 PEEP）。
> **两条贯穿全程的主线**：**CO₂ 走通气（VT × RR）；O₂ 走 FiO₂ + PEEP** —— 两条独立通路,调参不串台。

> [!note]- 本篇缩写速查（首次全称中英）
> - **PEEP** = positive end-expiratory pressure 呼气末正压
> - **auto-PEEP** = intrinsic / occult PEEP 内源性（隐匿）呼气末正压
> - **PIP / Peak** = peak inspiratory pressure 吸气峰压
> - **Plateau** = plateau pressure 平台压
> - **ET tube** = endotracheal tube 气管插管
> - **VT** = tidal volume 潮气量
> - **Crs** = respiratory system compliance 呼吸系统顺应性
> - **ΔP** = driving pressure 驱动压（= Plateau − PEEP）
> - **RR** = respiratory rate 呼吸频率
> - **IBW** = ideal body weight 理想体重
> - **ARDS** = acute respiratory distress syndrome 急性呼吸窘迫综合征
> - **ACS** = abdominal compartment syndrome 腹腔间隔室综合征
> - **COPD** = chronic obstructive pulmonary disease 慢性阻塞性肺疾病
> - **AECOPD** = acute exacerbation of COPD COPD 急性加重
> - **FiO₂** = fraction of inspired oxygen 吸入氧浓度
> - **ABG** = arterial blood gas 动脉血气
> - **PPV** = positive pressure ventilation 正压通气
> - **NIPPV** = noninvasive positive pressure ventilation 无创正压通气
> - **CPAP** = continuous positive airway pressure 持续气道正压
> - **BiPAP** = bilevel positive airway pressure 双水平气道正压
> - **WOB** = work of breathing 呼吸功
> - **AMS** = altered mental status 意识状态改变
> - **OHS** = obesity hypoventilation syndrome 肥胖低通气综合征
> - **OSA** = obstructive sleep apnea 阻塞性睡眠呼吸暂停
> - **I:E** = inspiratory-to-expiratory ratio 吸呼比
> - **V/Q** = ventilation/perfusion ratio 通气/血流比

> [!abstract]- 目录（点击跳转）
> 0. [[#第0步：上机决策 —— 无创通气 vs 插管|第0步 上机决策（无创 vs 插管）]]
> 1. [[#第1步：初始设置 —— 四个旋钮|第1步 初始设置（四个旋钮）]]
> 2. [[#第2步：评估 —— 测压力 + 查 ABG|第2步 评估（测压力 + 查 ABG）]]
> 3. [[#第3步：判读异常 → 调哪个钮 ⭐|第3步 判读异常 → 调哪个钮 ⭐]]
> 4. [[#第4步：特殊情景的调参约束 ⭐|第4步 特殊情景的调参约束 ⭐]]
> 5. [[#速记 Memory Hook|速记 Memory Hook]]

---

## 第0步：上机决策 —— 无创通气 vs 插管

> [!tip] 操作顺序：先评估能不能用无创，再判断是否必须插管
> 1. **够轻、神志清、能配合、无禁忌** → 先试 **NIPPV（无创）**：
>    - **BiPAP**：AECOPD（pH <7.35 且 PaCO₂ >45）、重症哮喘早期短试、OHS、部分心源性肺水肿 —— **既吹 CO₂ 又改善氧合**
>    - **CPAP**：OSA、部分心源性肺水肿 —— 撑开上气道/复张肺泡改善氧合，**不主动吹 CO₂**
> 2. **出现下列任一 → 跳过/中止无创，直接气管插管**：

| 插管指征 | 关键表现 |
|---|---|
| **呼吸衰竭逼近 (impending respiratory failure)** | 哮喘/COPD 的 **PaCO₂「本应低却正常或升高」+ pH↓** |
| **意识状态改变 (AMS)** | 脑灌注差 / CO₂ 麻醉 / 低氧 |
| **沉默肺 (silent chest)** | 气流太弱听不到喘鸣，比满肺哮鸣更危险 |
| **血流动力学不稳 / 极高呼吸功 (WOB)** | 大量动用辅助呼吸肌 |
| **NIPPV 短试无效** | <2 小时无改善或恶化 |

> [!danger]- 原理：为什么"PaCO₂ 本应低却正常/升高"= 危险信号
> 急性哮喘患者过度通气 → PaCO₂ **应该低**。若 PaCO₂ **正常或升高** = 呼吸肌疲劳、通气即将失败 = 呼吸衰竭逼近 → **插管**，而不是继续加雾化。
>
> | 情况 | PaCO₂ | pH | 意义 |
> |---|---|---|---|
> | 一般急性哮喘 | ↓ | ↑/正常 | 过度通气，还撑得住 |
> | **呼吸衰竭逼近** | **正常/↑** | ↓ | **喘不动了 → 插管** |

> [!info]- 原理：BiPAP「吹 CO₂」，CPAP「不吹」
> BiPAP 有**吸气压 + 呼气压两个水平**，吸气助力 → 增加潮气量 → **主动降 CO₂**；CPAP 是**单一持续正压**，只撑开气道/复张肺泡改善氧合，不增加潮气量 → 不吹 CO₂。
> **反射**：有高碳酸（需降 CO₂）→ 选 BiPAP，不选 CPAP。
> **禁忌反射**：哮喘 + AMS + silent chest + PaCO₂ 正常/↑ → 别试 NIPPV，直接插管。

---

## 第1步：初始设置 —— 四个旋钮

> [!tip] 操作：插管后设定起始参数
> 1. **潮气量 VT**：起始 **6–8 mL/kg 理想体重 (IBW)**（ARDS 直接 6，见第4步）
> 2. **呼吸频率 RR**：起始 ~12–16/min，按 CO₂ 目标调
> 3. **FiO₂**：起始可 100%，按血氧尽快下调（避免氧中毒）
> 4. **PEEP**：起始 ~5 cmH₂O，按氧合需求上调

> [!info]- 原理：两条独立通路（贯穿全篇的总纲）
> - **CO₂ ∝ 分钟通气量 = VT × RR** → 想动 CO₂ 就调 **VT 或 RR**
> - **O₂ ← FiO₂ + PEEP**（PEEP 复张肺泡、改善 V/Q 匹配）→ 想动氧合就调 **FiO₂ 和/或 PEEP**
> 两条通路**互不串台**，是后面所有调参决策的根。

> [!info]- 氧合滴定模板：FiO₂ 怎么撤 / PEEP 怎么加（ARDSnet）
> **① 目标氧合（够用就好，不追高）**
>
> | 人群 | SpO₂ | PaO₂ |
> |---|---|---|
> | 一般机械通气 | 92–96% | ~60–80 mmHg |
> | **ARDS（ARDSnet）** | **88–95%** | **55–80 mmHg** |
> | COPD / 慢性 CO₂ 潴留 | 88–92% | ~60 mmHg |
>
> **② 撤 FiO₂ 标准**：氧合一达标就撤，尽快降到 **≤0.6（60%）**。
> > FiO₂ >0.6 持续 >24–48h → **氧中毒**：活性氧 (reactive oxygen species, ROS)↑ → 肺损伤 + 吸收性肺不张 (absorption atelectasis)。
>
> **③ 加 PEEP 需求**：高 FiO₂（>0.6）仍压不住的**难治性低氧 (refractory hypoxemia)** / 肺泡塌陷（ARDS）→ PEEP 复张肺泡、增 FRC、改善 V/Q，**替 FiO₂ 分担**好把 FiO₂ 撤回 ≤0.6。
>
> **④ 配对阶梯表（lower-PEEP / higher-FiO₂，最常考）** —— FiO₂ 与 PEEP 成对联动，不单飞：
>
> | FiO₂ | 0.3 | 0.4 | 0.4 | 0.5 | 0.5 | 0.6 | 0.7 | 0.7 | 0.7 | 0.8 | 0.9 | 0.9 | 0.9 | 1.0 |
> |---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
> | **PEEP** | 5 | 5 | 8 | 8 | 10 | 10 | 10 | 12 | 14 | 14 | 14 | 16 | 18 | 18–24 |
>
> 氧合**不够 → 向右**走（俩一起↑）；**够了/超标 → 向左**撤（优先撤 FiO₂，PEEP 留着）。
>
> **⑤ 上限红线**：平台压 <30（防过度膨胀/气压伤/死腔↑）+ 不掉血压（PEEP↑→胸内压↑→静脉回流↓）。
>
> **⑥ 铁律**：**复张后别先撤 PEEP**（去复张 → 低氧反弹）；撤的顺序是先 FiO₂、后 PEEP。

> [!warning] 插管后第一件事：确认 ETT 深度（防右主支气管插管）⭐（Q4632）
> **ETT 尖端理想位置 = 隆突 (carina) 上 2-5 cm**。右主支气管与气管夹角小/更垂直 → **ETT 过深优先进右主支气管 (right mainstem intubation)** → 右肺过度通气 + 左肺不通气 → **左侧呼吸音明显减低 + 不对称胸廓起伏 + V/Q 失配低氧**。
> - **识别**：插管后**单侧（尤其左）呼吸音减低 + 无低血压**（无低血压区别于张力性气胸）。
> - **处理 = 后退导管 (pull back ETT)** 至隆突与声带之间 + 胸片确认。
> - ⚠️ **别反射放胸管**（[[mistakes/uworld-mistakes_2026-06#^Q4632]]）；**增加潮气量**会加重右肺过度通气 → 禁忌。
> - 机制（V/Q 失配）详见 [[完整笔记/专题笔记/pulmonary/pulmonary_低氧血症五机制]]。

---

## 第2步：评估 —— 测压力 + 查 ABG

> [!tip] 操作顺序：上机后这样读机器
> 1. **读峰压 (Peak/PIP)** —— 送气末、有气流时机器直接显示
> 2. **做吸气暂停 (inspiratory hold)** → 读 **平台压 (Plateau)**（无气流）
> 3. **做呼气暂停 (expiratory hold)** → 读 **Total PEEP** → 算 **auto-PEEP**
> 4. **抽 ABG** → 看 PaCO₂（通气够不够）+ PaO₂（氧合够不够）

| 压力 | 何时测 | 反映什么 | 正常值 |
|---|---|---|---|
| **峰压 Peak (PIP)** | 送气末、**有气流** | 阻力压 + 弹性压（总和） | — |
| **平台压 Plateau** | **吸气暂停**、无气流 | 弹性压 = 顺应性 Crs | ≤30 cmH₂O |
| **Total PEEP** | **呼气暂停**、呼气末 | 呼气末肺内残余压 | = 设定值（多出来 = auto-PEEP） |

> [!danger] 最高频陷阱：吸气暂停 vs 呼气暂停（测的是两件事）
> - **吸气暂停 → 平台压 → 顺应性**
> - **呼气暂停 → Total PEEP → 算 auto-PEEP**
> ❌ 别一看到「暂停后测压」就反射 PEEP —— 先看是**吸气**还是**呼气**暂停。

> [!info]- 原理：气道压 = 阻力压 + 弹性压（为什么暂停能拆开）
> 正压送气，机器端测到的压由两部分构成：
> - **阻力压 (resistive pressure)**：气体克服气道摩擦所需，**只在有气流时存在**（气流停 → 阻力压 = 0）
> - **弹性压 (elastic pressure)**：撑开肺与胸壁所需，反映顺应性；气流停了它依然在
>
> ```
> 送气中（有气流）         吸气暂停（无气流）
> ┌─────────────┐         ┌─────────────┐
> │  阻力压      │  气流停  │  阻力压 = 0  │
> │  ＋          │ ───────→ │             │
> │  弹性压      │          │  弹性压      │ ← 平台压 = 这个
> └─────────────┘         └─────────────┘
>    = 峰压 Peak              = 平台压 Plateau
> ```
> **关键**：消除气流 → 剩下的就是纯弹性压 = 平台压。

> [!info]- 原理：auto-PEEP 为什么"非呼气暂停不可"+ 公式
> 压力传感器装在**气道开口**，不是肺泡。呼气还在进行时（气流≠0），气道口与肺泡间隔着**气道阻力压差**，传感器被它掩盖 → 只读到设定 PEEP，看不到肺泡里困住的 auto-PEEP。
> **呼气暂停让气流 = 0 → 阻力压差消失 → 气道口压 = 肺泡压**，才读得到真实呼气末压。与吸气暂停同一个物理：no-flow 才能让气道口压 = 肺泡压。
> **公式：auto-PEEP = Total PEEP（呼气暂停测得）− Set PEEP（设定）**；Total = Set + auto。

> [!example]- 压力-时间波形图（正常 / 顺应性↓ / 阻力↑）
> > ![[{D0C0396C-363B-4477-89B8-C7B0EB32D002}.png]]
> - **上**：正常吸气暂停 —— 送气出现峰，暂停后回落到平台（Hold 实线），无暂停则直接衰减（No hold 虚线）。
> - **左下**：峰、平台**同步升高** → 顺应性↓（肺硬）。
> - **右下**：峰升高、平台**正常** → 阻力↑（管窄）。

---

## 第3步：判读异常 → 调哪个钮 ⭐

> [!tip] 操作：拿到压力 + ABG，按这张决策树调
> **A. 压力异常（峰压高）→ 找原因**
> ```
> 峰压 Peak 升高
>       │
>       ├── 平台压也升高 ──→ 顺应性↓（肺硬）
>       │   （差值正常）      肺水肿 / 气胸 / ARDS / ACS / 插管过深
>       │
>       └── 平台压正常 ────→ 阻力↑（管窄）
>         （Peak−Plateau↑）  支气管痉挛 / 黏液栓 / 咬管 / 管路扭折
> ```
> **B. ABG 异常 → 调对应旋钮**

| ABG 异常 | 病理 | 调哪个钮 |
|---|---|---|
| **PaCO₂ ↑**（呼酸） | 通气不足 | ↑ RR 或 ↑ VT（↑分钟通气） |
| **PaCO₂ ↓**（呼碱） | 通气过度 | ↓ RR 或 ↓ VT |
| **PaO₂ ↓**（低氧） | 氧合差 | ↑ FiO₂ 和/或 ↑ PEEP |

> [!info]- 原理：「平台看顺应性，峰−平差值看阻力」
> - **平台压 = 弹性压 → 顺应性**：平台↑ = 顺应性↓ = 肺硬
> - **Peak − Plateau 差值 → 气道阻力**：差值↑ = 管窄（差值来自只在有气流时存在的阻力压）

> [!question]- 自测：插管镇静患者做吸气暂停 2 秒，无气流时口端压力升高 —— 反映什么？
> **呼吸系统顺应性**。无气流 → 阻力压 = 0 → 测得 = 平台压 = 弹性压 = 顺应性；压力升高 = 顺应性↓（肺硬）。
> 干扰项：❌ PEEP（要用呼气暂停）；❌ 总气道阻力（是 Peak−Plateau 差值）；❌ 上气道阻力（插管已绕过 = 0）；❌ 呼气肌力（需清醒配合）。

---

## 第4步：特殊情景的调参约束 ⭐

> [!warning] 情景 A：ARDS → 肺保护性通气（唯一明确降死亡率）
> **操作**：
> 1. **VT 降到 6 mL/kg IBW** + **平台压 <30 cmH₂O**
> 2. 降 VT 后 CO₂ 必升 → **允许性高碳酸血症 (permissive hypercapnia)**：pH >7.15–7.20 就**接受**
> 3. pH 掉太低（<7.15）→ **升 RR 补分钟通气**（VT 为保肺不能加回，用 RR 补；⚠️ RR 太高撞 auto-PEEP）
> 4. 氧合另走 **PEEP + FiO₂**；**复张后别降 PEEP**
> 详见 [[完整笔记/专题笔记/pulmonary/pulmonary_ARDS]]。

> [!info]- 原理：平台压"不就是顺应性"吗？怎么去「限」它？
> **平台压 ≠ 顺应性**——平台压是压力读数，顺应性是斜率 Crs = ΔV/ΔP。靠公式连起来：
> **平台压 = PEEP + (VT / Crs)**，**驱动压 ΔP = Plateau − PEEP = VT / Crs**
> - **判读视角（第3步）**：VT 固定时，平台压唯一变量是 Crs → "平台↑=顺应性↓"成立（前提 VT 不变）。
> - **治疗视角（本步）**：ARDS 低顺应性是疾病决定、改不了；但 **VT 你能动** → 降 VT 把平台压读数压到 <30。限的是**压力读数 + 肺泡牵张**，不是固有顺应性。
> - **baby lung（婴儿肺）**：ARDS 可通气肺组织只剩一小块，正常 VT 会让这块独自吞下全部容量 → 过度牵张 (overdistension) → 容积伤 (volutrauma) / 气压伤 (barotrauma)。限平台 = 限肺泡最大牵张压。
> - **进阶**：驱动压 ΔP（=Plateau−PEEP）>15 与 ARDS 死亡率最相关，比单看平台或单看 VT 更准。

> [!question]- 自测：ARDS 患者 VT 8 mL/kg、PEEP 10、平台压 34，下一步怎么调（既保肺又不恶化氧合）？
> **降 VT 到 6 mL/kg IBW** 把平台压压到 <30（Crs 改不了就动 VT）。连带 **CO₂↑ → permissive hypercapnia，pH>7.15 接受；太低则加 RR**。**氧合不变**——走 PEEP/FiO₂ 独立通路，别因 CO₂ 去撤 PEEP。

> [!warning] 情景 B：COPD / 哮喘 → 防 auto-PEEP（气体陷闭）
> **操作**：呼气阻力高 + 呼气时间不足 → 气体陷闭 → auto-PEEP。处理：
> 1. **↓ RR、↓ VT**
> 2. **延长呼气时间（I:E 比拉长）**
> 3. 积极治支气管痉挛 (bronchospasm)

> [!warning] 情景 C：机械通气患者突发低血压 → 床旁两步鉴别
> **操作**：先想两件事 → **① 张力性气胸 (tension pneumothorax)**；**② auto-PEEP**。
> **断开呼吸机让肺被动完全排空**：血压随之回升 = **auto-PEEP 证实**（同时也排掉气体陷闭）；不回升 → 查张力性气胸（穿刺减压）。

> [!info]- 原理：正压通气 (PPV) 的血流动力学 —— 双刃
> PPV 对心脏是「卸负荷」：右室 (RV) 前负荷↓ + 左室 (LV) 前负荷↓ + 左室后负荷↓ → 利于左室充盈与射血。
> - **利**：**急性心源性肺水肿** → CPAP/BiPAP 快速缓解肺淤血。
> - **弊**：**低血容量 (hypovolemia)** 或 **auto-PEEP** 时，胸内压↑ → 静脉回流↓ → **低血压**（与情景 C 同源）。

> [!danger]- 原理：为什么"复张后别降 PEEP"
> ARDS 氧合一好转就撤 PEEP → 已复张的肺泡再次塌陷（去复张）→ 低氧反弹。**氧合好 ≠ 可撤 PEEP**。

---

## 速记 Memory Hook

> [!success] 锁定记忆（按操作流程）
> **总纲**：CO₂ 走通气（VT×RR）；O₂ 走 FiO₂+PEEP —— 两条独立通路。
> **测压力**：**吸气**暂停 → 平台压 = 顺应性（平台高 = 肺硬：水肿/气胸/ARDS/ACS）；**呼气**暂停 → auto-PEEP；**Peak−Plateau = 阻力**（差值大 = 管窄：痉挛/黏液栓/咬管）。
> **特殊情景**：
> - ARDS = 低 VT 6 mL/kg + 平台<30 + permissive hypercapnia（pH>7.15）+ 复张后别降 PEEP。
> - COPD/哮喘 = 防 auto-PEEP（降 RR、拉长呼气）。
> - 突发低血压 → 张力性气胸 or auto-PEEP（断机排气血压回升 = auto-PEEP）。
> - BiPAP 吹 CO₂，CPAP 不吹；有高碳酸选 BiPAP。
> - 哮喘 PaCO₂「本应低却正常/↑」= 呼吸衰竭逼近 → 插管（+AMS/silent chest）。

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes_2026-06#^Q4713]] 吸气暂停=平台压=顺应性（误选 PEEP）
  - [[mistakes/uworld-mistakes_2026-06#^Q4931]] 术后肺不张 ABG（通气生理）
  - [[mistakes/uworld-mistakes_2026-06#^Q4932]] 术后肺不张预防
  - [[mistakes/uworld-mistakes_2026-06#^Q4562]] ARDS 改善氧合 → 加 PEEP（氧合=PEEP+FiO₂；CO₂ 正常不动 RR/VT）
  - [[mistakes/uworld-mistakes_2026-06#^Q4632]] 右主支气管插管（插管后左侧呼吸音减低 → 后退导管，非胸管）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/pulmonary]]（Plateau 看顺应性 / Peak−Plateau 看阻力 段）
- 📚 相关专题：
  - [[完整笔记/专题笔记/pulmonary/pulmonary_HighYield速查总览]]（§气道压力判读 tip + 呼吸机旋钮）
  - [[完整笔记/专题笔记/pulmonary/pulmonary_ARDS]]（肺保护通气：低 VT + 平台压 <30）
  - [[完整笔记/专题笔记/pulmonary/pulmonary_气胸Pneumothorax]]（张力性气胸 → 平台压骤升）
- 🏥 跨学科：[[完整笔记/Peixuan分科笔记/外科]]（围术期/ICU 通气、ACS）
