---
tags:
  - USMLE-Step2
  - 心血管
  - 专题笔记
created: 2026-05-16
type: 专题笔记
parent_topic: AV Block 5 类型 ECG 鉴别 + 临床情景 + 处理决策
source_错题: Q3766（Mobitz I vs II 鉴别触发）
---

# _衍生_AV Block 完整鉴别诊断

> [!info] 笔记目的
> 整合 AV block 5 种类型的 ECG 识别、临床情景、病因、处理。USMLE Step 2 CK 高频考点，**心内传导阻滞题的统一框架**。
>
> 来源错题：Q3766（Mobitz I vs II, 2026-05-16）

---

## 1. 总览：5 种 AV Block 一张表

| 类型 | ECG 核心特征 | 阻滞部位 | 临床表现 | 处理 |
|---|---|---|---|---|
| **1°** | PR > 0.20s **恒定**，无漏 | AV 结 | 无症状 | 观察 |
| **2° Mobitz I** (Wenckebach) | **PR 渐进延长** → 漏 QRS → 重置 | AV 结（近端） | 多无症状，可有漏跳感 | 观察 + 去诱因 |
| **2° Mobitz II** | **PR 恒定** → 突然漏 QRS | His-Purkinje（远端） | 乏力、晕厥、可猝死 | **永久起搏器 (PPM)** |
| **2:1 AV block** | 每 2 P 跟 1 QRS（特殊型） | 不明，需 EPS / 运动试验 | 视类型 | 视类型 |
| **3° (Complete)** | P 与 QRS **完全分离** | 任何层级 | 晕厥 (Stokes-Adams)、心衰 | **PPM**（紧急 → 临时） |

---

## 2. ECG 特征详解

### 2.1 一度 AV Block

```
   P    P    P    P
   |    |    |    |
   QRS  QRS  QRS  QRS
   ←PR→ ←PR→ ←PR→ ←PR→
   恒定且 > 0.20s，每个 P 后都有 QRS
```

> [!info] UWorld 原图 — First-degree AV block
> ![[{B72502E7-99F3-4260-896B-CEDB1EF1AA5F}.png]]
> Key features：P-P 恒定 / **PR > 0.2 s 延长** / R-R 恒定（无漏拍）

> [!tip] 一句话
> **PR 长但都传，无漏拍**

### 2.2 Mobitz I (Wenckebach)

```
   P    P    P    P     P    P    P
   |    |    |    ✗     |    |    |
   QRS  QRS  QRS         QRS  QRS  QRS
   PR:  短   长   更长  漏    短   长   更长
                          ↑
                  漏拍后 PR 重置
```

**反直觉特点**：
- PR 延长的"增量"逐渐减小（160→240→280→300→漏）
- 因此 **R-R 间期反而逐渐缩短**，漏拍处 R-R 突然延长
- ECG 显示"**grouped beating**"（成组搏动）

> [!info] UWorld 原图 — Mobitz type I (Wenckebach)
> ![[{AD4EFF9A-879F-44F5-814D-771FB55A4507}.png]]
> 病理：AV 结传导紊乱（迷走 / 药物 / 缺血 / 退化）
> Key features：恒定 P-P / **PR 渐进延长** → 漏 QRS / R-R 渐短反直觉 / 通常窄 QRS

### 2.3 Mobitz II

```
   P    P    P    P    P
   |    |    ✗    |    |
   QRS  QRS       QRS  QRS
   PR:  恒定 恒定     恒定 恒定
                ↑
        PR 不变，突然漏，无预警
```

**特点**：
- PR 间期完全恒定
- 漏拍**随机**、无规律
- QRS 常**宽**（因为阻滞在 His 下，远端传导异常）

> [!info] UWorld 原图 — Mobitz type II
> ![[{837B7F59-8DF6-4EA3-AFDB-24D04D4ADF5B}.png]]
> 病理：AV 结**以下**传导紊乱（缺血 / 年龄相关传导退化）
> Key features：**恒定 PR** / 随机漏 QRS / QRS 可窄可宽

### 2.4 3° (Complete) AV Block

