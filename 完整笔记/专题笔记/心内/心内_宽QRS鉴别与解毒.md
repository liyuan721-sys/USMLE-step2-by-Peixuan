---
tags:
  - USMLE-Step2
  - 心血管
created: 2026-06-11
type: 专题笔记
---

# 宽 QRS 鉴别与解毒（Wide QRS — toxic/metabolic & antidotes）

> [!info] 用途
> 见"**宽 QRS（>120 ms，无既往 BBB）+ 中毒/代谢背景**"时，快速锁病因 + 对应解毒。
> 心电全景图见 [[完整笔记/专题笔记/心内/心内_代谢性ECG改变]]；本卡是"宽 QRS"这一条的鉴别 + 解毒纵深。

---

## §零 一张表锁死 ⭐

| 病因 | 标志性 ECG | 背景线索 | 解毒 / 处理 |
|---|---|---|---|
| **TCA（三环类）中毒** | **宽 QRS + R 波 aVR >3mm** ⭐ | 抗胆碱综合征（散瞳/口干/尿潴留）+ 长 QT + 窦速 | **IV NaHCO3（碳酸氢钠）** ⭐ |
| **高钾 Hyperkalemia** | **宽 QRS + T 高尖窄底**→ sine wave | CKD/透析漏做、ACEI+保钾利尿、挤压伤 | **IV Calcium gluconate（葡萄糖酸钙，不等血钾）** ⭐ |
| **CCB（非二氢吡啶 nondihydropyridine）中毒** | 主**Brady + AV block**，QRS 晚期才宽 | **低血压 + Brady + 高血糖** ⭐ | **Calcium（钙）+ 胰岛素-葡萄糖 + Glucagon（胰高血糖素）** |
| **Brugada 综合征** | **V1–V2 coved 型 ST 抬高**（RBBB 样）| 年轻男、夜间猝死/晕厥家族史、发热诱发 | **ICD**（不是解毒；电风暴用 Isoproterenol 异丙肾上腺素 / Quinidine 奎尼丁）|

> [!danger] 单题最快钥匙
> - 宽 QRS **+ R 波 aVR** → **TCA → NaHCO3**
> - 宽 QRS **+ T 高尖 / sine wave** → **高钾 → Calcium**
> - **Brady + 低血压 + 高血糖** → **CCB → Calcium/胰岛素**
> - **V1-V2 coved ST + 发热/夜间晕厥** → **Brugada → ICD**

---

## §一 逐个拆解

### 1.1 TCA 中毒 —— 钠通道阻断

```
机制：阻断心肌 Na 通道 → 0 相去极变慢 → QRS 增宽
危险阈值：QRS >100ms = 心律失常风险；>160ms = 室速/室颤风险
指纹：R 波 aVR >3mm（电轴右偏，钠通道阻断特征）
伴随：抗胆碱（散瞳、皮肤干热、尿潴留、谵妄）+ 长 QT + 低血压 + 癫痫
```

> [!info] NaHCO3 为什么有效 —— 两条通路（钠 + 碱各干一件事）⭐
> NaHCO3 = **Na⁺（钠负荷）+ HCO3⁻（碱化）**，两个成分分头解毒：
>
> **通路 1 · 钠负荷 (sodium load) — 拼浓度梯度**
> 给大量 Na⁺ → 细胞外 Na⁺↑ → 跨膜电化学梯度↑ → 即使部分通道被 TCA 占住，从**未被阻断的通道**驱动力更强、涌入更多 Na⁺ → 0 相恢复 → QRS 变窄。
> （类比：门堵一半，但门外压力加大，从没堵那半挤进去的反而更多。）
>
> **通路 2 · 碱化 (alkalinization, pH 7.45–7.55)**
> - ① 降低 TCA 对 Na 通道的**亲和力** → 药物解离 → 通道腾空（酸性环境反加重结合，故纠酸/碱化是关键）
> - ② 更多 TCA 与血浆蛋白结合 → **游离药↓** → 作用于心脏的活性药减少
>
> **合起来**：钠 = 加供给（旁路冲）；碱 = 减阻断（腾通道）→ 0 相恢复 → QRS 收窄 → 折返基质消失 → 室性心律失常终止。
>
> **指征**：QRS >100ms / 室性心律失常 / 低血压（不等骤停）；**目标** pH 7.45–7.55；不够时**过度通气**协同碱化。**QRS 宽度 > 血药浓度**作床旁实时读数。
>
> > [!tip] 同机制可推广
> > IC 类（Flecainide 氟卡尼）、**可卡因 cocaine**、苯海拉明 diphenhydramine、局麻药 local anesthetics 过量的宽 QRS —— 都是钠通道阻断，处理同（NaHCO3 碳酸氢钠）。Brugada 也是钠通道（先天功能丧失）→ 故 Brugada 患者要**避开**这些药。

