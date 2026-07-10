---
tags:
  - biobank
  - reference
title: Biobank 前沿发展方向 + Cedars-Sinai Biobank 情况介绍
date: 2026-07-10
type: 行业参考 / 谈资
note: 与 USMLE 备考无关，独立参考资料（用于与前 biobank 老板交流）
---

# Biobank 前沿发展 + Cedars-Sinai 情况介绍（2026-07-10）

> [!info] 用途
> 面向"跟前 biobank 老板介绍最新进展"的谈资资料。分两部分：**① 全行业前沿发展方向**、**② Cedars-Sinai Biobank 情况**。文末附**期刊/会议/标准/认证**速查 + 可直接开口的几句话。

---

## 第一部分：Biobank 前沿发展方向

一条主线：**从"存死样本的冷库" → "存活功能单元的实验平台" → "标准化、联邦化、AI 可算、监管认可的预测系统"。** 三个关键词：**living（活）、connected（联邦互操作）、predictive（AI-ready 可预测）**。

### 1. 从"冻存库" → living / functional biobank
- 过去 biobank = DNA / 血清 / FFPE（Formalin-Fixed Paraffin-Embedded，福尔马林固定石蜡包埋）组织切片（静态、一次性）
- 方向 = **living biobank**：organoid（类器官）、PDO（patient-derived organoid，患者来源类器官）、iPSC（induced pluripotent stem cell，诱导多能干细胞）系、conditionally reprogrammed cells——能复苏、扩增、给药、读表型
- 意义：从"回顾性关联研究素材" → "**前瞻性功能实验平台**"，同一患者可反复"重测"

### 2. 从"上皮 organoid" → 多细胞 / assembloid
解决 organoid 最大短板（缺 immune / stroma / vascular / microbiome）：
- **Assembloid**：epithelium + immune + fibroblast + neuron 按需拼装
- **Vascularized organoid**：解决尺寸 / 坏死核心 / 灌流
- **Organoid + microbiome co-culture / apical-out / gut-on-chip**
- 趋势：未来库里存的不只"上皮株"，而是**可重构细胞组件 + 装配协议**

### 3. 从"分散小库" → 标准化 + 联邦化 + AI-ready（含金量最高）
**(a) 标准化 / 去动物源**
- Matrigel → **defined synthetic hydrogel**（可控刚度/配体）
- conditioned medium → **recombinant factor**（重组 Wnt surrogate、R-spondin）
- SOP / ISO 认证 → 让不同库数据可比

**(b) 联邦化 + 数据可互操作**
- 单库规模有限 → **federated biobank network**：物理样本分散，metadata / omics / 表型可跨库检索
- **"Data, not samples"**：从"寄冰盒" → "**bring compute to the data**"
- **TRE（Trusted Research Environment）/ Secure Data Environment**：研究者进云端平台跑分析，数据不出门
- 遵循 **FAIR 原则**（Findable / Accessible / Interoperable / Reusable）

**(c) AI-ready + multi-omics 深注释**
- 每株样本带 WGS（whole-genome sequencing，全基因组测序）+ RNA-seq（RNA sequencing，转录组测序）+ 甲基化 + drug response + **high-content imaging（高内涵成像）**
- 喂 ML：从 genotype / omics 预测 drug response 与表型
- **"organoid foundation model / virtual cell"** 概念冒头

### 4. 技术前沿——单细胞、空间、液体活检
- **Single-cell + Spatial**：Human Cell Atlas 式的细胞级 / 空间转录组图谱；未来交付"带空间坐标的细胞级注释"
- **Liquid biopsy biobanking**（液体活检生物样本库）：cfDNA（cell-free DNA，游离 DNA）/ ctDNA（circulating tumor DNA，循环肿瘤 DNA）/ 外泌体采集-稳定-冻存 SOP（standard operating procedure，标准操作流程）成新标准品类，对接 MCED（multi-cancer early detection，多癌种早筛）
- **Microbiome biobank**：stool bank / 菌株库标准化、厌氧冻存

### 5. 临床落地 + 监管认可
- **Patient-derived organoid 指导个体化用药**：CRC（colorectal cancer，结直肠癌）/ PDAC（pancreatic ductal adenocarcinoma，胰腺导管腺癌）药敏预测最扎实；**CF（cystic fibrosis，囊性纤维化）的 organoid swelling assay 已进用药/报销决策**（organoid 进真实医疗决策的标志）
- **FDA Modernization Act 2.0（2022）** 松绑动物实验强制要求 → organoid / organ-on-chip 作为 **NAMs（New Approach Methodologies）** 被官方鼓励，打开制药/毒理市场
- biobank + CRO（contract research organization，合同研究组织）服务化 → 成为药物研发标准 preclinical（临床前）平台

