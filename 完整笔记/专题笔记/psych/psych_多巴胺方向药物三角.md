---
tags:
  - USMLE-Step2
  - 通用方法论
  - 神经药理
  - Psych
  - 神经
created: 2026-05-23
type: 专题笔记
source: 错题驱动 Q3375 Tourette + Q16066 TD + Q12152 PD psychosis + Q20930 tetrabenazine 钓饵（2026-05-23）整合 v1
---

# 多巴胺方向药物三角 — 神经药理 USMLE Step 2 全套

> [!success] 一句话总览
> **"DA 太多治 tic，ACh 太多治 EPS，DA 太少治 PD。"**
> 同一个药在不同诊断里**身份对调** — Tetrabenazine 在焦虑题是钓饵、在 Tourette/HD/TD 题是真答案；Risperidone/Haloperidol 在 schizophrenia 是主力、在 PD psychosis 禁用；Amantadine 在 PD 治运动、在 PD psychosis 是错答案。**判断身份关键看"题目问的是哪个 DA 通路病"。**

> [!info] 三角的内在逻辑
> 基底节 DA 通路 ↔ ACh 通路是一对**互相拮抗的天平**：
> - DA ↑ + ACh ↓ → 运动过度（tic / chorea / TD / dystonia 部分）
> - DA ↓ + ACh ↑ → 运动减少（PD / 药源性 parkinsonism）
> 
> 治疗 = 把天平拨回中位：DA 过多 → ↓ DA / ↑ ACh；DA 不足 → ↑ DA / ↓ ACh。**但 ACh 一侧药物（抗胆碱 / 拟胆碱）只用在"药源性"失衡场景**（D2 阻断后 ACh 相对↑ → EPS），不用于原发病。

---

## §一 三角整体图（ASCII art）

```
                       【 多巴胺方向药物三角 】

  DA ↑ 过多（tic / TD 部分 / chorea / 精神病阳性症状 / 呕吐）
       │
       ▼ 治法：↓DA
       ├─ VMAT2 抑制剂（耗竭突触前 DA） — Tetrabenazine / Deutetrabenazine / Valbenazine
       └─ D2 拮抗剂（阻断突触后） — FGA / SGA / 止吐药 Metoclopramide / Prochlorperazine

  ACh ↑ 相对过多（D2 阻断后的代偿失衡 → EPS：急性 dystonia / drug-induced parkinsonism）
       │
       ▼ 治法：↓ACh
       └─ 抗胆碱药 — Benztropine / Trihexyphenidyl / Diphenhydramine

  DA ↓ 不足（PD / RLS / hyperprolactinemia）
       │
       ▼ 治法：↑DA
       ├─ 前体 — Levodopa（+ Carbidopa 防外周转化）
       ├─ 直接激动剂 — Pramipexole / Ropinirole / Bromocriptine
       ├─ 增释放 / 阻 reuptake — Amantadine / 兴奋剂 methylphenidate / amphetamine
       └─ 减分解 — MAO-B 抑制剂 (Selegiline / Rasagiline) / COMT 抑制剂 (Entacapone / Tolcapone)


      ┌──────────────────────────────────────────────────────┐
      │  方向口诀：DA 太多治 tic，ACh 太多治 EPS，DA 太少治 PD  │
      └──────────────────────────────────────────────────────┘
```

---

## §二 各方向药物详表

### 2.1 ↓DA 药物（Anti-Dopaminergic — 治 tic / TD / chorea / 精神病阳性 / 呕吐）

#### A. VMAT2 抑制剂（突触前耗竭 DA）

| 药 | FDA 适应症 | 关键警戒 | 在 USMLE 的角色 |
|---|---|---|---|
| **Tetrabenazine** | Huntington chorea | **抑郁 / 自杀念头 BBW**（HD 患者特别注意） / Parkinsonism / 镇静 / 长 QT | Tourette 第 3 阶梯 / HD chorea 真答案 / 焦虑题钓饵（Q20930） |
| **Deutetrabenazine** | Huntington chorea + **Tardive Dyskinesia** | 同上但半衰期更长，剂量更稳 | TD 真答案（Q16066 不能停药时） |
| **Valbenazine** | **Tardive Dyskinesia** 专批 | QT 延长 + 嗜睡 | TD 题里看到 valbenazine → 锁 |

