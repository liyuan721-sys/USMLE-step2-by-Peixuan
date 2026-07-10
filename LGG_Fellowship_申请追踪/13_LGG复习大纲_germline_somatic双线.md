---
title: LGG 复习大纲 — germline / somatic 双线（从实验室真实业务出发）
type: LGG 备考-知识复习大纲
created: 2026-07-10
source: 姜楠同事对实验室二类检测业务的描述（遗传病检测 + NGS 肿瘤检测 + Epic + 分析 server）
---

# LGG 复习大纲 — germline / somatic 双线

> 返回 [[00_总览_行动清单]] · 技能自学计划 [[10_分子技能自学计划_2026-07]] · 教材学习 [[T&T遗传学学习/Ch04_突变与多态_Mutation]]

> [!info] 这篇是干嘛的
> 同事描述的实验室二类检测业务——**① 遗传病检测**（autism / 进行性肌营养不良 / 凝血因子 F8·F9）+ **② NGS 肿瘤基因检测**（血液病 / 肺癌 / 乳腺癌）+ 平台（Epic / 分析 server）——几乎就是 **LGG（Laboratory Genetics and Genomics，实验室遗传学与基因组学）fellowship 的核心工作范围本身**。本篇把它翻译成"复习地图 + 面试素材"：按 LGG 的 **germline（胚系/遗传性）** 和 **somatic（体系/肿瘤性）** 双线拆开，每个病配「方法学 → 判读要点 → 面试话术」三问。
>
> 与 [[10_分子技能自学计划_2026-07]] 的分工：**10 = 怎么学 + 资源清单**（ACMG/AMP 指南、ClinGen VCI、IGV、认证课程）；**13（本篇）= 学什么**（具体病种的知识骨架 + 面试能开口讲的内容）。两篇配套用。

> [!info]- 缩写全称对照（首次出现速查）
> - **LGG** = Laboratory Genetics and Genomics（实验室遗传学与基因组学，ABMGG 认证 fellowship）
> - **germline / constitutional** = 胚系 / 体质性变异（遗传性，全身细胞都带）· **somatic** = 体系变异（肿瘤后天获得，仅肿瘤细胞带）
> - **CMA** = Chromosomal Microarray（染色体微阵列）· **CNV** = Copy-Number Variant（拷贝数变异）
> - **MLPA** = Multiplex Ligation-dependent Probe Amplification（多重连接依赖式探针扩增，查大片段 del/dup）
> - **NGS** = Next-Generation Sequencing（二代测序）· **VAF** = Variant Allele Frequency（变异等位基因频率）
> - **ACMG/AMP** = American College of Medical Genetics and Genomics / Association for Molecular Pathology
> - **ASCO** = American Society of Clinical Oncology · **CAP** = College of American Pathologists
> - **EHR** = Electronic Health Record（电子病历系统，Epic 属此）· **LIMS** = Laboratory Information Management System（实验室信息系统）
> - **VUS** = Variant of Uncertain Significance（意义未明变异）· **HGVS** = 变异命名标准

---

## 一线：Germline / Constitutional 检测（遗传病）⭐

> [!tip] LGG 核心分野：先分清 germline vs somatic
> 面试官最爱确认你有没有这个"框架反射"：**同一个基因变异，胚系和体系的判读逻辑完全不同**。
> - germline → 用 **ACMG/AMP 2015**（五分类 P/LP/VUS/LB/B），关心遗传方式、家族风险、外显率
> - somatic → 用 **AMP/ASCO/CAP 2017**（四层 Tier I–IV），关心可用药性、预后、诊断分型
> 下面三个遗传病是这条线的经典代表，方法学各有一个"必须专门做否则漏诊"的坑。

### 1. 自闭症 Autism / 智力发育障碍（ID/DD/ASD）

```
检测阶梯（first-tier → 逐级）
  第一层  Chromosomal Microarray (CMA, 染色体微阵列)  ← 首选，查 CNV
          + Fragile X (FMR1 CGG 重复) 一起做
  第二层  Exome / Genome Sequencing（外显子/全基因组测序）
          ← 新指南（ACMG 2021）已推为先天异常/DD/ID 的一线之一
  ※ 常规核型（karyotype）敏感度低，已非首选（除非疑非整倍体/易位）
```