```
P 波节律 (规律, 房率 80):    P  P  P  P  P  P  P  P
                            ↓        ↓        ↓
QRS 节律 (规律, 室率 35):    QRS  ─  QRS  ─  QRS
                            ↑↑↑↑↑↑↑↑↑↑↑↑↑↑↑↑
                          P 和 QRS 互不相关 (AV 分离)
                          房率 > 室率
```

**关键概念 — 逸搏 (escape rhythm)**：
当上方传导被阻断，**下方的细胞自动接管起搏**以维持心室收缩。

> [!info] UWorld 原图 — Third-degree (complete) AV block
> ![[{327FB8C2-56F8-41E2-8ECF-726C2CCD2D02}.png]]
> Key features：心室率 <50 bpm（房率更快）/ **规则 P-P + 规则 R-R**（但互不相关）/ **P 波与 QRS 完全分离**

### 2.5 鉴别 Mobitz I vs II 的最简单方法 ⭐⭐⭐

> [!success] 一图记住
>
> ```
> 看到漏拍 → 比较"漏拍前一个 PR"和"漏拍后第一个 PR"
>    │
>    ├─ 漏前 PR > 漏后 PR → Mobitz I (Wenckebach) ⭐
>    │   原因：漏前 PR 是延长后的，漏后 PR 已重置
>    │
>    └─ 漏前 PR = 漏后 PR → Mobitz II
>        原因：PR 始终恒定，没有重置概念
> ```
>
> 不需要数完整一组，只看漏拍前后 2 个 PR 就够。

> [!success] Memory Hook — Wenckebach 漏拍模式
> **"渐长→漏→重置"是规律，"3:2、4:3、5:4"只是品种**
>
> - 关键不是"漏拍频率"
> - 关键是"**漏拍前 PR 一定比漏拍后 PR 长**"

