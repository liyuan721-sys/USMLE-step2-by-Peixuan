---
tags:
  - USMLE-Step2
  - 肾脏
created: 2026-05-29
type: 专题笔记
---

> [!info] 这一篇定位
> CK 酸碱紊乱的**完整判读 SOP**：三步法 + 代偿公式（分层标注哪些必背）+ Mixed 识别捷径。
> 核心理念：**只死记 1 个公式（Winter），其余靠"方向法"定性秒杀**，不背一堆小数系数。

# 酸碱代偿完整 SOP (Acid-Base Disorders)

## 一、三步法总流程 ⭐

```
① 看 pH    → acidemia / alkalemia / 极端 / 正常但 HCO3·PaCO2 异常
② 定原发    → HCO3 还是 PaCO2 朝 pH 偏离方向动 = 原发
③ 算代偿    → 用公式算 expected，比对实测 → 偏离即【第二原发】(mixed)
```

| 步骤 | 操作 |
|---|---|
| **① 看 pH** | <7.35 acidemia / >7.45 alkalemia / 极端值(<7.2 或 >7.6) / **正常但 HCO₃·PaCO₂ 异常 → 怀疑 mixed** |
| **② 定原发** | HCO₃↓→met acidosis / HCO₃↑→met alkalosis / PaCO₂↑→resp acidosis / PaCO₂↓→resp alkalosis（**朝 pH 偏离方向的就是原发**）|
| **③ 算代偿** | 用公式算 expected PaCO₂ 或 HCO₃，比对实测 → 偏离即第二原发 |

### 1.1 ABG 判读流程图（看哪个参数朝 pH 方向变 = 原发）⭐

```
                          pH（正常 7.4）
                ┌──────────────┴──────────────┐
            < 7.35 低                       > 7.45 高
          (acidemia 酸血症)              (alkalemia 碱血症)
          ┌───────┴────────┐            ┌────────┴────────┐
      HCO3↓(<24)      PaCO2↑(>40)    PaCO2↓(<40)     HCO3↑(>24)
          │                │             │               │
       原发紊乱         原发紊乱       原发紊乱         原发紊乱
       代谢性酸         呼吸性酸       呼吸性碱         代谢性碱
          │                │             │               │
       代偿(快)         代偿(慢/数天)  代偿(慢/数天)    代偿(快)
       呼吸性碱         代谢性碱       代谢性酸         呼吸性酸
       PaCO2↓          HCO3↑         HCO3↓           PaCO2↑
                                                  ↑袢/噻嗪利尿、呕吐
                                                   = 代碱最常见源
```

> [!tip] 一句话用法
> **HCO3 与 PaCO2 中，哪个"朝 pH 偏离方向"变了，哪个就是原发。** HCO3 高 → 代碱；HCO3 低 → 代酸；PaCO2 高 → 呼酸；PaCO2 低 → 呼碱。**急性呼吸紊乱时 HCO3 仍接近正常**（肾代偿要数天）；HCO3 明显异常 = 慢性或合并代谢紊乱。

### 1.2 ABG 实战判读（4 道错题串讲）⭐

