---
title: T&T 遗传学 · Ch4 突变与多态（Mutation & Polymorphism）
type: LGG 学习笔记
source: Thompson & Thompson Genetics and Genomics in Medicine, 9th ed
created: 2026-07-08
---

# Ch4 突变与多态（Mutation & Polymorphism）

> 教材 [[10_分子技能自学计划_2026-07]] · 返回 [[00_总览_行动清单]]
> LGG 视角带学：每小节末标"→ 变异解读里怎么用"。

> [!note] 这是"预习课"
> Lesson 1 是 2026-07-08 提前试讲的一课。**正式系统学从 9 月回 LA、有纸质 T&T 后启动**（计划见 [[10_分子技能自学计划_2026-07]] §三）。现在（7–8 月）你专注 OET + Step 2，这篇想翻可翻，不必赶。

---

> [!info]- 缩写全称（本章速查）
> **ACMG** = American College of Medical Genetics and Genomics（美国医学遗传学院）· **AMP** = Association for Molecular Pathology（分子病理协会）· **SNV** = Single Nucleotide Variant（单核苷酸变异）· **CNV** = Copy-Number Variant（拷贝数变异）· **SV** = Structural Variant（结构变异）· **LoF** = Loss-of-Function（功能丧失）· **VUS** = Variant of Uncertain Significance（意义未明变异）· **NGS** = Next-Generation Sequencing（二代测序）· **CMA** = Chromosomal Microarray（染色体微阵列）· **PVS1 / BA1 / BS1** = ACMG 证据码（Pathogenic Very Strong 1 / Benign Standalone 1 / Benign Strong 1）

## Lesson 1（2026-07-08）：术语 + 变异分类

### 一、术语的现代转向 ⭐（LGG 最爱考的第一课）

| 老说法 | 新说法（ACMG/AMP 现行） |
|---|---|
| **Mutation（突变）** = 致病的罕见改变 | 一律叫 **Variant（变异）** |
| **Polymorphism（多态）** = 常见(>1%)、良性 | 用**临床意义**分类，不用频率贴标签 |

> [!important] 核心观念
> 现代临床遗传**不再用 mutation / polymorphism 这对词**（带预设：mutation=坏、polymorphism=好，会误导）。统一称 **variant（变异）**，再按**临床意义五分类**判定：
> **Pathogenic(P，致病) / Likely Pathogenic(LP，可能致病) / VUS(意义未明) / Likely Benign(LB) / Benign(B)**。
> → 变异解读里怎么用：面试若问"mutation 和 polymorphism 区别"，高级答法是"我会避免这两个词，改用 variant + 意义分类"——直接体现你懂 ACMG 语言。

### 二、按"大小"分类变异

```
变异按大小谱系（小 → 大）
├─ SNV 单核苷酸变异（Single Nucleotide Variant）—— 1 个碱基替换
├─ Indel 小插入/缺失（Insertion/Deletion）—— 几~几十 bp
├─ SV 结构变异（Structural Variant）
│    ├─ CNV 拷贝数变异（Copy-Number Variant，缺失/重复）
│    ├─ Translocation 易位 · Inversion 倒位
└─ Aneuploidy 非整倍体（整条染色体增减，如 +21）
```

> → 变异解读里怎么用：**不同大小用不同技术+不同标准**。SNV/indel 走 NGS + ACMG/AMP 2015；CNV 走 CMA + ACMG/ClinGen CNV 标准；非整倍体走核型/CMA。这条决定你"该用哪套 SOP"。

### 三、按"对蛋白的效应"分类（编码区 SNV/indel）⭐⭐

| 类型 | 英文 | 效应 | LGG 关键 |
|---|---|---|---|
| 同义/沉默 | Synonymous / Silent | 氨基酸不变 | 多为良性 **但可能影响剪接** ⚠️ |
| 错义 | Missense | 换 1 个氨基酸 | 意义常不确定，需多证据 |
| 无义 | Nonsense | 提前终止密码子 | 常 **功能丧失 LoF** |
| 移码 | Frameshift | indel 非 3 倍数 → 阅读框错位 | 常 **LoF** |
| 整码插入/缺失 | In-frame indel | 增减氨基酸，框不变 | 效应中等 |
| 剪接位点 | Splice site | 破坏剪接 | 常严重 |
| 起始/终止丢失 | Start-loss / Stop-loss | 起始或终止异常 | 视情况 |

