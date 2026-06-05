---
tags:
  - USMLE-Step2
  - Biostats
---

# 📢 USMLE 药品广告题解题策略

> 顿悟于 2026-05-11，刷 Q7708 + Q7709 (Efrenzia 双题) 后总结。
> 这类题在 NBME / UWorld 每张卷子至少 1-2 道，**技巧性极强**，掌握 SOP + 5 大陷阱基本稳拿。

---

## 🎯 识别广告题的 3 大信号

> [!danger] **遇到这些信号 → 进入广告题解题模式**
>
> 1. **视觉元素**：药品名 + ®、彩色 bar chart、绿色箭头（"减少 X%"）、品牌色
> 2. **关键短语**：
>    - "Indicated to reduce..."
>    - "RRR / 相对降幅大数字"（如 20%, 28%）
>    - "Recommended as a treatment of choice"
>    - 小字脚注、角注、"Selected safety data"
> 3. **题目问法**：
>    - "Based on the drug ad..."
>    - "Most accurate interpretation..."
>    - "How many patients need to be treated..."

---

## 📋 广告题通用解题 SOP（5 步）⭐

```
┌────────────────────────────────────────────────────┐
│  Step 1: 识别 composite endpoint（复合终点）         │
│    → 广告通常报"总效果" = 多个 outcomes 打包         │
│    → 例：CV death + MI + stroke = 一个复合终点      │
├────────────────────────────────────────────────────┤
│  Step 2: 看 RRR vs ARR 的差异（戏剧化陷阱）          │
│    → 广告永远用 RRR（看起来大）                     │
│    → 但 ARR 才是临床真实效益                        │
├────────────────────────────────────────────────────┤
│  Step 3: 找"哪个 outcome 真正驱动了差异"             │
│    → 看小字 / footnote / 解释段                     │
│    → 通常只有 1 个 outcome 显著，其他不显著          │
├────────────────────────────────────────────────────┤
│  Step 4: 查 safety data（被刻意藏起来）              │
│    → 出血、副作用通常在最后一页 / 角注 / 小字        │
│    → "Selected safety data" = 信号词               │
├────────────────────────────────────────────────────┤
│  Step 5: 区分"广告说的"vs"题目问的"                  │
│    → 广告说："Recommended as treatment of choice"   │
│    → 题目可能问："最可能减少哪个 outcome？" → 找数据 │
└────────────────────────────────────────────────────┘
```

---

## ⚠️ 广告题 5 大经典陷阱 ⭐⭐

| 陷阱 | 广告手法 | 识别方法 |
|---|---|---|
| **① RRR 夸大效益** | 用 RRR（大数字）不用 ARR（小数字）| 找 ARR 算 NNT，看真实效益 |
| **② Composite endpoint 掩盖真相** | 打包多个 outcome 报"总效果"| 找哪个 outcome **真正**驱动差异 |
| **③ Safety 藏在小字** | Bleeding / 副作用放角注 / 最后页 | **永远读完所有页 / 角注** |
| **④ "Treatment of choice" 是营销语** | "Recommended as..." | 看 guideline 来源是否利益相关 |
| **⑤ Subgroup analysis 过度解读** | "Diabetes subgroup..." | 亚组分析是 hypothesis-generating，不是结论 |

---

## 🔍 Composite Endpoint（复合终点）深度解读

### 什么是复合终点？

**Composite endpoint** = 把**多个独立 outcome 打包成一个**，任一发生即算"事件"

```
例：CV death + non-fatal MI + non-fatal stroke = 1 个复合终点
病人 A：心梗了 → 算 1 个事件 ✓
病人 B：中风了 → 算 1 个事件 ✓
病人 C：CV death → 算 1 个事件 ✓
病人 D：心梗 + 中风都有 → 算 1 个事件（只取第一次）✓
```

### 为什么 RCT 用复合终点？（有正当理由）

1. **样本量小，事件少** → 打包 ↑ 事件率 → ↑ 统计 power → ↓ 样本量
2. **临床相关** → 病人在乎"任何坏事发生"
3. **缩短试验时间 + 降成本**

### 但是 → 暗黑面：可能掩盖真相

复合终点的**总差异**必须追问："是**所有 outcomes 都贡献**，还是**只有 1 个在贡献**？"

```
总差异 = outcome 1 差异 + outcome 2 差异 + outcome 3 差异
```

### 三种典型情况

> [!success] **情况 A：均匀贡献（理想 — 真正全面效益）**
>
> | Outcome | 对照组 | 治疗组 | 差异 |
> |---|---|---|---|
> | CV death | 50 | 40 | -20% |
> | MI | 60 | 48 | -20% |
> | Stroke | 40 | 32 | -20% |
> | **复合** | **150** | **120** | **-20%** |
>
> → 药全面降低所有 CV outcomes，最强证据

> [!warning] **情况 B：单一驱动（警惕 — Efrenzia 就是这种）**
>
> | Outcome | 对照组 | 治疗组 | 差异 |
> |---|---|---|---|
> | CV death | 50 | 49 | ≈0 不显著 |
> | MI | 80 | 60 | **-25% ⭐ 唯一驱动** |
> | Stroke | 20 | 20 | 0 不显著 |
> | **复合** | **150** | **129** | "**整体 -14%**" |
>
> → 广告写"复合 -14%"，真相是**只防 MI**，不防 stroke，不延寿