| Q# | pH | 关键参数 | 原发判读 | 一句话坑 |
|---|---|---|---|---|
| [[mistakes/uworld-mistakes#^Q2786]] | 7.49↑ | PaCO2 30↓ / HCO3 24 正常 | **uncompensated 呼吸性碱**（肺炎过度通气）| 呕吐诱选代碱，但 **HCO3 正常 → 不是代碱** |
| [[mistakes/uworld-mistakes#^Q2826]] | 7.47↑ | HCO3 31↑ / K↓Cl↓ | **代谢性碱**（袢利尿/收缩性碱）| 插管诱选呼碱，但 **HCO3 高 = 代碱**（呼碱 HCO3 低）|
| [[mistakes/uworld-mistakes#^Q13842]] | 7.30↓ | HCO3 16↓ / 乳酸↑ / PaCO2 34↓ | **高 AG 代酸**（AAA 夹闭乳酸）+ 呼吸代偿 | 肾代偿排 H⁺ 靠 **NH4⁺**；尿 Cl **排泄**↑（非重吸收）|
| [[mistakes/uworld-mistakes#^Q18881]] | 7.32↓ | HCO3 13↓ / AG 10 正常 / PaCO2 26 | **NAGMA → Type 1 RTA**；PaCO2 26 = Winter 代偿 | 代酸时 **尿 pH > 5.5 = 远端 RTA**；PaCO2 低是代偿非呼碱 |

> [!warning] 串讲核心：判原发先读数，别被病史词带偏
> 呕吐 → 不一定代碱（看 HCO3 升没升）；插管/呼吸机 → 不一定呼吸性（看 HCO3 方向）；FTT/疲劳 → 先算 AG + 看尿 pH。**数定原发，史定病因。**

---

## 二、第三步深挖：代偿 vs 第二原发 ⭐⭐

> [!warning] "第二原发"≠"没有代偿"
> - **代偿 (compensation)** = 身体对原发紊乱的**生理性反应**，可预测、有范围、**永远不会矫枉过正**（不会把 pH 拉过对侧）。代偿几乎总会发生。
> - **第二原发 (second primary disorder)** = 在第一个紊乱之上**又叠加一个独立紊乱**（= mixed disorder），不是身体的反应，是另一个病。
>
> 第三步用公式算 expected 值，本质是问：**"这个代偿是恰到好处，还是太多 / 太少？"** 太多太少都说明 mixed。

以**代谢性酸中毒**为例（Winter's formula）：

| 实测 PaCO₂ 相对 expected | 含义 |
|---|---|
| **正好等于**（±2 内）| 单纯代酸 + 适当呼吸代偿 |
| **高于** expected（CO₂ 排不够）| 叠加**呼吸性酸中毒**（第二原发）|
| **低于** expected（CO₂ 排过头）| 叠加**呼吸性碱中毒**（第二原发，如 salicylate）|

---

## 三、代偿公式表（分层标注 — 别全背！）

> [!info] 先记两个正常值（所有 Δ 计算的基准）⭐
> - 正常 **HCO₃⁻ ≈ 24** mEq/L
> - 正常 **PaCO₂ ≈ 40** mmHg
> - 正常 **Anion Gap ≈ 8–12**
>
> 公式里的 **Δ (delta) = 实测值偏离正常值多少**。例：PaCO₂ 60 → ΔPaCO₂ = 60 − 40 = **20**。

> [!danger] 🔴 第一层：唯一必死记
> **Winter's formula（代酸预期代偿）：expected PaCO₂ = 1.5 × HCO₃⁻ + 8 (±2)**
> 这是 CK 唯一需要你能动手算的代偿公式。
> 偷懒替代法（代酸专用）：适当代偿时 **expected PaCO₂ ≈ pH 小数点后两位**（pH 7.25 → PaCO₂ ≈ 25）。

> [!warning] ❌ 别记成"PaCO₂ ≈ HCO₃ 末两位" — 这是错的
> 流传的"HCO₃ 末两位"记法**不成立**：HCO₃ = 12 时 Winter 算出 26，而非 12。
> 正确的偷懒法是上面那条 **pH 小数点后两位**，且**只用于代谢性酸中毒**。

> [!warning] 🟡 第二层：记"方向 + 急慢"，不背小数系数
> 呼吸性紊乱的代偿系数 CK 几乎不让精算，只记定性规则：
> - **急性** → 肾还没反应，**HCO₃ 几乎不动**
> - **慢性(>2–3 天)** → 肾代偿建立，**HCO₃ 明显朝同方向动**
> 例：COPD 病人 PaCO₂ 高但 pH 接近正常 + HCO₃ 高 = **慢性呼酸**。

完整系数表（🟢 第三层，**查表用，不背**）：

| 原发紊乱 | 代偿公式 |
|---|---|
| **Metabolic acidosis** ⭐ | Winter's: expected PaCO₂ = 1.5 × HCO₃ + 8 (±2) |
| Metabolic alkalosis | ΔPaCO₂↑ = 0.7 × ΔHCO₃ |
| Acute resp acidosis | ΔHCO₃↑ = 0.1 × ΔPaCO₂ |
| Chronic resp acidosis | ΔHCO₃↑ = 0.35–0.4 × ΔPaCO₂ |
| Acute resp alkalosis | ΔHCO₃↓ = 0.2 × ΔPaCO₂ |
| Chronic resp alkalosis | ΔHCO₃↓ = 0.4–0.5 × ΔPaCO₂ |

### 3.1 这些公式到底在算什么？（人话版）⭐⭐

> [!info] 一句话：都在算"身体应该代偿到多少"
> 算出 expected 值 → 和实测比 → **相等 = 单纯 + 适当代偿；偏离 = 第二原发 (mixed)**。

统一心法（看懂这 4 点，整张表全通）：

```
1. Δ = 偏离正常多少（HCO₃ 正常 24，PaCO₂ 正常 40）
2. 原发动一个 → 代偿动另一个：
     代谢紊乱(HCO₃ 变) → 肺代偿调 PaCO₂ → 算 ΔPaCO₂
     呼吸紊乱(PaCO₂ 变) → 肾代偿调 HCO₃ → 算 ΔHCO₃
3. 系数 = 代偿"效率"：大 = 代偿充分，小 = 才刚开始
4. expected 算完和实测比 → 偏离即 mixed
```

逐行翻译成大白话：

| 公式 | 人话 |
|---|---|
| Met alkalosis: ΔPaCO₂↑ = 0.7 × ΔHCO₃ | HCO₃ 升(碱中毒) → 肺**少呼吸**让 PaCO₂ 升补偿；HCO₃ 每多 1，PaCO₂ 升 0.7 |
| Acute resp acidosis: ΔHCO₃↑ = 0.1 × ΔPaCO₂ | CO₂ 潴留(酸) → 肾**还没反应**，HCO₃ 微升（每 10 升 1）|
| Chronic resp acidosis: ΔHCO₃↑ = 0.35–0.4 × ΔPaCO₂ | 同样潴留但**拖几天** → 肾代偿建立，HCO₃ 升很多（每 10 升 3.5–4）|
| Acute resp alkalosis: ΔHCO₃↓ = 0.2 × ΔPaCO₂ | 过度通气吹低 CO₂ → 肾没反应，HCO₃ 微降 |
| Chronic resp alkalosis: ΔHCO₃↓ = 0.4–0.5 × ΔPaCO₂ | 过度通气**拖久** → 肾代偿，HCO₃ 降很多 |

### 3.2 为什么呼吸紊乱分"急性/慢性"，代谢不分？⭐

> [!tip] 关键：代偿速度不同
> - **肾代偿慢**（2–3 天才建立）→ 呼吸紊乱才有 **急性**（系数小，HCO₃ 几乎没动）vs **慢性**（系数大，HCO₃ 动足）之分
> - **肺代偿快**（分钟级）→ 代谢紊乱马上被肺代偿，**没有急慢之分**（代酸 / 代碱各只 1 个公式）

### 3.3 走一遍例子（COPD 老人）

> [!example] PaCO₂ = 60（正常 40），原发呼吸性酸中毒
> - ΔPaCO₂ = 60 − 40 = **20**
> - **急性**预期：HCO₃ = 24 + 0.1 × 20 = **26**
> - **慢性**预期：HCO₃ = 24 + 0.4 × 20 = **32**
> - 实测 HCO₃ = 31 → 接近慢性 32 → **慢性呼酸 + 适当肾代偿**
> - 若实测 HCO₃ 只有 25 → 远低于慢性预期 → 还**合并代谢性酸中毒**（第二原发！）

---

## 四、黄金捷径：方向法（不用公式秒判 mixed）⭐⭐⭐

> [!success] HCO₃ 和 PaCO₂ 同向还是反向？
> **单纯紊乱 + 代偿时，HCO₃ 和 PaCO₂ 永远同向变化（同升或同降）。**
>
> ```
> 同向变(都↑ 或都↓) → 单纯紊乱 + 代偿（再用 Winter 验证够不够）
> 反向变(一↑一↓)    → 一定是 MIXED！且 pH 会很极端
> ```

> [!info] 一眼定 mixed 的两种信号
> 1. **HCO₃ 和 PaCO₂ 反向动** → mixed（pH 极端）
> 2. **pH 正常，但 HCO₃ 和 PaCO₂ 都明显异常** → 也是 mixed（两个反向力量互相抵消，如 DKA + 重度呕吐）

---

## 五、Mixed 5 大典型组合（UW 高频）⭐

| 组合 | HCO₃ | PaCO₂ | pH | 经典 Stem |
|---|---|---|---|---|
| **Met acidosis + Resp acidosis** | ↓ | ↑ | **Very low** | Sepsis + lactic acidosis + 呼衰 / cardiac arrest |
| **Met alkalosis + Resp alkalosis** | ↑ | ↓ | **Very high** | Hyperemesis gravidarum + 妊娠过度通气 |
| **Met acidosis + Resp alkalosis** | ↓ | ↓ | Near normal | **Salicylate toxicity（经典）** / sepsis 早期 |
| **Met alkalosis + Resp acidosis** | ↑ | ↑ | Near normal | 过度利尿的 HF + 基础 COPD |
| **Met acidosis + Met alkalosis** | ↔ | ↔ | Near normal | DKA + 重度呕吐 |

> [!tip] 对照方向法
> 前两行 = HCO₃/PaCO₂ **反向** → pH 崩到极端；后三行靠"pH 接近正常但两值都异常"识别。

---

## 六、Sepsis 酸碱演化（理解题，不背公式）

| 阶段 | 机制 → 酸碱 |
|---|---|
| **早期** | tachypnea → **resp alkalosis** 主导（hyperventilation 应激）|
| **中期** | tissue hypoperfusion → **lactic (met) acidosis**；常 mixed met acidosis + resp alkalosis（salicylate-like pattern）|
| **晚期** | respiratory muscle fatigue → 不能再代偿 → **mixed met + resp acidosis（最危险，pH 崩塌）** |

> [!danger] 记忆点
> "晚期呼吸肌疲劳 → 不能再 hyperventilate 代偿 → pH 崩 = 最危险" — 一个公式都不用背。

---

## 七、Anion Gap + Delta-Delta（代酸配套）

> [!warning] Winter 的搭档：Anion Gap = Na⁻ − (Cl⁻ + HCO₃⁻)，正常 8–12
> 没有 AG 分不出"高 AG 代酸 vs 正常 AG 代酸"。**Winter + AG 一起记。**

> [!info] Delta-Delta（高 AG 代酸时查有没有"再叠加"）
> 比较 ΔAG 与 ΔHCO₃：
> - ΔAG ≈ ΔHCO₃ → 单纯高 AG 代酸
> - ΔAG < ΔHCO₃（HCO₃ 掉太多）→ **合并正常 AG 代酸**
> - ΔAG > ΔHCO₃（HCO₃ 掉太少）→ **合并代谢性碱中毒**

---

## 八、考前精简：只背这三句 ⭐

```
1. Winter:  expected PaCO₂ = 1.5×HCO₃ + 8 ±2  (+ Anion Gap = Na−Cl−HCO₃)
2. 急性不动 HCO₃，慢性才动（呼吸紊乱定性，不背系数）
3. HCO₃ 与 PaCO₂ 反向 = mixed；pH 正常但两值都异常 = 也 mixed
```

---

## 九、复习 Q&A

> [!question]- Q1. 酸碱判读三步法？
> ① 看 pH（定酸碱血症）→ ② 定原发（HCO₃/PaCO₂ 哪个朝 pH 偏离方向动）→ ③ 算代偿（Winter 等公式，比 expected 找第二原发）。

> [!question]- Q2. "第二原发"是什么意思？等于没有代偿吗？
> **不是**。第二原发 = 在原发之上又叠加一个独立紊乱（mixed）。代偿是身体生理反应、有范围、不过头；实测偏离 expected（太多/太少）→ 说明有第二原发。

> [!question]- Q3. CK 酸碱唯一必死记的公式？
> **Winter's formula**：expected PaCO₂ = 1.5 × HCO₃ + 8 (±2)，配 Anion Gap。

> [!question]- Q4. 不用公式怎么快速判 mixed？
> **方向法**：单纯紊乱时 HCO₃ 和 PaCO₂ 永远同向；**反向 = mixed（pH 极端）**；pH 正常但两值都异常 = 也 mixed。

> [!question]- Q5. Salicylate 中毒典型酸碱？
> **Met acidosis + Resp alkalosis**（同时刺激呼吸中枢 + 产酸），两个独立原发，pH 常接近正常。

> [!question]- Q6. COPD 病人 PaCO₂ 高、pH 接近正常、HCO₃ 高，怎么判？
> **慢性呼吸性酸中毒**（肾代偿已建立，HCO₃ 朝同方向明显上升）。急性时 HCO₃ 几乎不动。

> [!question]- Q7. 那 5 个代偿公式到底在算什么？为什么呼吸分急慢、代谢不分？
> 都在算"身体应该代偿到多少（expected）"，比实测找第二原发。Δ = 偏离正常（HCO₃ 24 / PaCO₂ 40）；原发动一个、代偿动另一个；系数 = 代偿效率。**肾代偿慢(2–3 天)→ 呼吸有急慢；肺代偿快(分钟)→ 代谢无急慢**。

## 🔗 关联

- 🔁 同主题错题：
  - *（暂无入库的酸碱紊乱错题 — 见 🌱 TODO，做到后补 Q 号）*
- 📚 主笔记：
  - [[完整笔记/Peixuan分科笔记/肾脏]]（酸碱 / 电解质主章节）
  - [[完整笔记/专题笔记/肾脏/肾脏_高钾血症完整体系]]（酸碱与钾的联动）
  - [[完整笔记/专题笔记/肾脏/_衍生_电解质急症速查]]
- 🏥 跨学科：
  - [[完整笔记/Peixuan分科笔记/pulmonary]]（呼吸性紊乱：COPD 慢性呼酸 / 过度通气呼碱 / 呼吸肌疲劳）
  - [[完整笔记/Peixuan分科笔记/endocrine]]（DKA 高 AG 代酸 / salicylate 中毒）
  - [[完整笔记/Peixuan分科笔记/外科]]（休克 / sepsis 酸碱演化 / cardiac arrest）
- 🌱 TODO（待生成衍生）：
  - 做到 ≥3 道酸碱错题 → 回填 🔁 区 Q 号，并按"反复错"升级状态
  - 积累高 AG 代酸题（MUDPILES）→ 可单独建 [[完整笔记/专题笔记/肾脏/肾脏_高AG代酸MUDPILES]]

## 📊 版本

| 版本 | 日期 | 变更 |
|---|---|---|
| v1 | 2026-05-29 | 填充原空壳文件：三步法 + 代偿 vs 第二原发概念 + 代偿公式分层（🔴Winter 必背 / 🟡呼吸定性 / 🟢系数表查阅）+ 方向法捷径（同向/反向判 mixed）+ Mixed 5 组合 + Sepsis 演化 + AG/Delta-Delta + 考前三句精简 + 6 道复习 Q&A |
| v1.1 | 2026-05-29 | §三补正常值基准 callout（HCO₃ 24 / PaCO₂ 40 / AG 8–12 + Δ 定义）；新增 §3.1 公式人话翻译 + 统一心法 4 点、§3.2 急慢性原理（肾慢肺快）、§3.3 COPD 算例；修正错误速记法（删"PaCO₂≈HCO₃ 末两位"，改为正确的"代酸 expected PaCO₂≈pH 小数点后两位"）；加 Q7 |
