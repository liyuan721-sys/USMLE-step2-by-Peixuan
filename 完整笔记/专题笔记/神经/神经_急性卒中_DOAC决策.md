---
tags:
  - USMLE-Step2
  - 神经
  - 心血管
  - Heme-Onc
  - 难记
created: 2026-05-26
type: 专题笔记
---

# Acute Ischemic Stroke + DOAC < 48 hr — 决策树与逆转药机制

> [!info] 笔记用途
> 跨学科高频 schema —— **神经（stroke 急救）× 心内（AF 抗凝）× Heme-Onc（DOAC 逆转）** 三科交汇。
> Step 2 CK 几乎每次都会出一道："AF on DOAC 患者突发卒中 + last dose < 48h，下一步？"
> 决策点不是"溶不溶"，而是**先判断 DOAC 是哪一类**，再决定 tPA / 逆转药 / 取栓的路径。
> 来源：用户对话深度推导（决策树 + andexanet 机制疑问）+ ANNEXA-I 试验（NEJM 2024）。

---

## 一、核心矛盾

急性缺血性卒中（acute ischemic stroke）的黄金治疗是 **tPA（alteplase）静脉溶栓**，但 tPA 的最大并发症是 **symptomatic intracranial hemorrhage（sICH）**，自然发生率 ~6%。

如果患者**正在服用 DOAC**（direct oral anticoagulant），体内仍有活性抗凝药 → 叠加 tPA 的纤溶 → 出血风险**指数级升高**。

> [!danger] 一句话
> **DOAC < 48 hr ≈ tPA 禁忌**，但卒中必须再灌注 —— 所以决策树的核心是：**能不能溶栓？不能溶栓还能怎么救？**

---

## 二、为什么是 "48 小时"

| DOAC | 半衰期（normal renal） |
|---|---|
| Rivaroxaban | 5–9 h |
| Apixaban | ~12 h |
| Edoxaban | 10–14 h |
| Dabigatran | 12–17 h |

- **3–5 个半衰期** ≈ 药物基本清除（剩 <5% 活性）
- **48 小时** ≈ 覆盖 3–4 个半衰期的保守线
- **前提**：renal function normal（DOAC 主要肾脏清除，CrCl ↓ → 半衰期 ↑↑ → 48h 仍可能不够）

> [!warning] 隐形陷阱：肾功能不全
> 题干常埋老年人 + Cr 1.8 + "last apixaban dose 36 hr ago" → **不能按 48h 判断**，药物仍有活性。
> 真实判断应结合：last dose 时间 + CrCl + 特异性凝血检测（anti-Xa level / dTT）。

---

## 三、Xa Inhibitor vs Dabigatran —— 决策树最考的分叉

### 3.1 Xa Inhibitors（-xaban 家族）= tPA 禁忌、无解药救场

`Rivaroxaban / Apixaban / Edoxaban`

- **机制**：直接抑制 **factor Xa**（凝血瀑布的关键汇合点）
- **逆转药**：**Andexanet alfa**（重组诱饵 Xa）—— 详见 §五
- **关键**：**FDA 没有批准 andexanet 用于 tPA 前的 reversal-to-thrombolysis**，且 andexanet 本身**促血栓**反而加重卒中
- **常规凝血检测**（PT/aPTT）**不可靠**：可能正常但药物仍在
- 决策树里那个"特殊情况"（normal aPTT + PT + ecarin clotting time + thrombin time + anti-Xa level < LLD）→ 全部正常才能"理论上"考虑 tPA，但这套检测**很少医院能在 stroke window 内做完** → 实操 = **禁忌**

### 3.2 Dabigatran = 有逆转通路、可桥接 tPA

- **机制**：直接抑制 **thrombin (factor IIa)**
- **逆转药**：**Idarucizumab (Praxbind)** —— **FDA 批准**的单克隆抗体片段，5 分钟内完全中和 dabigatran
- 给完 idarucizumab → 凝血状态回归正常 → **可以再给 tPA**

> [!tip] 记忆钩
> **"-xaban 没药救，-gatran 有 Idaru 救"**
> 题干 stroke + AF + dabigatran → **先 idarucizumab，再 tPA**。
> 题干 stroke + AF + rivaroxaban/apixaban → tPA 禁忌，直接跳 thrombectomy（if LVO）。

---

## 四、Mechanical Thrombectomy —— "救命的 Plan B"

### 4.1 为什么取栓不受抗凝影响

- **机械取栓**，**不引入溶栓药** → **不依赖凝血系统** → 抗凝状态**不是禁忌**
- 通路：股动脉 → 导管 → stent retriever / aspiration catheter 物理拉出血栓

### 4.2 LVO（Large Vessel Occlusion）—— 取栓的硬门槛