> [!tip] VMAT2 三兄弟记忆
> **Tetra → HD / Tourette / TD 通用；Deu → HD + TD；Val → TD 专属。** 都是耗竭突触前 DA 包装（VMAT2 = vesicular monoamine transporter 2），所以**不阻 D2 受体 → 无 EPS 风险**，但**仍可诱发抑郁 / 嗜睡 / parkinsonism**（DA 总量降低的副作用）。

#### B. D2 拮抗剂（突触后阻断）

| 药 | 代 | D2 强度 | 主用 | 关键警戒 |
|---|---|---|---|---|
| **Haloperidol** | 1 代 (FGA) | 强 | Schizophrenia / Tourette / 急性激越 | EPS / NMS / QT / **PD 禁用**（Q12152） |
| **Pimozide** | 1 代 (FGA) | 强 | Tourette（备选） | **QT 延长** → 用前查 ECG，低 K / 低 Mg 避开（Q3375） |
| **Risperidone** | 2 代 (SGA) | 中-高 | Schizophrenia / Tourette 临床较常用 | 高催乳素 / EPS / **PD 禁用**（Q12152） |
| **Olanzapine** | 2 代 (SGA) | 中 | Schizophrenia / 双相 | 代谢综合征 / 体重↑ / 镇静 |
| **Quetiapine** ⭐ | 2 代 (SGA) | **极弱** | Schizophrenia / 双相 / **PD psychosis 首选** | 镇静 / 体重↑（Q12152 答案） |
| **Clozapine** | 2 代 (SGA) | 弱 | 难治性 schizophrenia / **PD psychosis 备选** | **Agranulocytosis** → ANC 监测 / 痫性发作 / 心肌炎 |
| **Aripiprazole** | 3 代 部分激动 | D2 部分激动 | Schizophrenia / Tourette / 双相增效 | Akathisia / 较少代谢副作用 |
| **Pimavanserin** | 衍生 | **零 D2**（5-HT2A 反向激动） | **PD psychosis 唯一 FDA 专批** | 可及性 / 成本限制 / QT |

#### C. 止吐 / 促胃肠动力 D2 拮抗剂（GI / 妇产急诊高频）

| 药 | 用途 | 关键警戒 ⭐ |
|---|---|---|
| **Metoclopramide** | 胃轻瘫 / 化疗呕吐 / 围产期 | **D2 阻断穿 BBB → 长期用 TD / Parkinsonism 风险** / 急性 dystonia |
| **Prochlorperazine** | 偏头痛呕吐 / 化疗呕吐 | 急性 dystonia / 镇静 / EPS |
| **Promethazine** | 妊娠呕吐 / 过敏 | 镇静 / 偶有 EPS |

> [!warning] Metoclopramide 是"伪装的 D2 拮抗"
> Metoclopramide 在 GI 章节考"止吐 + 促胃动力"，但在 psych / neuro 角度它是**外周 + 中枢 D2 拮抗**。**长期使用 (>12 周) → TD / Parkinsonism 风险升 = BBW**。USMLE 高频考法：① 老年女性长期用 metoclopramide → 出现 lip smacking + 不自主运动 → 诊断 TD。② 急诊给 metoclopramide 后年轻人颈扭转 + 眼上翻 → 急性 dystonia → 抗胆碱 (benztropine / diphenhydramine)。

### 2.2 ↓ACh 药物（Anticholinergic — 治 EPS，**不治 tic / 不治 TD**）

| 药 | 主用 | 在 USMLE 的角色 |
|---|---|---|
| **Benztropine** | 急性 dystonia / drug-induced parkinsonism | EPS 急诊（Q2505）/ 抗精神病药副作用 |
| **Trihexyphenidyl** | drug-induced parkinsonism / 特发性震颤次选 | 慢性 EPS 维持 |
| **Diphenhydramine** | 急性 dystonia 急诊（含抗组胺 + 抗胆碱） | 急诊看到"颈扭转 + 眼上翻"想到 |
| **Amantadine** | 多重身份（见 §三） | **既可↑DA 也带轻度抗胆碱** — 治 drug-induced parkinsonism 也算 |

