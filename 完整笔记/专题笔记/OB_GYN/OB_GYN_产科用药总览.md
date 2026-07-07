---
tags:
  - USMLE-Step2
  - 妇产科
created: 2026-07-07
type: 专题笔记
---

# 产科用药总览：原理 · 适应症 · 禁忌 (Obstetric Pharmacology Map)

> [!tip] 一句话核心
> 产科用药考的不是"这个药能不能收缩子宫"，而是**"在这个临床场景 + 这个孕周 + 这个母体合并症下，哪个药该上、哪个药禁用"**。同一个方向（促宫缩 / 保胎 / 降压）往往有一线到多线，**排药靠禁忌**：产后出血看有没有 **高血压 / 哮喘**，降压看是不是 **ACEI/ARB**，保胎看**孕周**。把每类药和它的"一句话禁忌钩子"绑死，就能秒杀绝大多数题。

---

## 〇、总览：按"临床目的"分类

```text
产科用药
│
├─ 促宫缩 (让子宫收缩)
│    ├─ 引产/催产 (induction/augmentation) ── Oxytocin、Misoprostol/Dinoprostone(促宫颈成熟)
│    └─ 产后止血 (PPH 宫缩剂) ─────────────── Oxytocin → Methylergonovine → Carboprost → Misoprostol (+ TXA)
│
├─ 抑宫缩 (保胎 tocolysis) ──────────────────── Nifedipine / Indomethacin / Terbutaline   ▶见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_早产管理_孕周分层与药物]]
│
├─ 保护胎儿 (与宫缩无关)
│    ├─ 促胎肺成熟 ── Betamethasone / Dexamethasone (< 34–37 周)
│    └─ 神经保护 ─── Magnesium sulfate (< 32 周)              ▶见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_硫酸镁临床应用与镁中毒]]
│
├─ 母体合并症
│    ├─ 妊娠期高血压/子痫前期 ── 急性: Labetalol/Hydralazine/IR-Nifedipine；慢性: Labetalol/Nifedipine/Methyldopa
│    ├─ 子痫抽搐预防/治疗 ────── Magnesium sulfate
│    └─ VTE 预防/治疗 ─────────── LMWH / UFH (肝素不过胎盘；华法林禁用)
│
├─ 感染预防
│    ├─ GBS 产时预防 ── Penicillin G                          ▶见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_GBS_产时抗生素预防IAP]]
│    ├─ PPROM latency ─ Ampicillin + Azithromycin
│    └─ 绒毛膜羊膜炎 ── Ampicillin + Gentamicin               ▶见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_产科新生儿感染抗生素]]
│
├─ 同种免疫预防 ── Anti-D immunoglobulin (RhoGAM)             ▶见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_产后补充_疫苗Rhogam筛查]]
│
└─ 对症 ── NVP/剧吐: Pyridoxine(B6)+Doxylamine   ▶见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_早孕恶心呕吐与妊娠剧吐鉴别]]
```

> [!danger] 方向相反的药，题里放一起就是干扰项
> **保胎场景**里出现任何促宫缩药 (Oxytocin 缩宫素 / Misoprostol 米索前列醇 / Ergonovine 麦角新碱 / Mifepristone 米非司酮) → 一律排除。
> **产后止血 / 引产场景**里出现保胎药 (Nifedipine / Indomethacin / Terbutaline) → 一律排除。
> 先认场景方向，再挑禁忌，能砍掉一半选项。

---

## 一、缩宫素 Oxytocin（催产素）

> [!info] 原理 · 适应症 · 禁忌
> - **原理**：合成后叶催产素，激动子宫平滑肌 **oxytocin receptor** → 频率/强度依赖性宫缩；产后促子宫收缩压迫螺旋动脉止血。
> - **适应症**：① **引产 / 加强产程** (induction / augmentation)；② **产后出血 (PPH, postpartum hemorrhage) 一线预防与治疗**（第三产程常规给）；③ 流产/胎死宫内后促排。
> - **禁忌 / 注意**：
>   - **快速大剂量 IV 推注** → 低血压 (hypotension)、反射性心动过速；
>   - 结构类似 ADH (antidiuretic hormone, 抗利尿激素) → 长时间大量输注 + 低张液 → **水中毒 / 低钠血症 (hyponatremia)**；
>   - **子宫过度刺激 (tachysystole)** → 胎心异常；处理是**停缩宫素 + 侧卧 + 补液 + 吸氧**，必要时 **Terbutaline (特布他林) 急性宫缩抑制**。
>   - 头盆不称 / 横位等**不宜阴道分娩**者禁止引产。

---

## 二、产后出血 (PPH) 宫缩剂阶梯 ⭐

