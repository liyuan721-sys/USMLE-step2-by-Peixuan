---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-05-24
type: 专题笔记
---

# Biostats_OR / CI / 因果 三连陷阱（Case-Control + 关联 vs 因果 + Bradford Hill）

> [!info] 一句话定位
> USMLE 在 case-control 的 OR 题里**同时埋 3 个陷阱在 5 个选项里**：① **方向反**（"X compared to Y" → 弄反 X 是暴露还是 reference）② **risk vs odds**（case-control 无分母不能算 risk）③ **关联 ≠ 因果**（CI 不含 1 = 统计显著关联，不是 causality）。用户**同主题 3 次反复错**（2026-05-10 Q20227 + 2026-05-23 浩斯宾 Q22 + 2026-05-24 浩斯宾 Q20）→ 强制衍生。

> [!warning] 三次反复错家族
> | 次数 | 日期 | 错点角度 | 选 | 正解 |
> |---|---|---|---|---|
> | 1 | 2026-05-10 | 方向 + risk/odds 角度 | "NHW 是 Black 的 3 倍" (D) | "Black odds 是 NHW 3.07 倍" (C) |
> | 2 | 2026-05-23 浩斯宾 Q22 | CI ≠ causality 角度 | "CI 不含 1 → causality" (E) | "Black odds 是 NHW 3.07 倍" (C) |
> | 3 | 2026-05-24 浩斯宾 Q20 | 又回到 risk/odds 角度 | "risk 3.07 倍" (A) | "Black odds 是 NHW 3.07 倍" (C) |

---

## 一、四条铁律（USMLE 出题最常考的 4 个钉子）⭐

```
═══════════════════════════════════════════════════════════════
铁律 ①：方向 — "X compared to Y" → X 是暴露，Y 是 reference
铁律 ②：测量 — Case-control 只能算 OR，不能算 risk / RR（无分母）
铁律 ③：CI — CI 不含 1 = 统计显著关联（非偶然）≠ 因果
铁律 ④：因果 — 需 Bradford Hill 9 准则 + 排除偏倚 / 混杂 / 反向因果
═══════════════════════════════════════════════════════════════
```

> [!tip] 反射顺序（USMLE 考场看到 OR 题）
> 1. **圈出 "X compared to Y"** → X 是暴露
> 2. **看研究设计** → case-control 看到"risk"立刻警惕
> 3. **看 CI** → 含 1 = 不显著，不含 1 = 显著（**不等于因果**）
> 4. **看是否有 adjusted OR** → 仍显著 = unmeasured confounders / 完全到 1 = 完全由 confounders 解释

---

## 二、铁律 ① — OR 方向（"X compared to Y" 暴露在前）

### 钉死规则
- **OR 计算公式**：OR = (暴露组 odds of outcome) / (reference 组 odds of outcome)
- **OR > 1** → 暴露组 odds 高于 reference（关联）
- **谁是暴露 / 谁是 reference 看 stem 措辞**：
  - **"X compared to Y"** → **X 是暴露**，Y 是 reference
  - **"Y vs X"** → 一般还是 Y 是参照（先写的是数据组）
  - **"odds of [outcome] in X relative to Y"** → X 暴露 / Y reference

### 经典反向陷阱（USMLE 高频）
```
Stem：Black women compared to non-Hispanic White (NHW) women,
      adjusted OR for pregnancy-related death = 3.07 (95% CI 1.85-5.10)

✅ 正确解读：Black 是暴露，NHW 是 reference
            → Black 的死亡 odds 是 NHW 的 3.07 倍

❌ 钓饵陷阱：把先出现的 NHW 当主语（顺读习惯）
            → 误读 "NHW 是 Black 的 3.07 倍"（方向反）
```

### 反射钩
**"X compared to Y" → X 在前 = X 是暴露**。看到 OR 题第一动作 = **圈出 X 和 Y**，箭头标"X→暴露 / Y→reference"。

---

## 三、铁律 ② — Case-Control 只能算 OR，不能算 risk

### 钉死规则
| 研究设计 | 可以算的关联指标 | 不能算的 |
|---|---|---|
| **Cohort（前瞻）** | RR（risk ratio）/ OR / IR / HR | — |
| **Case-control（回顾）** | **OR**（仅此）/ exposure odds ratio | ❌ **不能算 RR / risk / cumulative incidence** |
| **Cross-sectional（横断）** | Prevalence ratio / OR | ❌ 不能算 incidence / risk（无时间维度）|
| **RCT** | RR / RD / NNT / HR | — |