| LVO 部位 | 说明 |
|---|---|
| **ICA**（internal carotid artery） | 颈内动脉 |
| **MCA M1/M2 段** | 大脑中动脉近端 |
| **Basilar artery** | 基底动脉 |
| **Vertebral artery** | 椎动脉 |

为什么必须是 LVO？

- 小血管（远端 MCA 分支、穿支动脉）→ 导管**进不去**
- 小血管闭塞梗死灶小 → 风险/获益比不划算
- **大血管闭塞预后极差**（M1 闭塞死亡率 ~30%，残疾率 ~70%）→ 介入获益大

### 4.3 时间窗（重要）

```
经典窗：症状起始 ≤ 6 小时
扩展窗：6 – 24 小时
        └─ 需 CT perfusion / MRI DWI-FLAIR mismatch 显示 salvageable penumbra
           （可挽救半暗带）
        └─ 依据：DAWN 试验 (6-24h) + DEFUSE-3 试验 (6-16h)
```

---

## 五、Andexanet Alfa 深度解析 —— 不只是 "tPA 前不能用"

### 5.1 FDA 批准的唯一适应症

> **Life-threatening or uncontrolled bleeding** associated with rivaroxaban / apixaban

也就是：**已经在大出血**（ICH / GI bleed / 腹膜后出血）—— 用它**止血救命**，不是预防或溶栓桥接。

商品名：**Andexxa**（2018 加速批准 accelerated approval）

### 5.2 为什么"反而加重血栓"—— 机制层面

Andexanet alfa 是个**重组诱饵 factor Xa**（catalytically inactive 突变体），原始设计逻辑：
- 用诱饵 Xa "吸住" 血液里的 -xaban → 内源性 Xa 重新可用 → 凝血恢复

**致命副作用**：

> 它**同时结合并耗竭 TFPI（tissue factor pathway inhibitor，组织因子通路抑制剂）**

TFPI 是人体内源性抗凝系统的关键刹车。TFPI 被耗竭后：

- TF–FVIIa–Xa 复合物失去抑制
- 凝血系统 **rebound 性激活**
- 进入 **promothrombotic state（促血栓状态）**，持续数小时

> [!danger] ANNEXA-I 试验震撼结果（NEJM 2024）
> 急性 ICH（脑出血）+ Xa inhibitor 患者随机 andexanet vs usual care（多为 4F-PCC）：
> - 止血效果：andexanet 稍好（67% vs 53% 良好止血）
> - **ischemic stroke 翻倍**（6.5% vs 1.5%）
> - **整体血栓事件**：10.3% vs 5.6%
> - 死亡率无差异
>
> 试验**提前终止**，因为安全性信号太强 → 临床偏好开始退缩。

### 5.3 为什么"tPA 前不能用"是衍生问题

套到卒中场景：

1. 患者已经**急性缺血性卒中**（本身就是血栓造成的）
2. 给 andexanet → **进一步促血栓状态** → 可能扩大梗死 / 新发血栓
3. 即使逆转了 Xa 抑制，再给 tPA：
   - 无 RCT 数据支持安全性
   - Andexanet 半衰期短（~1 小时），**rebound 效应**在 tPA 起效时段重叠
   - 凝血状态：reversed → procoagulant → 给 tPA 后又 fibrinolytic，整个凝血轴**剧烈震荡**

→ 指南（AHA/ASA 2019 + 2021 update）**明确不推荐** andexanet 用于 tPA 前桥接。

### 5.4 实际临床定位

| 场景 | Andexanet 怎么用 |
|---|---|
| Xa inhibitor + life-threatening bleed（ICH/GIB） | **FDA 批准，可考虑**（但 ~10% 血栓风险，很多中心首选 4F-PCC） |
| Xa inhibitor + 急性缺血性卒中 + 想 tPA | **不推荐**（促血栓 + 无证据 + 加重梗死） |
| Xa inhibitor + 急诊手术前 | **不推荐**（用 PCC 或延迟手术） |
| Dabigatran 任何场景 | **无效**（andexanet 不结合 dabigatran，用 idarucizumab） |

### 5.5 Andexanet vs 4F-PCC（实际临床偏好对比）

| 对比项 | Andexanet alfa | 4F-PCC（Kcentra） |
|---|---|---|
| 机制 | 诱饵 Xa + 耗竭 TFPI | 补充 II/VII/IX/X 凝血因子 |
| 价格 | **$24,750–49,500/剂** | ~$3,000–5,000/剂 |
| 血栓事件 | ~10% | ~4–8% |
| RCT 头对头 | ANNEXA-I 没赢过 usual care | — |
| 指南推荐 | 部分指南列为 alternative | **多数指南首选** |

### 5.6 Andexanet vs Idarucizumab —— 根本差异

