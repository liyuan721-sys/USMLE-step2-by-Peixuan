---
tags:
  - USMLE-Step2
  - psych
  - 神经
  - 专题笔记
created: 2026-05-19
type: 专题笔记
source: 2026-05-19 Q3762 Alprazolam withdrawal seizure 错题触发新建
---

# 停药综合征鉴别速查（Discontinuation / Withdrawal Syndromes）

> [!info] 本笔记定位
> 只回答一个问题：**药停了 / 漏药 / 减量后会出什么事** —— 哪些会 seizure、哪些会致命、各自是什么综合征。
>
> 这是**鉴别速查**，不是治疗手册。酒精 / 阿片 / 尼古丁戒断的**具体用药管理**见 [[完整笔记/专题笔记/psych_成瘾药物对照表]]；本笔记做两件互补的事：① 各类停药综合征的**横向鉴别**；② **抗抑郁药停药**（SSRI/SNRI/TCA —— 成瘾笔记不覆盖的部分）。
>
> **触发错题**：[[mistakes/uworld-mistakes#^Q3762]]（短效 BZD 漏药 2 天 → 新发 generalized tonic-clonic seizure）

> [!tip] 术语别混：Withdrawal ≠ Discontinuation
> - **Withdrawal（戒断）** —— 用于会产生**生理依赖**的物质：Alcohol / BZD / Barbiturate / Opioid。
> - **Discontinuation syndrome（停药综合征）** —— 专指 **SSRI/SNRI 等抗抑郁药**。刻意不叫 "withdrawal"，是为了强调抗抑郁药**不是成瘾物质**（无 craving、无 drug-seeking），只是突然撤药后的神经适应反跳。

---

## 目录

- [[#0. 核心三问决策框架|0. 核心三问决策框架]]
- [[#1. 停药综合征大一统对照表|1. 停药综合征大一统对照表]]
- [[#2. BZD 专题 — 半衰期决定 withdrawal 风险|2. BZD 专题 — 半衰期决定 withdrawal 风险]]
- [[#3. SSRI/SNRI Discontinuation Syndrome（FINISH 助记）|3. SSRI/SNRI Discontinuation（FINISH）]]
- [[#4. 用药本身 vs 停药 — seizure 来源鉴别|4. 用药本身 vs 停药 — seizure 来源鉴别]]
- [[#5. USMLE 高频陷阱|5. USMLE 高频陷阱]]
- [[#6. 记忆挂钩|6. 记忆挂钩]]
- [[#7. 自测题|7. 自测题]]
- [[#关联|关联]]

---

## 0. 核心三问决策框架

> [!tip] 拿到"停药 / 漏药 / 减量后出现新症状"的题，按 3 问走
> 1. **会不会 seizure？** —— 只有 **GABA 类**（Alcohol / BZD / Barbiturate）停药会 seizure。
> 2. **会不会致命？** —— 同样只有 **GABA 类**会（seizure + delirium / DT）。
> 3. **什么综合征性质？** —— GABA 类 = withdrawal（兴奋反跳）；阿片 = withdrawal（痛苦但不致命）；SSRI/SNRI = discontinuation（FINISH）。

```
新发症状 ← 最近停药 / 漏药 / 减量？
        │
        ▼
   是哪一类药？
        │
 ┌──────┼───────────────────┐
 ▼      ▼                   ▼
GABA 类   Opioid          抗抑郁药（SSRI / SNRI）
（酒/BZD/  → withdrawal     → discontinuation
 巴比妥）   吐/泻/痛/失眠/      FINISH（见 §3）
 → with-   竖毛/散瞳         不致命、无 seizure
   drawal  痛苦但不致命
   焦虑→震颤  无 seizure
   →自主神经
   →SEIZURE
   →delirium
   ⚠️ 可致命
```

> [!danger] 一句话锁定
> **能 seizure + 能致命的停药综合征只有 GABA 三兄弟（Alcohol / BZD / Barbiturate）。** 其它一律"难受但不死、不抽"。

---

## 1. 停药综合征大一统对照表

| 类别 | 机制 | 代表药 | Seizure? | 致命? | 特征症状 | 起病窗口 |
|---|---|---|---|---|---|---|
| **BZD withdrawal** | GABA-A 受体下调 → 停药失抑制 | Alprazolam（短效最危险）| ✅ | ⚠️ **可致命** | 焦虑、震颤、失眠 → 自主神经亢进 → **seizure** → delirium | 短效数小时-1 天；长效数天 |
| **Alcohol withdrawal** | 同上（GABA-A）| 乙醇 | ✅ | ⚠️ **可致命** | 6h 震颤 → 12-48h seizure / 幻觉 → 48-96h DT | 6-96h |
| **Barbiturate withdrawal** | 同上（GABA-A）| Phenobarbital | ✅ | ⚠️ **可致命** | 同 BZD（兴奋反跳）| 数天 |
| **Opioid withdrawal** | μ 受体撤药 | Heroin、Oxycodone | ❌ | ❌（痛苦但不致命）| 流泪流涕、散瞳、腹泻、肌痛、竖毛、打哈欠 | 短效 4-12h；长效 24-48h |
| **SSRI/SNRI discontinuation** | 5-HT 突然撤药、神经适应反跳 | Paroxetine、Venlafaxine（短半衰期最重）| ❌ | ❌ | **FINISH**（见 §3）| 停药后 1-3 天 |
| **TCA 停药** | 胆碱能反跳（rebound）| Amitriptyline、Clomipramine | ❌ | ❌ | 轻度 **cholinergic rebound**：恶心、腹泻、流泪、出汗、失眠 | 停药后 1-3 天 |

> [!warning] 读表要点
> - **Seizure + 致命 = 只有上 3 行（GABA 类）。** 这是本表最高频的考点。
> - **Opioid withdrawal 很痛苦但不致命**（成人）——"vital signs 大致正常"是它和 GABA 类戒断的决定性区别（详见 [[完整笔记/专题笔记/psych_成瘾药物对照表#3. Opioid（阿片）]]）。
> - **SSRI/SNRI discontinuation 综合征可以很难受，但绝不 seizure** —— "综合征严重 ≠ 会 seizure"是经典陷阱（见 §5）。
> - 酒精 / 阿片 / BZD 戒断的**具体处理用药**见 [[完整笔记/专题笔记/psych_成瘾药物对照表]]；本表只做"会不会出事"的鉴别。

---

## 2. BZD 专题 — 半衰期决定 withdrawal 风险

### 2.1 BZD 半衰期排序 = withdrawal / seizure 风险

| BZD | 半衰期 | Withdrawal / seizure 风险 | 临床用途 |
|---|---|---|---|
| **Triazolam** | 超短（2-5h）| ⚠️⚠️⚠️ 极高 | 失眠（短效催眠）|
| **Alprazolam (Xanax)** | 短（~12h）| ⚠️⚠️⚠️ **最高** | 焦虑、panic |
| **Lorazepam / Oxazepam / Temazepam** | 中（10-20h）| ⚠️⚠️ 中 | **"LOT" → 肝病 / 老年安全**（无活性代谢物，仅经肾排）|
| **Clonazepam** | 长（30-40h）| ⚠️ 低-中 | 癫痫、panic |
| **Chlordiazepoxide** | 长 | ⚠️ 低 | **酒精 withdrawal 首选** |
| **Diazepam** | 长（>24h，活性代谢物 >100h）| ⚠️ 低（**自我 taper**）| 抗焦虑、肌松、status epilepticus |

> [!danger] 一句话锁定
> 半衰期**越短 → 停药后血药浓度断崖式下跌 → withdrawal 越爆烈 → seizure 风险越高**。
> **Alprazolam = "the Xanax bar"**：短、强、快 → 最高滥用 + 最高 withdrawal。

### 2.2 BZD withdrawal 时间轴

```
长期 BZD 使用 ──► 突然停药 / 漏药
            │
            ▼
GABA-A 受体下调（chronic use 的代偿性适应）
            │
            ▼
突然失去 GABA 抑制 ──► 中枢过度兴奋
            │
   ┌────────┼────────────────────────────────┐
   ▼        ▼              ▼                  ▼
24h 内    1-3 天        严重               最严重
anxiety   autonomic      SEIZURES          psychosis
tremor    hyperactivity  （generalized      delirium
insomnia  （HTN、心动      tonic-clonic）    （可致命）
知觉异常    过速、出汗）
```

> [!info] 与酒精戒断同机制
> BZD 和酒精都作用于 **GABA-A**，所以 BZD withdrawal 和 alcohol withdrawal 的机制、时间轴、致命性**完全平行**。两者都能 seizure、都能进展到 delirium。

### 2.3 长效 BZD 的临床应用（半衰期逻辑的两个落地）

> [!tip] 长半衰期 = 自带"缓释 taper"（降落伞）
> - **戒酒 / 戒 BZD 首选长效**（Chlordiazepoxide / Diazepam）：长效药代谢慢，血药浓度自己平滑下降 = 内置 taper，避免短效药"停了又反跳"的循环。
> - **短效 BZD（Alprazolam）绝不能突然停** —— 必须换长效或缓慢递减，否则 withdrawal seizure。

> [!tip] LOT 法则 —— 肝病 / 老年首选
> **L**orazepam / **O**xazepam / **T**emazepam **不经肝代谢**（无活性代谢物，仅经肾结合排泄）→ 肝病、老年、危重患者首选。
> （详见 [[完整笔记/专题笔记/psych_成瘾药物对照表#1.2 【急性戒断期 6-96h】Benzodiazepines — 救命药 ⭐]]）

---

## 3. SSRI/SNRI Discontinuation Syndrome（FINISH 助记）

| 项 | 内容 |
|---|---|
| **高危药物** | **短半衰期**：Paroxetine（SSRI 最严重）、Venlafaxine（SNRI 最严重）|
| **低危药物** | **长半衰期**：Fluoxetine（半衰期长 + 活性代谢物 = 自动 taper，几乎不发生）|
| **起病** | 停药后 **1-3 天** |
| **持续** | **1-2 周** |
| **症状（FINISH）** | **F**lu-like（流感样）· **I**nsomnia · **N**ausea · **I**mbalance（头晕 / 失衡）· **S**ensory disturbance（"electric shocks" / brain zaps）· **H**yperarousal（焦虑 / 易激惹）|
| **关键** | **无 seizure**（这是它和 GABA 类 withdrawal 的根本区别）|
| **处理** | 恢复原药 → 之后**缓慢 taper**；或换成长半衰期的 Fluoxetine 过渡 |

> [!warning] 为什么 Fluoxetine 几乎不发生 discontinuation
> Fluoxetine 半衰期长（活性代谢物 norfluoxetine 更长达 1-2 周）→ 停药后血药浓度**自己缓降** = 自带 taper。短半衰期的 Paroxetine / Venlafaxine 停药后断崖式下跌 → 综合征最重。
> **半衰期决定停药反应严重度 —— 这条规律对 BZD（§2）和抗抑郁药完全一致。**

---

## 4. 用药本身 vs 停药 — seizure 来源鉴别

> [!danger] 本节是 USMLE 最爱的双向陷阱
> "某药 + seizure"出现时，必须分清 seizure 是**用药本身的副作用**还是**停药综合征**。同一组精神科药，有的怕"吃"、有的怕"停"、有的怕"起始 titrate"。

| 药物 / 类别 | **停药** → seizure? | **用药本身** → seizure? | 备注 |
|---|---|---|---|
| **Alprazolam**（短效 BZD）| ✅ **会**（withdrawal seizure，可致命）| ❌ | 用药本身风险是镇静、**依赖**；危险在"停" |
| **Bupropion**（NDRI）| ❌ | ✅ **会**（**剂量相关**）| **eating disorder（bulimia / anorexia）、癫痫史禁用**；电解质紊乱进一步↑风险 |
| **TCA**（Clomipramine / Amitriptyline）| ❌（仅轻度 cholinergic rebound）| ✅ **会**（**过量时**）| 过量三联征：**seizure + arrhythmia + anticholinergic** |
| **Lamotrigine** | ❌（仅在**已有癫痫**患者中诱发）| ❌（药本身的风险是 **SJS/TEN**）| 必须 **slow titration** 防皮疹；是双相维持首选 |
| **SSRI / SNRI** | ❌（discontinuation = FINISH，无 seizure）| ❌ | 综合征再重也不 seizure |
| **Mirtazapine** | ❌ | ❌ | 无明显停药综合征 |

> [!tip] 记忆抓手 —— 每个药都有"特征性风险时机"
> - **Bupropion → "吃的时候"怕 seizure**（瘦人 / eating disorder 禁用）
> - **TCA → "过量时"**三联征（seizure + 心律失常 + 抗胆碱）
> - **Lamotrigine → "起始 titrate 时"怕 SJS/TEN**
> - **Alprazolam → "停的时候"怕 seizure**

> [!warning] Lamotrigine 停药陷阱
> "Lamotrigine 停药 → seizure" 只在患者**本身已有癫痫**时成立（停了抗癫痫药当然会复发）。**无癫痫史的患者停 Lamotrigine 不会 seizure**。Lamotrigine 真正的标志性风险是**起始期 SJS/TEN**。

---

## 5. USMLE 高频陷阱

| 陷阱 | 真相 |
|---|---|
| "焦虑患者新发 seizure = 原发癫痫" | ❌ 先想**药物**（BZD withdrawal）/ **代谢**（电解质）/ **物质**（酒精 withdrawal）。无家族史 + 急性起病 + 漏药 → 药物因素。|
| "所有停药综合征都会 seizure" | ❌ 只有 **BZD + Alcohol + Barbiturate**（GABA 机制）。Opioid、SSRI/SNRI、TCA 都不会。|
| "Bupropion 突然停 → seizure" | ❌ Bupropion 的 seizure 是**用药本身、剂量相关的副作用**（eating disorder / 电解质紊乱时尤甚），**不是停药**。|
| "TCA 突然停 → seizure" | ❌ TCA seizure 是**过量副作用**（伴 arrhythmia + anticholinergic 三联征）；停药只引起轻度 cholinergic rebound，不 seizure。|
| "Lamotrigine 停药 → seizure" | ❌ 仅在**已有癫痫**的患者中诱发。无癫痫史 → 停药不 seizure。Lamotrigine 真正风险是**起始时 SJS/TEN**。|
| "Paroxetine / Venlafaxine 停药综合征严重 = 会 seizure" | ❌ **综合征严重 ≠ seizure**。SSRI/SNRI discontinuation = FINISH，**始终无 seizure**。|
| "Alprazolam 用药本身会 seizure" | ❌ BZD 用药本身是抗惊厥的；BZD 的 seizure 风险在**停药**。|

---

## 6. 记忆挂钩

> [!success] 一句话锁定
> "**Short-acting BZD + missed doses + seizure**" = Alprazolam 的经典 stem。

> [!tip] 四条口诀
> - **GABA 药物（BZD + 酒 + 巴比妥）withdrawal → 会 seizure、可致命**
> - **5-HT 药物（SSRI/SNRI）discontinuation → FINISH，不 seizure**
> - **Opioid withdrawal → 痛但不死**
> - **Bupropion / TCA 的 seizure → 用药副作用，不是停药**

> [!tip] 半衰期是贯穿全篇的主线
> - 短半衰期 BZD（Alprazolam / Triazolam）→ withdrawal 最爆烈
> - 短半衰期抗抑郁药（Paroxetine / Venlafaxine）→ discontinuation 最重
> - 长半衰期 = 自带"缓释 taper / 降落伞"：Diazepam 用来戒酒戒 BZD；Fluoxetine 几乎不发生停药综合征

---

## 7. 自测题

> [!question]- Q1：28 岁焦虑女性，PCP 处方某药 6 个月，无癫痫史、无酗酒、无家族史，漏药 2 天后新发 generalized tonic-clonic seizure + confusion。最可能服用的是哪一类药？为什么？
> **短效 BZD（Alprazolam 最典型）**。长期 BZD 使用 → GABA-A 受体下调；突然停药 → GABA 抑制丧失 → 中枢过度兴奋 → withdrawal seizure。短半衰期 = 停药后血药浓度断崖下跌 = withdrawal 最爆烈。无癫痫史 / 家族史 + 急性起病 + 漏药 → 指向药物因素而非原发癫痫。

> [!question]- Q2：把以下 BZD 按 withdrawal / seizure 风险从高到低排：Diazepam、Alprazolam、Lorazepam、Triazolam、Chlordiazepoxide。
> **Triazolam（超短）> Alprazolam（短）> Lorazepam（中）> Chlordiazepoxide ≈ Diazepam（长）**。规律：半衰期越短，风险越高。

> [!question]- Q3：患者停用 Paroxetine 2 天后出现流感样症状、失眠、恶心、头晕、"电击感（brain zaps）"。这是什么综合征？会 seizure 吗？怎么处理？
> **SSRI discontinuation syndrome**（FINISH：Flu-like / Insomnia / Nausea / Imbalance / Sensory disturbance / Hyperarousal）。**不会 seizure**。处理：恢复原药 → 之后缓慢 taper。Paroxetine 半衰期短，是 SSRI 中最易发生的。

> [!question]- Q4：为什么戒酒和戒 BZD 首选长效 BZD（Chlordiazepoxide / Diazepam），而不是 Alprazolam？
> 长半衰期药代谢慢、血药浓度自己平滑下降 = **内置"缓释 taper"**，避免短效药"停了又反跳 → 再给 → 再反跳"的循环。短效 Alprazolam 反而是 withdrawal 风险最高的药。

> [!question]- Q5：下列哪些药的"停药"会导致 seizure：BZD / Alcohol / Opioid / SSRI / TCA？
> **只有 BZD 和 Alcohol**（再加 Barbiturate）—— 都是 GABA-A 机制。Opioid、SSRI、TCA 停药都不会 seizure。

> [!question]- Q6：Bupropion 的 seizure 风险是"用药本身"还是"停药"引起的？哪些患者禁用？
> **用药本身**（剂量相关副作用），不是停药。禁用于 **eating disorder（bulimia / anorexia）和癫痫史**患者；电解质紊乱会进一步增加风险。

> [!question]- Q7：TCA 过量的三联征是什么？TCA 停药会怎样？
> 过量三联征：**seizure + arrhythmia（心律失常）+ anticholinergic（抗胆碱）**。停药则只引起轻度 **cholinergic rebound**（恶心、腹泻、流泪、出汗、失眠），**不 seizure**。

> [!question]- Q8：Lamotrigine 的两个标志性风险时机是什么？一个无癫痫史的双相患者突然停 Lamotrigine 会 seizure 吗？
> 两个时机：① **起始 titration 时 → SJS/TEN**（所以必须慢加量）；② **已有癫痫的患者停药 → 诱发 seizure**。无癫痫史的患者停 Lamotrigine **不会 seizure**。

---

## 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes#^Q3762]] ✅ Alprazolam withdrawal seizure（短效 BZD 漏药 → GTC seizure；触发本笔记新建）
  - 等积累 SSRI discontinuation / Bupropion 禁忌 / Alcohol withdrawal / Lamotrigine SJS 错题后横向连接
- 📚 主笔记：
  - [[完整笔记/Peixuan分科笔记/psych]]（抗焦虑 / 抗抑郁药 + 物质相关障碍）
  - [[完整笔记/专题笔记/psych_成瘾药物对照表]] ⭐ **互补专题**（对方 = 戒断 / 维持的**用药管理**；本笔记 = 各类停药综合征的**鉴别** + 抗抑郁药停药）
- 🏥 跨学科：
  - [[完整笔记/Peixuan分科笔记/neuro]]（seizure 鉴别 — 药物诱发 / 停药 vs 原发癫痫）
  - [[完整笔记/专题笔记/psych_物质急诊速查]]（急性中毒表现 vs 停药综合征，对照参考）
- 🌱 TODO（后续补充）：
  - 累积 SSRI/SNRI discontinuation 实战错题后 → 扩 §3（FINISH 各症状的 stem 写法）
  - 累积 Bupropion 禁忌 / Lamotrigine SJS 错题后 → 扩 §4 用药 vs 停药表
  - 累积 BZD 戒断 / DT 错题后 → 与成瘾笔记 §1、§4 交叉补强
  - 待积累后可考虑扫 psych / neuro 分科笔记找增量并整合

---

## 版本记录

- **v1（2026-05-19）**：Q3762（Alprazolam withdrawal seizure，✅做对题反向贡献）触发新建。覆盖核心三问框架、停药综合征大一统对照表、BZD 半衰期专题、SSRI/SNRI discontinuation（FINISH）、用药 vs 停药 seizure 来源鉴别、高频陷阱、自测 8 题。定位为 [[完整笔记/专题笔记/psych_成瘾药物对照表]] 的鉴别向互补专题。
