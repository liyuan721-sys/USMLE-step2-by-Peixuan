---
tags:
  - USMLE-Step2
  - 内分泌
created: 2026-06-21
type: 专题笔记
---

# 内分泌_高钙血症分层与PTH路径（诊断决策树 / PTH 依赖 vs 非依赖 / 严重度分层）

> [!info] 这张的定位
> 高钙血症 (hypercalcemia) 的内容散在两处：[[完整笔记/专题笔记/内分泌/内分泌_HighYield速查总览]] §五（夹在内分泌大总览里）+ [[完整笔记/专题笔记/肾脏/肾脏_电解质急症速查]] §三（纯治疗向）。
> 本张专做 **诊断分层主场** —— 把 **"先测 PTH" 决策树**当脊柱，PTH 依赖 vs 非依赖两大分支讲透；**治疗顺序铁律不重复**，交叉链到 [[完整笔记/专题笔记/肾脏/肾脏_电解质急症速查]]。

---

## 一、确诊高钙 + 临床表现 ⭐

> [!info] 先确认是"真高钙"
> 报 **校正钙 (corrected Ca²⁺) > 10.5 mg/dL** 或 **离子钙 (ionized Ca²⁺) > 1.3 mmol/L**。
> 白蛋白 (albumin) 每↓1 g/dL，总钙假性↓约 0.8 mg/dL → **低白蛋白时测离子钙**，别把"总钙正常但离子钙高"漏掉。

> [!tip] 症状助记 "Stones, Bones, Groans, Thrones, Psychiatric overtones"
> - **Stones**：肾结石 (nephrolithiasis)、肾钙质沉着
> - **Bones**：骨痛、病理性骨折
> - **Groans**：腹痛、便秘 (constipation)、消化性溃疡、**胰腺炎 (pancreatitis)**
> - **Thrones**：多尿 (polyuria)（高钙致肾性尿崩 nephrogenic DI）→ 脱水
> - **Psychiatric overtones**：乏力、抑郁、意识模糊 (confusion)
> - **ECG (electrocardiogram, 心电图)**：**短 QT (short QT)**（与高钾的"高尖 T"/低钙的"长 QT"反向记）

> [!info] 高钙伤肾机制 → 病人为什么是"低容量" → 为什么先补盐水 ⭐
> 这条解释整个治疗逻辑的根：**高钙病人几乎都容量不足 (hypovolemic)**。
> - **血管收缩 → GFR (glomerular filtration rate, 肾小球滤过率)↓**
> - **激活髓袢升支粗段 (TAL) 的钙敏感受体 (CaSR)** → **抑制 Na-K-2Cl 同向转运体 (NKCC2)**（= 内源性"袢利尿剂"效应）→ **利钠 (natriuresis)**
> - **阻断 ADH (antidiuretic hormone, 抗利尿激素) 介导的水重吸收** → **肾性尿崩 (nephrogenic DI)** → 多尿失水
> - 链条：**利钠 + 多尿 + 口服减少 → 容量耗竭 → 代谢性碱中毒 (metabolic alkalosis)**
>
> → 所以 **first step 永远是生理盐水补容量**（恢复 GFR + 促尿钙排）；**袢利尿剂 (loop diuretic) 非但不 routine，还会加重容量耗竭**——仅在已补足容量却容量过负荷 (HF) 时才用。

---

## 二、核心决策树：先测 PTH ⭐⭐⭐

> [!success] 一句话铁律
> **确认高钙后，病因学第一步永远是测血清 PTH (parathyroid hormone, 甲状旁腺激素)。**
> 尿钙、离子钙、维 D 水平、DEXA (dual-energy X-ray absorptiometry, 双能 X 线骨密度)、核素扫描、影像 **全排在 PTH 之后**。（NBME11A Q072 考点）

```
              确认高钙 (corrected Ca↑ / ion Ca↑)
                          │
                   ① 测血清 PTH ⭐
                          │
        ┌─────────────────┴─────────────────┐
   PTH 高 / 不当正常                      PTH 被抑制（低）
   = PTH 依赖                            = PTH 非依赖
   (PHPT/三发 · FHH · 锂 Li)             查 PTHrP / 维 D / SPEP
        │                                     │
   再查 24h 尿钙 分 PHPT vs FHH    ┌──────────┼──────────────┐
        │                       PTHrP↑     1,25-VitD↑      25-VitD↑
   ┌────┴────┐                  恶性(实体)  淋巴瘤/肉芽肿     维D中毒
 尿钙↑/正常   尿钙↓             溶骨(MM/乳/前列腺)
   PHPT      FHH
```