| | Idarucizumab | Andexanet alfa |
|---|---|---|
| 目标 | Dabigatran（IIa 抑制剂） | -xabans（Xa 抑制剂） |
| 结构 | 单克隆抗体片段（Fab）—— 抗原-抗体高亲和力 | 重组诱饵蛋白 |
| 作用 | 5 分钟内**完全清除** dabigatran 活性 | 部分中和 + 耗竭 TFPI |
| Rebound 促血栓 | **无** | **有**（~10% 血栓事件） |
| tPA 前桥接 | **可以**（指南支持） | **不可以** |
| 临床地位 | 干净利落的解药 | 有争议的止血手段 |

> [!success] 一句话定性
> **Andexanet 是"用血栓换止血"的双刃剑** —— FDA 批准范围窄（仅 life-threatening bleed），临床偏好在退缩。
> **Idarucizumab 是真正的解药** —— 不动凝血系统，可桥接 tPA。
> **这才是为什么 dabigatran 在 stroke 场景里反而比 -xaban "好对付"**。

---

## 六、No LVO + tPA 禁忌 → Supportive 路径

如果：

- tPA 不能给（DOAC 在体内）
- 又不是 LVO（thrombectomy 没适应症）

→ **没有急性再灌注手段**，只能：

1. **Permissive hypertension**（允许 BP 升高到 220/120，维持脑灌注）
2. **Antiplatelet**（aspirin 325 mg；若本来在 DOAC → 权衡出血风险，通常等 DOAC 清除后再决定长期方案）
3. **Secondary prevention**：找病因（AF? 大动脉粥样硬化? 小血管病? 心源性?）→ 调整长期抗凝/他汀/血压
4. **Supportive**：DVT 预防、吞咽评估、康复早期介入

> [!danger] 陷阱：不要急着用 heparin bridge
> 急性卒中 24–48h 内全身抗凝**增加出血转化**风险，无循证支持。
> 即便 AF 患者，guideline 建议**延迟 2 周左右**再恢复抗凝（梗死越大延迟越久，叫 **"1-3-6-12 rule"**）：
> - TIA → 1 天
> - 小梗死 → 3 天
> - 中梗死 → 6 天
> - 大梗死 → 12 天

---

## 七、完整决策树

```
Acute ischemic stroke + last DOAC dose < 48 hr
    │
    ▼
① CT 排除 hemorrhage（OK if 无）
    │
    ▼
② 评估 tPA candidacy（按 DOAC 类型分叉）
    │
    ├─ Direct Xa inhibitor (rivaroxaban / apixaban / edoxaban)
    │     ├─ Last dose < 48 hr + normal renal → tPA 禁忌
    │     │  └─ Andexanet 不能桥接 tPA（促血栓 + 无证据）
    │     └─ 特殊：所有凝血检测正常（aPTT + PT + ecarin + TT + anti-Xa < LLD）
    │              → 极个别中心理论上考虑（实操几乎不可行）
    │
    └─ Direct thrombin inhibitor (dabigatran)
          ├─ Last dose < 48 hr → tPA 禁忌
          └─ Idarucizumab reversal → 后可考虑 tPA
                                    （dabigatran 唯一有 FDA 批的逆转通路）
    │
    ▼
③ tPA 禁忌 + LVO（ICA / MCA M1-M2 / Basilar / Vertebral）
    → 首选 Mechanical Thrombectomy
       （6h 内首选；6-24h 需 CTP/DWI-FLAIR mismatch）
    │
    ▼
④ tPA 禁忌 + No LVO
    → 仅 supportive：permissive HTN + 抗血小板（权衡）+ 二级预防
    → ❌ 不急性全身抗凝（出血转化）；DOAC 恢复按 1-3-6-12 rule
```

---

## 八、Memory Hooks（必记）

> [!tip] 4 句话锁定整个决策树
> 1. **"-xaban 没药救"** —— Andexanet 不能桥接 tPA（促血栓 + ANNEXA-I 翻倍 ischemic stroke）
> 2. **"-gatran 有 Idaru 救"** —— Idarucizumab 5 min 完全逆转，可桥接 tPA
> 3. **"LVO 才取栓，小血管进不去"** —— ICA / MCA M1-M2 / Basilar / Vertebral
> 4. **"卒中后抗凝 1-3-6-12"** —— TIA / 小 / 中 / 大梗死的延迟恢复

> [!tip] 机制级 Memory Hook：Andexanet 为什么自相矛盾
> "诱饵 Xa 吸 -xaban，但**顺手把 TFPI 也吸了** → 内源性抗凝刹车失灵 → rebound 促血栓"
> = 一只手解抗凝，另一只手放血栓 → 双刃剑

---

## 九、USMLE 高频 Stem 模式

> [!question]- Q1. 78 yo F, AF on apixaban, last dose 20 hr ago, sudden right hemiparesis + aphasia 2 hr ago, CT no bleed. NIHSS 18. CTA shows left M1 occlusion. Next step?

