---
tags:
  - USMLE-Step2
  - 肺
created: 2026-06-12
type: 专题笔记
---

# 机械通气判读与调参 (Ventilator Interpretation & Adjustment)

> [!info] 一句话总览
> 本篇两条主线：**①压力波形判读（§一–四）** + **②旋钮/ABG 调参与模式决策（§五–十）**。
> **压力主线**：气道压 = **阻力压 (resistive pressure)** + **弹性压 (elastic pressure)**；用**吸气暂停 (inspiratory hold)** 拆开 → 测**平台压 (plateau pressure)** → 比 **Peak vs Plateau** 判断「肺硬了（顺应性↓）」还是「管子窄了（阻力↑）」。
> **三个压力反射**：
> **① 吸气暂停（无气流）测的压 = 平台压 = 弹性压 = 反映顺应性**；
> **② Peak − Plateau 差值 = 气道阻力**；
> **③ 呼气暂停 (expiratory hold) 才测 PEEP / auto-PEEP —— 别一见"暂停测压"就反射 PEEP。**
> **调参主线**：**CO₂ 走通气（VT × RR）**，**O₂ 走 FiO₂ + PEEP**——两条独立通路。

> [!note]- 本篇缩写速查（首次全称中英）
> - **PEEP** = positive end-expiratory pressure 呼气末正压
> - **auto-PEEP** = intrinsic / occult PEEP 内源性（隐匿）呼气末正压
> - **PIP** = peak inspiratory pressure 吸气峰压
> - **ET tube** = endotracheal tube 气管插管
> - **VT** = tidal volume 潮气量
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
> - **I:E** = inspiratory-to-expiratory ratio 吸呼比
> - **V/Q** = ventilation/perfusion ratio 通气/血流比