> [!tip] LoF（Loss-of-Function，功能丧失）四剑客 → ACMG **PVS1（Very Strong 致病证据）**
> **Nonsense（无义）· Frameshift（移码）· Canonical splice（经典剪接 ±1,2）· 起始密码子丢失** —— 这四类若发生在"**LoF 就是致病机制**的基因"上，直接触发最强的 PVS1 证据码。
> ⚠️ 前提：该基因的致病机制**确实是 LoF**（有些病是 gain-of-function，无义反而可能不致病）——这是 PVS1 最大的坑。

> [!warning] 反直觉点（爱考）
> - **同义变异 ≠ 一定良性**：可能破坏剪接位点 → 仍致病。别看到"氨基酸没变"就判 benign。
> - **等位基因频率高 = 良性证据**：某变异在 gnomAD 人群频率很高 → ACMG **BA1（独立良性）/ BS1**。这就是老"polymorphism"概念的现代量化版。

---

## 🔑 Lesson 1 Buzzwords

- **Variant（变异）** 取代 mutation/polymorphism
- **五分类**：P / LP / VUS / LB / B
- **LoF → PVS1**（前提：基因机制为 LoF）
- **同义变异查剪接**、**高频 → BA1/BS1**

> [!question]- Lesson 1 自测（5 题，先不看答案，答完我判分）
> 见对话；答完后判分详解追加到此处。

---

## Lesson 2（2026-07-10）：突变机制 + 动态突变

> [!note] 从今天起系统学
> OET 7 月考取消后，分子遗传学学习提前启动（见 [[10_分子技能自学计划_2026-07]] 时间线）。本课接 Lesson 1，讲**变异从哪来（机制）+ 一类 LGG 必考的特殊变异（动态突变）**。仍每小节末标 "→ 变异解读里怎么用"。

> [!info]- 本课缩写全称（速查）
> **NER** = Nucleotide Excision Repair（核苷酸切除修复）· **MMR** = Mismatch Repair（错配修复）· **HR** = Homologous Recombination（同源重组修复）· **DSB** = Double-Strand Break（DNA 双链断裂）· **XP** = Xeroderma Pigmentosum（着色性干皮病）· **8-oxoG** = 8-oxoguanine（8-氧代鸟嘌呤，氧化损伤碱基）· **UTR** = Untranslated Region（非翻译区）· **polyQ** = Polyglutamine（多聚谷氨酰胺）· **GoF / LoF** = Gain-/Loss-of-Function（功能获得 / 功能丧失）· **TP-PCR** = Triplet-Repeat-Primed PCR（三核苷酸重复引物 PCR）· **FXTAS** = Fragile X-associated Tremor/Ataxia Syndrome（脆性 X 相关震颤/共济失调综合征）· **FXPOI** = Fragile X-associated Primary Ovarian Insufficiency（脆性 X 相关卵巢早衰）· **MSI** = Microsatellite Instability（微卫星不稳定）· **SBS** = Single-Base-Substitution signature（单碱基替换突变特征，COSMIC）

---

### 一、变异从哪来：自发 vs 诱发（Spontaneous vs Induced）

```
变异来源
├─ 自发 Spontaneous（内源，不需外界诱变剂）
│    ├─ 复制错误 Replication error：DNA 聚合酶掺错碱基
│    │    └─ 重复序列处「打滑」Slippage → 小 indel（微卫星不稳定源头）
│    ├─ 自发脱氨 Deamination ⭐
│    │    ├─ C（胞嘧啶）→ U（尿嘧啶）→ UNG 修复（一般不致突变）
│    │    ├─ 5-methyl-C（5-甲基胞嘧啶）→ T（胸腺嘧啶）→ 难修 → C>T ⭐（CpG 热点，见 §二）
│    │    └─ A（腺嘌呤）→ hypoxanthine（次黄嘌呤）
│    ├─ 脱嘌呤 Depurination → 无碱基位点 abasic site
│    └─ 氧化 Oxidation：8-oxoG（8-氧代鸟嘌呤）与 A 错配 → G>T 颠换
└─ 诱发 Induced（外源诱变剂 Mutagen）
     ├─ 物理 Physical
     │    ├─ 紫外线 UV → 嘧啶二聚体 Pyrimidine dimer（胸腺嘧啶二聚体）→ NER 修复
     │    └─ 电离辐射 Ionizing radiation → 双链断裂 DSB → 染色体断裂/易位
     └─ 化学 Chemical
          ├─ 烷化剂 Alkylating agent（如亚硝胺）→ 加烷基改变配对
          ├─ 碱基类似物 Base analog（5-溴尿嘧啶）→ 掺入错配
          └─ 嵌入剂 Intercalating agent（吖啶橙 Acridine）→ 移码 Frameshift
```