> [!question]- Q2. 同样患者，但服用的是 **dabigatran**，last dose 18 hr ago，没有 LVO（CTA 显示远端 M3 分支闭塞）。Next step?

> [!question]- Q3. AF on rivaroxaban, last dose 12 hr ago, no LVO. Next step?

> [!question]- Q4. 患者吃 apixaban 因 ICH 入院，临床问哪个药最合适紧急止血？为什么很多中心仍用 4F-PCC 而非 andexanet？

> [!question]- Q5. Andexanet alfa 的作用机制是什么？为什么会"逆转抗凝的同时增加血栓事件"？

> [!question]- Q6. Dabigatran 用 idarucizumab 逆转 30 分钟后，可以给 tPA 吗？rivaroxaban 用 andexanet 逆转 30 分钟后呢？区别在哪里？

> [!question]- Q7. 一位 75 岁老年人 AF on apixaban 10 mg BID，Cr 2.1，last dose 36 小时前，急性大面积卒中。能按 "< 48 hr" 直接判 tPA 禁忌吗？如果不能，正确思路是？

> [!question]- Q8. 急性卒中入院 + AF 既往抗凝史，影像示大面积 MCA 梗死。问何时恢复 DOAC？说出 "1-3-6-12 rule"。

---

## 十、自测题（标记再考我 —— 答完再核对）⭐

> [!question]- 测 1. ANNEXA-I 试验对比 andexanet vs usual care（4F-PCC）治疗 Xa-inhibitor 相关 ICH，主要安全性发现是？

> [!question]- 测 2. 为什么常规 PT / aPTT 不能用来判断 Xa inhibitor 是否清除？应该测什么？

> [!question]- 测 3. 写出完整 LVO 部位清单（4 个动脉），并解释为什么 M3 远端闭塞**不算** LVO。

> [!question]- 测 4. 急性卒中 + 患者 36 小时前服了最后一次 dabigatran 110 mg BID + Cr 1.0。CT 无出血。无 LVO。下一步管理？

> [!question]- 测 5. Mechanical thrombectomy 的标准时间窗和扩展时间窗各是多少？扩展窗需要什么影像证据？

> [!question]- 测 6. Andexanet alfa 的结构是什么？为什么"重组诱饵 Xa"会导致 TFPI 耗竭？

> [!question]- 测 7. Heparin / LMWH / Warfarin / Dabigatran / Xa-DOAC / Fondaparinux 的拮抗剂分别是？（写出 6 对）

> [!question]- 测 8. 患者大面积右侧 MCA 梗死（NIHSS 22），既往 AF 服 apixaban。何时恢复抗凝？依据是？

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes#^Q4469]] AF 抗凝指征 — CHA₂DS₂-VASc 评分是抗凝触发器，不是"有 AF 就抗凝"
  - 抗凝药拮抗剂 4 对（2026-05-14 self-test 卡，无 Q 锚点）— 6 对拮抗剂总表 + Warfarin 急性出血 SOP
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/neuro]] / [[完整笔记/Peixuan分科笔记/心内]] / [[完整笔记/Peixuan分科笔记/hematology oncology]]
- 🏥 跨学科：
  - [[完整笔记/Peixuan分科笔记/心内]]（AF 抗凝是 DOAC 最常见适应症 → stroke + AF on DOAC 是经典叠加 stem）
  - [[完整笔记/Peixuan分科笔记/hematology oncology]]（DOAC 逆转药 / TFPI 机制 / 凝血瀑布）
  - [[完整笔记/Peixuan分科笔记/GI]]（DOAC 相关 GI 出血是 andexanet 另一适应症场景）
- 🌱 TODO（待生成衍生）：
  - 等积累 3+ 道 acute stroke 错题 → 整合 [[完整笔记/专题笔记/神经/神经_急性卒中_完整决策]]（涵盖 tPA candidacy + BP 管理 + 影像门槛 + thrombectomy + 病因二级预防）
  - 等积累 3+ 道抗凝逆转错题 → 整合 [[完整笔记/专题笔记/_衍生_抗凝药拮抗剂_4对]]（已在 2026-05-14 self-test 卡里 TODO）

---

## ✅ 复盘行动

- [ ] **7 天后**（2026-06-02）盲做 §十 8 道自测题
- [ ] 默写 §七 完整决策树（4 步 + 2 分叉）
- [ ] 默写 §五 Andexanet vs Idarucizumab 对比表（6 行）
- [ ] 找 UW 题库里所有 acute stroke + on anticoagulant 的题做一遍（搜索关键词：apixaban stroke / dabigatran stroke / DOAC reversal）
- [ ] 同主题题第 2 次错 → 升 🔴 + 加 #考前必看 + 整合到衍生