### 1.2 高钾 —— 最致命，先给钙

```
ECG 5 阶段：T 高尖 → P 平+PR长 → P 消失+QRS 宽 → sine wave → asystole
（口诀 Tent → Pass → Wide → Sine → Flatline）
宽 QRS 出现在 K ≈7.5-8.0，已属危急
```

- **ECG 一异常 → Calcium gluconate（葡萄糖酸钙）不等血钾**（稳定心肌膜，几分钟起效，不降钾）
- 随后降钾：**胰岛素+葡萄糖、β激动剂（如 albuterol 沙丁胺醇）、利尿/透析**
- 深度见 [[完整笔记/专题笔记/肾脏/肾脏_高钾血症完整体系]]

> [!warning] 别和 TCA 搞混
> 都可宽 QRS，但**高钾有 T 高尖 / sine wave + 肾衰背景**；**TCA 有 R aVR + 抗胆碱 + 精神药过量史**。解毒完全相反（钙 vs 碳酸氢钠）。

### 1.3 CCB（维拉帕米 verapamil / 地尔硫卓 diltiazem）中毒 —— 其实主征不是宽 QRS

> [!warning] 纠偏
> 非二氢吡啶 CCB 的**核心三联 = Brady + 低血压 + 高血糖**（钙依赖的胰岛素分泌被抑制 → 血糖升高，是和 β-blocker 中毒的关键区别）。
> ECG 主要是 **PR 延长 / AV 阻滞 / 窦缓**；**宽 QRS 只在重度晚期**出现。不要把"宽 QRS"当 CCB 首要线索。

| 维度 | β-Blocker | CCB（verapamil/diltiazem）|
|---|---|---|
| 血糖 | **低**（β2 抑制糖原分解）| **高**（抑制胰岛素分泌）⭐ |
| 解毒 | **Glucagon（胰高血糖素）** ⭐ | **Calcium 钙（高剂量）+ 胰岛素-葡萄糖 + lipid emulsion（脂肪乳）** |

### 1.4 Brugada 综合征 —— 不是中毒，是通道病

```
心电：V1-V2 "coved 型" ST 抬高（下斜）+ RBBB 样形态（≠ 真宽 QRS 全导联）
机制：SCN5A 钠通道功能丧失（loss-of-function）
诱发：发热、钠通道阻断药、可卡因、迷走张力高（夜间/睡眠）
高危：夜间猝死 / 不明晕厥家族史（东南亚男性）
处理：ICD（唯一确证有效）；急性电风暴 → isoproterenol 异丙肾上腺素 / quinidine 奎尼丁
退热：发热会暴露/加重 → 积极退热
```

> [!tip] 和高钾对比记
> Brugada 的"钠通道功能↓"和 TCA 的"钠通道被药阻断"机制同源 → **发热 + 钠通道阻断药会诱发/加重 Brugada**。所以 Brugada 患者要避开 TCA / IC 类 / 可卡因。

> [!info]- 电风暴急性药物：为什么是 isoproterenol / quinidine（一推一拉）
> **电风暴 (electrical storm)** = 24h 内 ≥3 次室速/室颤（或 ICD 放电 ≥3 次），危及生命。ICD 负责"电回来"，但反复发作需药物从机制上压住。
>
> **病根**：SCN5A 钠通道功能丧失 → 0 相 Na⁺↓ → 右室心外膜 phase 1 外向钾电流 **Ito 相对占上风** → 动作电位**穹顶 (dome) 丢失** → **phase 2 折返** → VF。
> 失衡本质 = **内向电流（Na/Ca）太弱 vs 外向电流（Ito）太强**。
>
> | 药 | 给药 | 机制 | 纠失衡 |
> |---|---|---|---|
> | **Isoproterenol（异丙肾上腺素）** | IV，急性 | β激动 → ↑L 型钙电流 ICa + 加快心率 | **补内向电流** + 对冲"慢心率/夜间迷走加重" |
> | **Quinidine（奎尼丁）** | 口服，后续/长期 | IA 类 → 阻断 **Ito 外向钾电流** | **削外向电流** → 穹顶恢复，消除 phase 2 折返 |
>
> **一句话**：内向太弱、外向 Ito 太强 → 穹顶塌。**Isoproterenol 从下顶（加钙+提心率），Quinidine 从上压（堵 Ito）**，一推一拉撑回穹顶。
>
> **考试优先级**：根本/确证治疗仍是 **ICD**（高危：晕厥/骤停/自发 1 型 ECG）；isoproterenol/quinidine 是电风暴的**补充**不是替代；**发热要积极退热**（诱发 1 型）。

