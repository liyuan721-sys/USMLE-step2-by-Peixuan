---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-06-21
type: 专题笔记
version: v1
---

# 似然比 + Pretest / Posttest Probability（贝叶斯更新）

> [!info] 定位
> 本笔记聚焦 **"检查如何把怀疑程度从 pretest 推到 posttest"** 的贝叶斯逻辑 + **Likelihood Ratio (LR, 似然比)** 这个推动力。
> 是 [[完整笔记/专题笔记/Biostats/Biostats_诊断4指标动态_PPV陷阱]] 的姊妹篇：那篇讲 **Sn/Sp/PPV/NPV 静态指标**（Sensitivity 敏感度 / Specificity 特异度 / Positive Predictive Value 阳性预测值 / Negative Predictive Value 阴性预测值），本篇讲 **检查前后概率的动态更新**。
> 核心目标：解决"低 pretest 人群阳性 = 多半假阳性"、"LR≈1 检查无用"、"stress test 只在中等 pretest 做"这类 stem。

---

## 一、核心定义

| 概念 | 英文 | 含义 |
|---|---|---|
| **检验前概率** | **Pretest probability** | 做检查**之前**估计的患病概率 ≈ 该人群的 **Prevalence (患病率)** |
| **检验后概率** | **Posttest probability** | 拿到检查结果（+/−）**之后**修正的患病概率 |
| **似然比** | **Likelihood Ratio (LR)** | 一个检查结果把 pretest 推向 posttest 的"力度"|

> [!warning] "≈" 是故意的 — Pretest ≈ Prevalence，但会被个体信息修正 ⭐
> 上表写 Pretest **≈**（约等于）Prevalence，不是 **=**。区别正是 CK 高频考点：
>
> - **无任何个体线索时**（只知道"他属于这人群"）→ pretest **= prevalence**（人群基线）。
> - **一旦 stem 给症状 / 病史 / 危险因素 / 查体** → pretest 被往上/下修正，**不再等于人群 prevalence**（例：典型胸痛 + 危险因素老人，CAD pretest ≫ 人群平均；见 §3.1）。
> - **链式检查 (sequential testing)**：上一个检查的 **posttest = 下一个检查的 pretest** —— 贝叶斯可一步步叠。
>
> ```
> 人群 Prevalence
>       │  + 病史/症状/危险因素
>       ▼
>   Pretest（个体化后，已 ≠ prevalence）
>       │  + 检查结果（LR 推）
>       ▼
>   Posttest ──► 若还要做下一个检查，它就成了下一步的 Pretest
> ```
>
> 一句话：**没线索时 pretest = prevalence；有线索 / 有前一个检查结果时，pretest 被修正。**

> [!tip] 一句话本质
> **检查不给诊断，它只移动概率。** Pretest 是起点，LR 是推力，Posttest 是终点。

```
        检查结果 (+/−)
Pretest ───────────────►  Posttest
 概率          ↑              概率
        Likelihood Ratio
        (LR 在推动它)
```

---

## 二、Likelihood Ratio（似然比）公式 + 解读 ⭐

$$LR+ = \frac{Sensitivity}{1 - Specificity} \qquad LR- = \frac{1 - Sensitivity}{Specificity}$$

- **阳性结果**用 **LR+** 把概率往**上**推 → posttest ↑（用来 rule **in**）
- **阴性结果**用 **LR−** 把概率往**下**推 → posttest ↓（用来 rule **out**）

### 2.1 LR 数值锚点（CK 记这几个就够）⭐⭐⭐

| LR 值 | 对 posttest 的影响 | 临床意义 |
|---|---|---|
| **LR+ > 10** | 大幅升高 | 基本确诊（strong rule **in**）|
| LR+ 5–10 | 中等升高 | — |
| LR+ 2–5 | 小幅升高 | — |
| **LR ≈ 1** | **几乎不动** | **该检查无诊断价值（posttest = pretest）** ⭐ |
| LR− 0.1–0.5 | 小至中幅降低 | — |
| **LR− < 0.1** | 大幅降低 | 基本排除（strong rule **out**）|