- **方法学**
  - CMA 查 **拷贝数变异 CNV**（微缺失/微重复），DD/ID/ASD 的诊断率约 15–20%。
  - Fragile X = **FMR1 基因 5' UTR 的 CGG 三核苷酸重复扩增**：正常 <45 / 中间 45–54 / 前突变 55–200 / 全突变 >200(伴甲基化)。用 PCR + Southern blot(或 TP-PCR)，普通测序测不出重复数。
- **判读要点**
  - CNV 判读用 **ACMG/ClinGen 2020 五分类 + 打分**（cnvcalc.clinicalgenome.org）：看基因内容、已知致病区、大小、遗传自父母还是 de novo。
  - de novo + 覆盖已知致病基因/区 → 权重高;遗传自正常父母 → 倾向良性。
- **面试话术**：*"For ASD/DD I'd start with CMA plus fragile X testing as first-tier, then move to exome if negative — that's the ACMG-recommended algorithm, and I'd score any CNV with the ClinGen calculator."*

### 2. 进行性肌营养不良 Progressive Muscular Dystrophy（DMD / BMD）

```
DMD（dystrophin，Xp21，人类最大基因，79 外显子），X-linked recessive
检测阶梯
  第一步  MLPA / aCGH  查大片段外显子 del(≈65–70%) / dup(≈10%)
  第二步  若 MLPA 阴  → 测序查点突变/小 indel(≈25–30%)
关键规则：Reading-frame rule（阅读框规则，Monaco）
  out-of-frame（移码）→ 无功能 dystrophin → Duchenne（重）
  in-frame（保框）    → 部分功能 dystrophin → Becker（轻）
  ≈90% 病例符合此规则
```

- **方法学坑**：**大片段缺失是主因** → 必须先做 **MLPA**（普通测序对整个外显子纯合缺失反而会"看不到 = 假阴/漏判"）。这是 germline 检测里"选错方法就漏诊"的经典例子。
- **判读要点**：拿到 del/dup 后**先算阅读框**判 Duchenne vs Becker，直接影响预后与治疗（如 exon-skipping 反义寡核苷酸药按具体外显子设计）。
- **面试话术**：*"DMD is deletion-rich, so MLPA comes before sequencing; once I have the deletion I apply the reading-frame rule to predict Duchenne versus Becker."*

### 3. 凝血因子 F8 / F9（血友病 Hemophilia A / B）

```
Hemophilia A = F8 缺陷（Xq28）  |  Hemophilia B = F9 缺陷
两者均 X-linked recessive
F8 检测关键坑：intron 22 inversion（22 号内含子倒位）
  → 占「重型」血友病 A 约 45–50%！
  → 普通测序 / NGS 测「不出」倒位（断点在重复序列）
  → 必须专门做 inverse-shifting PCR / long-range PCR / Southern
阶梯：重型 A 先查 Inv22 → 阴再查 intron1 倒位 → 再测序
F9：以点突变为主 → 直接测序即可
```

- **方法学坑（面试高频）**：**结构变异（倒位）标准测序漏检** → 重型血友病 A 必须先做倒位专项。和 DMD 一样，都是"技术选择决定成败"的招牌案例。
- **判读要点**：X 连锁 → 女性携带者风险评估、产前诊断意义;F8 抑制物风险与突变类型相关。
- **面试话术**：*"Severe hemophilia A is driven by the intron-22 inversion in ~45% of cases, which NGS can't see — so I'd run inversion-specific PCR first before sequencing."*

> [!success] 一线小结：三个"方法学决定诊断"的招牌
> Autism→**先 CMA**（不是核型）· DMD→**先 MLPA**（不是测序）· 重型 HemA→**先查 Inv22**（测序漏）。
> 这三条串起来讲，就展示了 LGG 核心能力：**根据变异类型选对技术**（CNV/结构变异 vs 点突变各有专属方法）。

---