> [!danger] 抗胆碱药"只治药源性 EPS，不治原发性运动障碍"
> ❌ **不治 tic**（Tourette 是原发 DA 过度活跃 — 见 Q3375 的 A 选项陷阱）
> ❌ **不治 TD**（TD 是慢性 D2 阻断 → ACh 已相对偏低 → 抗胆碱会火上浇油，反而加重 — 见 Q16066）
> ❌ **不治 Huntington chorea**（HD 是原发 DA 通路异常）
> ✅ 只治：**急性 dystonia / drug-induced parkinsonism / 神经阻滞剂诱发 EPS**

### 2.3 ↑DA 药物（Pro-Dopaminergic — 治 PD / RLS / hyperprolactinemia / DA 不足症）

#### A. 前体 + 直接激动剂

| 药 | 机制 | 主用 | 关键警戒 |
|---|---|---|---|
| **Levodopa (+ Carbidopa)** | DA 前体，过 BBB | PD 金标准 | 长期 → on-off / dyskinesia / **psychosis（Q12152）** |
| **Pramipexole** | 直接 D2/D3 激动 | PD / **RLS 一线** | **冲动控制障碍**（赌博 / 暴食 / 性欲↑ — DA dysregulation syndrome） / 嗜睡发作 |
| **Ropinirole** | 直接 D2/D3 激动 | PD / RLS 一线 | 同 pramipexole |
| **Bromocriptine** | 直接 D2 激动 | PD / **Hyperprolactinemia（prolactinoma）** / 抑乳 | 同上 + 心瓣膜纤维化（高剂量） |

#### B. 增释放 / 阻 reuptake / 减分解

| 药 | 机制 | 主用 | 关键警戒 |
|---|---|---|---|
| **Amantadine** | 增 DA 释放 + 抑 reuptake + 抗 NMDA + 轻度抗胆碱 | 早期 PD / levodopa 诱导 dyskinesia / 流感 M2（少用） | **PD psychosis 加重剂**（Q12152 错答案） |
| **Methylphenidate / Amphetamine** | 阻 DAT/NET reuptake + 增释放 | ADHD | **加重 tic**（Q3375） / 心血管 / 失眠 / 滥用 |
| **Selegiline / Rasagiline** | MAO-B 抑制 → 阻 DA 降解 | PD 早期 / 辅助 | 高剂量失选择性 → **tyramine HTN crisis 风险（Q4879）** / 与 5-HT 药 → SS 风险 |
| **Entacapone / Tolcapone** | COMT 抑制 → 延长 levodopa 半衰期 | PD（与 levodopa 共用） | Tolcapone → 肝毒 / Entacapone → 腹泻 + 尿橙色 |

> [!tip] DA dysregulation syndrome（冲动控制障碍）
> 长期高剂量 DA 激动剂（尤其 pramipexole / ropinirole）→ 中脑边缘 DA 通路过度激活 → **赌博 / 暴食 / 性欲亢进 / 强迫购物**。**USMLE stem**：PD 患者新报告 "最近开始大额赌博 / 网购成瘾 / 性欲突然旺盛" → 答 "reduce / discontinue dopamine agonist"。这与 Q12152 PD psychosis 是同一机制（中脑边缘 DA 过多）的不同临床表型。

---

## §三 同一药 / 同一通路在不同诊断里的"身份对调" ⭐ 核心

> [!danger] USMLE 出题人最爱的"反差陷阱"
> 把同一个药放在两种不同 context 下出题，**测你能不能"按诊断定位身份"而非"按药名反射"**。下表 5 条全部是 USMLE 经典考法。

### 表 1｜Tetrabenazine 双面身份（Q3375 ↔ Q20930 完美反向对照）

| Context | Tetrabenazine 的身份 | 出题方式 |
|---|---|---|
| **焦虑题**（GAD / SAD / panic） | ❌ **钓饵划掉** | Q20930：儿童 GAD stem 给 fidget + 完美主义 + 担心未来 → tetrabenazine 是 E 选项干扰 |
| **Tourette 题** | ✅ **真答案**（第 3 阶梯 VMAT2） | Q3375：HRT + α2 失败 → 升级抗 DA → tetrabenazine 是答案之一 |
| **Huntington chorea 题** | ✅ **真答案** | HD 患者舞蹈样动作 → tetrabenazine 一线（注意抑郁 BBW） |
| **Tardive Dyskinesia 题** | ✅ **真答案** | TD 不能停抗精神病药 → tetrabenazine / deutetrabenazine / valbenazine（Q16066） |

