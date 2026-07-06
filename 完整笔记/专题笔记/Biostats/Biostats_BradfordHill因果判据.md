---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-07-06
type: 专题笔记
---

# Bradford Hill 因果判据（Bradford Hill criteria）

> [!info] 一句话定位
> **相关（association）≠ 因果（causation）**。观察性研究只能证明相关；要从相关推向因果，需要用 **Bradford Hill 因果判据** 逐条加权。NBME 常给你其中**一条特征**（最爱 dose-response / 剂量反应），让你叫出它的名字。

---

## 一、为什么需要这套判据

```
observational study 观察性研究
  ↓
只能证明 X 与 Y 相关（correlation）
  ↓
无法单独证明 X → Y（causation）
  ↓
用 Bradford Hill 判据「加分」
  ↓
满足越多条 → 因果越可信
```

> [!warning] 核心陷阱
> 题干常强调 "**500 studies over 50 years**" 或 "关联很稳定"，诱你答"已经证明因果"。**证据再多、样本再大，只要是 observational，就不能单靠它宣判因果**。这些描述本身也不是某条判据的名字——先看它给的是**哪一条特征**。

---

## 二、9 条判据（Hill's 9 criteria）

| 判据 (英) | 中文 | Stem 触发词 |
|---|---|---|
| Temporality | 时序（因在果前）| exposure precedes disease |
| Strength | 关联强度 | 高 RR / OR |
| Dose-response (biologic gradient) | 剂量反应 | 暴露越多、风险越高 |
| Consistency | 一致性 | 多个研究/人群结果一致 |
| Specificity | 特异性 | 一因对一果 |
| Biologic plausibility | 生物学合理性 | 有机制可解释 |
| Coherence | 连贯性 | 与已知病理不矛盾 |
| Experiment | 实验证据 | 去除暴露后风险下降 |
| Analogy | 类比 | 类似暴露有类似效果 |

> [!tip] 三金刚优先
> 考试里出现频率最高的三条：**Temporality（时序）+ Dose-response（剂量反应）+ Strength（强度）**。见题先在这三条里对号入座。
> - **Temporality 是唯一「必须满足」的**——因必须在果之前，否则谈不上因果。

---

## 三、本题考点 — Dose-response（剂量反应）

> [!success] 判定钥匙
> "**increased risk correlates with number of cigarettes smoked daily**" = 暴露量与结局**同步单调上升** → **dose-response relationship（剂量反应关系）**。
>
> 这是最"像因果"的一条：随机误差/单纯混杂很难制造出漂亮的单调梯度。

```
more cigarettes per day 吸得越多
  ↓
higher cardiovascular risk 风险越高
  ↓
exposure ↑ and outcome ↑ 同步单调
  ↓
= dose-response（剂量反应）
```

> [!danger] 干扰项拆解
> | 干扰项 | 为什么错 |
> |---|---|
> | Temporal relationship 时序 | 题目没强调"暴露在结局之前"这个时间箭头 |
> | Biologic plausibility 生物学合理性 | 需要给「机制解释」，本题给的是量效数据不是机制 |
> | Consistency 一致性 | 描述的是「500 项研究都一致」这类背景，不是本题问的那条 |
> | "已证明因果" | observational 单独永不成立 |

---

## 四、复习题

> [!question]- 观察性研究里，哪一条 Hill 判据是「必须满足」的？
> **Temporality（时序）**——暴露必须发生在结局之前，否则因果无从谈起。其余各条是"加分项"。

> [!question]- Stem 说"每天吸烟支数越多，心血管风险越高"，问符合哪条因果判据？
> **Dose-response relationship（剂量反应 / biologic gradient）**。暴露量与结局同步单调上升是最强的因果线索之一。

> [!question]- "500 项观察性研究、跨 50 年都显示相关"能否证明因果？
> **不能**。无论证据量多大，纯 observational 设计不能单独证明因果；这也不等于任何单一 Hill 判据被满足。

---

## 🔗 关联

- 🔁 错题：待补
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
- 🏥 跨学科：所有 EBM / 药物流行病学题都先分「关联 vs 因果」，观察性数据只提示、RCT 才能证因果。
- 🌱 反链：[[NBME/nbme-records/NBME 11/NBME11A_S1_breakdown#^Q009]]
  - 相关专题：[[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]（铁律 ④ 详列 Hill 9 准则）