## 二线：Somatic / Oncology 检测（NGS 肿瘤基因）⭐ 你的主场

> [!tip] 这条线是你的锚
> 你有病理科背景 + 分子科研经验（gene rearrangement / molecular markers / 肿瘤分子机制），肿瘤 somatic 是你最能接得上、面试最能出彩的部分。核心技能 = **变异分层判读（AMP/ASCO/CAP 2017 四层）** + **germline/somatic 桥接**。

### 1. 血液病 Hematologic malignancies

```
Myeloid panel（AML/MDS/MPN）常见基因
  点突变类  FLT3(ITD/TKD) · NPM1 · CEBPA · IDH1/IDH2 · DNMT3A · TP53 · RUNX1 · ASXL1
  融合基因  PML-RARA(APL 急性早幼粒白血病,急需) · BCR-ABL1(CML 慢性粒细胞白血病) · CBFB-MYH11 · RUNX1-RUNX1T1
判读联动 WHO/ICC 分型 + 预后分层（ELN）+ 靶向（FLT3i / IDHi）
```

- **要点**：血液肿瘤强调 **VAF（变异等位基因频率）** 解读——区分克隆性造血 vs 真肿瘤、监测 MRD（Measurable Residual Disease，可测残留病）；**融合基因**需 RNA/靶向测序或 FISH，DNA panel 可能漏。

### 2. 肺癌 NSCLC

```
可靶向驱动基因（查到即改变治疗）
  EGFR（exon19 del / L858R 敏感；T790M 耐药）
  ALK 融合 · ROS1 融合 · RET 融合 · NTRK 融合
  BRAF V600E · KRAS G12C · MET exon14 skipping · ERBB2(HER2)
```

- **要点**：**驱动基因互斥**、决定一线靶向药;耐药突变(T790M)决定换药。融合基因优先 RNA-based NGS。

### 3. 乳腺癌 Breast

```
somatic  PIK3CA（→ 阿培利司 alpelisib）· ESR1（内分泌耐药）· TP53
扩增     HER2/ERBB2（IHC 免疫组化 / FISH 荧光原位杂交）
germline BRCA1/2（→ PARP 抑制剂 奥拉帕利 olaparib）← 肿瘤检测里查出胚系的经典桥
```

- **要点（面试金句）**:乳腺/卵巢肿瘤 panel 常"顺带"查出 **germline BRCA** → 触发 **germline confirmation + 遗传咨询 + 家族级联筛查**。这是"肿瘤检测里冒出胚系发现"的招牌场景。

### 4. Somatic 变异分层：AMP/ASCO/CAP 2017（Li MM et al.）

| Tier | 含义 | 例子 |
|---|---|---|
| **Tier I** | 强临床意义(A:该瘤种 FDA 批准药/指南;B:充分证据) | 肺癌 EGFR L858R;乳腺 HER2 扩增 |
| **Tier II** | 潜在临床意义(C:别瘤种批准/试验;D:提示性证据) | 跨瘤种 BRAF V600E |
| **Tier III** | VUS(意义未明) | 罕见错义无证据 |
| **Tier IV** | 良性/likely benign | 已知多态 |

- **判读要点**：somatic 看的是**可用药性/预后/诊断**，不是"致病 vs 良性";证据来自 **OncoKB / CIViC / COSMIC**。
- **面试话术**：*"For somatic variants I use the four-tier AMP/ASCO/CAP framework — tiering by therapeutic and prognostic significance — and I pull evidence from OncoKB and CIViC, not the germline ACMG rules."*

---

## 三线：平台与信息学 —— Epic 其实不是"数据库"⚠️

> [!warning] 一个要说对的概念坑（面试别混）
> 同事说"资料库叫 Epic，全美国都用"——**Epic 是 EHR（电子病历系统）**，负责把报告发回临床、给医生看，**不是遗传实验室的分析核心**。LGG 实际干活分三层，说错会露怯：