> [!quote] 图源：UWorld "Diagnosis of hypercalcemia" 算法
> 与本张 §二 一一对应。注意 **锂 (lithium) 在 PTH 依赖侧**（升 PTH）、**噻嗪 (thiazide) 在 PTH 非依赖侧**（drug-induced，PTH 不升）——两个利尿/精神药别混到同一支。

![[{7A0D3FD3-00ED-4439-9500-52A74F8AFC9F}.png]]

> [!warning] PTH 是"不当正常"也算依赖
> 高钙时 PTH **本应被抑制到测不出**；若 PTH "正常范围"但钙高 = **不当正常 (inappropriately normal)** = 仍是 PTH 依赖（甲状旁腺没被反馈关掉）→ 当 PHPT/FHH 处理，**别因"PTH 不算高"就排掉甲旁亢**。

---

## 三、PTH 依赖分支（PTH 高 / 不当正常）

> [!info] 三大病因：PHPT / FHH / 锂 —— PHPT vs FHH 靠 24h 尿钙区分
> 三者都表现"高钙 + 高/不当正常 PTH"。**锂 (lithium)** 上调 CaSR 设定点 → 刺激 PTH 分泌（用药史即可定，停药后多缓解）；PHPT vs FHH 的处理天差地别（一个手术、一个不治）。

| 鉴别点 | 原发性甲旁亢 PHPT | 家族性低尿钙性高钙 FHH |
|---|---|---|
| 全称 | primary hyperparathyroidism | familial hypocalciuric hypercalcemia |
| 机制 | 甲状旁腺腺瘤 (adenoma) 自主分泌（85%）| **CaSR (钙敏感受体) 失活突变** → 阈值上移 |
| 血钙 / PTH | 高钙 + 高/不当正常 PTH | 高钙 + 高/不当正常 PTH |
| 血磷 | **低磷 (↓phosphate)** ⭐ | 正常-轻低 |
| **24h 尿钙** ⭐⭐ | **高 / 正常** | **低（< 100 mg/d；FECa (尿钙排泄分数, fractional excretion of calcium) < 1%）** |
| 起病 / 家族史 | 中老年、散发、可有症状 | **终身高钙、无症状、家族史 +、年轻即有** |
| 处理 | 符合指征 → **甲状旁腺切除** | **不治疗、不手术**（手术无效） |