> [!tip] → 变异解读里怎么用：机制 ↔ 修复缺陷 ↔ 突变特征
> 每种诱变机制对应一条**修复通路**，通路缺陷 = 一个**肿瘤易感综合征** + 一种可识别的**突变特征（mutational signature）**：
> - UV / 二聚体 → **NER 缺陷 = 着色性干皮病 Xeroderma Pigmentosum（XP）**；肿瘤里留下 COSMIC（Catalogue of Somatic Mutations in Cancer，癌症体细胞突变目录）**SBS7**（UV 特征，C>T）
> - 错配修复 MMR 缺陷 → **Lynch 综合征（HNPCC，遗传性非息肉病性结直肠癌）** + **微卫星不稳定 MSI**（→ 免疫治疗 pembrolizumab 派姆单抗敏感）
> - 同源重组 HR 缺陷 → **BRCA1/2 相关乳腺/卵巢癌** + HRD（Homologous Recombination Deficiency，同源重组缺陷）特征（→ PARP 抑制剂 奥拉帕利 olaparib）
> - 吸烟 → SBS4（C>A 颠换）
> 面试能把「机制 → 修复 → 综合征 → 用药」串起来讲，非常加分。

---

### 二、Transition vs Transversion + CpG 热点 ⭐

> [!important] 两个必须秒答的概念
> - **Transition（转换）**：嘌呤↔嘌呤 或 嘧啶↔嘧啶（A↔G、C↔T）。**更常见**（约占 2/3），尽管可能的类型更少。
> - **Transversion（颠换）**：嘌呤↔嘧啶（如 C↔A、G↔T）。较罕见。
> 记法：**Trans*i*tion = 同类内换（i 想成 "identical 环结构"）**；transversion = 跨类换。

> [!warning] CpG 热点（LGG 最爱考的突变机制）
> **CpG 二核苷酸**（5'-C 后接 G）里的 C 常被**甲基化**成 5-methyl-C（5-甲基胞嘧啶）→ 自发脱氨变成 **T** → 造成 **C>T（或对链 G>A）transition**。
> - CpG 位点突变率比其他位点高约 **10–40 倍** → 全基因组的**突变热点**。
> - 后果：同一致病位点在**互不相关的多个患者**反复出现（recurrent variant），常见于 *TP53*、*MECP2*、*FGFR3*（软骨发育不全 Achondroplasia 的 G1138A 复现突变）等。

> [!tip] → 变异解读里怎么用
> CpG 位点的**复现性**本身就是致病证据：ACMG 证据码 **PS1**（同一氨基酸改变已知致病）、**PM5**（同一位点不同改变致病）常因 CpG 复现而触发。看到"多个无关患者同一 C>T 位点"，先想 CpG 热点。

---

### 三、动态突变 / 三核苷酸重复扩增 ⭐⭐（Dynamic Mutation / Trinucleotide Repeat Expansion）

> [!important] 核心概念：不稳定重复 + 遗传早现 Anticipation
> 一段短重复序列在**代际传递中不断变长**（unstable expansion）→ 表现为 **anticipation（遗传早现）**：一代比一代**发病更早、更重**。这是动态突变病的临床指纹。

```
三核苷酸重复扩增病（按重复位置 → 机制方向）
├─ 编码区 CAG →（多聚谷氨酰胺 polyQ）→ 毒性获得 Gain-of-Function
│    ├─ 亨廷顿病 Huntington disease  HTT 基因(CAG)  常染色体显性 AD
│    └─ 多种脊髓小脑共济失调 SCA · 脊髓延髓肌萎缩 SBMA
├─ 5'UTR（5' 非翻译区）CGG → 甲基化沉默 → Loss-of-Function
│    └─ 脆性 X 综合征 Fragile X  FMR1 基因(CGG)  X 连锁
├─ 3'UTR（3' 非翻译区）CTG → RNA 毒性（剪接紊乱）
│    └─ 强直性肌营养不良 1 型 Myotonic dystrophy type 1  DMPK 基因(CTG)  AD
│         （2 型 DM2 = CCTG 四核苷酸重复, CNBP 基因）
└─ 内含子 Intron  GAA → 转录沉默 → Loss-of-Function  ⚠️双重例外
     └─ 弗里德赖希共济失调 Friedreich ataxia  FXN 基因(GAA)  常染色体隐性 AR
        （唯一常见的「AR + 内含子重复」，与其余"AD + 编码/UTR"都不同）
```