### 6. 治理 / 伦理 / 可持续（易忽略但正在定型）
- **Dynamic consent（动态知情同意）**：活体样本能无限扩增/商业化/编辑，旧的一次性同意不够用 → 可撤回、可分层、数字化；**return of results**（返还有临床意义发现）成新责任
- **Benefit-sharing / IP**：organoid 商业化后患者权益（HeLa 老问题）、niche factor 专利集中（HUB，Hubrecht Organoid Technology，荷兰 Clevers 组衍生的类器官技术公司 等）
- **Sustainability / Green labs**：**-80℃ → -70℃** 省能耗（Freezer Challenge，实验室冰箱节能挑战）、**sample right-sizing**（样本等份合理化）、耗材减塑（ESG，Environmental / Social / Governance，环境-社会-治理 压力真实）

### 7. 最新动向（2025–2026）
- **ISBER 2026 Global Biobanking Congress 首次落地中国大陆**：2026-04-21~23 **深圳**。五大 track：① Bench to Biobank to **One Health**、② **Biospecimen Research**（样本科学）、③ People/Policy & Biobanking、④ **Smart Biobank: AI / Automation / Digitalization**（最热）、⑤ Innovative Technology
- **CAP 认证量翻倍**：CAP Biorepository Accreditation Program（BAP）2012 设立，**2018 年 53 家 → 2024 年 12 月 104 家**（全球）

---

## 第二部分：Cedars-Sinai Biobank 情况介绍

结构是 **"一个企业级中央库 + 若干专病垂直库"**，而且 2024 年已经上了 living biobank（正好卡在上面的前沿趋势）。

### A. 旗舰：Biobank and Research Pathology Resource（企业级中央库）
- **定位**：全院统一 enterprise-wide biorepository，主打 research + precision medicine，提供**高质量、临床注释（clinically-annotated）**样本
- **规模**：**> 150 万份样本**（患者/志愿者捐赠的剩余组织、血液、体液）；支撑**每月 30+ 临床研究**、每年 ~3,500 服务请求、服务 ~120 个实验室；建库 10 年以上，起步有 NIH 部分资助
- **四大 service area**：
  1. Biobanking（采集/QC/冻存）
  2. Histology（组织学）
  3. Research pathology（病理注释、cohort building、**digital pathology**）
  4. Microscopy & image analytics（显微成像 + 图像分析）
- **服务能力**：fee-for-service，含 DNA purification、组织学、成像与图像分析；覆盖"患者入组 → 采集 QC → 组织学表征 → 病理注释 → 队列构建 → 数字病理"全流程
- **Director**：V. Krishnan Ramanujan, PhD, MHDS
- **⭐ 2024 新增 living biobank（含 3D organoid）**——从"死冻存"往"活的功能样本"转，是很新鲜的可聊点

### B. 认证（最能拿出来说的资本）
- **College of American Pathologists（CAP）国际认证，且四个领域全拿**（biobanking / histology / research pathology / microscopy & image analytics）
- **已连续第三年 reaccreditation**，是**全加州仅 6 家**拿到该认证的库之一
- 呼应第一部分的 CAP + ISO 治理话术——Cedars 就是"四领域全认证"的标杆案例

### C. 专病垂直库

**MIRIAD IBD Biobank**（IBD（inflammatory bowel disease，炎症性肠病）Institute 下，很硬核）
- 全称 Material and Information Resources for Inflammatory And Digestive diseases（炎症与消化疾病材料与信息资源）
- 收集**横跨 30 年**，**> 15,000 名 IBD 研究对象**（含 extended family 家系）
- 其中 **~12,000 人有 whole-exome / whole-genome 测序 + GSA（Global Screening Array，全基因组分型芯片）基因分型**
- 带**纵向临床 metadata + 全基因型 + serotype**，定制化 LIMS（Laboratory Information Management System，实验室信息管理系统）管理
- 是 **IBD Genetics Consortium（IBDGC）** 的遗传研究中心之一，样本（含健康对照）分发全球合作者
- 科研影响力：**TL1A（TNFSF15）× Crohn's** 遗传关联研究的重镇之一（2025 有 TL1A×Paneth/microbiota bioRxiv 预印本出自这套体系）

**OncoBiobank**（Cedars-Sinai Cancer 下）
- 肿瘤专库，近年新任命 director——印证"中央库 + 多专病垂直库"的组织架构

### D. 一句话总结 Cedars-Sinai
> **CAP 四领域全认证的企业级中央库（150 万+ 样本、全流程数字病理）+ 专病垂直库（MIRIAD IBD 15,000 人带 WGS、OncoBiobank 肿瘤），2024 年刚上 3D organoid living biobank——从"存样本"往"活的功能样本 + AI/数字病理"方向转，卡在行业最新趋势上。**

---

## 附：期刊 / 会议 / 学会 / 标准 速查

### 核心期刊
| 期刊 | 地位 |
|---|---|
| **Biopreservation and Biobanking**（Mary Ann Liebert） | **本行旗舰**，ISBER 官方刊 |
| **Cell and Tissue Banking**（Springer） | 组织库老牌（移植材料） |
| Open Journal of Bioresources | 资源描述型（可引用 bioresource descriptor） |
| GigaScience / Scientific Data（Nature） | 数据侧 data descriptor，AI-ready 方向 |

大队列**科学产出**通常发 Nature / Nature Genetics / Nature Medicine / Lancet / NEJM（UK Biobank、All of Us 等）。

