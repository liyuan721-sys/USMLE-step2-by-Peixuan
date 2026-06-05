---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-06-05
type: 专题笔记
version: v1.0
---

# 统计显著 vs 临床显著（Statistical vs Clinical Significance）

> [!info] 定位
> 本笔记解决一类高频 CK 陷阱：**CI 显示"统计显著"，但 effect size 太小 → 临床无意义**。
> 教学目标（First Aid / UWorld）：**"A statistically significant finding may or may not be clinically relevant."**
> 由错题 [[mistakes/uworld-mistakes_2026-05#^Q106495]] 驱动新建。

---

## 一、两个独立问题（核心）⭐

| 问题 | 答案来源 | 判定 |
|---|---|---|
| **统计显著？**（不是偶然？）| **CI / p 值** | 差值 CI 不含 **0**，或比值（RR/OR/HR）CI 不含 **1** → 显著（p<0.05）|
| **临床重要？**（差得够多值得用？）| **effect size vs 阈值（MCID）** | effect size ≥ 题给的最小临床重要差异 → 重要 |

> [!danger] 最大误区
> **"CI 不含 null"只回答统计显著，绝不回答临床重要性**。两者完全独立——必须分两步各判一次。

---

## 二、Effect size（效应量）是什么 ⭐⭐⭐

**Effect size = 效应有多大（差异 / 关联的"量级"），与样本量无关。** 它回答"差多少、值不值得在意"（= 临床重要性那一问），**不是**"是不是偶然"（那是 p / CI 的事）。

> [!info] 不是单一公式，而是一类指标 —— 按结局类型选

| 结局类型 | Effect size 指标 | 公式 / 取值 |
|---|---|---|
| **连续变量**（均数）| 组间均数差 mean difference | mean₁ − mean₂（Q106495 的 −0.05 天就是这个）|
| 连续变量（标准化）| **Cohen's d** | d = (mean₁ − mean₂) / SD_pooled |
| **二分类**（事件率）| ARR / RRR / RR / OR / HR | 见 [[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]] |
| 相关 | 相关系数 r | −1 ~ +1，越远离 0 越强 |

> 关键认知：你学过的 **ARR / RRR / RR / OR / 均数差本身就是 effect size** —— 它们衡量"效应大小"；CI / p 只衡量"是否显著"。

### Cohen's d（最常被单独叫"effect size"的那个）

把均数差用标准差"标准化"，便于跨研究比较：

```
d = (mean₁ − mean₂) / SD_pooled（合并标准差）
```

| d 值 | 效应大小 |
|---|---|
| ≈ 0.2 | small（小）|
| ≈ 0.5 | medium（中）|
| ≈ 0.8 | large（大）|

---

## 三、四种组合 ⭐

| 统计 | 临床 | 含义 | 典型场景 |
|---|---|---|---|
| 显著 | 重要 | 真正有价值 | 理想结果 |
| **显著** | **不重要** ⭐ | **大样本放大微小差异** | 本笔记重点（Q106495）|
| 不显著 | （看似大效应）| 可能 **underpowered**（n 不足）| 宽 CI、小样本 |
| 不显著 | 不重要 | 无效 | — |

> [!warning] 大样本陷阱
> 样本量足够大时，**任何微小差异都能"统计显著"**（p<0.05）。所以 p 小 ≠ 有用。
> 反之样本太小（underpowered）时，**真实的大效应也可能"不显著"**——别误判为"无效"。

---

## 四、CK 解题两步法 ⭐⭐⭐

```
第 1 步：统计显著？
   差值结局 → CI 含 0 吗？  不含 0 = 显著
   比值结局 → CI 含 1 吗？  不含 1 = 显著

第 2 步：临床重要？
   ① 找题给的临床阈值（"≥X 才算 clinically significant / MCID"）
   ② 把 effect size（含 CI 边界）换算成同一单位
   ③ effect size 是否达到阈值？达到=重要，没达到=不重要
```

> [!tip] 单位换算陷阱
> 阈值与结果单位常不同（阈值给"小时"，结果给"天"）→ **必须换算成同单位再比**。
> Q106495 实例：CI 最大边界 0.085 天 × 24 = 2.04 小时 < 3 小时阈值 → **临床不重要**（即便统计显著）。

> [!example] 实例 — 拿差值比阈值（Norelia 广告题 Q20724）
> 阈值：绝对差 **≥ 10%** 算临床显著（MCID）。6 个月"非经期盆痛"应答率 vs 安慰剂：
> 
> | 剂量 | 差值 | 97.5% CI | ① 统计（含 0?）| ② 临床（≥10%?）|
> |---|---|---|---|---|
> | 低 150 | 11 | (2–20) | 不含 0 → ✅ 显著 | 11 ≥ 10 → ✅ 显著 |
> | 高 200 | 27 | (18–36) | 不含 0 → ✅ 显著 | 27 ≥ 10 → ✅ 显著 |
> 
> 两组都"统计 + 临床都显著"。
> - **统计**：结局是**绝对差（百分点）→ null = 0**（不是比值的 1）；CI 不含 0 = 显著。
> - **临床**：把**点估计差值**比阈值 → 11、27 都 ≥ 10 → 达标。
> - **正反对照**：Q106495 差值/CI 都 < 阈值 → 临床不显著；本题差值 ≥ 阈值 → 临床显著。
> - 细节：用 **97.5% CI**（不是 95%）因为两剂量多重比较校正；逻辑不变（不含 null = 显著）。

---

## 五、Stem 反射钩

| Stem 信号 | 反射 |
|---|---|
| "≥X 才算 clinically significant / MCID 为 X" | 题在考**临床显著性**——把 effect size 换算后比 X |
| "CI 不含 0/1" + 选项有"clinically significant" | 警惕：统计显著 ≠ 临床显著，别直接选"两者都显著" |
| 超大样本 + 极小差异 + p<0.05 | "统计显著但临床不重要"的经典组合 |
| p>0.05 但看似大效应 + 小样本 | 怀疑 **underpowered**（查 n / Power），不是"无效" |

---

## 六、Memory Hook

> [!success] 记忆挂钩
> - **"CI 不含 null = 统计显著；effect size vs 阈值 = 临床显著。两步分开判。"**
> - **"p 小 ≠ 有用"**——大样本能让芝麻大差异也 p<0.05。
> - **"统计是法医（说不是巧合），effect size 是医生（说值不值得用）。"**
> - **单位对齐**：阈值给小时、结果给天 → 先换算再比。

---

## 七、🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes_2026-06#^Q106495]] 统计显著 vs 临床显著（CI 不含 0 但 effect size < 阈值）⭐ 源头
  - [[mistakes/uworld-mistakes_2026-05#^Q3941]] Null Hypothesis（CI/p 与 H₀ 基础）
  - [[mistakes/uworld-mistakes_2026-05#^Q21248]] OR-CI 表格判读（CI 含/不含 null）
  - [[mistakes/uworld-mistakes_2026-05#^Q20227]] CI 不含 1 ≠ 因果（CI 越界陷阱谱系）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
- 📋 邻近笔记：
  - [[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]（CI 不含 null 的"统计 vs 因果"阶梯 — 与本卡"统计 vs 临床"互补，构成 CI 判读双陷阱）
  - [[完整笔记/专题笔记/Biostats/Biostats_α_β_Power]]（underpowered / Power 概念）
  - [[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]]（effect size = ARR/RRR/RR 等具体指标）
- 🌱 TODO：累积 3+ 道 effect size / MCID 题 → v2 加"常见 MCID 阈值表 + underpowered 判断流程"

---

## 八、✅ 默写测试

> [!question]- 默写题 1
> 一个结果"统计显著"和"临床重要"分别由什么判定？为什么 CI 不含 null 不能说明临床重要？

> [!question]- 默写题 2
> 阈值"≥3 小时算临床显著"，结果 CI 为 −0.085 ~ −0.015 天。这个结果统计显著吗？临床重要吗？（写出换算）

> [!question]- 默写题 3
> 一个 RCT p=0.08（不显著）但点估计效应看起来很大、样本只有 30 人。最可能的问题是什么？该怎么改善？

> [!question]- 默写题 4
> 什么是 effect size（效应量）？它和 p 值各回答什么问题？连续变量结局常用哪两个 effect size 指标？

> [!question]- 默写题 5
> 写出 Cohen's d 的公式，并说出 d ≈ 0.2 / 0.5 / 0.8 分别对应 small / medium / large 中的哪个。