> [!success] 记忆链：缩宫素 → 麦角(避高血压) → 前列腺素(避哮喘) → 米索(啥都能用)
> 每一步的"跳过条件"就是它的禁忌，这正是 UWorld 最爱考的钩子。

| 顺序 | 药物 (中英) | 原理 | 一句话禁忌钩子 |
|---|---|---|---|
| 1 | **Oxytocin 缩宫素** | 激动缩宫素受体 | 一线；快推致低血压 |
| 2 | **Methylergonovine 甲基麦角新碱** (麦角碱, ergot alkaloid) | 直接使子宫平滑肌**强直性收缩** | **高血压 / 子痫前期禁用**（血管收缩→高血压危象、卒中） |
| 3 | **Carboprost 卡前列素** (15-methyl PGF2α, Hemabate) | 前列腺素 F2α，促肌层收缩 | **哮喘禁用**（支气管痉挛）；相对慎用于高血压 |
| 4 | **Misoprostol 米索前列醇** (PGE1) | 前列腺素 E1，促宫缩 | 几乎无绝对禁忌，**哮喘/高血压都能用**，常温稳定→资源受限首选 |
| 辅 | **Tranexamic acid 氨甲环酸 (TXA)** | 抗纤溶（抑制纤溶酶原激活） | 产后 **3 小时内**加用；活动性血栓栓塞慎用 |

> [!warning] 高频陷阱：先判母体合并症再选药
> - stem 给 **哮喘 (asthma)** → 别选 Carboprost，选 **Oxytocin / Methylergonovine / Misoprostol**。
> - stem 给 **高血压 / 子痫前期 (HTN/preeclampsia)** → 别选 Methylergonovine，选 **Oxytocin / Carboprost / Misoprostol**。
> - 两个都占（哮喘 + 高血压）→ **Oxytocin / Misoprostol**。
> - 别忘了 PPH 第一步永远是 **子宫按摩 (uterine massage) + 缩宫素**，宫缩乏力 (uterine atony) 是 PPH 最常见病因。
>
> 📌 源错题：[[mistakes/uworld-mistakes_2026-07#^Q16489]]（子宫乏力 PPH + 慢性高血压 → 避开甲基麦角新碱）

---

## 三、引产 / 促宫颈成熟 (Cervical ripening & Induction)

> [!info] 原理 · 适应症 · 禁忌
> - **前列腺素类促宫颈成熟**（Bishop 评分低、宫颈未成熟时）：
>   - **Misoprostol 米索前列醇 (PGE1)**：口服/阴道，促宫颈软化 + 宫缩；也用于药物流产（+ Mifepristone）、PPH。
>   - **Dinoprostone 地诺前列酮 (PGE2)**：阴道栓/凝胶促宫颈成熟。**哮喘、青光眼慎用**；用后需间隔再上缩宫素。
> - **机械法**：Foley 球囊 (mechanical dilation)——**哮喘/心脏病等前列腺素禁忌时的替代**。
> - **Oxytocin**：宫颈已成熟后加强产程。
>
> [!danger] 前列腺素 + 子宫瘢痕 = 子宫破裂
> 有 **既往剖宫产 / 子宫手术史 (prior C-section / uterine surgery)** 尤其**古典式切口**者，用 Misoprostol/Dinoprostone 促宫颈成熟 → **子宫破裂 (uterine rupture)** 风险显著升高，**禁用前列腺素引产**；TOLAC (trial of labor after cesarean, 剖宫产后试产) / VBAC (vaginal birth after cesarean, 剖宫产后阴道分娩) 走机械法 + 谨慎缩宫素。

---

## 四、保胎药 Tocolytics（抑制宫缩）

> [!note] 详见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_早产管理_孕周分层与药物]]，此处速查禁忌
> **总适应症**：确诊早产临产 (preterm labor：规律宫缩 + 宫颈变化)，孕 **24–33 6/7 周**，目的只是**延迟分娩 ~48h** 给倍他米松起效争取时间；**≥34 周一般不再保胎**。

| 药物 (中英) | 原理 | 首选孕周 | 关键禁忌 |
|---|---|---|---|
| **Indomethacin 吲哚美辛** (NSAID, 非甾体抗炎药) | 抑制前列腺素合成 | **< 32 周** | **≥32 周禁用**：动脉导管早闭 + 羊水过少（胎肾灌注↓） |
| **Nifedipine 硝苯地平** (CCB, 钙通道阻滞剂) | 阻钙内流→平滑肌松弛 | **32–34 周** | 母体低血压；与硫酸镁合用叠加低血压/神经肌肉抑制 |
| **Terbutaline 特布他林** (β2 激动剂) | 升 cAMP→子宫松弛 | 仅急性救援 ≤48–72h | 母体心脏病/心律失常、未控糖尿病；FDA 禁长期维持 |

> [!tip] 口诀：早用吲哚(<32)，中用硝苯(32–34)，特布只救急