> [!danger] **情况 C：相反信号（极危险 — 药害被掩盖）**
>
> | Outcome | 对照组 | 治疗组 | 差异 |
> |---|---|---|---|
> | CV death | 50 | 65 | **+30% ⚠️ 增加（被掩盖）** |
> | MI | 30 | 15 | -50% 显著 |
> | Stroke | 20 | 20 | 0 |
> | **复合** | **100** | **100** | "**无差异**" |
>
> → 广告说"复合无差异 = 安全等同"，真相是 MI 降但**死亡增加**！

---

## 🆚 Hard vs Soft Outcomes（识别复合终点质量）

| Hard outcomes（硬终点）| Soft outcomes（软终点）|
|---|---|
| Death（all-cause, CV-specific）| Hospitalization（住院）|
| MI | Revascularization（再次手术）|
| Stroke | Symptom relief（症状缓解）|
| 客观、可量化、临床重要 | 主观、可改、临床意义低 |

> [!warning] **复合里如果**硬终点 + 软终点混合 → 警惕差异来自软终点
>
> **All-cause mortality** 是最硬的硬终点，如果它没差异 → 药再多"减少 X"也要打折扣

---

## 🔬 看到 Composite Endpoint RCT 后问 6 个问题

```
1. 复合包含哪些 outcomes？（数一下，列出来）
2. 是 hard outcomes 为主，还是 soft outcomes 为主？
3. 总效果显著吗？(p < 0.05)
4. 各 component 单独看，谁显著谁不显著？⭐ 关键
5. Mortality 单独看有没有差异？
6. 有没有反方向的信号？（治疗组某 outcome 反而增加）
```

---

## 📊 广告题"读图 SOP"

> [!tip] **每看到药品广告，按顺序读 4 个区域**
>
> 1. **大标题** → 广告想让你以为药能干什么
> 2. **Bar chart + 绿箭头** → 看 RRR vs ARR 两套数字
> 3. **小字 / 角注 / footnote** → safety、subgroup limitations、p value
> 4. **最后一页** → 通常藏 safety data + guideline 来源
>
> 不要被大标题忽悠，所有区域读完再判断

---

## 🆚 广告题 vs 临床决策题（区分问法）

| 类型 | 问法 | 答题思路 |
|---|---|---|
| **广告题** | "Based on the ad..." | 基于广告数据回答（即使广告夸大）|
| **临床决策题** | "Best treatment for this patient?" | 基于真实证据 + guideline |
| **批判广告题** | "What is misleading about this ad?" | 找陷阱（RRR / composite / safety）|

---

## 🎴 Memory Hook

> [!success] **核心 3 句话**
>
> 1. **"打包数字看着大，拆开才知真相在哪一只"** 📦
> 2. **"RRR 大字骗眼睛，ARR 小字才真心"**
> 3. **"先看大标题再看小字，最后看 safety"**

---

## 📐 复合终点拆解思维框架

```
复合终点的总差异
    │
    ▼
拆开看 individual components
    │
    ├─ 谁显著？谁不显著？
    ├─ 是硬终点还是软终点显著？
    ├─ Mortality 有没有差异？
    └─ 有没有反方向信号（治疗反而害人）？
    │
    ▼
判断药的真实价值
    │
    ├─ 全面有效（情况 A，最强）
    ├─ 单一驱动（情况 B，需评估临床意义）
    └─ 相反信号（情况 C，可能害人）
```

---

## 🎯 USMLE 怎么考这个概念

> [!warning] **常见考法**
>
> 1. **直接问**：广告/摘要里 "Drug X most reduces which outcome?" → 找 individual component
> 2. **批判性问**："What is a limitation of using a composite endpoint?" → "可能由单个 component 驱动"
> 3. **图表题**：给 forest plot，让识别"哪个 component 显著"
> 4. **临床决策题**：病人主要担心 stroke，药对 stroke 无差 → 不推荐

---

## 🔗 关联

- 🔁 关联错题：
  - [[mistakes/uworld-mistakes_2026-05#^Q7708-Q7709-Efrenzia]] Efrenzia Item 1 — 复合终点拆解
  - [[mistakes/uworld-mistakes_2026-05#^Q7709]] Efrenzia Item 2 — NNT + 亚组限定
  - [[mistakes/uworld-mistakes_2026-05#^Q107183]] RRR 计算（"半步陷阱"）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
- 🌱 TODO（待生成衍生）：未来积累更多广告题后，请 Claude Code 整合 → 扩充本笔记 + 生成 [[完整笔记/专题笔记/_衍生_高频陷阱/Critical Appraisal 综合]]

---

## ✅ 复习行动

- [ ] 默写 **5 步 SOP** 和 **5 大陷阱**
- [ ] 默写 **复合终点 3 种情况**（均匀 / 单一驱动 / 相反信号）
- [ ] 默写 **6 个问题 framework**
- [ ] 找 3 道 NBME 广告题练习（关键词 "drug ad" / "promotional material"）
- [ ] 下次遇到广告题，**主动按 5 步 SOP 走**
