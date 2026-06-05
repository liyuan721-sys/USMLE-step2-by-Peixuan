---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-06-05
type: 专题笔记
version: v1.0
---

# Study Design 决策树（观察性研究识别 + 能算什么 + 经典陷阱）

> [!info] 定位
> 整合 6 道 study design 错题（Q7688 / Q20090 / Q20283 / Q20058 / Q20435 / Q20376）+ 生态学研究（Q20503）。
> **核心目标**：① 一眼判定是哪种 design ② 知道每种 design **能算 / 不能算**什么指标 ③ 躲开 4 个经典陷阱。
> 用户 **cohort vs case-control 反复错（🔴）** —— Q20435 + Q20376 两次没反射"比较发病风险 → cohort"。RCT 分期/factorial 见 [[完整笔记/专题笔记/USMLE/USMLE_临床试验分期]]。

---

## 一、两大分类：Descriptive vs Analytic

| 类别 | 目的 | 包含 | 能否检验关联 |
|---|---|---|---|
| **Descriptive（描述性）** | **生成假设** | case report、case series、（描述型）cross-sectional、ecological | ❌ 只描述 time/place/person |
| **Analytic（分析性）** | **检验假设** | case-control、cohort、（分析型）cross-sectional、RCT | ✅ 检验 risk factor ↔ disease |

> 口诀：**"描述生成假设，分析检验假设。"** case report/series 永远是描述性（证据等级最低）。

---

## 二、核心决策树 ⭐⭐⭐

```
                         研究怎么分组 / 收集数据？
                                  │
        ┌──────────────┬──────────┴───────┬──────────────────┐
        │              │                  │                  │
   按 EXPOSURE 分    按 OUTCOME 分     同时测 exp+out      只有群体数据
        │              │                  │              (无个体记录)
        ▼              ▼                  ▼                  ▼
     COHORT        CASE-CONTROL      CROSS-SECTIONAL      ECOLOGICAL
   (算 RR/risk)   (算 OR，永远回顾)   (算 prevalence)    (人群层面关联)
        │
   ┌────┴────┐
   │         │
 结局未发生  结局已发生
 前瞻追踪    查历史病历
   │         │
PROSPECTIVE RETROSPECTIVE
```

> **唯一判定标准 = "先按什么分组"**：按 exposure → cohort；按 outcome → case-control；都不分、同时测 → cross-sectional；只有群体率 → ecological。

---

## 三、3 步判定 SOP

```
Q1：研究问 "A → B"？
    → A = exposure，B = outcome（不管 A 叫不叫 "diagnosis"）

Q2：先按什么分两组？
    ├─ 按 exposure 分 → COHORT
    │     ├─ outcome 未发生、前瞻追 → Prospective
    │     └─ outcome 已发生、查历史 → Retrospective
    ├─ 按 outcome 分 → CASE-CONTROL（always retro，算 OR）
    └─ 同时测 exp + out → CROSS-SECTIONAL（算 prevalence）

Q3：算什么指标？
    Cohort → RR / incidence ；Case-Control → OR ；Cross-sectional → Prevalence
```

---

## 四、Observational Study 五类对比表 ⭐

| 维度 | Case-Control | Cohort (Retro) | Cohort (Pro) | Cross-Sectional | Ecological |
|---|---|---|---|---|---|
| **分组依据** | Outcome（有病/无病）| Exposure | Exposure | 不分组，同时测 | 群体（无个体）|
| **方向** | 回顾找暴露 | 回顾查结局 | 前瞻追结局 | 横断 snapshot | 群体率比较 |
| **算什么** | **OR** | **RR** | **RR** | **Prevalence** | 群体层面关联 |
| **能算 incidence/risk** | ❌ | ✅ | ✅ | ❌ | ❌（个体） |
| **适用** | 罕见病、长潜伏 | 罕见暴露、多结局 | 观察性中因果最强 | 现况调查、生成假设 | 群体暴露 vs 群体结局 |
| **Stem 触发词** | "cases vs controls" | "exposed vs non-exposed, review records" | "follow up for X years" | "at one point in time" | "county/country-level data" |

---

## 五、每种 design "能算什么"（反复错核心）⭐⭐⭐