---

## 五、产前糖皮质激素 (Antenatal corticosteroids)

> [!info] 原理 · 适应症 · 禁忌
> - **原理**：**Betamethasone 倍他米松 / Dexamethasone 地塞米松**穿过胎盘 → 加速 **II 型肺泡细胞产生表面活性物质 (surfactant)** → 降低 **RDS (新生儿呼吸窘迫综合征)**、**IVH (脑室内出血)**、**NEC (坏死性小肠结肠炎)**、新生儿死亡。
> - **适应症**：有早产风险、孕 **< 34 周**（ACOG, 美国妇产科医师学会 可放宽至 **34–36 6/7 周** late preterm 晚期早产单疗程）；PPROM (未足月胎膜早破) 也用。**24h 起效、48h 达峰**——保胎争取的就是这 48h。
> - **禁忌 / 注意**：临床绒毛膜羊膜炎不因激素而延误分娩；母体血糖会短暂升高（GDM, gestational diabetes mellitus, 妊娠期糖尿病 需监测）。选 Betamethasone/Dexamethasone 是因为**能过胎盘**——泼尼松/氢化可的松被胎盘 11β-HSD2 大量灭活，达不到胎儿。

---

## 六、硫酸镁 Magnesium sulfate

> [!note] 详见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_硫酸镁临床应用与镁中毒]]
> - **原理**：拮抗 NMDA / 稳定膜 + 竞争钙 → 抗惊厥 + 平滑肌松弛。
> - **两大适应症**（务必分清）：
>   1. **子痫抽搐预防与治疗** (eclampsia seizure prophylaxis/treatment)——**子痫前期伴严重表现 (preeclampsia with severe features) / 子痫**首选，不是降压药！
>   2. **胎儿神经保护** (fetal neuroprotection)——孕 **< 32 周**早产，降脑瘫。
> - **禁忌 / 中毒**：**重症肌无力 (myasthenia gravis) 禁用**（可致危象）；肾功能不全减量。
>   - **镁中毒序列**：深腱反射消失 (loss of DTR) → 呼吸抑制 → 心脏骤停；
>   - **解毒剂 = 葡萄糖酸钙 (calcium gluconate)**。

---

## 七、妊娠期高血压用药 (Antihypertensives)

> [!success] 分两个场景：急性重度 vs 慢性维持
> **降压不等于抗抽搐**——子痫抽搐用硫酸镁，血压 ≥160/110 才用降压药，两者常同时上。

| 场景 | 一线药 (中英) | 原理 |
|---|---|---|
| **急性重度高血压** (≥160/110，需 30–60min 内降) | **Labetalol 拉贝洛尔** (IV, α/β 阻滞) · **Hydralazine 肼屈嗪** (IV, 直接扩血管) · **即释 Nifedipine 硝苯地平** (po) | 快速降压、器官保护 |
| **慢性 / 维持** | **Labetalol · Nifedipine (缓释) · Methyldopa 甲基多巴** (中枢 α2 激动) | 长期控压，胎儿安全数据好 |

> [!danger] 妊娠期降压绝对禁忌（致畸，见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_孕期致畸药]]）
> - **ACEI / ARB（普利类 / 沙坦类）禁用**：中晚孕致**胎儿肾发育不良 (renal dysgenesis)、羊水过少 (oligohydramnios)、颅骨发育不全**。
> - **Atenolol 阿替洛尔**：与 **胎儿生长受限 (FGR)** 相关，避免。
> - **硝普钠 (Nitroprusside)**：久用**氰化物 (cyanide) 蓄积**风险，仅极端难治时短用。

---

## 八、感染预防用药

> [!info] 三个经典组合
> - **GBS (B 组链球菌) 产时预防**：**Penicillin G 青霉素 G** 首选（详见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_GBS_产时抗生素预防IAP]]）。
>   - 青霉素过敏低危 → **Cefazolin 头孢唑林**；高危(过敏性休克史) → 药敏定 **Clindamycin 克林霉素**，耐药则 **Vancomycin 万古霉素**。
> - **PPROM latency（未足月胎膜早破延长孕周）**：**Ampicillin 氨苄西林 + Azithromycin 阿奇霉素**（7 天），延长潜伏期 + 降感染。
> - **绒毛膜羊膜炎 (chorioamnionitis)**：**Ampicillin + Gentamicin 庆大霉素**（剖宫产加 Clindamycin/甲硝唑覆盖厌氧）+ **尽快分娩**（唯一根治）。

---

## 九、Rh 同种免疫预防 (Anti-D immunoglobulin, RhoGAM)