> [!abstract]- 目录（点击跳转）
> **A. 压力波形判读**
> 1. [[#一、核心概念：气道压的两个成分|一、核心概念：阻力压 + 弹性压]]
> 2. [[#二、三种压力：各测什么、怎么测|二、三种压力（Peak / Plateau / PEEP）]]
> 3. [[#三、波形图（吸气暂停三联）|三、波形图（吸气暂停三联）]]
> 4. [[#四、判读决策：Peak vs Plateau ⭐|四、判读决策：Peak vs Plateau ⭐]]
>
> **B. 旋钮 / 调参 / 模式决策**
> 5. [[#五、呼吸机旋钮与 ABG 调参（给一份 ABG，调哪个钮）⭐|五、旋钮与 ABG 调参 ⭐]]
> 6. [[#六、auto-PEEP / 气体陷闭（用呼气暂停测）|六、auto-PEEP / 气体陷闭]]
> 7. [[#七、肺保护性通气（ARDS）|七、肺保护性通气（ARDS）]]
> 8. [[#八、正压通气的血流动力学（PPV → 急性心源性肺水肿）|八、PPV 血流动力学]]
> 9. [[#九、无创通气 NIPPV：CPAP vs BiPAP 怎么选|九、NIPPV：CPAP vs BiPAP]]
> 10. [[#十、插管指征（呼吸衰竭逼近 impending respiratory failure）⭐|十、插管指征 ⭐]]
>
> **C. 速记**
> 11. [[#十一、Memory Hook|十一、Memory Hook]]

---

## 一、核心概念：气道压的两个成分

> [!tip] 气道压 = 阻力压 + 弹性压
> 正压通气送气进肺，呼吸机端测到的压力由两部分构成：
>
> - **阻力压 (resistive pressure)** —— 气体克服气道摩擦所需，**只在有气流时存在**（气流停 → 阻力压 = 0）。取决于气道口径、管路。
> - **弹性压 (elastic pressure)** —— 撑开肺与胸壁所需，反映**呼吸系统顺应性 (respiratory system compliance)**。气流停了它依然在（肺被撑开的张力）。
>
> 关键推论：**只要消除气流，剩下的压力就纯粹是弹性压**——这正是吸气暂停的原理。

```
送气中（有气流）         吸气暂停（无气流）
┌─────────────┐         ┌─────────────┐
│  阻力压      │  气流停  │  阻力压 = 0  │
│  ＋          │ ───────→ │             │
│  弹性压      │          │  弹性压      │ ← 平台压 = 这个
└─────────────┘         └─────────────┘
   = 峰压 Peak              = 平台压 Plateau
```

---

## 二、三种压力：各测什么、怎么测

| 压力 | 英文 | 何时测 | 反映什么 | 正常值 |
|---|---|---|---|---|
| **峰压** | Peak (PIP) | 送气末、**有气流时** | 阻力压 + 弹性压（总和）| — |
| **平台压** | Plateau | **吸气暂停**、无气流时 | 弹性压 = **呼吸系统顺应性** | ≤30 cmH₂O |
| **呼气末正压** | PEEP / auto-PEEP | **呼气暂停**、呼气末 | 呼气末肺内残余压 | 设定值（auto-PEEP 为意外升高）|

> [!danger] 最高频陷阱：吸气暂停 vs 呼气暂停
> 两种「暂停测压」测的是**完全不同**的东西，stem 用哪个动作决定答案：
>
> - **吸气暂停 (inspiratory hold)** → 测 **平台压 → 顺应性**（本主题主战场）
> - **呼气暂停 (expiratory hold)** → 测 **auto-PEEP / PEEP**（COPD/哮喘气体陷闭）
>
> ❌ 别一看到「暂停后测得压力」就反射 PEEP —— 先看是**吸气**暂停还是**呼气**暂停。

---

## 三、波形图（吸气暂停三联）

> [!example]- 压力-时间波形（正常 / 顺应性↓ / 阻力↑）
>
> ![[{D0C0396C-363B-4477-89B8-C7B0EB32D002}.png]]
>
> - **上**：正常吸气暂停 —— 送气出现峰，暂停后压力回落到平台（Hold 实线），无暂停则直接衰减（No hold 虚线）。
> - **左下**：峰、平台**同步升高** → 顺应性↓（肺硬）。
> - **右下**：峰升高、平台**正常** → 阻力↑（管窄）。

---

## 四、判读决策：Peak vs Plateau ⭐

> [!tip] 一句话钥匙：「平台看顺应性，峰-平差值看阻力」
> - **平台压 = 弹性压 → 顺应性**：平台↑ = 顺应性↓ = **肺硬**
> - **Peak − Plateau 差值 → 气道阻力**：差值↑ = **管窄**

| 模式 | 病理 | 典型病因 |
|---|---|---|
| Peak↑ + **Plateau↑**（差值正常）| 顺应性↓（肺硬）| 肺水肿 (pulmonary edema)、气胸 (pneumothorax)、ARDS、腹腔间隔室综合征 (ACS)、主支气管插管过深 |
| Peak↑ + **Plateau 正常**（差值↑）| 气道阻力↑（管窄）| 支气管痉挛 (bronchospasm)、黏液栓 (mucus plugging)、咬管 (biting ET tube)、管路扭折 |

```
峰压 Peak 升高
      │
      ├── 平台压也升高 ──→ 顺应性↓（肺硬）
      │                    肺水肿 / 气胸 / ARDS / ACS
      │
      └── 平台压正常 ────→ 阻力↑（管窄）
        （Peak−Plateau↑）  痉挛 / 黏液栓 / 咬管 / 扭折
```

> [!question]- 自测：插管镇静患者做吸气暂停 2 秒，无气流时口端压力升高 —— 这个压力反映什么？
> **呼吸系统顺应性 (respiratory system compliance)**。无气流 → 阻力压 = 0 → 测得的就是平台压 = 弹性压 = 顺应性。压力升高 = 顺应性↓（肺硬）。
> 干扰项辨析：
> - ❌ PEEP / 呼气末压 → 要用**呼气**暂停测，本题是吸气暂停
> - ❌ 总气道阻力 → 是 **Peak − Plateau 差值**，不是平台压本身
> - ❌ 上气道阻力 → 插管已绕过上气道 = 0
> - ❌ 呼气肌力 → 需清醒配合，镇静被动患者测不了

---

## 五、呼吸机旋钮与 ABG 调参（给一份 ABG，调哪个钮）⭐

> [!tip] 两条独立通路：CO₂ 走通气，O₂ 走 PEEP/FiO₂
> - **CO₂ ∝ 分钟通气量 (minute ventilation) = 潮气量 VT × 呼吸频率 RR** → CO₂ 异常 → 调 **VT 或 RR**
> - **O₂ ← FiO₂ + PEEP**（PEEP 复张肺泡、改善 V/Q 匹配）→ 低氧 → 调 **FiO₂ 和/或 PEEP**

| ABG 异常 | 病理 | 调哪个钮 |
|---|---|---|
| **PaCO₂ ↑**（呼吸性酸中毒）| 通气不足 | ↑ RR 或 ↑ VT（↑分钟通气）|
| **PaCO₂ ↓**（呼吸性碱中毒）| 通气过度 | ↓ RR 或 ↓ VT |
| **PaO₂ ↓**（低氧血症）| 氧合差 | ↑ FiO₂ 和/或 ↑ PEEP |

> [!danger] 关键反射：肺泡复张后不要降 PEEP (Do not decrease PEEP once alveoli recruited)
> ARDS 氧合一好转就撤 PEEP → 肺泡再塌陷（去复张）→ 低氧反弹。**氧合好≠可撤 PEEP**。

---

## 六、auto-PEEP / 气体陷闭（用呼气暂停测）

> [!warning] auto-PEEP (内源性呼气末正压) = 呼气不完全 → 肺内气体陷闭 (air trapping)
> **COPD / 哮喘 (asthma, 哮喘)** 呼气阻力高 + 呼气时间不足 → 呼气末肺泡未排空 → 残余正压堆积。
> - **怎么测**：**呼气暂停 (expiratory hold)** —— 呼应 §二「吸气暂停测平台/顺应性，呼气暂停测 PEEP」
> - **后果**：胸内压↑ → 静脉回流↓ → **低血压**；气压伤 (barotrauma)；触发呼吸机困难
> - **怎么减**：↓ RR、↓ VT、**延长呼气时间（I:E 比拉长）**、积极治支气管痉挛 (bronchospasm)

> [!tip] 床旁鉴别：机械通气患者突发低血压
> 想两件事 → **① 张力性气胸 (tension pneumothorax, 张力性气胸)**；**② auto-PEEP**。
> **断开呼吸机让肺被动完全排空**，若血压随之回升 = auto-PEEP 证实（同时也排掉气体陷闭）。

---

## 七、肺保护性通气（ARDS）

> [!success] 低潮气量 + 限平台压 = 唯一明确降死亡率的通气策略
> - **低潮气量 VT 6 mL/kg 理想体重 (IBW)** + **平台压 (plateau) <30 cmH₂O** → 减少容积伤 (volutrauma) / 气压伤 (barotrauma)
> - 配适度 PEEP 复张肺泡改善氧合
> 详见 [[完整笔记/专题笔记/pulmonary/pulmonary_ARDS]]。

---

## 八、正压通气的血流动力学（PPV → 急性心源性肺水肿）

> [!info] PPV (正压通气) 对心脏是「卸负荷」
> 正压 → **右室前负荷↓ (RV preload↓)** + **左室前负荷↓ (LV preload↓)** + **左室后负荷↓ (LV afterload↓)** → 利于 LV 充盈与射血 → 肺淤血↓、氧供↑。
> - **用途**：**急性心源性肺水肿 (acute cardiogenic pulmonary edema, 急性心源性肺水肿)** —— CPAP/BiPAP 快速缓解。
> - **双刃**：**低血容量 (hypovolemia)** 患者上 PPV → 前负荷骤降 → 低血压。

---

## 九、无创通气 NIPPV：CPAP vs BiPAP 怎么选

| 模式 | 适应证 | 重点 |
|---|---|---|
| **BiPAP**（双水平）| AECOPD（pH <7.35 且 PaCO₂ >45）、重症哮喘早期短试、OHS、部分心源性肺水肿 | **既改善通气（吹 CO₂）又改善氧合** |
| **CPAP**（单一持续正压）| 阻塞性睡眠呼吸暂停 (OSA, 阻塞性睡眠呼吸暂停)、部分心源性肺水肿 | 主要撑开上气道/复张肺泡改善氧合，**不主动吹 CO₂** |

> [!warning] NIPPV 的禁忌反射
> 需要 BiPAP 降 CO₂（有高碳酸）→ 选 BiPAP 不选 CPAP（CPAP 不吹 CO₂）。
> **哮喘出现 AMS（意识改变）+ PaCO₂ 正常/↑ + silent chest（沉默肺）→ 跳过 NIPPV 直接插管**。

---

## 十、插管指征（呼吸衰竭逼近 impending respiratory failure）⭐

> [!danger] 最高频陷阱：哮喘/COPD 的 PaCO₂「本应低却正常或升高」
> 急性哮喘患者过度通气 → PaCO₂ **应该低**。若 PaCO₂ **正常或升高** = 肌肉疲劳、通气失败 = **impending respiratory failure（呼吸衰竭逼近）→ 气管插管**，不是继续加雾化。

| 情况 | PaCO₂ | pH | 意义 |
|---|---|---|---|
| 一般急性哮喘 | ↓ | ↑ / 正常 | 过度通气，还撑得住 |
| **呼吸衰竭逼近** | **正常 / ↑** | ↓ | **喘不动了 → 插管** |

> [!info] 其它插管征象（出现即低阈值插管，别等血气崩）
> - **AMS（意识状态改变）** —— 脑灌注差 / CO₂ 麻醉 / 低氧
> - **silent chest（沉默肺）** —— 气流太弱听不到喘鸣，比满肺哮鸣更危险
> - **大量动用辅助呼吸肌、WOB（呼吸功）极高、血流动力学不稳**
> - NIPPV 短试（<2 小时）无改善或恶化

---

## 十一、Memory Hook

> [!success] 锁定记忆
> **压力判读**：
> 「**吸气**暂停无气流 → **平台压 = 弹性 = 顺应性**（平台高 = 肺硬：水肿/气胸/ARDS/ACS）。
> **呼气**暂停才测 **PEEP/auto-PEEP**。
> **Peak − Plateau = 阻力**（差值大 = 管窄：痉挛/黏液栓/咬管）。」
>
> **调参与决策**：
> - **CO₂ 走通气（VT×RR），O₂ 走 FiO₂+PEEP** —— 两条独立通路。
> - **肺泡复张后别降 PEEP**；ARDS = 低 VT 6 mL/kg + 平台 <30。
> - **机械通气突发低血压 → 张力性气胸 or auto-PEEP**（断机排气血压回升 = auto-PEEP）。
> - **BiPAP 吹 CO₂，CPAP 不吹**；有高碳酸选 BiPAP。
> - **哮喘 PaCO₂「本应低却正常/↑」= 呼吸衰竭逼近 → 插管**（+AMS/silent chest）。

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes_2026-06#^Q4713]] 吸气暂停=平台压=顺应性（误选 PEEP）
  - [[mistakes/uworld-mistakes_2026-06#^Q4931]] 术后肺不张 ABG（通气生理）
  - [[mistakes/uworld-mistakes_2026-06#^Q4932]] 术后肺不张预防
  - [[mistakes/uworld-mistakes_2026-06#^Q4562]] ARDS 改善氧合 → 加 PEEP（氧合=PEEP+FiO₂；CO₂ 正常不动 RR/VT）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/pulmonary]]（Plateau 看顺应性 / Peak−Plateau 看阻力 段）
- 📚 相关专题：
  - [[完整笔记/专题笔记/呼吸/呼吸_HighYield速查总览]]（§气道压力判读 tip + 呼吸机旋钮）
  - [[完整笔记/专题笔记/pulmonary/pulmonary_ARDS]]（肺保护通气：低 VT + 平台压 <30）
  - [[完整笔记/专题笔记/pulmonary/pulmonary_气胸Pneumothorax]]（张力性气胸 → 平台压骤升）
- 🏥 跨学科：[[完整笔记/Peixuan分科笔记/外科]]（围术期/ICU 通气、ACS）