> [!danger] 用户反复错点 — 比较"发病风险"只能 cohort
> 题问 **"compare RISK of DEVELOPING disease between exposed vs unexposed"** → **cohort**（[[mistakes/uworld-mistakes_2026-06#^Q20376]]）。
> - **Case-control 不能算 risk**：从"已有病 vs 没病"倒推暴露，cases 按定义已得病 → 只能算 **OR**。
> - **Cross-sectional 不能算 risk/incidence**：无时间维度 → 只能算 **prevalence**。
> - **Ecological 不能推个体风险**：只有群体数据。

| Stem 关键词 | 选哪个 design |
|---|---|
| "risk of developing" / "incidence" / "compare exposed vs unexposed 发病" | **Cohort** |
| "cases（已有病）vs controls，回看暴露" / 罕见病 / 长潜伏期 | **Case-control** |
| "at one point in time" / prevalence / 现况 | **Cross-sectional** |
| 群体/county/国家层面的率与暴露% | **Ecological** |
| 随机分配干预 vs 对照 | **RCT**（见 [[完整笔记/专题笔记/USMLE/USMLE_临床试验分期]]）|

---

## 六、Ecological Study + Ecological Fallacy 专节 ⭐

**Ecological study**：观察单位是**群体**（county / 国家 / 地区），测群体的率与暴露%，无个体数据。

| 想下的结论 | 生态学研究能否支持 |
|---|---|
| "**人群层面**有统计显著关联"（CI 不含 null）| ✅ 可以（[[mistakes/uworld-mistakes_2026-06#^Q20503]] 正解）|
| "**某个体**风险更低/相同"（individual-level）| ❌ **Ecological fallacy（生态学谬误）** |
| "X **导致/预防** Y"（causality）| ❌ 观察性 + 群体只生成假设 |

> [!warning] Ecological fallacy
> 人群层面观察到的关联，**不代表**该人群中任一**个体**也有同样关联。选项出现 "an individual / a subject" + 数据是群体层面 → 多半是这个陷阱。

---

## 七、四大经典陷阱 ⭐

> [!danger] 陷阱地图
> 1. **Diagnosis ≠ Outcome**："diagnosis of X" 是中性词，可作 exposure（精神病诊断→AMI）也可作 outcome（吸烟→肺癌诊断）。判定看"研究问 A→B 的方向"，不被名词触发反射。
> 2. **Matched ≠ Case-Control**：matching 是控制混杂的统计手段，cohort 和 case-control **都能用**。判定 design 只看"按什么分组"。
> 3. **Retrospective Cohort ≠ Case-Control**：两者都用历史数据，但 retro cohort 按 **exposure** 分组查结局，case-control 按 **outcome** 分组查暴露。
> 4. **"比较发病风险" ≠ Case-Control**：要算/比 risk 必须 cohort（[[mistakes/uworld-mistakes_2026-06#^Q20376]]）。

---

## 八、证据等级（Evidence Hierarchy）

```
        强 ▲  系统综述 / Meta-analysis
           │  RCT（随机对照）
           │  Cohort（前瞻 > 回顾）
           │  Case-control
           │  Cross-sectional
           │  Case series / Case report  ← 仅生成假设，无对照
        弱 ▼  专家意见
```

> Case series 局限（[[mistakes/uworld-mistakes_2026-05#^Q20090]]）：**无对照组、无法检验关联、易选择偏倚** → 只能描述、生成假设。

---

## 九、Memory Hooks（干货版）

- **"判 design 只看'先按什么分组'：exposure→cohort，outcome→case-control，同时测→cross-sectional，群体→ecological。"** ⭐
- **"比'发病风险'→ cohort；case-control 只出 OR 不出 risk；cross-sectional 只出 prevalence。"** ⭐⭐⭐
- **"Diagnosis 是中性词，看 A→B 方向定 exposure/outcome。"**
- **"Matching ≠ case-control；retro cohort ≠ case-control（看分组依据）。"**
- **"群体数据推个体 = ecological fallacy；观察性推因果 = 错。"**
- **"描述生成假设（case report/series 最低），分析检验假设。"**

---

## 十、🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes_2026-05#^Q20435]] 🔴 Study Design 判定（Diagnosis≠Outcome / Matched≠Case-Control）
  - [[mistakes/uworld-mistakes_2026-06#^Q20376]] 🔴 比较发病风险 → cohort
  - [[mistakes/uworld-mistakes_2026-06#^Q20503]] 生态学研究 + ecological fallacy
  - [[mistakes/uworld-mistakes_2026-05#^Q20283]] Case-Control vs Cohort 场景适配
  - [[mistakes/uworld-mistakes_2026-05#^Q20090]] Case Series 局限 + 证据等级
  - [[mistakes/uworld-mistakes_2026-05#^Q7688]] Study Design 识别（Factorial）
  - [[mistakes/uworld-mistakes_2026-05#^Q20058]] Clinical Trial Phase III 识别
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
- 📋 邻近笔记：
  - [[完整笔记/专题笔记/USMLE/USMLE_临床试验分期]]（RCT phase I-IV + factorial 等干预性设计）
  - [[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]（case-control 只能算 OR + 关联≠因果）
  - [[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]]（RR/OR/ARR/RRR 算出来之后的指标家族）
- 🌱 TODO：累积 interaction / effect modification、survival analysis 实题 → 扩 v2

---

## 十一、✅ 默写测试

> [!question]- 默写题 1
> Study Design 3 步判定 SOP 是什么？判定 cohort vs case-control 的**唯一标准**是什么？

> [!question]- 默写题 2
> 4 类观察性研究分别能算什么指标（OR / RR / prevalence）？哪些能算 incidence？

> [!question]- 默写题 3
> 题问"比较暴露组 vs 非暴露组**发生某病的风险**"，选哪种 design？为什么 case-control 不行？

> [!question]- 默写题 4
> 什么是 ecological study？什么是 ecological fallacy？数据是 county-level 时，能下"某个体风险更低"的结论吗？

> [!question]- 默写题 5
> 解释三个陷阱：① Diagnosis ≠ Outcome ② Matched ≠ Case-Control ③ Retrospective Cohort ≠ Case-Control。