> [!info] 原理 · 适应症 · 禁忌
> - **原理**：被动输入的**抗-D 抗体**结合并清除进入母体的胎儿 RhD+ 红细胞 → 阻止母体**主动致敏 (alloimmunization)** 产生自身抗-D。
> - **适应症**：**Rh(D) 阴性、抗体筛查阴性 (unsensitized)** 的孕妇：① 孕 **28 周**常规；② 分娩后 **72h 内**（若新生儿 Rh+）；③ 任何**致敏事件**后（流产、异位妊娠、羊穿、外倒转、腹部外伤、产前出血）。
> - **禁忌 / 无效**：**已致敏（抗体筛查阳性）→ RhoGAM 无用**（此时管理转为监测胎儿贫血 MCA 多普勒）；Rh 阳性母亲不需要。详见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_产后补充_疫苗Rhogam筛查]]。

---

## 十、其他对症 & "孕期禁用"红名单

> [!info] 对症
> - **NVP / 妊娠剧吐 (nausea/vomiting, hyperemesis)**：一线 **Pyridoxine 维生素 B6 ± Doxylamine 多西拉敏**；升级 antihistamine → Metoclopramide 甲氧氯普胺 / Ondansetron 昂丹司琼（详见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_早孕恶心呕吐与妊娠剧吐鉴别]]）。
> - **VTE (venous thromboembolism, 静脉血栓栓塞) 预防/治疗**：**LMWH 低分子肝素 / UFH 普通肝素**——**不过胎盘**，孕期抗凝首选；**华法林 (Warfarin) 禁用**（致畸）。

> [!danger] 孕期常见"禁用/致畸"药（选择题黑名单，详见 [[完整笔记/专题笔记/OB_GYN/OB_GYN_孕期致畸药]]）
> ACEI/ARB · Warfarin 华法林 · Valproate 丙戊酸 / 其他部分抗癫痫药 · Isotretinoin 异维A酸 · Methotrexate 甲氨蝶呤 · Tetracyclines 四环素类 · Fluoroquinolones 氟喹诺酮 · Aminoglycosides 氨基糖苷（耳毒）· 中晚孕 NSAIDs（导管早闭）· Misoprostol（想保胎时）。

---

## 复习自测

> [!question]- Q1. 阴道分娩后宫缩乏力大出血，缩宫素 + 按摩后仍出血。既往哮喘史。下一步宫缩剂选？
> **Methylergonovine 甲基麦角新碱**（若无高血压）。**不能选 Carboprost 卡前列素**——哮喘诱发支气管痉挛。若同时有高血压 → 选 **Misoprostol 米索前列醇**。

> [!question]- Q2. 产后出血，患者有子痫前期（BP 168/112）。麦角碱能用吗？
> **不能**。Methylergonovine 收缩血管 → 高血压危象/卒中。选 **Oxytocin / Carboprost（无哮喘时）/ Misoprostol**。

> [!question]- Q3. 孕 30 周先兆早产，该上哪些药、各自目的？
> ① **Betamethasone 倍他米松**（<34 周，促胎肺成熟）；② **Magnesium sulfate 硫酸镁**（<32 周，胎儿神经保护）；③ **Tocolytic**（如 Indomethacin，<32 周首选）延迟分娩 48h 让激素起效；④ 据 GBS 状态预防。

> [!question]- Q4. 子痫前期伴严重表现，BP 165/115 且诉头痛。硫酸镁是用来降压的吗？
> **不是**。硫酸镁是**抗抽搐（子痫预防）**；降压另用 **Labetalol / Hydralazine / 即释 Nifedipine**。两者同时上。

> [!question]- Q5. 既往古典式剖宫产史，需引产。为什么不用 Misoprostol？
> 前列腺素 (Miso/Dinoprostone) 在**子宫瘢痕**上显著增加**子宫破裂**风险，禁用；改机械法（Foley）± 谨慎缩宫素，并权衡直接再次剖宫产。

> [!question]- Q6. Rh 阴性孕妇，本次抗体筛查阳性。还给 RhoGAM 吗？
> **不给**——已致敏，RhoGAM 无效。转为**监测胎儿贫血**（MCA, middle cerebral artery, 大脑中动脉 峰值流速多普勒）等。

---

## 关联笔记

- 🔁 源错题：[[mistakes/uworld-mistakes_2026-07#^Q16489]]（PPH 宫缩剂禁忌配对：高血压禁麦角 / 哮喘禁卡前列素）
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_早产管理_孕周分层与药物]]（保胎/激素/硫酸镁孕周阈值）
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_硫酸镁临床应用与镁中毒]]
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_孕期致畸药]]
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_GBS_产时抗生素预防IAP]]
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_产科新生儿感染抗生素]]
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_产后补充_疫苗Rhogam筛查]]
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_早孕恶心呕吐与妊娠剧吐鉴别]]
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_孕期出血鉴别]]
- 分科参考：[[完整笔记/OB]]、[[完整笔记/GYN]]