```
临床工作流三层（别混）
  ① EHR（Epic 等）        患者层：下医嘱、发报告、临床看结果
  ② LIMS（实验室信息系统）  样本层：样本追踪、流程、报告生成
  ③ Bioinformatics pipeline / 分析 server  数据层：
        FASTQ → 比对(BAM) → variant calling(VCF) → 注释 → 过滤 → 判读(IGV 看图)
        ← 同事说的"分析软件(server)"，也是 LGG 最看重、最易露怯处
```

- **对你的启示**：同事建议"回协和练 Epic + 分析 server",对 LGG 价值最大的是**后者（bioinformatics/server）**——那是临床医生背景申请人最常见的短板，恰是 LGG 核心。
- **LGG 硬要求**：懂 **pipeline 的验证(validation)**——CLIA/CAP 规定的 analytical validity（sensitivity / specificity / LOD 检测下限 / reproducibility）。面试可能问"如何验证一条 NGS pipeline"。
- 详细工具与练法见 [[10_分子技能自学计划_2026-07]] §四（IGV / Galaxy / GATK / VEP）。

---

## 四、面试高频问题 + 你的话术库

> [!question]- Q1. germline 变异和 somatic 变异判读有何不同？
> germline 用 **ACMG/AMP 2015 五分类**（P/LP/VUS/LB/B），围绕致病性、遗传方式、家族风险、人群频率(gnomAD)；somatic 用 **AMP/ASCO/CAP 2017 四层**（Tier I–IV），围绕可用药性、预后、诊断分型，证据来自 OncoKB/CIViC。同一变异两套逻辑。

> [!question]- Q2. 给一个 DD/ID/ASD 患儿，你怎么安排检测？
> First-tier **CMA + Fragile X**，阴性再 **exome/genome**（ACMG 2021 已把 exome 推为一线之一）；任何 CNV 用 ClinGen calculator 打分分类。

> [!question]- Q3. 为什么有些变异标准 NGS 会漏？
> **结构变异 / 大片段 / 重复扩增** NGS 易漏——举三个招牌：DMD 大片段缺失(→MLPA)、重型血友病 A 的 **F8 intron 22 倒位**(→倒位专项 PCR)、Fragile X CGG 扩增(→TP-PCR/Southern)。技术要匹配变异类型。

> [!question]- Q4. 肿瘤 panel 查出一个 BRCA1 变异，下一步？
> 判断像 germline 还是 somatic（VAF≈50% + 在正常组织也有 → 疑 germline）→ 建议 **germline 确认检测 + 遗传咨询 + 家族级联筛查**;若确 germline 致病 → PARP 抑制剂适应 + 家系风险。体现 germline/somatic 桥接意识。

> [!question]- Q5. 你为什么从病理转 LGG？（结合你的背景）
> 病理科副主任 + 大量分子/基因组研究 + gene rearrangement / molecular marker 经验 → 已有分子科研根基，正系统转向**临床级分子诊断**（ACMG/AMP 判读 + 生信）。话术细节见 [[11_文书主模板_Yale三标准]]。

---

## 五、关联

- 🎯 怎么学 + 资源 + 认证课：[[10_分子技能自学计划_2026-07]]（ACMG/AMP 精读、ClinGen VCI 实操、IGV、ACMG Genetics Academy 拿证）
- 📚 教材逐章学习：[[T&T遗传学学习/Ch04_突变与多态_Mutation]]（Thompson & Thompson，9 月起系统学）
- 📄 文书/面试叙事：[[11_文书主模板_Yale三标准]]（把本大纲的方法学案例写进 letter of intent）
- 🗂️ 项目全局：[[00_总览_行动清单]] · [[01_项目详情卡]] · [[12_全项目总表_2026-07]]
- 🤝 目标校短板反馈：[[邮件存档/Yale_耶鲁]]（clinical genetics / bioinformatics / variant analyst 三标准）· [[邮件存档/Pittsburgh_匹兹堡]] / [[邮件存档/Penn_CHOP_费城]]

> [!info] 用词红线（沿用 [[10_分子技能自学计划_2026-07]]）
> 说自己"completed [course] / completed N ClinGen curations"，**别写 "certified in..."**（会被当成执照级认证）。本大纲是知识框架，不代表已获认证。
