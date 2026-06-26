---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-06-26
type: 专题笔记
---

# 生存分析 — Kaplan-Meier / Hazard Ratio / Log-rank（time-to-event 一站式）

> [!info] 这张卡解决什么
> 把 **time-to-event（到事件的时间）数据**这一族考点串成一条反射：**KM 曲线**（怎么读）→ **censoring 删失**（竖线是什么）→ **log-rank**（有没有差异）→ **Cox 回归 → HR**（差异多大）→ **HR 判读 + 天花板**（降幅=1−HR、CI 跨 1、要查 ARR/NNT）。
> 此前 HR 只作为"相对 measure"散落在 [[完整笔记/专题笔记/Biostats/Biostats_广告题_相对vs绝对measures]] §四，本卡为独立体系。

---

## 一、核心概念:Hazard（风险率）vs Hazard Ratio（HR 风险比）

| 概念 | 定义 | 一句话 |
|---|---|---|
| **Hazard（风险率/瞬时风险）** | 在某一瞬间，**尚未发生事件的人**接下来一刻发生事件的**速率** | "此刻还没出事的人，下一秒出事的快慢" |
| **Hazard Ratio（HR 风险比）** | 两组 hazard 的**比值**（治疗/暴露组 ÷ 对照组），来自 **Cox 比例风险回归** | 整个随访期"事件发生得多快"的相对比较 |

> [!info] HR 来自哪里
> **time-to-event 数据 → Kaplan-Meier（KM）曲线描述 → Cox proportional hazards regression（Cox 比例风险回归）量化 → 产出 HR**。
> HR 的独门优势:既用"**是否发生**"，又用"**何时发生**"，还能处理 **censoring（删失）**——这是 RR 做不到的。

---

## 二、HR 解读（比值，null = 1）⭐

| HR | 含义 | 降幅/升幅 = \|1 − HR\| |
|---|---|---|
| **HR = 1** | 两组速率相同 → **无差异（null）** | 0 |
| **HR < 1** | 事件更慢/更少 → **保护性（治疗有效）** | HR 0.71 → 降 **29%** |
| **HR > 1** | 事件更快/更多 → **有害** | HR 1.50 → 升 **50%** |

> [!danger] 最高频陷阱:HR 值 ≠ 降幅
> **降幅 = 1 − HR**。
> - HR **0.71** → 降 **29%**（**不是**降 71%）
> - HR **0.75** → 降 **25%**
> 干扰项最爱写"降低 75%"把 HR 值当降幅。

---

## 三、显著性判读:CI 跨 1 = 不显著（同 RR/OR）

HR 是比值 → **null = 1** → **95% CI 跨过 1.0 就不显著**（与 p>0.05 永远自洽，可互相验算）。

| HR (95% CI) | 跨 1? | 显著? |
|---|---|---|
| 0.61 (0.38–0.97) | ❌ 不跨 | ✅ 显著 |
| 0.96 (0.55–1.66) | ✅ 跨 1 | ❌ 不显著 |