### 为什么 case-control 不能算 risk？
- **risk = (患病人数) / (total 暴露人数)** — 需要"暴露人群的总分母"
- Case-control **从结局倒推暴露**：先选 cases + controls（结局已固定），再回顾暴露状态
- → 没有"total exposed"的分母 → 无法算 risk
- → 只能比较 cases 中暴露 odds vs controls 中暴露 odds = **OR**

### USMLE 钓饵
- 选项里说 **"risk of X is 3 times higher"** + 题干是 **case-control** → **立刻警惕**
- 这是 USMLE 测你是否分得清 study design ↔ 可算指标

### 反射钩
**"Case-control + 选项有 'risk' = 红灯"**；OR 永远不是 risk，即使数值看起来像。

---

## 四、铁律 ③ — CI 不含 1 ≠ 因果

### 钉死规则
| CI 状态 | 统计含义 | 因果含义 |
|---|---|---|
| **CI 不含 1（OR/RR）或 不含 0（差值）** | **统计显著**（p < 0.05）| ❌ **不一定是因果** |
| CI 含 1 / 含 0 | 不显著（不能拒绝 null） | 既不证伪也不证实因果 |
| 95% CI 越窄 | 估计越精确 | — |
| 95% CI 越宽 | 样本量小 / 变异大 | — |

### 三层概念阶梯（USMLE 钓饵分层）

```
统计显著（statistical significance）
   ▲ CI 不含 1 → 是的，p < 0.05
   │
关联（association）
   ▲ 数据显示暴露与结局共同变化
   │
因果（causation）⭐ USMLE 钓你停在这层
   ▲ 需要 Hill 9 准则 + 排除偏倚 / 混杂 / 反向因果
```

### 钓饵陷阱（5-23 浩斯宾 Q22 用户踩坑）
```
Stem：adjusted OR = 3.07 (95% CI 1.85-5.10)
       → 选项 E："Because 95% CI does not include 1, causality is established"

❌ E 错在：把"统计显著"= "因果" — 跳过了"关联→因果"那一阶
✅ 正解 C："Black odds 是 NHW 的 3.07 倍"（描述关联，不上升因果）
```

### 反射钩
**"CI 不含 1 = 统计显著 ≠ 因果"**；任何说"CI/p 值 → 因果"的选项 = 钓饵划掉。

---

## 五、铁律 ④ — 因果推断需 Bradford Hill 9 准则

### 9 准则（背熟）

