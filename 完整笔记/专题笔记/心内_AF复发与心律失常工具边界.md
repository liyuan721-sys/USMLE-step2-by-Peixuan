---
tags:
  - USMLE-Step2
  - 心血管
  - 专题笔记
created: 2026-05-18
type: 专题笔记
source: 2026-05-18 Claude.ai 草稿 v2 整合（触发错题 Q21530）
---

# AF 复发管理 + 心律失常诊断工具适用边界

> [!info] 笔记定位（v2）
> 整合三块相互关联的高频考点：
> 1. **AF 复发的可逆病因筛查清单**（为什么单纯 cardioversion 不够）
> 2. **心律失常诊断/操作工具的适用边界**（CSM / Adenosine / Atropine / EPS — 各自能做什么、不能做什么）
> 3. **AV block 定位**（nodal vs infranodal — Atropine 反应是关键判断点）+ MI 部位 vs AV block 对应规律（不是 100% 固定）+ 非 MI 病因（Lyme / 退行性 / 先天性等）+ 实战判断流程
>
> **触发错题**：[[mistakes/uworld-mistakes#^Q21530]]（AF 复发 + BMI 35，误选 CSM "定位起搏点"）

---

## 目录

- [[#Part 1. AF 复发 — 可逆病因筛查|Part 1. AF 复发可逆病因筛查]]
- [[#Part 2. 心律失常诊断/操作工具 — 适用边界|Part 2. 工具适用边界]]
- [[#Part 3. AV Block 定位 — Atropine 反应判断|Part 3. AV Block 定位决策]]
- [[#Memory Hooks|Memory Hooks]]
- [[#自测题|自测题]]
- [[#关联|关联]]

---

## Part 1. AF 复发 — 可逆病因筛查

### 1.1 临床场景

**Trigger 模式**：
- Paroxysmal AF 复发（cardioversion 后又发）
- 常规 workup（echo / 电解质 / TFT）阴性
- 没有明显急性诱因

→ 不要继续重复 cardioversion，要找**可逆的潜在病因**。

### 1.2 必查清单（USMLE 高频）

| 病因 | 筛查 | Stem 提示 | 干预 |
|---|---|---|---|
| **OSA** ⭐ | Sleep study (PSG) | **BMI ≥30**, snoring, daytime fatigue | CPAP + 减重 |
| Hyperthyroidism | TSH | Weight loss, tremor, heat intolerance | 抗甲状腺药 / RAI |
| Alcohol | History | "Holiday heart" / binge | 戒酒 |
| HTN | BP monitoring | LVH on echo | 降压 |
| Valvular (Mitral Stenosis) | Echo | Diastolic murmur | 瓣膜修复 |
| HFpEF | Echo (diastolic dysfunction) | DOE, edema | 减重 / 利尿 |
| PE（急性诱发）| CTPA, D-dimer | Chest pain, syncope, hypoxia | 抗凝 |
| Pheo（罕见）| Plasma metanephrines | Episodic HTN + headache + sweating 三联征 | 切除 |

### 1.3 OSA 促 AF 的机制

```
        肥胖 (BMI 35) + 上气道软组织松弛
                       ↓
              夜间反复气道塌陷 = OSA
                       ↓
        ┌──────────────┴──────────────┐
        ↓                              ↓
  Nocturnal hypoxemia          Nocturnal hypoventilation
        ↓                              ↓
  ↑ Sympathetic tone           Hypoxic pulmonary
  (慢性交感↑)                   vasoconstriction
        ↓                              ↓
  ↑ Atrial automaticity        ↑ Pulmonary artery pressure
  (心房自律性↑)                 ↓
        ↓                       Right atrial dilation
        └──────────┬────────────────┘
                   ↓
        Atrial remodeling (结构 + 电重构)
                   ↓
        AF 复发 / 持续
```

> [!tip] 一句话锁定
> **AF 复发 + BMI ≥30 + 常规检查阴性 → Sleep study**

---

## Part 2. 心律失常诊断/操作工具 — 适用边界

### 2.1 核心对照表

| 工具 | 适用 | 机制 | ❌ 不适用 / 陷阱 |
|---|---|---|---|
| **Carotid Sinus Massage (CSM) / Vagal** | AVNRT, AVRT（规则窄 QRS SVT）；房扑揭示 F 波 | ↑迷走 → ↑AV 阻滞 | ❌ AF（已不规则）；❌ 不定位起搏点 |
| **Adenosine 6 mg IV** | AVNRT 一线终止；房扑揭示 F 波；宽 QRS 鉴别 SVT vs VT | 短暂完全 AV 阻滞 | ❌ AF；❌ 不定位起搏点；哮喘/COPD 慎用 |
| **Atropine 0.5 mg IV** | 症状性 bradycardia；症状性 AV block；**鉴别 nodal vs infranodal** | 抗迷走 → ↑SA 放电 + ↑AV 传导 | ❌ AF（反而加速室率）；❌ 不定位起搏点 |
| **EPS (electrophysiology study)** | **精确定位起搏点 / mapping 折返环 / 消融** | 心内电极标测 | 创伤性，难治 SVT/VT 才用 |

### 2.2 易混三连击（USMLE 高频陷阱）

#### 陷阱 1：CSM 用在 AF 上

> [!tip] 口诀锁定 — **"CSM 治 R 不治 I"**
> **R**egular SVT 有用，**I**rregular AF 没用。
>
> **适用（Regular 节律）**：
> - AVNRT / AVRT 终止（规则窄 QRS SVT 的一线非药物试验）
> - 揭示**房扑 F 波**（延缓 AV 传导让 F 波"裸露"出来）
> - 宽 QRS 鉴别 SVT with aberrancy vs VT（SVT 可中断、VT 不变）
>
> **不适用 / 陷阱（Irregular 节律）**：
> - ❌ **AF**（已是不规则乱搏，CSM 毫无诊断 / 治疗价值）— Q21530 的核心错点
> - ❌ **不定位起搏点**（CSM / Adenosine / Atropine 都不是 GPS；只有 **EPS** 能精确 mapping）
>
> **机制**：刺激颈动脉窦压力感受器 → ↑迷走张力 → ↑AV 阻滞（延缓房室传导）。
>
> "CSM 可以区分起搏点位置吗？" — **不能**。它的作用只是**延缓 AV 传导**，让规则节律的折返环或 F 波"暴露"出来。

#### 陷阱 2：Atropine 用来"定位起搏点"
> "Atropine 是不是有定位功能？" — **不是定位起搏点**。
> Atropine 唯一接近"定位"的用途 = **鉴别 AV block 的阻滞位置**（nodal vs infranodal），见 Part 3。

#### 陷阱 3：把 SVT 诊断流程套到 AF 上
> AF 一旦确诊，问题层级就变了：不再是"诊断什么心律失常"，而是"如何长期管理 / 找可逆病因"。
> 看到 AF + 复发 → 思路立刻切到 **Part 1 的可逆病因清单**。

### 2.3 操作选择决策树

```
                    心律失常?
                       ↓
        ┌──────────────┴──────────────┐
        ↓                              ↓
   规则节律                        不规则节律
        ↓                              ↓
   窄 QRS SVT?                      AF / Aflutter (变传导)
        ↓                              ↓
   是 → CSM / Adenosine            → 不用 CSM/Adenosine
        - 终止 AVNRT                  → Rate control (β/CCB)
        - 揭示房扑 F 波                → 抗凝 (CHA₂DS₂-VASc)
        - 鉴别 SVT vs VT (宽 QRS)      → 找可逆病因 (Part 1)

   慢心律? (Brady/AV block)
        ↓
   症状性 → Atropine 0.5 mg
        ↓
   有效? → Nodal (良性, 观察)
   无效? → Infranodal (危险, TCP → 永久起搏器)
```

---

## Part 3. AV Block 定位 — Atropine 反应判断

> [!info] 与 [[完整笔记/专题笔记/心内_AV_Block完整鉴别]] 的分工
> - **那一份**：5 种 AV block 的 ECG 识别（PR 模式 / QRS 宽度 / 漏拍前后比较 / UWorld 原图）— "看图分类型"
> - **本节**：用 Atropine 反应 + MI 部位 + 非 MI 病因来**定位**（nodal vs infranodal）+ 决策起搏器 — "拿什么治"

### 3.1 解剖基础

```
        SA node
            ↓
        心房
            ↓
    ━━━━━━━━━━━━━━━━━━━ 受迷走支配
            ↓
        AV node ◄── Nodal (结上)
            ↓
    ━━━━━━━━━━━━━━━━━━━ 不受迷走支配
            ↓
        His bundle
        Bundle branches  ◄── Infranodal (结下)
        Purkinje fibers
            ↓
        心室
```

**关键事实**：
- AV 结 = **迷走密集分布**（副交感支配）
- His-Purkinje = **几乎无迷走支配**

### 3.2 Nodal vs Infranodal 对照

| 特征 | Nodal (AV 结) | Infranodal (His 以下) |
|---|---|---|
| **类型** | 1° AVB, Mobitz I (Wenckebach) | Mobitz II, 3° 高位完全 AV block |
| **QRS escape** | **窄** (junctional 40-60 bpm) | **宽** (ventricular 20-40 bpm) |
| **PR 模式** | 渐进延长后漏搏 | 突然漏搏（PR 固定）|
| **诱因** | **下壁 MI** (RCA → AV 结缺血), ↑迷走 (运动员) | **前壁 MI** (LAD → His 缺血), 退行性传导病 |
| **Atropine 反应** | ✅ 改善（迷走支配可解除）| ❌ 无效甚至恶化 |
| **预后** | 良性，多自限 | **危险，进展 → 起搏器** |
| **治疗** | 观察 / 治病因 | TCP → **永久起搏器**（即使后续恢复也装） |

### 3.3 为什么 Atropine 对 Infranodal 会恶化

```
        给 Atropine (抗迷走)
              ↓
        SA 放电↑ → 心房率从 60 → 100
              ↓
        但 His-Purkinje 已损伤，传不动这么多冲动
              ↓
        房室传导比例 2:1 → 3:1 或 4:1
              ↓
        心室率反而下降 ⚠️
```

> [!danger] 临床教训
> 怀疑 infranodal 时**不要依赖 atropine**，直接经皮起搏 (TCP) + 备永久起搏器。

### 3.4 高频题型

#### 题型 A：下壁 MI + AV block
> 65 岁男性，急性下壁 STEMI，3° AV block，HR 38，**窄 QRS escape 45**。给 atropine → 心率↑80，传导恢复。
>
> **诊断**：Nodal（RCA 供应 AV 结 90%）
> **处理**：Atropine, 通常自限，**不**需永久起搏器

#### 题型 B：前壁 MI + AV block
> 70 岁男性，急性前壁 STEMI，Mobitz II，HR 35，**宽 QRS escape**，atropine **无反应**。
>
> **诊断**：Infranodal（LAD → His 缺血）
> **处理**：立刻 TCP → **永久起搏器**（即使后续恢复也装）

#### 题型 C：运动员迷走过强
> 25 岁运动员，HR 45，1° AVB，PR 220 ms，**窄 QRS**，无症状。
>
> **诊断**：迷走张力高 → Nodal
> **处理**：观察，不治疗

### 3.5 冠脉解剖 — 为什么下壁/前壁 MI 对应不同 block

| 传导系统部位 | 主要血供 |
|---|---|
| SA node | RCA (~60%) / LCx (~40%) |
| **AV node** | **RCA (~90%)** / LCx (~10%) ⭐ |
| **His 束 + 束支** | **LAD (septal branches)** + 少量 RCA |
| Purkinje | 心内膜下，双重供应 |

```
        RCA (下壁 MI)               LAD (前壁 MI)
            ↓                            ↓
        供应 AV 结                   供应 His + 束支
            ↓                            ↓
        AV 结缺血                    His-Purkinje 缺血
            ↓                            ↓
        Nodal block                  Infranodal block
        窄 QRS, atropine 有效        宽 QRS, atropine 无效
        多自限                       需起搏器
```

### 3.6 对应规律 — 强倾向但**不是 100% 固定** ⚠

> [!warning] USMLE 默认规律
> - 下壁 MI + AV block → **默认 nodal** → atropine + 观察
> - 前壁 MI + AV block → **默认 infranodal** → 起搏器
>
> 但 ECG (QRS 宽度) + Atropine 反应才是**金标准**，MI 部位只是先验概率。

**三类例外**：

**例外 A**：大面积下壁 MI 偶尔造成 infranodal（累及间隔下部 / RCA+LCx 双病变）→ 按 ECG + atropine 反应处理

**例外 B**：前壁 MI 的 AV block 罕见为 nodal 起源，但**临床原则**：前壁 MI 出现的任何 AV block 都倾向于装永久起搏器（His 受损隐患极高）

**例外 C**：非 MI 病因

| 病因 | 倾向位置 | Stem 关键词 |
|---|---|---|
| **退行性传导病** (Lenegre / Lev) | Infranodal | 老年人，无 MI，渐进出现 |
| **迷走过度** | Nodal | 运动员、夜间、Valsalva |
| **药物** (β-blocker, CCB, digoxin, amiodarone) | Nodal | 用药史 |
| **Lyme 病** ⭐ | Nodal | **年轻人 + tick exposure + erythema migrans + 高位 AV block** |
| **结节病、淀粉样变** | Infranodal | 浸润性疾病侵及 His-Purkinje |
| **先天性 3° AVB** | Nodal（位置高）| 母亲 SLE / **抗 SSA (Ro) 抗体** |
| **主动脉瓣置换术后** | Infranodal | 手术机械损伤 His |

### 3.7 实战判断流程（不要只看 MI 部位）

```
              AV block 患者
                   ↓
        ECG: escape rhythm QRS 宽度 ⭐
                   ↓
        ┌──────────┴──────────┐
        ↓                      ↓
   窄 QRS (40-60)         宽 QRS (20-40)
   junctional escape      ventricular escape
        ↓                      ↓
   倾向 Nodal             倾向 Infranodal
        ↓                      ↓
   验证: atropine         验证: atropine
        ↓                      ↓
   有效 → 确认 Nodal      无效 → 确认 Infranodal
        ↓                      ↓
   良性，观察 / 治病因    危险，TCP → 永久起搏器
```

> [!tip] USMLE 命题哲学
> 题目通常把所有线索**对齐**（部位 + QRS + atropine 三个都指向同一答案）。
> 偶尔"反着出"考鉴别：**以 ECG 和 atropine 反应为准，不是 MI 部位**。

---

## Memory Hooks

> [!success] 核心口诀
> 1. **"BMI ≥30 + AF 复发 + 常规检查正常 → 闭眼选 Sleep Study"**
> 2. **"CSM 治 R 不治 I"**：Regular SVT 有用，Irregular AF 没用
> 3. **"Atropine 是油门，不是 GPS"**：能治 brady，但不定位起搏点；唯一"定位"用途 = AV block 的 nodal/infranodal
> 4. **"窄良宽危，下壁活前壁亡"**：窄 QRS escape = nodal = 良性；宽 QRS escape = infranodal = 危险
> 5. **"治 AF 不治 OSA = 救火不关煤气"**：cardioversion 治标，找可逆病因才治本
> 6. **"部位是概率，ECG + atropine 是金标准"**：下壁→nodal、前壁→infranodal 只是先验，QRS 宽度 + atropine 反应才能确诊

---

## 自测题

> [!question]- Q1：60 岁男性，BMI 32，paroxysmal AF cardioversion 后 3 周复发。Echo / TFT / 电解质均正常，无 chest pain，daytime O2 98%。下一步？
> *（先写答案再展开）*

> [!question]- Q2：急性前壁 STEMI 患者出现 3° AV block，escape rhythm 宽 QRS 30 bpm，atropine 无反应。下一步？
> *（先写答案再展开）*

> [!question]- Q3：CSM 在以下哪些场景中有用？(多选)
> a) 终止 AVNRT
> b) 终止 AF
> c) 揭示房扑 F 波
> d) 定位异位起搏点（junctional vs 远端）
> e) 鉴别规则窄 QRS SVT 类型
> *（先写答案再展开）*

> [!question]- Q4：下壁 STEMI 患者出现 Mobitz I AV block，HR 42 有症状。给 atropine 后心率↑80 且传导恢复 1:1。这说明阻滞位置在？预后？
> *（先写答案再展开）*

> [!question]- Q5：22 岁男性，最近露营回来后出现疲劳和心悸，ECG 示 3° AV block，HR 40，**窄 QRS**。右下肢有环形红斑。最可能病因？阻滞位置？
> *（先写答案再展开）*

> [!question]- Q6（反着出鉴别）：72 岁男性，急性**下壁** STEMI，出现 3° AV block，HR 28，**宽 QRS escape**，atropine 无反应。下一步？为什么不按"下壁→nodal→atropine"处理？
> *（先写答案再展开）*

---

## 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes#^Q21530]] AF 复发筛 OSA + CSM/Atropine 适用边界（2026-05-18 触发本笔记）
  - 等积累后续：AVNRT 急性处理 / 房扑揭示 F 波 / 下壁 vs 前壁 MI + AV block / Lyme carditis 等
- 📚 主笔记：
  - [[完整笔记/Peixuan分科笔记/心内]] §AF + §AV block 章节
  - [[完整笔记/专题笔记/心内_AV_Block完整鉴别]] — AV block 5 类 ECG 识别（PR/QRS 模式 + UWorld 原图）
  - [[完整笔记/专题笔记/心内_抗凝抗板_急性血栓]] §E.2 AFib 长期抗凝（评分驱动抗凝面 + Trigger vs Substrate + Holiday Heart）
- 🏥 跨学科：
  - [[完整笔记/Peixuan分科笔记/pulmonary]]（OSA = AF 最重要可逆病因）
  - [[完整笔记/Peixuan分科笔记/endocrine]]（甲亢 → AF；Pheo 三联征）
  - [[完整笔记/Peixuan分科笔记/感染]]（Lyme carditis → 高位 AV block，年轻人 + 蜱叮咬 + 环形红斑）
- 🌱 TODO（待扩充本笔记 / 拆出衍生）：
  - 等积累 3-5 道 SVT 急性处理题（AVNRT / AVRT / 房扑变传导）→ 扩展 §Part 2 工具适用边界
  - 等积累 2-3 道非 MI 病因 AV block（Lyme / Lenegre-Lev / 主动脉瓣术后）→ 在本笔记 §3.6 例外 C 加详细鉴别 SOP
  - 等积累 AF rate vs rhythm 抉择题 → 在本笔记 Part 1 加 §1.4 长期管理决策（抗凝 + rate 优先 vs rhythm 时机）
