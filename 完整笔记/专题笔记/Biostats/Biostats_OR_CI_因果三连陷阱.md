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

### 补充：从文字反推 OR 点估计（"X% greater / lower odds"）⭐

- **"X% greater odds"** → OR = **1 + X%**（"55% greater odds" → OR = **1.55**，不是 1.22）
- **"X% lower / reduced odds"** → OR = **1 − X%**（"55% lower odds" → OR = **0.45**）
- 选好点估计后用 p 值卡 CI：**p < 0.05 ⟺ 95% CI 不含 1**；若选项点估计对、但 **CI 含 1**，与"p 显著"自相矛盾 → 划掉。
- 来源 [[mistakes/uworld-mistakes_2026-06#^Q22326]]（LupMAB 狼疮肾炎广告题：55% greater odds + p=0.031 → OR 1.55 (1.01–2.31)）

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

### 3.1 对照组怎么选 — 按结局，绝不按暴露 ⭐（Q108443）

case-control **先按结局（outcome）把人分成 cases / controls**，再回头比两组的**暴露频率**。所以对照的选取必须**与暴露无关**。

| 角色 | 选取标准 | 铁律 |
|---|---|---|
| **Cases** | **有目标疾病** | 按结局选 |
| **Controls（对照）** | **无目标疾病，且不论是否暴露** | 按结局选，**绝不按暴露选** |

> [!danger] 为什么不能按暴露选对照
> - 研究目的 = 比较 cases vs controls 的**暴露频率**（暴露是待测变量）。
> - 若**预先固定对照的暴露状态**（如"只选无暴露的人当对照"）→ 破坏了这个比较 = **循环论证 / selection bias**，人为制造或抹掉关联。
> - 对照的暴露分布要能**代表源人群**（理想:对照 = "如果他们得了病、本会成为 case 的那群人"）。

> [!warning] 选项地图（Q108443 类）
> - ✅ 对照 = **无病 + 不论暴露**。
> - ❌ "有病"的人当对照（混淆 case/control 由结局定义）。
> - ❌ "无病**且**无暴露"当对照（过度限定 → 按暴露选 = selection bias）。

> [!success] Memory Hook
> **「case-control 对照 = 无病 + 不论暴露（按结局选人，绝不按暴露选）。」**
> 常与**独立变量**（年龄/性别）做 matching 控混杂，但**绝不按待测暴露** matching。

### 3.2 Case-control ↔ Cohort 镜像 + 无随访（Q21684）⭐

- **镜像**:case-control 按 **outcome** 选人 → **锁死 1 个 outcome、可查多个 exposure**;cohort 按 **exposure** 分组 → **锁死 1 个 exposure、可查多个 outcome**。
  - 钓饵:把"case-control 只能评 1 个结局"**反成**"只能评 1 个暴露"（A 型方向反）。
- **无随访**:case-control 回顾性 → **没有 follow-up** → "失访偏倚 / 测 time-to-event / 耗时昂贵" 安在它头上**全错**（那是 cohort/RCT）;case-control **快又便宜**。
- 完整镜像表 → [[完整笔记/专题笔记/Biostats/Biostats_HighYield速查总览]]（§四）。

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

### 6.1 多结局 / 多分层 OR·RR 表 / 图怎么读（Q20420 / Q22187）⭐

题给**多个结局或多个分层（三分位）× CI**（可能含 unadjusted/adjusted 两列），问"关于关联最恰当结论"。

> [!danger] 三条反射
> 1. **下结论只读 adjusted（调整）列**——它去了混杂，是"真实关联";unadjusted 全显著常是混杂制造的假象。
> 2. **显著性是"是非题"，不可排名**:看 CI **含不含 1.0** 判 yes/no，**绝不能按 RR/OR 偏离程度 / CI 宽窄说"谁更显著"**。
> 3. **"趋势 / dose-response"要每一层都显著且单调**:某一层（如中间三分位）**CI 跨 1** → **没有显著梯度**，不能说"随 X 增加而显著增加/降低"。⭐（Q22187 错点）
>
> - 典型钓饵:"hospice RR 1.84 最大 = 最显著"（按大小排）/ "随三分位显著上升趋势"（中间层跨 1 却硬说趋势）。
> - 正解套路:**逐层 / 逐结局查 CI 是否含 1**——adjusted 列里 CI 不含 1 的那（几）个 = 唯一显著关联;方向看 **baseline 是哪一层**。
> - **反向问法**:问"哪个**两组最相似 / 无差异**" → 找 **CI 含 1（HR/OR≈1）** 的那个（Q7686:major bleeding HR 0.96, CI 0.84–1.10）;**"最显著/最不同" → CI 离 1 最远且排除 1**。别只凭点估计"看着接近 1"。
> - 配套:[[完整笔记/专题笔记/Biostats/Biostats_统计显著vs临床显著]]（显著=非黑即白 vs 临床显著看效应量）。

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
  - [[mistakes/uworld-mistakes_2026-06#^Q20466]] Case-control 零假设 = OR=1（铁律②：只能 OR；做对）
  - [[mistakes/uworld-mistakes_2026-05#^Q12685]] Reporting bias（同 Biostats 偏倚谱）
  - [[NBME11_错题本#^Q061]] NBME11 甲肝暴发 case-control 选指标 = OR（**新角度：设计→可算指标**，误选 attributable risk；铁律②实例）
  - [[mistakes/uworld-mistakes_2026-06#^Q20420]] adjusted vs unadjusted + CI 含 1 → 显著性不可排名（铁律③；只读 adjusted 列）
  - [[mistakes/uworld-mistakes_2026-06#^Q108443]] Case-control 对照组 = 无病 + 与暴露无关（铁律②延伸：设计→选人逻辑）
  - [[mistakes/uworld-mistakes_2026-06#^Q12674]] 分层效应不等 = effect modification → 精准医学（vs confounding）
  - [[mistakes/uworld-mistakes_2026-06#^Q22187]] 🔴 多三分位 OR 图 — 只有 CI 排除 1 的层显著，趋势需每层显著（§6.1）
  - [[mistakes/uworld-mistakes_2026-06#^Q21684]] Case-control 镜像 — 单 outcome 多 exposure + 无随访（§3.2）
  - [[mistakes/uworld-mistakes_2026-06#^Q7686]] "两组最相似" = CI 含 1（§6.1 反向问法）
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