| # | 准则 | 含义 | USMLE 高频题 |
|---|---|---|---|
| 1 | **Strength of association（强度）** | OR/RR 越大越支持因果 | OR 10 vs OR 1.2 — 前者更强 |
| 2 | **Consistency（一致性）** | 不同人群 / 设计 / 时间得相同结果 | 多研究 meta-analysis |
| 3 | **Specificity（特异性）** | 1 暴露 → 1 结局（弱准则，多因多果常见）| 仅烟瘤 — 但弱 |
| 4 | **Temporality（时序）⭐** | **暴露在结局之前**（必要条件）| 唯一**必须满足**的准则 |
| 5 | **Biological gradient（剂量反应）⭐** | dose↑ → effect↑ | [[mistakes/uworld-mistakes_2026-05#^Q20787]] 高频考点 |
| 6 | **Plausibility（生物学合理性）** | 有合理机制 | 流行病学 + 实验室一致 |
| 7 | **Coherence（连贯性）** | 与既往知识不矛盾 | — |
| 8 | **Experiment（实验证据）** | RCT 介入证实 | 戒烟可降肺癌 = experiment |
| 9 | **Analogy（类比）** | 类似暴露有类似效应 | thalidomide → rubella 类比 |

### USMLE 三金刚（最常考）
- **Temporality**（必要）
- **Dose-response / biological gradient**（线性剂量增加 → 效应增加）
- **Strength of association**（OR/RR 大 → 不易被 confounders 完全解释）

### 反射钩
**"Bradford Hill 9 准则 / 因果推断 = Temporality + Dose-response + Strength 三金刚优先"**；看 stem 给的是哪条 → 对应选答。

---

## 六、Adjusted OR vs Unadjusted OR 解读

| 情况 | 含义 | 例子 |
|---|---|---|
| **Adj OR ≈ Unadj OR**（变化小） | 这些 confounders 没解释关联 → 真实关联 / 或有 unmeasured | Adj OR 3.0 vs Unadj 3.1 |
| **Adj OR < Unadj OR 但仍显著** | 部分由 confounders 解释 + **残留有 unmeasured** ⭐ | Adj OR 2.65 vs Unadj 3.07（[[mistakes/uworld-mistakes_2026-05#^Q20227]]）|
| **Adj OR → 1 / 失去显著** | 关联**完全由**调整的 confounders 解释 | Adj OR 1.05 (CI 含 1) |

> [!tip] USMLE 高频考点
> "Adjusted OR 仍显著 → 还有未测量的 confounders / 残余结构性因素（如 structural racism）" — 常出在种族健康差异 vignette。

---

## 七、5 个干扰项一刀切（[[mistakes/uworld-mistakes_2026-05#^Q20227]] 类）

经典 case-control + OR 3.07 (CI 不含 1) 题，5 个选项各踩什么坑：

| 选项 | 表达 | 踩的坑 |
|---|---|---|
| A | "risk 3.07 倍" | ❌ **case-control 不能算 risk**（铁律 ②）|
| B | "NHW odds = Black 3.07 倍" | ❌ **方向反**（铁律 ①）|
| **C ⭐** | "Black odds = NHW 3.07 倍" | ✅ |
| D | "race 是 causal factor" | ❌ **关联 ≠ 因果**（铁律 ④）|
| E | "CI 不含 1 → causality" | ❌ **CI 显著 ≠ 因果**（铁律 ③）|

**结论**：USMLE 的 OR 题就是用这 4 个钓饵围攻 1 个正解。**记住"四条铁律 + 5 个选项的对应错点"**，下次见同型题 0.5 秒锁 C。

---

## 八、Memory Hook

> [!success] 记忆挂钩
> - **四条铁律口诀**：**"X 在前是暴露（方向）/ Case-Ctrl 算 odds 不算 risk（测量）/ CI 不含 1 是显著不是因果（CI）/ 因果要 Hill 9 准则（推断）"**
> - **5 选 1 反射**：case-control + OR 题 → 划掉"risk" / 划掉"反方向" / 划掉"causality" / 划掉"因果由 CI 得出" → 剩下"X odds 是 Y 多少倍" = 正解
> - **类比记忆**：
>   - 方向：**"赛跑成绩 A 比 B 快" → A 是被比对象（暴露），B 是基准（reference）**
>   - 测量：**"case-control 是回头看，没分母 → 算 odds 不算 risk"**
>   - 因果：**"CI 是统计的法医（说不是巧合），不是法官（不能宣判因果）"**
> - **Hill 三金刚**：**"时序-剂量-强度"**（temporality / dose-response / strength）
> - **Adj OR 解读**：**"残留 = 未测"**（adj 仍显著 → 还有 unmeasured confounders）

---

## 九、🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes_2026-05#^Q20227]] 🔴 OR 方向 + Case-control 不能算 risk + CI ≠ causality（**3 次反复错家族源头**）
  - [[mistakes/uworld-mistakes_2026-05#^Q20787]] Bradford Hill — Dose-Response（铁律 ④ 实例）
  - [[mistakes/uworld-mistakes_2026-05#^Q20283]] Case-Control vs Cohort 场景适配
  - [[mistakes/uworld-mistakes_2026-05#^Q21248]] OR-CI 表格判读 + Confounding
  - [[mistakes/uworld-mistakes_2026-05#^Q12685]] Reporting bias（同 Biostats 偏倚谱）
  - [[NBME11_错题本#^Q061]] NBME11 甲肝暴发 case-control 选指标 = OR（**新角度：设计→可算指标**，误选 attributable risk；铁律②实例）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
- 📋 邻近笔记：[[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]] / [[完整笔记/专题笔记/Biostats/Biostats_α_β_Power]]
- 🏥 跨学科：[[完整笔记/Peixuan分科笔记/OB]]（pregnancy-related death 流行病学 / 种族差异 — [[mistakes/uworld-mistakes_2026-05#^Q20227]] 原 stem）
- 🌱 TODO：等积累 5+ 道 OR / RR / 因果推断错题 → v2 扩"adjusted vs crude 完整对照表 + Mantel-Haenszel + interaction vs confounding 区分"

---

## 十、✅ 用户行动（默写清单）

- [ ] 默写 **四条铁律**（方向 / 测量 / CI / 因果）
- [ ] 默写 **Hill 9 准则**（背完整 9 条，三金刚优先）
- [ ] 默写 **5 个选项 5 个错点对照**（case-control OR 题钓饵地图）
- [ ] **反射训练**：见 OR 题 → ① 圈"X compared to Y" → ② 圈研究设计 → ③ 圈 CI → ④ 圈"causality / risk" 钓饵
- [ ] 连对 2 道 OR 题 → 可降级 [[mistakes/uworld-mistakes_2026-05#^Q20227]] 从 🔴 回 🟡