> [!info] UWorld Mobitz I vs II 鉴别表（高密度对照，必背）⭐
> ![[{076A3A14-4304-48E4-9091-BA4F9A7417A9}.png]]
> 6 维对照：阻滞水平 / ECG / QRS 宽度 / 迷走 ↓ 反应 / 迷走 ↑ 反应 / 进展完全 AVB 风险（→ PPM 指征）
> 同图在 [[mistakes/uworld-mistakes#^Q3766]]

---

## 3. 完全 AV Block 的逸搏定位 ⭐⭐⭐

> [!warning] USMLE 反直觉高频考点

### 3.1 简化版（USMLE 要求）

| QRS 宽度 | 逸搏类型 | 解剖位置 | 频率 | 稳定性 |
|---|---|---|---|---|
| **窄** (< 120 ms) | **Junctional escape** | AV 结 / His 近端 | 40-60 bpm | 稳定 |
| **宽** (> 120 ms) | **Ventricular escape** | His 远端 / 浦肯野 / 心室 | 20-40 bpm | 不稳定，易猝死 |

> [!tip] 一句话记忆
> - 窄 = 近端 = 稳定 = junctional
> - 宽 = 远端 = 危险 = ventricular

### 3.2 解剖逻辑

```
  SA 结
    ↓
  心房
    ↓
  ┌──────────────────────┐
  │ AV 结 / AV junction  │ ← Junctional escape 起源 (窄 QRS)
  │ + His 束近端         │
  └──────────────────────┘
    ↓
  His 束远端
    ↓
  束支系统
    ↓
  浦肯野 / 心室肌         ← Ventricular escape 起源 (宽 QRS)
```

### 3.3 临床意义

| 逸搏类型 | 预后 | 处理紧迫性 |
|---|---|---|
| 窄 QRS (junctional) | 较好，可能自愈 | PPM 但不那么紧急 |
| 宽 QRS (ventricular) | 差，易心脏停搏 | **紧急临时起搏 → 尽快 PPM** |

> [!warning] 不要细分"结性 vs 希氏束"
> 这两者解剖上几乎相连，USMLE 统称 **junctional escape**，不细分。
> 真要区分需要电生理检查 (EPS) 测 H 波，超纲。

---

## 4. 临床情景 → 病因速查 ⭐

### 4.1 按 Stem 关键词定位

| Stem 关键词组合 | 最可能诊断 | 备注 |
|---|---|---|
| 老年人 + 体检 + PR 0.24s 无症状 | **1° AV block (退化)** | 不需治疗 |
| 28 岁运动员 + 体检 PR 0.22s | **1° AV block (高迷走)** | 生理性 |
| 漏跳感 + 慢性 + 无症状 + PR 渐长漏拍 | **Mobitz I** | 观察 |
| 晕厥 + PR 恒定突然漏 + QRS 宽 | **Mobitz II** | **PPM** |
| 晕厥 + HR 35 + AV 分离 | **3° AV block** | **PPM** |
| **新生儿** HR 慢 + AV 分离 + 母亲自身免疫病 | **先天性 3° AV block** | 抗 SSA/Ro 跨胎盘 ⭐ |
| **蜱叮咬 + 游走性红斑 + Bell 麻痹 + AV block** | **Lyme 心肌炎** | 多西环素，**不需 PPM** ⭐ |
| **儿童 + 链球菌咽炎后 + 关节痛 + 1° AV block** | **风湿热** | Jones 主要标准 |
| **急性下壁 STEMI** + 新发 AV block | **RCA 闭塞引起**，多 Mobitz I，可逆 |
| **急性前壁 STEMI** + 新发 AV block | **LAD 闭塞引起**，多 Mobitz II/3°，需 PPM ⭐ |
| 主动脉瓣置换术后 + 新发 AV block | **术后机械性损伤**，常需 PPM |
| A-fib + 突然规则缓慢心室律 | **A-fib + 3° AV block** (地高辛中毒经典) |

> [!info] UWorld 原图 — Atrial fibrillation with rapid ventricular response（鉴别参考）
> ![[{CF935E23-DD70-4220-B76D-D892959A6B68}.png]]
> **AFib RVR 关键特征**：>100 bpm / **不规则不规则的 R-R** / **无 P 波 + fibrillatory waves**
>
> **AFib vs Mobitz I 都是 irregular rhythm，怎么区分？**
> - AFib：**无 P 波** + fibrillatory waves + R-R 完全乱
> - Mobitz I：**有 P 波** + PR 渐长 + grouped beating（漏拍后 R-R 突然延长）
> - 一句话：**P 波在不在 = AFib vs AVB 第一刀**

### 4.2 病因系统分类

**先天性**：
- 母亲抗 SSA/Ro (SLE / Sjögren) → 新生儿 3° AV block ⭐

**药物性**：
- β-blocker
- CCB (non-dihydropyridine: 维拉帕米、地尔硫卓)
- Digoxin
- Amiodarone

**缺血性**：
- 下壁 MI (RCA) → 多 Mobitz I，可逆
- 前壁 MI (LAD) → 多 Mobitz II / 3°，不可逆

**感染性**：
- **Lyme 心肌炎** (Borrelia burgdorferi) ⭐ — 多西环素，不需 PPM
- **风湿热** (链球菌感染后) — 1° AV block 是 Jones 主要标准
- 病毒性心肌炎、Chagas 病、心内膜炎扩展

**自身免疫 / 浸润性**：
- 淀粉样变 (amyloidosis)
- 结节病 (sarcoidosis)
- 血色病 (hemochromatosis)
- SLE 心肌受累

**退行性变**：
- **Lenègre 病** (特发性传导系统纤维化)
- **Lev 病** (传导系统钙化，伴主动脉瓣/二尖瓣环钙化)

**电解质 / 代谢**：
- 高钾血症 → 1° AV block + T 波高尖
- 甲状腺功能减退

**医源性**：
- 心脏手术 (主动脉瓣置换、室间隔肌切除)
- 导管消融术后

---

## 5. 急性 MI 与 AV Block 的解剖逻辑 ⭐⭐⭐

> [!success] USMLE 超高频考点

### 5.1 冠脉供血解剖

| 冠脉 | 供血结构 | MI 后传导问题 |
|---|---|---|
| **RCA** (右冠) | SA 结 + AV 结 + 下壁 | 窦缓、1°、**Mobitz I** |
| **LAD** (左前降) | 室间隔 + His + 前壁 | **Mobitz II、3°、束支阻滞** |

### 5.2 临床推理金句

> [!tip] 必背
> **下壁 MI + AV block**：阻滞在 AV 结 → Mobitz I 为主 → **多可逆，多观察**
>
> **前壁 MI + AV block**：阻滞在 His 下 → Mobitz II / 3° 为主 → **不可逆，需 PPM**

### 5.3 处理决策

```
急性 MI + 新发 AV block
    │
    ├─ 下壁 MI (RCA) → Mobitz I / 1°
    │    └─ 大多观察、阿托品有效、可逆
    │
    └─ 前壁 MI (LAD) → Mobitz II / 3°
         └─ 临时起搏 → PPM (不可逆)
```

---

## 6. 自主神经 / 药物试验：鉴别近端 vs 远端阻滞

| 干预 | 机制 | Mobitz I / AV 结阻滞 | Mobitz II / His 下阻滞 |
|---|---|---|---|
| **阿托品** | 抑制迷走 → AV 结加速 | **改善** | 无效或加重 |
| **运动** | 交感 ↑ | **改善** | 加重 |
| **颈动脉按压** | 迷走 ↑ | **加重** | 改善（罕见用法） |
| **β-blocker** | 抑制 AV 结 | 诱发 / 加重 | 影响小 |
| **CCB (维拉帕米/地尔)** | 抑制 AV 结 | 诱发 / 加重 | 影响小 |
| **Digoxin** | 增强迷走 | 诱发 / 加重 | 影响小 |

> [!warning] 反推
> 如果患者 AV block 在阿托品后**改善** → 阻滞在 AV 结 (近端)
> 如果阿托品**无效甚至恶化** → 阻滞在 His 下 (远端) → 危险

---

## 7. 处理总决策树

```
AV Block 患者
    │
    ├─ 1° AV block
    │    └─ 几乎全部观察 (除非药物诱发 → 减药)
    │
    ├─ 2° Mobitz I (Wenckebach)
    │    ├─ 无症状 → 观察 + 去诱因 (停药、治疗 Lyme 等)
    │    └─ 有症状 → 阿托品 / 临时起搏
    │
    ├─ 2° Mobitz II
    │    └─ 几乎全部 PPM (即使无症状)
    │       例外：Lyme → 抗生素观察
    │
    ├─ 2:1 AV block
    │    ├─ QRS 窄 / PR 长 / 阿托品改善 → 近端，按 Mobitz I 处理
    │    └─ QRS 宽 / PR 正常 / 阿托品恶化 → 远端，按 Mobitz II 处理 (PPM)
    │
    └─ 3° (Complete) AV block
         ├─ 急性不稳 → 临时经皮 / 经静脉起搏
         ├─ Lyme / 药物诱发 → 治病因，可能可逆
         └─ 其他几乎全部 PPM
```

---

## 8. PPM vs ICD（容易混淆）

| | **PPM** | **ICD** |
|---|---|---|
| **全称** | Permanent Pacemaker | Implantable Cardioverter-Defibrillator |
| **主要作用** | 起搏 (治慢) | 除颤 (治快 / 防猝死) |
| **针对问题** | 心动过缓 | 室速 / 室颤 |
| **核心适应症** | AV block、病窦、症状性心动过缓 | EF < 35%、既往室颤、HOCM 高危 |

> [!success] 一句话
> **PPM 救慢，ICD 救快**

---

## 9. 关键临床综合征

### 9.1 Stokes-Adams 综合征 ⭐
- 完全 AV block 患者**突然晕厥**
- 原因：心室停搏数秒 → 脑灌注不足
- USMLE 经典 buzzword

### 9.2 先天性完全 AV block ⭐
- 病因：**母亲抗 SSA/Ro 和/或 抗 SSB/La 抗体跨胎盘**
- 母亲疾病：**SLE** 或 **Sjögren 综合征**（可能无症状仅抗体阳性）
- 机制：抗体攻击胎儿 AV 结 → 炎症 + 不可逆纤维化
- 出生时即有，常需新生儿期 PPM
- 母亲下一胎复发风险高

### 9.3 Lyme 心肌炎 ⭐
- 病程：Lyme 病**早期播散期** (蜱叮咬后数周-数月)
- 三联：游走性红斑 + Bell 麻痹 + AV block
- AV block 可动态变化 (1° → Mobitz I → 3°)
- 治疗：**多西环素** (成人) / **阿莫西林** (孕妇 / 儿童 < 8 岁)
- **即使是 3° AV block 也不需要 PPM**（抗生素后可逆，可临时起搏过渡）

---

## 10. 高频陷阱总结

> [!danger] 常见错误

1. **"漏 QRS" ≠ 自动 Mobitz II**：必须看 PR 模式
2. **R-R 间期 ≠ PR 间期**：AV block 必须看 PR
3. **Wenckebach 的 R-R 实际逐渐缩短**（反直觉）
4. **下壁 vs 前壁 MI 后 AV block 走向完全不同**
5. **Lyme 3° AV block 不需要 PPM**（特殊处理）
6. **完全 AV block + 窄 QRS → AV 结/junction，不是浦肯野**
7. **先天性 3° AV block**：要追问母亲 SLE/Sjögren 病史 / 抗 SSA/Ro
8. **1° AV block 在儿童 + 链球菌后**：想 **风湿热**（Jones 主要标准）

---

## 11. ECG 阅读 SOP（养成习惯）

### 11.1 12 导联 ECG 标准布局

> [!tip] 一份标准 12 导联 ECG 长这样
> ```
> ┌─────────┬─────────┬─────────┬─────────┐
> │  I      │  aVR    │  V1     │  V4     │ ← 上半部分：12 导联
> ├─────────┼─────────┼─────────┼─────────┤   每个导联仅 2.5 秒
> │  II     │  aVL    │  V2     │  V5     │   (4 列 × 3 行 = 12 导联)
> ├─────────┼─────────┼─────────┼─────────┤
> │  III    │  aVF    │  V3     │  V6     │
> ├─────────┴─────────┴─────────┴─────────┤
> │  Rhythm Strip (通常导联 II) — 10 秒     │ ← 下半部分：节律条
> └───────────────────────────────────────┘   选 1-3 个导联拉长记录
> ```

### 11.2 节律条用哪个导联？— 看医院 / 机器 / 题目设置

| 模式 | 节律条导联 | 备注 |
|---|---|---|
| **最常见** | **导联 II** ⭐ | P 波在 II 导联最大、最清楚 |
| 多导联节律条 | II + V1 + V5 | 高级 ECG 机，3 条同步 |
| 特殊情况 | V1 | 看 P 波形态（如双相 P 提示左房扩大）|
| **Q3766 这道题** | **V5** | UWorld 的选择，可能因为这道题 V5 看 Wenckebach 最清楚 |

### 11.3 不同导联各自的优势

> [!info] 节律分析时各导联的特长
>
> | 导联 | 看什么最好 |
> |---|---|
> | **II** ⭐ | **P 波**（节律分析金标准）、下壁缺血 |
> | V1 | P 波形态（双相 → 左房扩大）、右心病变、RBBB |
> | V5 | LBBB、左室肥厚 |
> | aVR | 反向看心电活动、急性 ACS 总体提示 |

> [!success] Memory Hook — 节律导联默认
> **看节律 → 优先看节律条（rhythm strip）→ 默认看 II 导联**
> II 导联是 P 波的"主场"（电向量方向最匹配）

### 11.4 ECG 阅读 7 步 SOP

```
1. 心率：R-R 间隔 / 大格子数
2. 节律：R-R 是否规则？P-P 是否规则？
3. P 波：每个 QRS 前有 P 吗？P 形态正常吗？
4. PR 间期：恒定？延长？渐进延长？  ← AV block 题关键
5. QRS：窄 / 宽？形态？
6. ST / T：抬高？压低？倒置？
7. QT：长 / 短？
```

> [!warning] AV block 题永远不能跳过第 4 步

---

## 12. 关联

- 🔁 **同主题错题**：
  - [[mistakes/uworld-mistakes#^Q3766]] Mobitz I vs II 鉴别（本笔记来源 ⭐）
  - 等束支阻滞 / 病窦 / 急性 MI + 传导阻滞题积累
- 📚 **主笔记 + 已有衍生**：
  - [[完整笔记/Peixuan分科笔记/心内]]
  - [[完整笔记/专题笔记/_衍生_Vaughan_Williams抗心律失常药对照]] **Part 7.6**（ACLS 症状性心动过缓决策树 + atropine 起效部位）/ **Part 7.6.x**（传导系统病变 7 大病因，来源 Q4456）— ⭐ 与本衍生**互补分工**：
    - 本衍生 = AV block **5 类型完整鉴别 + 病因系统分类 + ECG 详解 + 处理决策**
    - VW 7.6 = 症状性心动过缓 **ACLS 急救流程 + atropine 适用性**（更聚焦于急救场景）
    - 未来若 AV block 错题持续积累，可考虑把 VW 7.6 中 AV block 相关部分迁入本衍生统一管理
- 🏥 **跨学科**：
  - [[完整笔记/Peixuan分科笔记/感染]]（Lyme 心肌炎 / 风湿热 → AV block）
  - [[完整笔记/Peixuan分科笔记/儿科]]（先天性 3° AV block + 母亲抗 SSA/Ro）
  - [[完整笔记/Peixuan分科笔记/OB]]（妊娠期 SLE 抗体跨胎盘）
- 🌱 **待扩展**：
  - 等束支阻滞 (LBBB / RBBB / fascicular block) 题积累后 → 合并到本笔记或拆出 [[完整笔记/专题笔记/_衍生_束支阻滞鉴别]]
  - 等病窦综合征 (SSS) 题积累后 → 整合到"缓慢心律失常"框架
  - 等心律失常类错题积累 → 整合到 [[完整笔记/专题笔记/_衍生_不规则心律鉴别诊断]]

---

## 13. 自测题库（已生成）

> [!question]- Q1: 28 岁运动员，体检 ECG PR 0.22s，无症状，下一步？
> **答案：C. 观察 + 无需治疗**
> 高迷走张力 → 1° AV block 是生理性变异

> [!question]- Q2: 65 岁男性，急性前壁 STEMI 后，ECG: PR 恒定 + 随机漏 QRS + QRS 宽，处理？
> **答案：C. 永久起搏器 (PPM)**
> 前壁 MI (LAD) → His 下不可逆损伤 → Mobitz II → PPM

> [!question]- Q3: 3 周龄新生儿，HR 55，房率 130 / 室率 55，AV 分离，母亲最可能病史？
> **答案：B. SLE / Sjögren**
> 抗 SSA/Ro 跨胎盘 → 先天性 3° AV block

> [!question]- Q4: 35 岁男性，新英格兰露营后 2 周，PR 0.28s + Bell 麻痹 + 游走性红斑，治疗？
> **答案：B. 多西环素**
> Lyme 心肌炎，抗生素治疗，不需 PPM

> [!question]- Q5: 70 岁老人，HR 38，晕厥，完全 AV block + QRS **窄**，阻滞部位？
> **答案：A. AV 结（结性/junctional 逸搏）**
> 窄 QRS = 近端阻滞，逸搏来自 AV 结或 His 近端 (USMLE 统称 junctional)
> 不要选浦肯野/His 远端 (那些对应宽 QRS)

---

## 版本历史

- **v1 (2026-05-16)**：来源 Q3766 错题分析。整合 AV block 5 种类型 ECG 鉴别 + 临床情景 + 逸搏定位 + MI-AV block 解剖逻辑 + 自主神经鉴别工具 + PPM/ICD 区分 + 3 大临床综合征 (Stokes-Adams / 先天性 / Lyme)
- v2 待补充：束支阻滞 / 病窦综合征整合（待相关错题积累）