> [!danger] 最常见考点：LR ≈ 1 = 废检查
> Stem 给一个检查的 **LR 约等于 1** → 不管结果阳性阴性，**posttest ≈ pretest**，概率没动 → 这个检查**对诊断毫无帮助**。识别到 LR≈1 直接选"无用 / 不改变处理"。

### 2.2 Posttest = Pretest × LR（贝叶斯相乘逻辑）⭐⭐⭐

**Posttest 由 pretest 和 LR 两个输入共同决定，缺一不可** —— 这是贝叶斯定理 (Bayes' theorem) 的核心。

| 输入 | 角色 |
|---|---|
| **Pretest** | 起点高度（病人本身多像有病；由危险因素决定）|
| **LR** | 推力大小（阳性用 LR+ 往上、阴性用 LR− 往下）|
| **Posttest** | 落点 = 两者**相乘**的结果 |

机制上是 **odds (比值) 相乘**（概率不能直接乘，转成 odds 才行）：

```
Pretest 概率 ──转odds──► Pretest odds
                              × LR
                              ▼
Posttest 概率 ◄──转回──── Posttest odds

        Pretest odds × LR = Posttest odds
```

> CK **不要求手算**此公式（偏定量是 Step 1 内容），但要懂"**乘法**"这层逻辑 —— 它解释了 §三"pretest 决定一切"。

**同一个 LR 作用在不同 pretest 上，posttest 天差地别**（这就是 §三的数学根源）：

| Pretest（起点）| × 同一 LR+ = 8（阳性）| Posttest（落点）|
|---|---|---|
| **很低**（~2%）| 往上推 | **仍偏低** → 多半假阳性 |
| **中等**（~50%）| 往上推 | **明显升高** → 推向确诊 |
| **很高**（~90%）| 往上推 | 几乎确诊（本就高）|

> [!danger] 核心洞察：强 LR 也救不回极低 pretest
> 因为是**乘法**：起点 (pretest odds) 太小，乘个大数仍然小。所以**低 pretest 人群阳性 = 多半假阳性**——不是检查不好（LR 可能很强），是**起点太低**。两个输入缺一不可。

> [!tip] 一句话锁定 + 全篇逻辑链
> **"Posttest = pretest × LR（odds 相乘）。Pretest 定起点，LR 定推力，两个一起决定落点。"**
>
> ```
> 危险因素 ──定──► Pretest ──┐
>                           ├──(贝叶斯相乘)──► Posttest（= 阳性后的 PPV）
> 检查结果 + LR ─────────────┘
> ```

---

## 三、Pretest 概率决定一切 ⭐⭐⭐（UW 最爱挖的坑）

**同一个检查、同样的 Sn/Sp/LR**，在不同 pretest 概率下意义完全不同：

```
Pretest 太低 ──► 即使阳性，posttest 仍低 ──► 多半 FALSE POSITIVE 假阳性
                                              → 不该做 / 阳性别当真

Pretest 中等 ──► 检查最有价值 ──► 能明确推向 rule in 或 rule out
                                  → 该做

Pretest 太高 ──► 即使阴性，posttest 仍高 ──► 多半 FALSE NEGATIVE 假阴性
                                              → 阴性不能排除，直接上确诊/治疗
```

| Pretest 水平 | 检查价值 | 关键陷阱 |
|---|---|---|
| **很低** | 低 | 阳性 = 多半假阳性（PPV 低）→ 不该做/别轻信 |
| **中等 (intermediate)** ⭐ | **最高** | 这才是值得做检查的人群 |
| **很高** | 低 | 阴性 = 多半假阴性 → 阴性也不能排除 |

> [!warning] CK 经典应用：心脏运动负荷试验
> Exercise stress test (运动负荷试验) 只推荐用于**中等 pretest 概率**的胸痛病人。
> - 低 pretest（无症状年轻人）→ 阳性多半假阳性，别筛。
> - 高 pretest（典型胸痛 + 多危险因素老人）→ 阴性也排除不了，直接冠脉造影 / 处理。

### 3.1 "中等 pretest" 怎么认 — 数字区间 + CAD 落地 ⭐⭐⭐

以冠心病 (CAD, Coronary Artery Disease, 冠状动脉疾病) 为例，pretest 有具体档位：

| 档位 | Pretest 概率 | 含义 | 下一步 |
|---|---|---|---|
| **低 (low)** | **< 10–15%** | 基本不像 | 别做 stress test，找别的病因 |
| **中等 (intermediate)** ⭐ | **≈ 15–85%** | 真不确定 | **做 exercise stress test** |
| **高 (high)** | **> 85–90%** | 几乎肯定 | 跳过 stress test，直接冠脉造影 (coronary angiography) / 按 CAD 处理 |

> 边界不用死记（各教材 10–90% 略有出入）；CK 考的是**"给个不确定的中年人 → 判它是中等档"**。

**怎么定 CAD 的 pretest = 年龄 + 性别 + 胸痛性质 (chest pain quality)**。胸痛三特征：① 胸骨后 ② 劳累诱发 ③ 休息/硝酸甘油 (nitroglycerin) 缓解。

| 胸痛分类 | 占几条 |
|---|---|
| **Typical angina (典型心绞痛)** | 3 条 |
| **Atypical angina (非典型心绞痛)** | 2 条 |
| **Non-anginal (非心绞痛性胸痛)** | ≤1 条 |

| Stem 画像 | Pretest 档 | 下一步 |
|---|---|---|
| 30 岁女性 + non-anginal 胸痛 | **低** | 别做 stress test |
| **50 岁男性 + atypical 胸痛** ⭐ | **中等** | **做 exercise stress test** |
| **中年女性 + typical angina** | **中等** | **做 stress test** |
| 65 岁男性 + typical angina + 糖尿病 (diabetes) + 吸烟 | **高** | 直接冠脉造影 / 按 CAD 处理 |

> [!tip] 一句话识别"中等档"
> **"中年人 + 胸痛但说不清是不是心绞痛 (atypical)" = 中等 pretest 招牌画像** → exercise stress test 黄金适应人群。
> 年轻 + 不像心绞痛 = 低（别做）；老年 + 典型心绞痛 + 一堆危险因素 = 高（直接确诊检查，stress test 阴性也信不过）。

> [!danger] CK 出题陷阱
> 题给**老年 + 典型胸痛 + 多危险因素**（高 pretest）问"下一步"→ 陷阱选 "exercise stress test"，**正解是直接冠脉造影**。高 pretest 下 stress test 阴性排除不了 = 浪费。**识别 pretest 档 = 选对下一步。**

---

## 四、Posttest probability 与 PPV/NPV 的关系 ⭐

| 检查结果 | 对应的"posttest 患病概率" | 等于 |
|---|---|---|
| **阳性后** | posttest probability of disease | **= PPV（阳性预测值）** |
| **阴性后** | posttest probability of disease | **= 1 − NPV** |

> [!tip] 串起两篇笔记
> - **Posttest(阳性) = PPV**，而 **PPV 随 prevalence (=pretest) 变化** → 低 pretest 人群 PPV 必然低 → 阳性多半假阳性。
> - 这正是 [[完整笔记/专题笔记/Biostats/Biostats_诊断4指标动态_PPV陷阱]] §二/§四 "↑Prev → ↑PPV" 的另一种说法：**pretest 就是 prevalence，posttest 就是预测值。**
> - 区别：**Sn/Sp/LR 是 tool 的固有属性**（不随 pretest 变）；**posttest/PPV 随 pretest 变**。

---

## 五、CK Stem 反射钩 ⭐

| Stem 信号 | 反射诊断 |
|---|---|
| 检查 **LR ≈ 1** | 无诊断价值，posttest = pretest，不改变处理 |
| **低患病率人群**（无症状/罕见病）阳性 + "这阳性可信吗" | posttest/PPV 仍低 → **多半假阳性** → 别当真/复查 |
| **高 pretest**（典型症状 + 危险因素）检查阴性 | 多半假阴性 → 阴性不能排除 → 直接确诊/治疗 |
| "无症状年轻人做 stress test 阳性" | 低 pretest → 假阳性 → 不该筛 |
| "中等 pretest 胸痛 + stress test 阳性" | posttest 升高 → 下一步冠脉造影 |
| 给 LR+ 很大（>10）的检查阳性 | 大幅升 posttest → 基本确诊 |
| 给 LR− 很小（<0.1）的检查阴性 | 大幅降 posttest → 基本排除 |

---

## 六、Memory Hooks（干货版）

- **"检查不给诊断，只移动概率：Pretest → (LR 推) → Posttest"** ⭐
- **"LR ≈ 1 = 废检查（posttest = pretest，没动）"** ⭐⭐⭐
- **"LR+ > 10 → rule in（确诊）；LR− < 0.1 → rule out（排除）"** ⭐
- **"低 pretest 阳性 = 多半假阳性；高 pretest 阴性 = 多半假阴性"** ⭐⭐⭐
- **"检查最值钱的人群 = 中等 pretest（intermediate）"** ⭐ — stress test 经典
- **"Posttest(阳性) = PPV；PPV 随 pretest/prevalence 变 → 所以 pretest 决定一切"**
- **"Sn/Sp/LR 是 tool 出厂属性（不随 pretest 变）；posttest/PPV 是放进具体人群用出来的结果"**

---

## 🔗 关联

- 🔁 同主题错题：
  - [[NBME/NBME11_错题本#^Q003]] 低患病率(<1%) + "我这阳性可信吗" → PPV 低（pretest 低 → 多半假阳性；误选 +LR）
  - [[NBME/NBME11_错题本#^Q073]] 胰腺癌 (pancreatic cancer) 阳性 + 患病率 1% → 低 pretest 不高危（🔴 同 Q003 反复错）
  - 待 UW / NBME 出现 LR+ / LR− 数值题、stress test pretest 题后继续回填具体 Q 锚
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]（PPV/NPV/LR 基础）
- 🏥 跨学科：
  - [[完整笔记/专题笔记/Biostats/Biostats_诊断4指标动态_PPV陷阱]]（姊妹篇：Sn/Sp/PPV/NPV 静态指标 ↔ 本篇 pretest/posttest 动态更新；posttest=PPV 是接口）
  - [[完整笔记/Peixuan分科笔记/心内]]（exercise stress test 的 pretest 选择 = 本篇 §三的临床落地）
- 🌱 TODO：
  - 累积 ≥3 道 LR / pretest 数值题后回填具体 Q 锚 + 升级数值演算例
  - 出现 ROC (Receiver Operating Characteristic, 受试者工作特征曲线) / AUC (Area Under the Curve, 曲线下面积) 实题 → 与 [[完整笔记/专题笔记/Biostats/Biostats_诊断4指标动态_PPV陷阱]] §11 协调，考虑独立 `Biostats_ROC_AUC_cutoff选择`

---

## ✅ 学习清单（建议顺序）

1. 默写 LR+ / LR− 公式（Sn/Sp 怎么组）
2. **LR 数值锚点**：>10 rule in / ≈1 无用 / <0.1 rule out ⭐⭐⭐
3. **Pretest 三档**（低→假阳性 / 中→最值钱 / 高→假阴性）⭐⭐⭐
4. **Posttest(阳性) = PPV** 的接口关系
5. Stress test "只在中等 pretest 做"的临床落地
6. Stem 反射钩 7 类