> 实例:[[mistakes/uworld-mistakes_2026-06#^Q12674]] LcPUFA 分层表——lowest tertile HR 0.61 (CI 0.38–0.97) 显著驱动获益;middle/highest tertile CI 跨 1 → 无显著获益。**整体 HR 显著 ≠ 每个亚组都显著。**

---

## 四、HR vs RR vs OR（三个比值的分工）⭐⭐

| | **HR** | **RR**（相对危险度）| **OR**（比值比）|
|---|---|---|---|
| 全称 | Hazard ratio | Risk ratio | Odds ratio |
| 数据 | **time-to-event（含时间 + 删失）** | 固定时点累积风险 | odds（含 case-control）|
| 来自 | KM 曲线 / **Cox 回归** | Cohort / RCT | Case-control / logistic 回归 |
| 回答 | 全期"事件发生得**多快**" | 某时点"患病风险几倍" | "暴露 odds 几倍" |
| null | **1** | 1 | 1 |

> [!tip] 三者关系
> - **事件不常见时:HR ≈ RR ≈ OR**（数值接近）。
> - HR 独门优势 = **利用"何时发生" + 处理 censoring**;有人中途失访 / 研究结束仍无事件，RR 算不进，Cox 能。

---

## 五、Kaplan-Meier 曲线 + Censoring（删失）

```
无事件存活比例
  1.0 ┤■■■□
      │   ■■■□        □ = censored（删失）记号:小竖线
      │      ■■■■□    ■ 台阶下降 = 一个事件发生
  0.5 ┤··········■■■···· ← 降到 0.5 对应的时间 = median survival（中位生存期）
      │            ■■■□
  0.0 ┤              ■■■
      └────────────────── 随访时间 →
```

| 元素 | 含义 |
|---|---|
| **纵轴** | 无事件存活比例（survival probability）|
| **台阶下降** | 每个台阶 = 一个事件（死亡/复发/终点）|
| **竖线/记号（censored）** | 该对象**中途退出**或**研究结束仍无事件** → 信息只用到那一刻 |
| **Median survival（中位生存期）** | 曲线降到 **0.5** 对应的时间;**从曲线读，HR 不直接给** |

> [!info] Censoring（删失）一句话
> **"还没出事就离场" = censored**——不是事件、也不是无事件，是"信息到此为止"。删失让 KM/Cox 能用上不完整随访的对象。

---

## 六、Log-rank test vs Cox 回归(HR) — 分工

| 工具 | 回答 | 产出 |
|---|---|---|
| **Log-rank test** | 两条 KM 曲线**是否不同** | 只给 **p 值**（有没有差异，**不给大小**）|
| **Cox 回归** | 差异**多大** + 可校正混杂 | **HR**（+ CI + 可多变量）|

> [!success] 一句话锁定
> **「Log-rank 说有没有差异，HR（Cox）说差异多大。」**
> 想比较生存曲线"是否不同" → **log-rank**;想量化"风险比多少 / 校正混杂" → **Cox → HR**。

---

## 七、HR 的天花板（CK 干扰项重灾区）⭐

> [!warning] HR 是相对 measure，不告诉你这三样
> 1. **绝对获益**:HR 0.71 漂亮，但基线风险低时 ARR（absolute risk reduction，绝对风险降低）可能很小 → 查 **ARR / NNT（number needed to treat，需治疗人数）**（"相对放大、绝对真实"）。
> 2. **中位生存期**:从 KM 曲线读（降到 50% 的时间），**HR 不直接给**。
> 3. **比例风险假设（proportional hazards）**:HR 假设两组风险比**全程恒定**;若 **KM 曲线交叉** → 单一 HR 失真，不能用。

---

## 八、CK Stem 反射钩

| Stem 信号 | 反射 |
|---|---|
| "HR = 0.75，最恰当结论?" | 降 **25%**（≠75%）+ CI 不跨 1 才显著 |
| "复合终点 HR 0.75，降低 CV（cardiovascular，心血管）死亡 X 例?" | ❌ **复合终点不可拆** |
| "比较两组生存曲线是否不同用什么检验?" | **Log-rank test** |
| "KM 曲线上的竖线/记号是什么?" | **Censored（删失）对象** |
| "曲线降到 0.5 的时间?" | **Median survival 中位生存期** |
| "HR 显著但 ARR 很小说明?" | 相对获益大、绝对小 → 看 **NNT** |
| "KM 两曲线交叉，能用单一 HR 吗?" | ❌ **违反比例风险假设** |

---

## 九、Memory Hooks

> [!success] 记忆挂钩
> - **「HR = 比值，null = 1;降幅 = 1 − HR（0.71 → 降 29%，别当 71%）。」**
> - **「HR 来自 time-to-event;log-rank 问有没有，HR(Cox) 问多大。」**
> - **「HR 是相对脸——再漂亮也要查 ARR/NNT 的绝对脸。」**
> - **「KM 竖线 = 删失（还没出事就离场）;曲线降到 0.5 = 中位生存期。」**
> - **「KM 曲线交叉 → 比例风险假设破，单一 HR 失效。」**
> - **「事件罕见时 HR ≈ RR ≈ OR。」**

---

## 🔗 关联

- 🔁 同主题错题/做对题:
  - [[mistakes/uworld-mistakes_2026-06#^Q12674]] LcPUFA 分层 HR 表 — CI 跨 1 定位获益亚组（effect modification → 精准医学）
  - [[mistakes/uworld-mistakes_2026-06#^Q12673]] 同 vignette NNT=1/ARR（HR 的"绝对脸"）
  - [[mistakes/uworld-mistakes_2026-06#^Q21323]] HR 0.75 = 降 25% + 复合终点不可拆（做对）
  - [[mistakes/uworld-mistakes_2026-05#^Q7688]] HR 解读
  - [[mistakes/uworld-mistakes_2026-06#^Q7690]] HR 多结局判读（别下没测过的结论）
  - [[mistakes/uworld-mistakes_2026-06#^Q20420]] CI 跨 1 = 显著性是非题（同判读逻辑）
- 📚 主笔记:[[完整笔记/Peixuan分科笔记/Biostats_Master]]（分科主笔记，只读）
- 📋 邻近专题:
  - [[完整笔记/专题笔记/Biostats/Biostats_广告题_相对vs绝对measures]]（§四 HR 降幅 + 复合终点 — HR 作为相对 measure）
  - [[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]（CI 跨 null 判读 + 比值 null=1）
  - [[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]]（ARR/NNT 绝对 measure — HR 的天花板互补）
  - [[完整笔记/专题笔记/Biostats/Biostats_统计检验选择决策树]]（log-rank 在检验选择中的定位）
  - [[完整笔记/专题笔记/Biostats/Biostats_HighYield速查总览]]（§3.3 CI 无效值 + §四 研究设计 → 可算 HR）
- 🏥 跨学科:[[完整笔记/Peixuan分科笔记/hematology oncology]]（肿瘤生存曲线 / median survival / 复发风险）/ [[完整笔记/Peixuan分科笔记/心内]]（心血管复合终点 RCT）
- 🌱 TODO:积累 KM 曲线读图 / median survival / 比例风险假设破坏 实题后 → 补具体 Q 锚 + 扩"曲线交叉案例"

---

## ✅ 学习清单（建议顺序）

1. 默写 HR 定义（瞬时事件率之比，来自 Cox）+ **降幅 = 1 − HR**
2. **HR 值 ≠ 降幅**（0.71 → 降 29%）⭐
3. CI 跨 1 = 不显著（与 p 自洽）
4. HR vs RR vs OR 分工表（数据来源 + 何时近似）
5. KM 曲线四元素（台阶 / 竖线删失 / median survival / 纵轴）
6. **Log-rank（有没有）vs Cox-HR（多大）** ⭐
7. HR 三天花板（绝对获益 / median / 比例风险假设）
8. Stem 反射钩 7 类