**身份切换钥匙**：题问的是"DA 过度活跃疾病"（tic / chorea / TD） → 真答案；题问的是"焦虑 / 抑郁 / 强迫" → 钓饵。

### 表 2｜D2 拮抗 SGA 不均质（Q12152）

| 药 | Schizophrenia / Tourette | PD psychosis |
|---|---|---|
| **Haloperidol**（FGA 强 D2） | ✅ 主力 | ❌ **禁用**（会让 PD 患者瘫） |
| **Risperidone**（SGA 中-高 D2） | ✅ 主力 | ❌ **禁用**（仍会恶化 parkinsonism） |
| **Olanzapine**（SGA 中 D2） | ✅ 可用 | ❌ 一般不用（D2 仍偏强） |
| **Quetiapine**（SGA 极弱 D2） | ✅ 可用 | ✅ **临床首选** |
| **Clozapine**（SGA 弱 D2） | ✅ 难治性 schizophrenia | ✅ 备选（agranulocytosis 风险） |
| **Pimavanserin**（零 D2） | ❌ 不用 | ✅ FDA 唯一专批 |

**身份切换钥匙**：题问的是"原发精神病阳性症状" → 走 D2 用，强 D2 也行；题问的是"PD 患者的精神症状" → **躲着 D2 走**，只有 Quet / Cloz / Pim 三家可用。

### 表 3｜Amantadine 多重身份

| Context | Amantadine 的身份 |
|---|---|
| **早期 PD / 轻型 PD 单药** | ✅ 一线辅助（增 DA 释放） |
| **Levodopa 诱导的 dyskinesia** | ✅ 抑制 dyskinesia（抗 NMDA 机制） |
| **Drug-induced parkinsonism** | ✅ 可用（增 DA 抗衡 D2 阻断） |
| **NMS** | ✅ 可用（bromocriptine 同类替代） |
| **流感 M2 阻断** | 历史用药，现少用（耐药） |
| **PD psychosis**（Q12152） | ❌ **绝对错答案** — 多巴胺能药"火上浇油" |

**身份切换钥匙**：题问的是"PD 运动症状 / 药源性 parkinsonism / 抗精神病药副作用" → 真答案；题问的是"PD 病人出现幻觉 / paranoia" → 错答案。

### 表 4｜Bromocriptine 双身份

| Context | Bromocriptine 的身份 |
|---|---|
| **PD（早期/辅助）** | ✅ DA 激动剂 |
| **Prolactinoma / Hyperprolactinemia** | ✅ 一线（D2 激动 → ↓PRL） |
| **NMS** | ✅ 治疗（↑ 中枢 DA 对抗 D2 阻断） |
| **抑乳（产后不哺乳）** | 历史用药，现 cabergoline 替代 |

**身份切换钥匙**：所有应用本质都是"**↑DA 方向**"，但临床问题不同 — PD 是运动，prolactinoma 是激素，NMS 是急救。

### 表 5｜Metoclopramide 双身份（GI ↔ Psych/Neuro）

| Context | Metoclopramide 的身份 |
|---|---|
| **GI 章节**：胃轻瘫 / 化疗呕吐 / 围产期止吐 | ✅ D2 拮抗 + 促胃肠动力 |
| **Psych/Neuro 章节**：长期用 (>12 周) → TD / Parkinsonism | ❌ **BBW** — D2 阻断穿 BBB → 老年女性高风险 |
| **急诊给药后急性 dystonia** | 反向考点：用 benztropine / diphenhydramine 急救 |

**身份切换钥匙**：GI 急性场景 = 工具药；老年长期用 / 急性 dystonia 出现 = D2 阻断的副作用。

---

## §四 七大 USMLE 陷阱

