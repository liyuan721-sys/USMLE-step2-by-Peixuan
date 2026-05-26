---
tags:
  - USMLE-Step2
  - Ethics
  - research
created: 2026-05-25
type: 专题笔记
version: v1
---

# Ethics Research Ethics — COI + RCT Design + Vulnerable Populations

## 📋 目录

> [!tip]- 点击跳转章节（4 大节 + 子节）
>
> - [[#§一 Research Ethics 总览 — 4 大支柱]]
>   - [[#§1.1 Conflict of Interest (COI) 完整 SOP ⭐（Q106885 锚定）]]
>   - [[#§1.5 DSMB 完整 SOP ⭐（Q107273 锚定 — v1.4.2 新增）]]
> - [[#§二 RCT Ethical Considerations ⭐（图 5 做对题 — v1.4 新增）]]
>   - [[#Stopping RCT Early — 3 类详细 + DSMB 角色 ⭐（v1.4.1 扩充）]]
> - [[#§三 Vulnerable Populations Research Recruitment + Inducement ⭐（v1.4.1 新增）]]
> - [[#§四 Informed Consent for Research vs Clinical 区分（TODO 速记）]]
> - [[#🔗 关联]]
> - [[#✅ 学习清单]]

---

> [!info] 文件起源
> 从 [[完整笔记/专题笔记/_衍生_Ethics精简框架]] §十 拆出（2026-05-25 拆分，方案 2）。原文超大（4362 行），按主题分文件后单文件 ≈ 400 行可一次看完。
> 主题专注：Research ethics 4 大支柱 + COI mitigation + DSMB + RCT control 选择 + Stopping early + Vulnerable populations。

> [!tip] 适用场景速查
> - Industry-employed statistician 做 analysis → §一 COI 核心
> - DSMB vs IRB 角色区分 → §一.5
> - Placebo control 何时 ethical → §二
> - Stopping RCT early 3 类 → §二（benefit/harm/futility）
> - Vulnerable population recruitment / inducement → §三
> - Research vs Clinical informed consent 区分 → §四

---

## §一 Research Ethics 总览 — 4 大支柱

> [!info] 反射钩
> Research ethics 4 大支柱：① **Equipoise**（RCT 必备）② **COI mitigation**（disclosure + independent analysis + IRB）③ **Informed consent for research**（不同于 clinical informed consent）④ **Appropriate control selection**（不已知 inferior + 符合 standard of care）。

> [!info] 深度理解 — Research ethics 为什么是 clinical ethics 的**独立分支**
>
> **核心区别**：临床伦理保护 **the patient in front of me**（眼前这个人）；研究伦理保护 **future patients receiving findings**（未来受益于研究结果的人）+ **research subjects themselves**（参与研究的人）。这两个利益群体的保护机制完全不同。
>
> **历史根源 — 4 大丑闻塑造现代 research ethics**：
> 1. **Nazi 人体试验**（WWII）→ **Nuremberg Code (1947)** — 确立 voluntary consent 必需
> 2. **Tuskegee Syphilis Study**（1932-1972 美国黑人 syphilis 患者被故意不治疗 40 年）→ **Belmont Report (1979)** — 确立 respect for persons / beneficence / justice 三原则
> 3. **Willowbrook hepatitis 实验**（智障儿童故意感染 hepatitis）→ vulnerable population 额外保护
> 4. **Sponsorship bias 案例**（pharma 资助研究反复出现偏向赞助方结果）→ COI mitigation
>
> 这些惨痛历史让现代 research ethics 有 **3 层独立监管**（不是临床 ethics 的延伸）：
> - **IRB (Institutional Review Board)** — 研究开始前审批
> - **DSMB (Data Safety Monitoring Board)** — 研究进行中独立监视 interim data
> - **Informed consent for research** — 比 clinical informed consent 多 elements（voluntary + right to withdraw + research nature disclosure）
>
> ## 4 大支柱深度解析
>
> ### 支柱 1：Equipoise（均势）— RCT 的伦理根基
>
> **定义**：在研究开始时，**真诚的临床不确定性** — 专业社区对 treatment A vs treatment B 哪个更好**没有共识**。
>
> **为什么 RCT 需要 equipoise**：
> 如果已经知道 A 比 B 好 → 给 control group B 就是**故意 deprive** 他们更好的治疗 → 违 nonmaleficence。
> 例：已知 aspirin 减心梗后死亡率 → 新 RCT 设 placebo control 让一半患者吃 placebo = **unethical**（应用 active control，aspirin 作 baseline 加新药 vs aspirin 加 placebo）。
>
> **CK 考点**：placebo control 只 ethical 当 **no established effective treatment** 时；有 standard of care 必用 active control。
>
> ### 支柱 2：COI mitigation — Disclosure 不够，必须 independent analysis
>
> **核心反直觉**：直觉认为 "disclose financial relationship 就 OK 了"。**错**。
>
> Disclosure 仅是**透明度**手段，**不消除** bias 本身。Industry-employed statistician 即使 disclose 仍可能（有意或无意）做出 favor sponsor product 的分析选择（哪些 subgroup 报告 / 哪个 endpoint 优先 / outliers 怎么处理）。
>
> **真正 mitigation 必须 independent analysis** — 数据交给与 sponsor 无关的独立 statistician/team 做。这是 COI 章节最重要的 takeaway。
>
> **为什么 double-blinding 不能 mitigate analysis bias**：
> Blinding 保护**数据收集阶段**（patient + assessor 不知道分组）→ 减 measurement bias。
> 但**分析阶段** statistician 必须 unblind 才能做对比 → 此时 industry-employed analyst 仍可能 bias → **blinding ≠ COI mitigation for analysis**。
>
> ### 支柱 3：Informed Consent for Research（比 Clinical 多 elements）
>
> 临床 informed consent 5 elements (见 [[完整笔记/专题笔记/_衍生_Ethics精简框架]] §十一) + 研究专有 elements：
> - **Voluntary participation** — 参与是 voluntary 不影响 standard care
> - **Right to withdraw at any time** — 任何时候可退出，不损 future care
> - **Research nature disclosure** — 明确告知"这是研究不是 standard care"
> - **Risks specific to research** — 包括 unknown risks
>
> **Therapeutic misconception**：患者常误以为"参加研究 = 接受最先进治疗"（实际可能 placebo / 实验药未证有效）。Informed consent 必须 actively 破除这个误解。
>
> ### 支柱 4：Vulnerable Populations + Inducement
>
> **Vulnerable population 清单**：low-income / institutionalized / cognitively impaired / pregnant women + fetuses / minors / prisoners / critically ill。
>
> **为什么需要额外保护** — coercion / 操控的 baseline 风险高：
> - Prisoners — "参与可减刑" 即使 implicit 暗示也是 coercion
> - Low-income — 经济压力下 unacceptable risks 也接受
> - Cognitively impaired — capacity 不足 / 易 manipulation
>
> **Inducement 临界判断**：compensation = 参与时间合理 hourly wage + 实际开销（transportation / childcare）→ OK；compensation 远 > 这个（如 6 周薪水换 12 hr study）→ **inducement** → 让经济弱势的人接受 unacceptable risks → undermine voluntary consent。
>
> **CK 怎么考**：
> - 题眼 1：Industry-employed statistician 做 analysis → COI（disclosure 不够，需 independent analysis）
> - 题眼 2：Placebo control + 已有 standard treatment → unethical（应 active control）
> - 题眼 3：Compensation $X >> hourly wage × hours → inducement
> - 题眼 4：Patient 想参加研究但误以为是 standard care → 必须 break therapeutic misconception
> - 钓饵：① "Double-blind 已 mitigate COI"（错 — blinding 不 cover analysis bias）② "Disclosure alone is sufficient"（错 — 需 independent analysis）③ "Higher compensation increases retention so it's ethical"（错 — proportionate to time，不是 retention 工具）。

### §1.1 Conflict of Interest (COI) 完整 SOP ⭐（Q106885 锚定）

#### COI 4 大判定要素

| 要素 | 是否 COI | 例子 |
|---|---|---|
| **Industry funding 覆盖 salary / 项目费** | ❌ 单独不构成 COI | 厂家给钱 cover PI 工资 / equipment / 受试者补助 |
| **Investigator 个人 financial incentive 与 product 挂钩** | ✅ COI | Stocks / royalties / **speaking fees** / consulting fees |
| **Industry-sponsored personnel 参与 study design** | ✅ COI | 厂家派 scientist co-design protocol |
| **Industry-sponsored personnel 参与 data analysis** | ✅ **COI 核心** ⭐ | 厂家派 statistician 做 primary endpoint analysis |

#### COI Mitigation 阶梯

```
① Disclosure（financial relationships → IRB + subjects + publications）⭐ 必做但不够
     │
     ▼
② Independent analysis（数据分析交给 non-industry-affiliated 独立团队）⭐ 关键
     │
     ▼
③ IRB oversight（disclose financial relationships → IRB 决定 require independent analysis / 拒绝研究）
     │
     ▼
④ DSMB（Data Safety Monitoring Board，independent，定期看 interim data — 详 §1.5）
     │
     ▼
⑤ PI 责任：comply with IRB recommendations 才能 proceed
```

### §1.5 DSMB 完整 SOP ⭐（Q107273 锚定 — v1.4.2 新增）

> [!info] DSMB / Independent Data Monitoring Committee
> RCT 进行中，**external monitoring committee (DSMB, Data Safety Monitoring Board / Independent Data Monitoring Committee)** 定期 review **interim data** → 保 human subject safety + data integrity + detect/report safety concerns。

#### DSMB 组成 + 独立性要求 ⭐

| 维度 | 要求 |
|---|---|
| **组成** | Biostatisticians + 其他 experts（临床医生 / 伦理 / 流行病学）|
| **独立性 ① External to research team** | 不能是 study investigators / data analysts |
| **独立性 ② External to study sponsor** ⭐ | 不能是 industry sponsor 雇员 / 关联人 — 防 sponsor bias + COI |
| **数据形式** | Research team submit **secured + deidentified** data → committee 在 **unblinded form** review（committee 知道 group assignment 才能识别 differential safety signals）|
| **报告方式** | Detect + report safety concerns to PI / sponsor / IRB |

#### DSMB Review 的 3 大目标

```
① 高 SAE incidence / severity（adverse events 超预期）
② Treatment futility（统计上无法达到 power）
③ Data integrity 问题（dropout 异常 / 不一致 / missing 严重）
```

#### IRB vs DSMB 角色区分（USMLE 高频陷阱）⭐

| 维度 | **IRB**（Institutional Review Board）| **DSMB**（Data Safety Monitoring Board）|
|---|---|---|
| **隶属** | 与 academic trial investigators **affiliated 的 institution** | **External**（与 research team + sponsor 双独立）|
| **角色阶段** | **Pre-study + 启动审批** | **Study 进行中持续 interim monitoring** |
| **任务** | ① Approve research protocol ② Ensure research conforms to proper scientific + ethical standards ③ Confirm presence of appropriate informed consent + data monitoring plan | ① Periodic interim data statistical analysis ② Detect safety concerns ③ Recommend stop early（详 §二 — benefit / harm / futility 3 类）|
| **统计分析 interim data** | ❌ **不做**（IRB 没这个 function — 这是 DSMB 工作）| ✅ 核心任务 |
| **看 data 形式** | 总结性 / 报告 | **Unblinded interim data** |
| **常见 USMLE 陷阱** | "IRB 应 annually analyze data" → ❌ 这是 DSMB 的事 | — |

#### USMLE 经典 stem（Q107273）

| Stem 元素 | 暗号 |
|---|---|
| **"Multicenter, double-blind RCT"** + 长期 follow-up（6 yr）| 高 DSMB 必要性 |
| **"IRB approval obtained, trial started"** + 问 ongoing oversight | 测 IRB ≠ DSMB |
| **"50% in 2-arm RCT 受试者会被分到 inferior arm"** | 强调 DSMB protect 这些人的必要性 |

#### 关键陷阱

> [!warning]
> - "**Dedicated biostatistician on research team** 做 oversight"（A）→ ❌ 必须 **external** 防 bias / COI
> - "Oversight restricted to research team members for patient confidentiality"（B）→ ❌ Deidentified data 解决 confidentiality；oversight 必须 external
> - "**IRB** annually analyze data for protocol adherence"（C）→ ❌ IRB 不做 interim statistical analysis；这是 DSMB 工作 ⭐ 核心陷阱
> - **D 正确**：Regularly submit secured data to independent committee for oversight

#### Double-blinding + Randomization 能/不能 mitigate 什么 ⭐

| Bias 类型 | Blinding/Randomization 能 mitigate？ |
|---|---|
| **Selection bias**（分组阶段）| ✅ Randomization 解决 |
| **Performance bias**（治疗执行）| ✅ Blinding 解决 |
| **Detection bias**（outcome assessment）| ✅ Outcome assessor blinding 解决 |
| **Analysis bias**（数据分析阶段 selective reporting / inappropriate test）| ❌ **不能** — 需 independent analysis team ⭐ |
| **Funding source bias / sponsorship effect** | ❌ **不能** — 需 IRB oversight + 独立 analysis ⭐ |

> [!danger] 核心反 pattern
> "**双盲 RCT = 万能 bias 解药**" = ❌ 反射陷阱。Blinding 只 reduce trial **执行阶段** investigator-generated bias，**不 mitigate** analysis 阶段 industry statistician 的 bias。
> Industry-sponsored statistician 可通过 selective reporting / inappropriate statistical test / outlier handling 等系统引入 favorable bias — **与 blinding 无关**。

---

## §二 RCT Ethical Considerations ⭐（图 5 做对题 — v1.4 新增）

| 维度 | 标准 |
|---|---|
| **Appropriateness of RCT** | Intervention arms 在 **equipoise**（intervention 不已知 superior to control）|
| **Appropriateness of control** | ① Equivalent to **accepted standard of care** ② Does not pose **unacceptable risks** to participant |
| **Appropriateness of inactive placebo** | ① 当 effective standard of care **不明 / 不存在**；OR ② Effective standard exists 但 **temporarily withholding 不 harm** participant |
| **Appropriateness of stopping RCT** | Interim data analysis 显示 **clear, highly significant benefit OR harm** |

### Control 选择决策树

```
本研究 intervention 是？
    │
    ├─ 单一药物 / 单一干预 → Control 可以是 placebo 或 standard care
    │
    └─ Multicomponent intervention（如 IBS 多模式治疗：peer support + exercise + multidisciplinary）
            │
            ▼
        Control 应是 multicomponent standard care
            （不应是单一 medication — 不匹配 active intervention 的 multimodal nature）
```

### Inactive Placebo 何时 ethical / 何时不

| Placebo 是否 ethical | 条件 |
|---|---|
| ✅ Ethical | Effective standard care 不明 / 不存在；OR 短期 trial + withholding 不 harm |
| ❌ Not ethical | Effective standard care 存在 + withholding **会 harm**（如 STEMI / sepsis / 严重感染 / 致死病）|

### 关键陷阱

> [!warning]
> - "Inert placebo 永远 OK in RCT" → ❌ 仅 standard care 不存在 / 短期不 harm 时 OK
> - "Multicomponent intervention 用单一药 control" → ❌ Control 应与 active intervention 复杂度匹配（multicomponent → multicomponent）
> - "Academic-center-only intervention 作为 general population RCT control" → ❌ 不可 generalize；不适合 diverse participant population
> - "Refractory-subset intervention 作为 mild symptom 患者 control" → ❌ 过度治疗 + bias 结果

### Stopping RCT Early — 3 类详细 + DSMB 角色 ⭐（v1.4.1 扩充）

> [!info] DSMB / External Monitoring Committee
> RCT 进行中，**external monitoring committee (DSMB, Data Safety Monitoring Board)** 定期 review **interim data** → 保 human subject safety + data integrity。
> Committee 可推荐 **stop early**，当 continuation 暴露 participants 于 **unnecessary risk**。
> DSMB 是 **independent**（与 PI / sponsor 利益无关）— 与 §一.1 COI mitigation 阶梯第 ④ 项呼应。

### 3 大 Stopping Criteria（USMLE 高频）

| 类型 | 触发数据 | 例子 |
|---|---|---|
| **① Evidence of benefit** ⭐ | 在 clinically important end points 上有 **highly significant differences**（如 **p < 0.0005**，比 study-end reporting 用的 0.05 严得多）favoring intervention，且无 excess SAE | SPRINT-like：intensive BP control vs standard，p<0.0001 + p<0.0003 in MI / all-cause mortality → stop early，让 standard 组也能接受 intensive |
| **② Evidence of harm** | Intervention 组 outcomes 显著更差 / excess incidence of adverse events | 新药 → unexpected serious adverse events |
| **③ Evidence of futility** | Study hypothesis 因 statistical 原因 **not provable**（excessive dropout / insufficient recruitment / 无法达到 statistical power）| 招募极慢 + dropout 高 → effect size 永远测不出 |

### Stopping Early 的 ethical 逻辑

```
Interim data 显示明确 benefit / harm / futility
    │
    ▼
继续 = 仍在 control 组 / inferior arm 的 participants
       被 unnecessarily 暴露于 inferior outcome
    │
    ▼
Stop early → 让所有 participants 接受 superior treatment（benefit case）
              或 避免继续暴露 harm（harm case）
              或 不浪费资源（futility case）
```

> [!success] 关键 reframe
> Stop early 不是"研究失败"或"violation of protocol" — 是 **ethical obligation** to protect 仍在 inferior arm 的 participants。
> Why stricter threshold (p<0.0005)：interim analysis 看多次会 inflate type I error → 用更严 alpha 控制 false-positive stopping。

### 关键陷阱

> [!warning]
> - "External validity 不够 → 不能 stop early" → ❌ External validity 是 generalizability 问题，不是 ethical justification 来源；与 stopping 决策无关
> - "Sample size 还没达到 → 必须继续 enroll" → ❌ DSMB 优先 participant safety > pre-specified sample size
> - "Stopping early = study failure" → ❌ Stopping for benefit = protocol success（intervention 比预期更有效）；stopping for harm / futility = ethical protection

---

## §三 Vulnerable Populations Research Recruitment + Inducement ⭐（v1.4.1 新增）

> [!info] 反射钩
> Research stem 给 "vulnerable population"（low-income / institutionalized / 囚犯 / 难民 / 儿童 / cognitively impaired）+ "compensation excessive"（如 6 周薪水 for 6 周 × 2 hr 参与）→ 反射识别 **inducement** = unethical recruitment。
> 历史上 vulnerable groups 因 unethical / disproportionate recruitment 受过 exploitation（Tuskegee / Willowbrook 等）→ research community 现有 3 大 recruitment 原则。

### Research Recruitment 3 大伦理原则 ⭐

| 原则 | 内容 | 反 pattern |
|---|---|---|
| **① Compensation proportionate to actual participation** | 按 hourly wage × 参与小时数 + 关联 expenses（transportation / childcare）补偿 | **Excessive compensation = inducement**（如 12 hr 参与 → 给 6 周薪水）|
| **② Recruitment plan relates directly to primary objectives** | 招募 demographic 应与研究问题相关（如研究 low-income 群体 depression → 招 low-income OK）| **Convenience-driven**（仅因 community resource center 方便招）不是 valid 理由 |
| **③ Range of demographic groups（默认）** | 除非 research goals specify，应招 diverse demographics → equitable risk distribution + ↑ generalizability | **集中招单一 demographic**（如仅 low-income）→ risk 不公分布 + ↓ generalizability |

### Inducement 详细机制

> [!danger] Inducement 为什么是问题
> Inducement = **过度 compensation** incentivize participants overlook otherwise unacceptable personal risks → undermine **autonomy during informed consent**。
> Vulnerable populations 经济上更需钱 → inducement risk 更高 → 历史上反复发生 exploitation。
> 临界判断：compensation = 参与时间的合理 hourly wage + 实际开销 → OK；compensation > 这个 → potential inducement。

### Vulnerable Population 经典清单

| Population | Why vulnerable | 额外保护 |
|---|---|---|
| **Low-income / 经济弱势** | 易因 financial incentive 接受 unacceptable risks | Compensation proportionate; IRB 额外审 |
| **Institutionalized**（养老院 / 精神病院 / 监狱）| Coercion 风险（机构 / staff 压力）| 独立 advocate; voluntary consent 严验 |
| **Cognitively impaired**（mild dementia / ID / severe psych）| Capacity 不足 / 易 manipulation | Surrogate consent + assent; **Mild ID 仍按 [[完整笔记/专题笔记/_衍生_Ethics精简框架]] §二 facilitate understanding** 先评 patient 自己 capacity |
| **Pregnant women + fetuses** | 双 subject（母 + 胎）+ fetus 不能 consent | Minimal risk default + IRB 额外审 |
| **Minors** | 不能 legal consent + 长期 outcome 未知 | Parental consent + child assent（如 ≥ 7 岁）|
| **Prisoners** | Coercion 风险（早释 / privilege 暗示）| 极严限制；仅 prisoner 群体直接相关 research |
| **Critically ill / 危急患者** | Decision under duress | 实际 surrogate；emergency exception 限定 |

### Inducement 经典 stem 暗号

| Stem 元素 | 通常暗示 |
|---|---|
| **"$X for Y hours" where $X >> hourly wage × Y** | Inducement |
| **"Vulnerable population exclusively"**（不招其他群体）| 违 ③ Range of demographics 原则 + 可能 exploitation |
| **"Compensation includes meals / 6 weeks' salary"** for 12 hr study | Excessive → inducement |
| **"Recruited from community resource center for convenience"** | 违 ② Recruitment relates to objectives 原则 |

### 关键陷阱

> [!warning]
> - "Vulnerable group 招募本身 = unethical" → ❌ Vulnerable groups 参与 research 常 **appropriate**（如 low-income depression 研究招 low-income）；问题是 **disproportionate + 无 valid 关联** 招募
> - "Compensation 提高 = 增 retention，伦理 OK" → ❌ Compensation 必须 proportionate to actual participation time + expenses，不是 retention 工具
> - "MRI / 高科技 treatment 受益不到 low-income 患者 → 不该招" (A 选项陷阱) → 部分正确但**不是核心 ethical issue**；inducement + 招募 disproportionate 才是核心
> - "Depression + 经济压力 increase 风险 → 招 low-income 满足 inclusion criteria 合理"（D 选项陷阱）→ Inclusion criteria 合理 ≠ inducement 合伦理；两个问题分开

---

## §四 Informed Consent for Research vs Clinical 区分（TODO 速记）

| 维度 | Clinical informed consent | Research informed consent |
|---|---|---|
| **目的** | 治疗 patient | 产生 generalizable knowledge |
| **要求** | Capacity ✓ + understand + appreciate + rationale | + Voluntary participation + **right to withdraw at any time** + **disclosure of research nature**（不是 standard care）|
| **IRB 审批** | 不需 | **必需** |
| **特殊 populations**（minor / prisoner / cognitively impaired）| Standard 决策树 | **额外保护**（minimal risk + 额外 consent / 替代决策机制）|

---

## 🔗 关联

- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Ethics_Master]] / [[完整笔记/专题笔记/_衍生_Ethics精简框架]]（核心 ethics 框架）
- 🔁 跨节联动：
  - 本文件 §一 COI ↔ [[完整笔记/专题笔记/_衍生_Ethics精简框架]] §十一 Medical Legal（informed consent SOP）
  - 本文件 §三 Vulnerable populations ↔ [[完整笔记/专题笔记/_衍生_Ethics精简框架]] §二 Capacity（cognitively impaired 评估）
- 🏥 跨学科：
  - [[完整笔记/Peixuan分科笔记/Biostats_Master]]（Bias 5 大类 + RCT 设计 + interim analysis 多次看会 inflate type I error / SPRINT 临床试验）
- 🌱 TODO：累积 IRB / informed consent for research / 更多 vulnerable population 题 → 衍生进一步扩展

### 错题锚定汇总
- **Q106885**（COI in clinical research — industry-employed statistician 做 analysis = 核心 COI / 双盲不能 mitigate analysis bias）⭐ v1.4 新增
- **RCT control selection 知识补充**（equipoise + multicomponent intervention 需 multicomponent control + inactive placebo 条件 — Q 题做对未入库）⭐ v1.4 新增
- **Stopping RCT early 3 类**（benefit/harm/futility）+ DSMB 角色（SPRINT-like example — Q 题做对未入库）⭐ v1.4.1 新增
- **Vulnerable Populations Research Recruitment + Inducement**（Compensation proportionate + Recruitment relates to objectives + Range of demographics — Q 题做对未入库）⭐ v1.4.1 新增
- **Q107273（DSMB external to research team AND study sponsor 双独立 / IRB ≠ DSMB / unblinded data review）⭐ v1.4.2 新增**

---

## ✅ 学习清单

- [ ] 默背 §一 Research ethics 4 大支柱（Equipoise / COI / IC for research / Control selection）
- [ ] 默背 §1.1 COI 4 大判定要素 + Mitigation 阶梯
- [ ] 默背 §1.5 **IRB vs DSMB 角色区分**（CK 高频）
- [ ] 默背 Double-blinding/Randomization 能/不能 mitigate 什么
- [ ] 默背 §二 Inactive placebo 何时 ethical
- [ ] 默背 §二 Stopping RCT early 3 类（benefit/harm/futility）
- [ ] 默背 §三 Vulnerable populations 7 类 + Recruitment 3 原则
- [ ] 默背 §四 Research vs Clinical informed consent 区分
