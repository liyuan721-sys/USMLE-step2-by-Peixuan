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

<!-- Lesson 2 待续：Ch4 剩余（突变机制/自发 vs 诱发、CpG 热点、动态突变三核苷酸重复） -->