> [!danger] 反复错点警戒 — 每条都对应至少 1 道 UW 错题
> 这 7 条是 Q3375 / Q16066 / Q12152 / Q20930 全部错因的"普适规则"提炼。每次看到对应 stem 模式 → 直接反射"踩刹车"。

### 陷阱 1｜"Tic 是不自主运动 → 选抗胆碱" ❌
- **错误反射**：tic = 运动症状 → benztropine 治运动症状（EPS） → 选它
- **正解**：tic 是**原发**性 DA 过度活跃，抗胆碱只治**药源性**的 D2 阻断后 ACh 优势失衡 — **方向完全相反**
- **对应错题**：[[mistakes/uworld-mistakes_2026-05#^Q3375]]
- **反射钩**：看到运动症状选项先问 — **药源 vs 原发？** 药源 → 抗胆碱 / VMAT2 / 停药；原发 → 看具体疾病通路

### 陷阱 2｜"Tetrabenazine 看起来生僻 → 划掉" ❌
- **错误反射**：陌生药名 = 钓饵 → 划掉
- **正解**：tetrabenazine 是 VMAT2 抑制剂，**Tourette / HD / TD 真答案**；只有出现在焦虑题里才是钓饵
- **对应错题**：[[mistakes/uworld-mistakes_2026-05#^Q20930]]（焦虑题钓饵）↔ [[mistakes/uworld-mistakes_2026-05#^Q3375]]（Tourette 真答案）
- **反射钩**：判断 tetrabenazine 身份**只看诊断**，不看"药名生僻不生僻"

### 陷阱 3｜"PD 患者出现幻觉 → 上 risperidone / haloperidol" ❌
- **错误反射**："幻觉 = 精神病 = 上抗精神病药" → 选强 D2 拮抗
- **正解**：PD psychosis **躲着 D2 走** — 只有 quetiapine / clozapine / pimavanserin 三家
- **对应错题**：[[mistakes/uworld-mistakes_2026-05#^Q12152]]
- **反射钩**：PD + 幻觉 → 默认 **quetiapine**；除非题干特意强调"零 D2"或"已用 quetiapine 无效"

### 陷阱 4｜"ADHD + Tourette → 上 methylphenidate" ❌
- **错误反射**：ADHD 一线就是兴奋剂
- **正解**：兴奋剂 ↑DA → **加重 tic**；Tourette + 共病 ADHD **优先用 α2 激动剂（guanfacine / clonidine）或 atomoxetine（NRI 非兴奋剂）**
- **对应错题**：[[mistakes/uworld-mistakes_2026-05#^Q3375]]
- **反射钩**：Tourette + ADHD + "兴奋剂选项" → 警铃；α2 一石二鸟

### 陷阱 5｜"TD 是运动障碍 → 用抗胆碱药" ❌
- **错误反射**：EPS 用抗胆碱 → TD 也是 EPS 类 → 用抗胆碱
- **正解**：TD 是慢性 D2 阻断后 **D2 超敏**，ACh 已相对偏低 → 抗胆碱**加重 TD**；正解 = **停药（if feasible）/ VMAT2 抑制剂（valbenazine / deutetrabenazine）**
- **对应错题**：[[mistakes/uworld-mistakes_2026-05#^Q16066]]
- **反射钩**：TD 和急性 dystonia / DIP **不在同一治疗方向** — TD 要"减 DA 信号"（停药 / 耗竭），不是"减 ACh"

### 陷阱 6｜"长期 metoclopramide 没事，是 GI 药" ❌
- **错误反射**：metoclopramide 是止吐药 → 与 EPS / TD 无关
- **正解**：metoclopramide = **外周 + 中枢 D2 拮抗**，穿 BBB → **>12 周用 → TD / Parkinsonism 风险（BBW）**
- **典型 stem**：老年女性长期胃轻瘫用药 + 新出现 lip smacking / 不自主舌动
- **反射钩**：看到 "metoclopramide + 老年 + 长期 + 不自主运动" → 想 D2 阻断诱发 TD

### 陷阱 7｜"Pimozide 看起来强 → 选它治 Tourette" ❌
- **错误反射**：D2 拮抗最强 = 治 tic 最有效
- **正解**：pimozide 强 D2 + **QT 延长** → 已 QT 长 / 低 K / 低 Mg 患者禁用；选 risperidone / tetrabenazine 更安全
- **对应错题**：[[mistakes/uworld-mistakes_2026-05#^Q3375]]
- **反射钩**：pimozide 选项出现时必看 stem — 有"QT" / "low K" / "low Mg" / "心电图异常" → 避开

---

## §五 Memory Hook 汇总

### 一句话锁定
**"DA 太多治 tic，ACh 太多治 EPS，DA 太少治 PD。"** — 三方向，三药篮子，对号入座不混淆。

### 类比 1｜"踩油门 vs 踩刹车"
- 脑子 DA **油门踩太死**（tic / chorea / TD / 精神病阳性）→ **踩刹车**（↓DA：D2 拮抗 / VMAT2 耗竭）
- 抗胆碱药 = **修"刹车踩过头后的副作用"**（治 EPS — D2 阻断后 ACh 优势失衡）
- 兴奋剂 / DA 激动剂 = **再踩一脚油门**（在 tic / 精神病题里 = 加重；在 PD 题里 = 治疗）
- PD = **油门没了**（DA 不足）→ 加油门（前体 / 激动剂 / 阻分解 / 增释放）

### 类比 2｜"同一药两种身份"钩
- **Tetrabenazine** = 关 4 个 DA 水龙头 → 治 tic / HD / TD；焦虑题里看到 → 钓饵划掉
- **Risperidone / Haloperidol** = D2 重锤 → schizo / Tourette 主力；PD 患者看到 → 禁用
- **Amantadine** = 多巴胺能药 → PD 治；PD psychosis 看到 → 火上浇油
- **Bromocriptine** = D2 激动 → PD 治 + prolactinoma 减 PRL（同方向不同病）
- **Metoclopramide** = D2 拮抗 → 急性止吐 + 长期 TD/Parkinsonism 风险

### 反射钩｜"看到 X 想 Y"
- 看到 "**HRT + α2 失败 → next step**" → 抗 DA（VMAT2 / D2 拮抗）（Q3375）
- 看到 "**长期抗精神病药 + lip smacking + 不自主舌动**" → TD → 停药 / VMAT2（Q16066）
- 看到 "**PD + paranoia + 减药失败**" → quetiapine（Q12152）
- 看到 "**儿童多领域 worry + 完美主义 + tetrabenazine 选项**" → 钓饵划掉，选 sertraline（Q20930）
- 看到 "**抗精神病药 + 急性颈扭转 + 眼上翻**" → 抗胆碱（benztropine / diphenhydramine）

### 升级题"用了一段时间仍恶化"钩
- Tourette α2 失败 → 升抗 DA（Q3375）
- PD psychosis 减药失败 → 升 quetiapine（Q12152）
- TD 不能停药 → 升 VMAT2（Q16066）
- 通用 SOP：**升级题不在同阶梯横移**，纵向升下一阶梯

---

## §六 关联（v2 四类齐全）

- 🔁 同主题错题（按时间倒序）：
  - [[mistakes/uworld-mistakes_2026-05#^Q3375]] Tourette 药物升级（2026-05-23；**三角原始来源** — HRT + α2 失败 → 抗 DA / Tetrabenazine 双面身份 / Pimozide QT）
  - [[mistakes/uworld-mistakes_2026-05#^Q12152]] PD psychosis 第 5 步用药（2026-05-23 🔴 反复错；**↑DA 方向药物 vs ↓DA 方向药物的边界** — quetiapine 首选 / Pimavanserin / Clozapine 三选一；Risperidone/Haloperidol PD 禁用 / Amantadine 错答案）
  - [[mistakes/uworld-mistakes_2026-05#^Q20930]] 儿童 GAD + Tetrabenazine 钓饵（2026-05-23；**同一药两种身份的反向对照** — 焦虑题里 tetrabenazine = 钓饵，与 Q3375 完美互证）
  - [[mistakes/uworld-mistakes_2026-05#^Q16066]] TD 识别 + EPS 四兄弟（2026-05-20；**↓DA 方向药 vs ↓ACh 方向药的边界** — TD 用 VMAT2 / 停药，**不用抗胆碱**）
  - [[mistakes/uworld-mistakes_2026-05#^Q2505]] 急性 dystonic reaction（2026-05-21；**↓ACh 方向药的真适应症** — 抗胆碱治急性 dystonia，与本衍生第 6 陷阱"metoclopramide 急诊 dystonia"互证）
  - [[mistakes/uworld-mistakes_2026-05#^Q11898]] Akathisia + propranolol（2026-05-21；**EPS 四兄弟另一治疗谱** — β 阻断 ≠ 抗 DA / 抗胆碱方向）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/psych]] / [[完整笔记/Peixuan分科笔记/neuro]] / [[完整笔记/Peixuan分科笔记/GI]]（metoclopramide 止吐 + 长期 TD 风险）
- 🏥 跨学科：
  - [[完整笔记/专题笔记/psych/psych_Tourette诊断与治疗]]（Tourette 三级阶梯 + 共病模式 — 本衍生第 §2.1 §3 表 1 互证）
  - [[完整笔记/专题笔记/psych/psych_四大EPS诊断治疗对照]]（急性 dystonia / akathisia / parkinsonism / TD 四治疗谱 — 与本衍生 §2.2 §三表 2 互证）
  - [[完整笔记/Peixuan分科笔记/心内]]（Pimozide / Haloperidol / Valbenazine QT 延长监测）
- 🌱 TODO（待扩展）：
  - 等积累 hyperprolactinemia / prolactinoma 错题 → 扩 §2.3 DA 激动剂的 prolactin 应用（cabergoline > bromocriptine）+ 男性 HRT 抑制 prolactin 框架
  - 等积累 5-HT-DA 交互错题（SGA 5-HT2A 阻断 / pimavanserin 纯 5-HT2A 反向激动机制）→ 扩 §三 加入"5-HT2A 通路与 DA 通路的交叉"专节
  - 等积累 RLS / DA dysregulation syndrome 错题 → 扩 §2.3 DA 激动剂的冲动控制障碍框架（赌博 / 暴食 / 性欲↑）
  - 等积累 ADHD 兴奋剂 + 心血管 / 滥用错题 → 扩 §2.3 兴奋剂的"↑DA 方向但非 PD 应用"专节
  - 配合 [[mistakes/uworld-mistakes_2026-05#^Q12152]] 反复错 → 触发 [[完整笔记/专题笔记/_衍生_治疗阶梯升级SOP]]（与本衍生互补 — 那个讲"何时升级"，本衍生讲"升级到哪个方向"）

---

## §七 复习节奏建议

### 第一遍（建衍生当天 — 2026-05-23）
- 默写 §一 三角整体图（DA 多 / ACh 多 / DA 少 三方向 + 各方向代表药）
- 默写 §五 一句话口诀 + "踩油门 vs 踩刹车"类比
- 串读 Q3375 + Q20930（tetrabenazine 双面身份反向对照）

### D+3（2026-05-26）
- 默写 §三 表 1-5（5 个"同一药两种身份"对调表）
- 重做 Q3375 + Q16066 — 第一眼锁方向，不查表
- 把 §四 7 陷阱在脑中演练"看到 stem 关键词 → 反射对应陷阱编号"

### D+7（2026-05-30）
- 重做 Q12152（PD psychosis 反复错点；自测 quetiapine 首选 vs Pimavanserin 暗号 vs Clozapine 二线）
- 默写 §2.1-2.3 各方向药物详表（不看本衍生，写完对答）
- 找 3 道类似题（Tourette pharmacotherapy / TD VMAT2 / PD psychosis / Huntington chorea 治疗）

### D+14（2026-06-06）
- 全衍生通览 + 每个陷阱讲解给"假想学生"听（教学输出 = 最高级复习）
- 检查 §六 TODO 项是否已积累足够错题触发扩展
- 评估状态升降：4 道触发题（Q3375 / Q16066 / Q12152 / Q20930）若再次全做对 → 可降 🟡 → 🟢

### 考前冲刺（最后 7 天）
- 重读 §四 7 陷阱（高 ROI — 全部直接对应 USMLE 高频题模式）
- 重读 §三 5 个"身份对调表"（这是 USMLE 出题人最爱的考法）
- §一 三角图能盲画 → 任何 DA 通路题 30 秒锁方向