### 学会 / 组织
- **ISBER**（International Society for Biological and Environmental Repositories）—— 全球最重要，出标准 + 办年会
- **BBMRI-ERIC**（Biobanking and BioMolecular resources Research Infrastructure – European Research Infrastructure Consortium，欧洲生物样本库与生物分子资源研究基础设施）—— 欧洲国家级 biobank 基础设施联盟（federated network 标杆）
- **ESBB** —— 欧洲学会
- 区域：CTRNet（加）、ABNA（澳新）、P3G

### 核心会议
- **ISBER Annual Meeting**（全球头号；2026=深圳 Global Biobanking Congress）
- **Europe Biobank Week (EBW)**（BBMRI-ERIC + ESBB，欧洲头号）
- **NCI（National Cancer Institute，美国国家癌症研究所）Biospecimen Research Network (BRN) Symposium**（样本科学，学术味最重）
- **SLAS**（Society for Laboratory Automation and Screening，实验室自动化与筛选学会）——自动化 / LIMS / 机械臂库
- **AGBT**（Advances in Genome Biology and Technology，基因组生物学与技术进展）——测序组学前沿

### 标准 / 认证
- **ISO 20387:2018**（Biotechnology — Biobanking — General requirements）—— biobank 唯一国际通用认证标准
- **CAP Biorepository Accreditation Program（BAP）**
- **NCI Best Practices for Biospecimen Resources**
- **ISBER Best Practices**（行业事实标准）

---

## 附：三句"开口即镇场"（人话版 —— 先能懂再能说）

> [!tip] 用法
> 先说**【人话版】**（你自己完全懂、能顺口说）。想在老板面前显专业，再从**术语表**里挑一两个洋词点缀——但每个词你都得先知道它啥意思，别硬背。

### 第一句：现在比什么
- **【人话版】**"现在大库比的不是谁样本多，是谁给**每个样本配的数据全**、能不能直接拿去做 AI 分析。英国那个五十万人的大库，把所有人都做了全基因组测序、还测了五千多种蛋白，等于把行业标准重新定了。"
- **【原理一句话】** 从前拼"存了多少管样本"，现在拼"每管样本背后挂了多少层数据（基因、蛋白、影像）"。

### 第二句：这行在往哪转
- **【人话版】**"这行现在从'只管存样本'转向'靠数据说话'——样本不用寄来寄去，研究者进一个**安全的云平台**里做分析，数据一步都不出门，既合规又能算。"
- **【原理一句话】** 值钱的是数据不是样本本身；样本分散各地，数据集中在云端安全分析。

### 第三句：下一波是什么
- **【人话版】**"下一波是'**活样本 + AI**'——类器官已经能帮医生定用药了（美国 2022 年还立法允许它替代一部分动物实验）；大库的数据拿去训练 AI 大模型，biobank 就从'存东西的仓库'变成'能做预测的平台'。连 Cedars 自己 2024 年都上了类器官活体样本库。"
- **【原理一句话】** 样本从"死冻存"变"能培养的活样本"，再叠上 AI，从素材库升级成预测平台。

---

### 小术语表（想点缀时用，每个都先弄懂再说）

| 洋词/简写 | 大白话意思 |
|---|---|
| **per-sample 组学深度** | 每一个样本上挂了多少层数据（基因组/蛋白组/代谢组/影像），层越多越值钱 |
| **AI-ready 注释** | 数据整理成 AI 能直接拿去训练的格式 |
| **WGS（whole-genome sequencing）** | 全基因组测序（把一个人 DNA 全测一遍） |
| **proteomics** | 蛋白质组学（一次测成千上万种蛋白，不只测基因） |
| **wet biobank → data biobank** | 实体样本库 → 数据库（重心从"存瓶子"移到"管数据"） |
| **data not samples** | "值钱的是数据不是样本"——这行现在的口头禅 |
| **TRE（Trusted Research Environment）** | 可信研究环境，就是那个"数据不出门"的安全云平台 |
| **federated learning** | 联邦学习：各家数据不汇总，只联合一起算，保护隐私 |
| **living biobank** | 活体样本库：存能培养、能复苏的活样本（如类器官） |
| **organoid** | 类器官：用病人细胞在体外养出的迷你器官，能拿来测药 |
| **FDA Modernization Act 2.0** | 美国 2022 年法案，允许用类器官/器官芯片替代部分动物实验 |
| **foundation model** | 基础大模型（像 ChatGPT 那种大模型，这里指生物医学版） |

> [!warning] 提醒
> 你自己聊时**首选人话版**就够镇场了。术语顶多点一两个（比如 "data not samples"、"类器官/organoid"）——一句话塞五个洋词反而像背稿，还怕被追问。真被问某个词，就用术语表里的大白话解释回去。

---

*核实来源：Cedars-Sinai 官网 Biobank and Research Pathology Resource / CAP 认证新闻稿 / MIRIAD IBD Biobank 页 / OncoBiobank 新闻；ISBER 2026 Shenzhen 会议页；CAP BAP 10 年综述（Biopreservation and Biobanking）。*