---

## §二 速记口诀

> [!success] Memory Hook
> **宽 QRS 四问**：①有 R aVR + 抗胆碱? → TCA → **碳酸氢钠**｜②有 T 高尖 + 肾衰? → 高钾 → **钙**｜③Brady+低压+**高血糖**? → CCB → **钙/胰岛素**｜④V1-V2 coved + 发热夜间晕厥? → Brugada → **ICD**。
> **钠通道阻断家族**（TCA/IC/可卡因/Brugada 诱发）→ 都怕钠通道，治/防都围绕钠。

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes_2026-06#^Q4487]] TCA 过量 QRS 130ms → 碳酸氢钠（误选葡萄糖酸钙）✅ §1.1 锚点
  - [[mistakes/uworld-mistakes_2026-05#^Q19929]] 高钾宽 QRS / sine wave
  - [[mistakes/uworld-mistakes_2026-05#^Q4454]] Digoxin 中毒（鉴别用，digoxin 不增宽 QRS）
  - （等积累 Brugada / CCB 中毒各 1-2 道补锚点）
- 📚 主笔记：
  - [[完整笔记/Peixuan分科笔记/心内]]（心律失常 / ECG）
  - [[完整笔记/Peixuan分科笔记/肾脏]]（高钾）
- 🏥 跨学科：
  - [[完整笔记/专题笔记/心内/心内_代谢性ECG改变]]（ECG→病因 全景，宽 QRS 是其中一行）
  - [[完整笔记/专题笔记/心内/心内_QT间期长短与TdP]](TCA 同时长 QT / 高钾同时 short QT)
  - [[完整笔记/专题笔记/肾脏/肾脏_高钾血症完整体系]](高钾 ECG 深度 + 急救)
  - [[完整笔记/专题笔记/心内/心内_Vaughan_Williams抗心律失常药]](IC 类钠通道阻断同机制)
  - [[完整笔记/专题笔记/USMLE/USMLE_重金属中毒对照铅砷汞铁]](中毒解毒对照思路)
- 🌱 TODO：
  - ✅ TCA 过量错题已接入（[[mistakes/uworld-mistakes_2026-06#^Q4487]]）
  - 等收齐 **Brugada（coved ST / 发热诱发）** 错题 → §1.4 补锚点
  - 等收齐 **CCB vs BB 中毒（血糖方向）** 错题 → §1.3 补锚点

## ✅ 复盘行动

- [ ] 默写宽 QRS 四问（R aVR→TCA / T高尖→高钾 / Brady+高血糖→CCB / coved ST→Brugada）
- [ ] 默写四个解毒：碳酸氢钠 / 钙 / 钙+胰岛素 / ICD
- [ ] 默写 TCA 危险阈值（QRS>100 风险，>160 室速）
- [ ] 默写 BB vs CCB 血糖方向（BB 低 / CCB 高）+ 解药（glucagon vs 钙）
- [ ] 默写 Brugada 诱发因素（发热 / 钠通道阻断药 / 夜间迷走）

---

## 版本记录

- **v1**（2026-06-11）：四病因鉴别（TCA / 高钾 / CCB / Brugada）+ 对应解毒；含 CCB"主征非宽 QRS"纠偏（核心是 Brady+低压+高血糖）+ 钠通道阻断家族（TCA/IC/可卡因/Brugada）串联。
- **v1.1**（2026-06-11）：补全药名中英双语（葡萄糖酸钙 calcium gluconate / 胰高血糖素 glucagon / 维拉帕米 verapamil / 地尔硫卓 diltiazem / 异丙肾上腺素 isoproterenol / 奎尼丁 quinidine / 氟卡尼 flecainide / 苯海拉明 diphenhydramine / 脂肪乳 lipid emulsion / 沙丁胺醇 albuterol），遵守 [feedback_bilingual_disease_drug]。
- **v1.2**（2026-06-11）：§1.4 补"电风暴"折叠详解块（电风暴定义 + Brugada phase 2 折返机制 + isoproterenol 从下顶/quinidine 从上压 的一推一拉 + ICD 仍为根本治疗的优先级）。