> [!warning] 前突变 vs 全突变（Premutation vs Full mutation，以脆性 X 为例，接 [[13_LGG复习大纲_germline_somatic双线]]）
> *FMR1* CGG 重复数分档：
> - 正常 <45 · 中间 45–54 · **前突变 55–200**（不甲基化，携带者可发 **FXTAS 震颤/共济失调** 或 **FXPOI 卵巢早衰**）· **全突变 >200**（甲基化沉默 *FMR1* → 智力障碍 Intellectual disability）。
> - **母源传递**时前突变→全突变的扩增风险最高（是否扩增与性别、重复数相关）。

> [!tip] → 变异解读里怎么用（承 [[13_LGG复习大纲_germline_somatic双线]] 的"技术要匹配变异类型"）
> **标准 NGS / Sanger 测不出重复数**（GC 富集、同聚物区读不准）→ 临床怀疑动态突变时必须用 **TP-PCR（三核苷酸重复引物 PCR）/ Southern blot**。
> 面试线索链：**家族里一代比一代早发（anticipation）→ 想动态突变 → 选重复专项检测**，而不是套 NGS。

---

### 四、变异的功能后果（承 Lesson 1 的 PVS1 坑）

> [!info] 三种致病方向，决定"无义/移码是不是就致病"
> - **功能丧失 LoF（Loss-of-Function）**：无义/移码/经典剪接使蛋白失活。若该基因**致病机制确实是 LoF** → 触发 ACMG **PVS1（最强致病证据）**。单倍剂量不足 Haploinsufficiency 属此。
> - **功能获得 GoF（Gain-of-Function）**：如亨廷顿 polyQ 毒性、软骨发育不全 *FGFR3* 组成性激活。⚠️ 这类基因上**无义突变反而可能不致病**（把蛋白敲没了反而没毒性）——这就是 Lesson 1 说的 **PVS1 最大的坑**。
> - **显性负性 Dominant-negative**：突变蛋白干扰正常等位基因产物（如部分成骨不全 Osteogenesis imperfecta 的胶原突变）。
>
> 对照动态突变：亨廷顿(CAG/polyQ) = **GoF**；脆性 X(CGG 沉默 *FMR1*) = **LoF**——同是重复扩增，机制方向相反。深度机制留待后续课。

---

## 🔑 Lesson 2 Buzzwords

- **自发脱氨**：5-methyl-C → T = **CpG C>T transition 热点**（复现变异 → PS1/PM5）
- **Transition（A↔G/C↔T）> Transversion**；同类内换记 "i = identical 环"
- **UV → 嘧啶二聚体（NER/XP）**；**氧化 8-oxoG → G>T 颠换**；机制↔修复缺陷↔肿瘤综合征↔用药
- **动态突变 → anticipation（遗传早现）**；**CAG 编码 = polyQ = GoF（亨廷顿）**；**CGG 5'UTR = FMR1 沉默 = LoF（脆性 X）**；**GAA 内含子 = Friedreich = AR 例外**
- **重复扩增 NGS/Sanger 测不出 → TP-PCR / Southern**

> [!question]- Lesson 2 自测（5 题，先不看答案，答完我判分）
> 1. 一个 C>T 变异在多个互不相关的患者身上反复出现在**同一个** CpG 位点。从突变**机制**角度，为什么这个位点是热点？这种"复现性"对应哪个/哪些 ACMG 证据码？
> 2. 弗里德赖希共济失调 Friedreich ataxia 在动态突变病里有两个"反常"特征，是哪两个？（提示：遗传方式 + 重复所在位置）
> 3. 为什么标准 NGS panel 测不出脆性 X 的 CGG 扩增？临床怀疑时该改用什么方法？
> 4. 亨廷顿病(CAG)和脆性 X(CGG)都是重复扩增病，但致病机制方向相反——分别是 gain 还是 loss of function？为什么脆性 X 是 loss？
> 5. 紫外线 UV 主要造成哪种 DNA 损伤？由哪条修复通路修复？该通路缺陷对应哪个遗传病（中英文）？
> 
> （答完后判分详解追加到此处。）

---

<!-- Lesson 3 待续：Ch4 收尾 → 转 Ch7 单基因遗传方式（AD/AR/X-linked/线粒体、外显率、镶嵌）；或按需先补"变异的功能后果"深度机制 -->

## 🔗 关联

- 📚 怎么学 + 资源：[[10_分子技能自学计划_2026-07]]
- 📚 学什么（germline/somatic 双线 + 面试话术）：[[13_LGG复习大纲_germline_somatic双线]]（脆性 X CGG、DMD、血友病 F8 倒位的方法学坑正是本课 §三"技术匹配变异类型"的应用）
- 🎯 目标校三标准：[[邮件存档/Yale_耶鲁]]（variant analyst / bioinformatics 短板）
- 🗂️ 项目全局：[[00_总览_行动清单]]