> [!danger] 钉死："肾结石 + 高钙 ≈ PHPT 直到排除"
> PHPT 是**门诊高钙最常见原因**。慢性高钙四联（**便秘 + 多尿 + 乏力 + 肾结石**）+ 高钙 → 先想 PHPT（来源 [[mistakes/uworld-mistakes_2026-06#^Q3151]]：此背景下急性单关节炎 → CPPD 假性痛风）。

> [!info] PHPT 手术指征（任一即 parathyroidectomy，必考）
> - **症状性**（肾结石、骨病、神经精神症状）
> - 钙 > 上限 1 mg/dL（约 > 11.5）
> - **年龄 < 50 岁**
> - 肾功能受损（eGFR (estimated GFR, 估算肾小球滤过率) < 60）/ 高钙尿 / 肾钙化
> - **DEXA T 值 ≤ −2.5** 或脆性骨折

> [!warning] 别和"继发性甲旁亢"搞混
> **继发性甲旁亢 (secondary hyperparathyroidism)** = CKD (chronic kidney disease, 慢性肾病) → 磷排不出 → 钙↓ → 刺激 PTH = **高磷 + 低钙 + 高 PTH**（不是高钙！与原发相反）。详见 [[完整笔记/专题笔记/肾脏/肾脏_CKD并发症与矿物骨病管理]]。
> **三发性甲旁亢 (tertiary)** = 长期继发后腺体自主化 → 才变成 **高钙 + 高 PTH**。

---

## 四、PTH 非依赖分支（PTH 低）

> [!info] PTH 被抑制 = 钙不是甲状旁腺驱动的 → 找外源
> 第一梯队永远是**恶性肿瘤**（住院高钙最常见原因）。下一步查 **PTHrP + 1,25-VitD + 25-VitD + SPEP/UPEP（血清/尿蛋白电泳, serum/urine protein electrophoresis）**。

| 机制 | 关键介质 | 典型肿瘤 / 病因 | 钥匙 |
|---|---|---|---|
| **PTHrP**（体液性高钙血症 HHM, humoral hypercalcemia of malignancy）⭐ | PTH 相关肽 (PTH-related peptide) | **鳞癌 (SCC, squamous cell carcinoma)**：肺/头颈/食管/肾细胞癌/膀胱；乳腺 | PTHrP↑、PTH↓；类 PTH 作用（高钙 + **低磷**）|
| **溶骨性 (osteolytic)** ⭐ | 局部细胞因子 | **多发性骨髓瘤 (MM)** ⭐ / 乳腺癌 / 前列腺癌（骨转移）| 溶骨灶；MM 看 **CRAB** |
| **1,25-VitD↑** | 活性维 D | **淋巴瘤 (lymphoma)** / 肉芽肿（结节病 sarcoidosis、结核 TB, tuberculosis）| 巨噬细胞 1α-羟化酶↑ |
| **25-VitD↑** | 储存型维 D | 维生素 D 中毒（过量摄入）| 摄入史 |
| 其他 | — | 维生素 A 中毒、Milk-alkali、长期制动、甲亢、肾上腺危象 | 各自钥匙 |

![[{B5A48FAA-9EC8-432D-AC17-E6ABC7435EB0}.png]]

*图源 UWorld/Inner Circle：恶性高钙三机制（PTHrP ~80% / 骨转移溶骨 / 1,25-VitD 淋巴瘤）+ Milk-alkali 综合征化验三联。*

> [!warning] PTH 非依赖内部再分：看磷 + 1,25-VitD ⭐⭐（兑现原 TODO）
> PTH 都被抑制了，再分两组靠**磷**：
> - **PTH 样作用（PTHrP 介导恶性）→ 排磷 → 低磷 (↓PO4)**
> - **维 D 介导（淋巴瘤 + 肉芽肿）→ 肠道同时吸 Ca 与磷 → 高/正常磷 (↑PO4)**
>
> > [!question]- 恶性 (PTHrP) vs 肉芽肿维 D 中毒，化验都"↑Ca、↓PTH"，查什么分？
> > 查 **1,25-VitD（高 → 维 D 介导）+ PTHrP（高 → 副肿瘤）**，再用**病史**定方向：结节病/TB vs 肺部肿块。

> [!tip] Milk-alkali 综合征 (milk-alkali syndrome) 三联 ⭐
> 大量**钙 + 可吸收碱**（如碳酸钙/抗酸剂）摄入 → 经典三联：**高钙 + 代谢性碱中毒 + 急性肾损伤 (AKI)**，PTH 被抑制。治疗 = **停用诱因 + 等张盐水后给呋塞米**。

> [!tip] 制动 (immobilization) 致高钙 ⭐
> 长期卧床/瘫痪（如车祸截瘫数周后）→ **破骨性骨吸收↑**，尤**高骨转换者**（年轻人 / Paget 病）→ **高钙 + 低 PTH**；治疗 = **双膦酸盐 (bisphosphonate)**。

> [!danger] MM "CRAB" —— 老年 + 不明高钙必想
> **C**a↑ / **R**enal failure（肾衰）/ **A**nemia（贫血、全血细胞减少）/ **B**one lesion（溶骨）+ M 蛋白。
> ⚠️ 但 **MM 确诊（骨髓活检 bone marrow biopsy）等急症治疗后再做** —— 见下方反复错钉子。

> [!tip] 噻嗪是 PTH 非依赖（锂归 PTH 依赖，见 §三）
> **噻嗪利尿剂 (thiazide)** 减少尿钙排泄 → 多在已有亚临床 PHPT 背景上**揭示/加重**轻度高钙，PTH 不升（drug-induced）。停药后仍高 → 回 §二 查 PTH 找真因。

---

## 五、严重度分层 + 治疗"在哪治"（详表见电解质急症速查）

> [!info] 本节只给骨架，避免重复
> 完整 3 级分层表 + 6 选治疗对照 + 急救顺序铁律 → [[完整笔记/专题笔记/肾脏/肾脏_电解质急症速查]] §三。这里只锁"分层阈值 + 一句话治什么"。

| 严重度 | 阈值 | 一句话处理 |
|---|---|---|
| **Severe / 症状性** ⭐ | **Ca > 14** 或任何症状（confusion/呕吐/严重多尿）| **生理盐水 (NS, normal saline) 补液 + 降钙素 (calcitonin)** 立刻 → 双膦酸盐 (bisphosphonate) 维持 |
| **Moderate** | Ca 12–14 | 无症状可不急；症状性按 severe |
| **Mild / 无症状** | Ca < 12 | 不急救；**避开 thiazide / 锂 / 脱水 / 长卧床** + 查病因 |

> [!danger] 反复错钉子（🔴 来源 [[mistakes/uworld-mistakes_2026-06#^Q2169-R0605]]，第 3 次同坑）⭐⭐⭐
> **Ca > 14 或症状性 = 急症，先治不诊断。**
> 即使全血细胞减少强烈怀疑 MM → **也先 NS + 降钙素救命，骨髓活检/影像延后做**。
> 我连续 3 次（5-28 / 5-31 / 6-5）被"诊断 MM"诱去选 bone marrow biopsy → 钉死："先稳住钙，确诊靠后排"。

> [!tip] 几个"何时用特殊治疗"钥匙（机制详见电解质急症速查）
> - **糖皮质激素 (glucocorticoid)** → 仅 **维 D 中毒 / 肉芽肿 (结节病/TB) / 淋巴瘤**（抑 1,25-VitD）
> - **呋塞米 (furosemide)** → 仅 **容量过负荷（心衰 HF, heart failure）**，不 routine（routine 用反致急性肾损伤 AKI）
> - **血液透析** → 仅 **肾衰 / HF 不能耐受补液**
> - **双膦酸盐起效慢 2–4 天** → 是 long-term 不是急救；其不良反应（ONJ/AFF/食管炎）见 [[完整笔记/专题笔记/内分泌/内分泌_双膦酸盐不良反应]]

---

## 六、一眼速查：高钙 5 套"指纹" ⭐

| 化验组合 | 指向 |
|---|---|
| 高钙 + **高/不当正常 PTH** + **低磷** + 尿钙高 | **PHPT**（门诊最常见）|
| 高钙 + 高/不当正常 PTH + **尿钙低** + 家族史 | **FHH**（不治）|
| 高钙 + **PTH 低** + **PTHrP↑** + 低磷 + 鳞癌史 | **恶性体液性 (PTHrP)** |
| 高钙 + PTH 低 + **贫血/肾衰/溶骨 + M 蛋白** | **MM**（CRAB；活检延后）|
| 高钙 + PTH 低 + **1,25-VitD↑ + 高/正常磷** + 双肺门淋巴结/肉芽肿 | **结节病 / 淋巴瘤** |
| 高钙 + PTH 低 + **代谢性碱中毒 + AKI** + 钙/抗酸剂摄入史 | **Milk-alkali** |

> [!warning] 反向参照——磷的两步用法
> 1. **磷不能单独定甲旁亢**："高钙 + 低磷"既见 PHPT，也见 PTHrP 介导恶性（模拟 PTH）→ 先靠 **PTH 高还是低**分。
> 2. **PTH 都低之后**，磷再帮你二分：**低磷 = PTHrP 类**，**高/正常磷 = 维 D 介导（淋巴瘤/肉芽肿）**。

---

## 🔗 关联

- 🔁 同主题错题：
  - [[NBME11_错题本#^Q072]] 高钙 workup 第一步 = 测 PTH 分流（本笔记源卡 · NBME11A Q072）
  - [[mistakes/uworld-mistakes_2026-05#^Q2169]] 重度高钙急救（先 NS + 降钙素，不先骨髓活检；🔴 反复错原卡）
  - [[mistakes/uworld-mistakes_2026-06#^Q2169-R0605]] 同上·第 3 次同坑追踪卡
  - [[mistakes/uworld-mistakes_2026-06#^Q3151]] 慢性高钙四联 → PHPT 背景上的 CPPD 假性痛风
  - [[mistakes/uworld-mistakes_2026-05#^Q106299]] CKD-MBD 继发性甲旁亢（高磷低钙高 PTH，与本张原发相反）
  - [[mistakes/uworld-mistakes_2026-06#^Q2298]] HOA 鉴别中 PTH 作为干扰项（甲旁亢致骨痛但无杵状）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/endocrine]]（钙磷骨代谢）/ [[完整笔记/Peixuan分科笔记/肾脏]]
- 📚 专题：[[完整笔记/专题笔记/内分泌/内分泌_HighYield速查总览]]（§五 PTH workup 同源）/ [[完整笔记/专题笔记/肾脏/肾脏_电解质急症速查]]（§三 治疗详表）/ [[完整笔记/专题笔记/内分泌/内分泌_双膦酸盐不良反应]]（长期治疗药不良反应）
- 🏥 跨学科：[[完整笔记/Peixuan分科笔记/hematology oncology]]（MM CRAB / 淋巴瘤 1,25-VitD）/ [[完整笔记/专题笔记/pulmonary/pulmonary_结节病Sarcoidosis]]（肉芽肿 1,25-VitD↑ 致高钙）/ [[完整笔记/专题笔记/风湿/风湿_HighYield速查总览]]（CPPD 假性痛风）
- 🌱 TODO：PTH 非依赖内部"磷"二分 ✅ 已整合（见 §四 warning + §六）；剩 **PTHrP 体液性 vs MM 溶骨的 ALP (碱性磷酸酶) 差异**（溶骨/骨转移 ALP 多↑，纯 PTHrP 体液性 ALP 常正常）→ 待新题驱动
