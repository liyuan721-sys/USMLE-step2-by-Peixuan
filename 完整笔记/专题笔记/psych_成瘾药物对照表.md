---
tags:
  - USMLE-Step2
  - psych
  - 神经
  - 专题笔记
created: 2026-05-19
type: 专题笔记
source: 2026-05-19 Claude.ai 草稿 v1 整合（Q12541 AUD vs 戒烟药 触发 — 错题卡待入库）
---

# 成瘾药物全景对照（Addiction Pharmacotherapy）
#难记

> [!info] 本笔记定位
> 用于一次性厘清 4 大成瘾领域的用药逻辑：**戒酒药 / 戒烟药 / 戒阿片药 / 急性戒断对症药**。
>
> 核心难点：**"患者当前是否还在用该物质"决定选哪个药**，这是 USMLE 最常考的临床决策点。
>
> **触发错题**：[[mistakes/uworld-mistakes#^Q12541]]（AUD 一线药选 Bupropion 误选 — 错题卡待入库）

---

## 目录

- [[#0. 核心决策框架（先看这个）|0. 核心决策框架]]
- [[#1. Alcohol（酒精）|1. Alcohol]]
- [[#2. Nicotine（烟草）|2. Nicotine]]
- [[#3. Opioid（阿片）|3. Opioid]]
- [[#4. Acute Withdrawal — 对症急救药（按物质分）|4. Acute Withdrawal]]
- [[#5. 大一统决策树|5. 大一统决策树]]
- [[#6. USMLE 高频陷阱（一句话总结）|6. USMLE 高频陷阱]]
- [[#7. 记忆挂钩|7. 记忆挂钩]]
- [[#8. 自测题（建议 3 天后做，看自己能否盲答）|8. 自测题]]
- [[#关联|关联]]

---

## 0. 核心决策框架（先看这个）

```
拿到一道成瘾题，按 3 步走：

Step 1 — 是哪种物质？
  └─ alcohol / nicotine / opioid / 多种共存

Step 2 — 患者现在什么状态？
  ├─ 急性戒断期（withdrawal）  → 对症药（救命，防 DT / 癫痫 / 心律失常）
  ├─ 仍在用，想戒（active use） → 维持期药（看能不能边用边启动）
  └─ 已戒断，防复饮（abstinent） → 维持期药（看是否需要"已戒断"前提）

Step 3 — 有无禁忌？
  └─ 肝/肾/心功能 / 共用其它成瘾物 / 怀孕 / 精神病史
```

---

## 1. Alcohol（酒精）

> [!info] 本章按"用药时间从早到晚"组织
> §1.1 时间轴 → §1.2 急性戒断（0-72h）→ §1.3 维持期（终身）→ §1.4 Naltrexone 双重身份补丁

### 1.1 时间轴速览 + AWS/alcohol withdrawal syndrome 4 阶段表

```
时间轴：
最后一杯酒 ─► 6-24h 轻度戒断 ─► 12-48h seizure/hallucinosis ─► 48-96h DT ─► 维持期（终身）
                  ↓                      ↓                         ↓               ↓
            BZD 起始              BZD（防进展 + 控制 seizure）   ICU + 大剂量 BZD   Naltrexone/
            （急性期药）              （急性期药）                  （急性期药）       Acamprosate/Disulfiram
                                                                                     （维持期药）
```

#### AWS 4 阶段完整表 ⭐⭐⭐（Q3187 触发入库）

| 阶段 | 时间窗 | 表现 | 定向力 / 生命体征 |
|---|---|---|---|
| **Mild withdrawal** | **6-24h** | 焦虑、失眠、震颤、出汗、心慌、胃肠不适 | 定向力**正常** |
| **Withdrawal seizure** | **12-48h** | 单次 / 多次 generalized **tonic-clonic** | 发作后 postictal |
| **Alcoholic hallucinosis** | **12-48h** | 视 / 听 / 触幻觉 | 定向力**正常** + 生命体征**稳定** ⭐ |
| **Delirium tremens (DT)** | **48-96h** | 混乱、躁动、发热、心动过速、高血压、出汗、幻觉 | 定向力**丧失** + 自主神经**风暴** + 可致死 |

> [!warning] Alcoholic hallucinosis vs DT — 别混淆
> 都出现在 12-96h 窗口且都有幻觉，但严重度天壤之别：
> - **Alcoholic hallucinosis** = 幻觉 + 定向力**正常** + 生命体征**稳定** → BZD + 支持即可
> - **DT** = 幻觉 + **定向力丧失** + 自主神经**风暴**（HR↑/BP↑/T↑）→ ICU + 大剂量 BZD，**可致死**

> [!tip] AWS 时间窗口口诀 "6-12-12-48"
> **6**h 颤 / **12**h 抽 / **12**h 幻 / **48**h 谵 — 越晚出现越严重。

### 1.2 【急性戒断期 6-96h】Benzodiazepines — 救命药 ⭐

| 药物 | 特点 | 适用 |
|---|---|---|
| **Chlordiazepoxide** | 长效（半衰期长，自我递减）| 肝功能正常患者首选 |
| **Lorazepam** | 短效，**仅经肾排泄**（无活性代谢产物）| **肝病/老年/危重患者**首选（LOT 法则：Lorazepam, Oxazepam, Temazepam）|
| **Diazepam** | 长效，起效快 | 严重戒断、DT |

> [!tip] LOT 法则记忆
> **L**orazepam / **O**xazepam / **T**emazepam — 这三个 **不经肝代谢**（无活性产物），**老年/肝病** 首选。

#### AWS seizure 用药对比 — 干扰项陷阱 ⭐（Q3187 触发）

| 药物 | 用于 AWS seizure | 机制 | 备注 |
|---|---|---|---|
| **Benzodiazepines** ⭐ | ✅ **First-line** | 直接激动 **GABA-A** → 恢复抑制张力 | Lorazepam / Diazepam IV 起效快 |
| **Phenobarbital** | ✅ 备选（status epilepticus 时加于 BZD 之上）| 也作用 **GABA-A** | 大剂量 BZD 抑制不够时补位 |
| **Phenytoin** | ❌ **无效** ⚠️ | **Na 通道阻断** — 不针对 GABA 失衡 | **USMLE 高频干扰项** |

> [!danger] 陷阱：Phenytoin 治 AWS seizure ❌
> AWS seizure 是 **GABA-A 受体脱敏 + rebound overexcitation** 引起 → 必须**补 GABA 抑制**（BZD 一线，Phenobarbital 补位）。
> Phenytoin 是 **Na 通道阻断**（针对过度兴奋的电传导），**作用点错** → 对 AWS seizure 完全无效。
> 口诀："**抗惊厥三候选**（BZD / Phenobarbital / Phenytoin）都是 seizure 题常见选项，但机制分两派 —— **GABA 派**（BZD + Phenobarbital，沾 GABA-A）vs **Na 通道派**（Phenytoin）；AWS seizure = GABA 失衡 → **只有 GABA 派有效**"。

> [!info] 名字别混：Phenobarbital vs Pentobarbital
> 都是 barbiturate，名字相似但临床角色完全不同：
> - **Pheno**barbital = **长效 AED**（抗癫痫药）—— AWS / status epilepticus **二/三线 + 维持**用药
> - **Pento**barbital = **短效麻醉级 barbiturate** —— **难治性 SE** ICU 持续输注（插管+昏迷诱导）/ 颅高压
>
> **"Pheno → 抗癫痫；Pento → 麻醉重症"**。neuro 笔记 status epilepticus 难治期写的 pentobarbital 是后者。

> [!danger] AUD 戒断会致死
> DT（震颤谵妄）+ 戒断性癫痫 → BZD 是**必给**药，不是可选。
> 注意：alcohol / BZD / barbiturate 三类戒断都依赖 GABA-A 系统，**只有这三类戒断会致死**（见 §4）。

> [!warning] 高频场景：术后 / 住院突发 seizure
> 长期酗酒患者术后 24-72h 内 seizure + 自主神经亢进 + 震颤 + 定向力差 → **首想 AWS**（不是 sepsis / meningitis / 头外伤）。
> 住院 / 术后患者常 **underreport alcohol use** —— USMLE 经典"住院后突发症状"鉴别陷阱。

→ 同源酒精指纹见 [[完整笔记/专题笔记/USMLE_实验室指纹诊断大全#5.5 慢性酒精性多系统指纹]]（MCV↑ + AST/ALT≥2:1）
→ 错题反链：[[mistakes/uworld-mistakes#^Q3187]] AWS withdrawal seizure / Phenytoin 陷阱（2026-05-19 入库，触发本节扩展）

### 1.3 【维持期 终身】3 药对比 ⭐⭐⭐（USMLE 高频考点）

| 维度 | **Naltrexone** | **Acamprosate** | **Disulfiram** |
|---|---|---|---|
| **一线/二线** | First-line | First-line | Second-line |
| **机制** | μ-opioid 拮抗 → 喝了不爽 → 减渴 | NMDA/GABA 调节 → 防戒断后稳态失衡 | ALDH 抑制 → 乙醛蓄积 → 喝了想吐（厌恶疗法）|
| **患者是否需先戒酒？** | ❌ **不需要**（边喝边启动）| ✅ **建议先戒酒**（用于已戒断的维持）| ✅ **必须先戒酒**（否则触发反应）|
| **核心适应症** | 渴望强烈、heavy drinking | 已戒断、防复饮 | 高动机、监督下用药 |
| **关键禁忌** | 急性肝炎/肝衰、用阿片（包括术后镇痛）| 严重肾损（CrCl<30）| 心衰、近期使用甲硝唑/含酒精药物 |
| **剂型亮点** | 有月剂型 IM（提高依从性）| 一日 3 次（依从性差）| 需家属/诊所监督 |

> [!danger] 一句话锁定（USMLE 必考）
> - **"Cravings too strong" + still drinking** → **Naltrexone**
> - **"Already abstinent" + 防复饮 + 肝病** → **Acamprosate**（肝衰也能用！）
> - **"Highly motivated" + abstinent + 监督环境** → **Disulfiram**

> [!warning] Disulfiram = second-line，"三必备"缺一不选 ⭐（Q15104 触发）
> 上表 Disulfiram "高动机、监督下用药" 还不够 —— 完整条件是 **3 个必须同时满足**：
> 1. **First-line 失败**（Naltrexone / Acamprosate 试过无效）
> 2. **Highly motivated**（戒酒决心铁 —— 不是"想喝酒"！USMLE 反向陷阱）
> 3. **Supervised**（有人监督服药防作弊，如配偶给药）
>
> 缺任何一条 → 回 first-line。
>
> **核心机制差异**：Disulfiram **不降 craving**（只靠"喝了难受"威慑）→ 有 craving 的患者恰恰需要 **anti-craving 药**（Acamprosate / Naltrexone 直接降冲动），不该用依赖意志力的 Disulfiram。

> [!tip] AUD 药物决策树（Q15104）
> ```
> moderate-severe AUD 需要药物
>   ├─ 有 withdrawal 症状 → Benzodiazepine（短期脱毒，≠ 长期治疗）
>   ├─ 已戒酒 + craving / 复发风险（first-line）
>   │    ├─ 肝病 / 用阿片药 → Acamprosate（肾排泄，肝安全）
>   │    ├─ 肾病 → Naltrexone
>   │    └─ 无禁忌 → Naltrexone 或 Acamprosate 均可
>   └─ first-line 失败 + motivated + supervised → Disulfiram
> ```

### 1.4 Naltrexone 双重身份警告 ⚠️（AUD vs OUD 启动时机）

| 用于 | 启动时机 |
|---|---|
| AUD | **边喝边启动 OK**（喝酒不会触发问题）|
| OUD | **必须先脱毒 7-10 天**（否则诱发严重戒断！）|

> [!warning] 反直觉点
> 同一个药，AUD 时"宽松"，OUD 时"严苛"——因为 AUD 患者体内没阿片，拮抗剂对他无所谓；OUD 患者体内有阿片，拮抗剂会立刻把阿片踢下受体 → 急性戒断爆发。

---

## 2. Nicotine（烟草）

### 2.1 是否还在抽烟 — 影响 NRT 和 Varenicline 启动时机

| 药物 | 机制 | 启动时机 | 关键禁忌 |
|---|---|---|---|
| **NRT**（贴片/口香糖/含片/吸入剂/喷雾）| 尼古丁替代 | **Quit Day 当天**起始（贴片）；或减量阶段开始 | 急性 MI / 严重心律失常（相对禁忌）|
| **Bupropion**（NDRI 抗抑郁药）| ↑ DA + NE 释放 | **戒烟前 1-2 周**启动，达到稳态后定 Quit Day | ❌ **癫痫** / **饮食障碍**（bulimia/anorexia）/ 近期 MAOI |
| **Varenicline**（α4β2 nAChR 部分激动剂）| 部分激动 → 缓解戒断，又阻断尼古丁奖赏 | **戒烟前 1 周**启动 | 严重肾损调整剂量；既往精神病史需评估 |

> [!warning] Bupropion 双重身份
> - 戒烟（Zyban 商品名）
> - 抗抑郁（Wellbutrin 商品名）
> - **不引起性功能障碍**（对比 SSRI 的优势）
> - **不引起体重增加**（饮食障碍患者吸引但 ❌ 禁用，因癫痫风险↑）

### 2.2 一线 vs 二线

| 一线 | 二线 |
|---|---|
| NRT / Bupropion / Varenicline（任选 1 或组合）| Nortriptyline / Clonidine（副作用大，少用）|

> [!tip] 组合方案
> NRT 长效贴片 + 短效口香糖 / 含片：基础+按需，效果优于单药

### 2.3 分阶段行为干预（Stage of Change）

> [!info] 烟草成瘾 = 三个层面，药物只覆盖前两个
> - **生理依赖**（physical）—— 戒断、craving → NRT / varenicline / bupropion 处理
> - **心理依赖**（psychological）—— 靠抽烟缓解压力
> - **习惯行为**（habitual）—— 饭后、开车、晨起自动点烟 → **只能靠行为咨询**处理
>
> 所以光给药不够，多数患者还需要 **behavioral counseling**；而行为干预要**按患者所处的"改变阶段"匹配**，不能一刀切。

| 阶段 | 干预重点 |
|---|---|
| **未准备戒**（not ready）| 动机访谈（**4R**：**R**elevance 相关性 / **R**isks 风险 / **R**ewards 益处 / **R**oadblocks 障碍）；每次就诊重复；可给 varenicline 走"边减边戒"策略 |
| **准备戒**（ready）| 定**明确 quit date** + 丢掉所有烟具；行为咨询 + 调动支持系统；开始药物（varenicline / bupropion / NRT）|
| **戒得吃力 / 反复早期复吸**（struggling）| **肯定部分成就**（不否定）；**识别触发 → 链接替代活动**；生物反馈（呼气 CO 监测 / app gamification）|
| **刚戒断**（recently quit）| 祝贺 + 持续支持；药物**再续约 12 周**；引导主动反思"生活有什么改变" |

> [!tip] 核心行为策略：触发 → 替代活动链接（trigger-linking）⭐
> 用于 **struggling 阶段**（已行动、但守不住、反复早期复吸）的患者：
> - 大多数烟瘾是**一过性的，只持续 5-10 分钟** → 熬过去就消退
> - **识别习惯性触发**（晨起咖啡、排便、开车）→ 把它**链接到一个分散注意力的替代活动**（剔牙、嚼口香糖）
> - 替代活动**最好由患者自己提出**（依从性更高）
> - 对**当天第一支烟**做这个链接尤其有效；**能延长"醒来 → 第一支烟"的时间 = 戒烟成功的强预测因子**

> [!warning] 阶段匹配陷阱（USMLE 高频）
> - **已进入 action 阶段**（已定药、已参加支持小组）的患者 → 不要再让他"列戒烟的益处和坏处" —— 那是 **not-ready 阶段**动机访谈的内容；已行动的人需要**具体行为策略**，不是再被说服。
> - **struggling 患者** → 不要简单"重定一个 quit date"：再错过会强化挫败、加重复吸循环。应做**触发识别 + 替代活动链接**。
> - **不要要求"压力降到最低再戒"** —— 生活压力是常态，戒烟咨询本身就包含教患者用更健康的方式应对压力。
> - 恐吓式（烟盒贴病变图）靠 guilt，可能促成一时决心，但**改变不了触发-习惯回路** → 不是持久策略。

---

## 3. Opioid（阿片）

> [!info] 本章按"用药时间从早到晚"组织
> §3.1 时间轴 → §3.2 急性过量（救命）→ §3.3 急性戒断（对症）→ §3.4 维持期 → §3.5 Precipitated Withdrawal 警告 → §3.6 三阶段绑死（防混淆，跨酒精对比）

### 3.1 时间轴速览

```
时间轴：
急性过量（RR↓+针尖瞳）─► 急性戒断（4-72h，痛苦不致死）─► 维持期（脱毒后 7-10 天起）
        ↓                          ↓                              ↓
    Naloxone                Methadone / Buprenorphine          Naltrexone（防复吸）
    IV/IM/IN                或 Clonidine（α2 对症）            Methadone/Buprenorphine 也可
   （救命药）                     （急性期药）                       （维持期药）
```

### 3.2 【急性过量】Naloxone — 救命药 ⭐

| 维度 | Naloxone |
|---|---|
| **触发场景** | 呼吸抑制（RR <8-10）+ 针尖瞳孔 + 昏迷 |
| **给药途径** | IV / IM / IN（鼻喷 Narcan）|
| **半衰期** | 短（30-90 min）—— 短于多数阿片，可能需重复给药 |
| **机制** | 短效 μ 拮抗 → 把阿片踢下受体 → 呼吸/意识恢复 |
| **重要预期** | 救命同时**会把患者推入急性戒断**（短暂、可控，但患者会很难受）|

> [!warning] 不要混淆 Naloxone ≠ Naltrexone
> 同为 μ 拮抗，但 Naloxone **短效救命**、Naltrexone **长效维持** —— 详见 §3.6 三阶段绑死。

### 3.3 【急性戒断 4-72h】Methadone / Buprenorphine / Clonidine — 对症药

| 药物 | 机制 | 用法 / 启动时机 | 注意 |
|---|---|---|---|
| **Methadone** | μ 完全激动剂（长效替代）| 仅 OTP 持牌诊所启动，可立即给 | 过量风险高（呼吸抑制致死）|
| **Buprenorphine** | μ 部分激动剂 + κ 拮抗 | 等 COWS ≥ 12 出现轻度戒断再给 | 门诊医生可开；过早给 → precipitated withdrawal（见 §3.5）|
| **Clonidine** | α2 激动 → 抑制蓝斑交感 | 对症缓解（流涕/心慌/出汗）| 辅助药，不解决核心激动剂缺失 |
| **对症辅助** | — | Loperamide（止泻）/ Ondansetron（止吐）/ NSAID（肌痛）| 按需 |

> [!info] 阿片戒断 = "症状指纹（必现）" + "体检发现（可有可无）" ⭐（Q3189 触发反思）
> UW 教学文本严格分两层（用词差异 = 诊断分层关键）：
>
> **Symptoms（"primarily include"，必现 = 指纹）**：
> - Sleep disturbance（失眠）
> - Nausea / vomiting
> - **Abdominal cramping**（绞痛）
> - **Diarrhea**（水样腹泻）
> - **Myalgia / arthralgia**（肌痛 / 关节痛）
>
> **Examination findings（"may also be evident"，可有可无 = 补充）**：
> - Dilated pupils (mydriasis)
> - Yawning（打哈欠）
> - Piloerection（鸡皮疙瘩）
> - Lacrimation / rhinorrhea（流泪 / 流鼻涕）
> - **Hyperactive bowel sounds**
> - Diaphoresis
>
> **诊断关键**：症状 4-5 联齐全（吐/泻/痛/失眠/酸痛）= 强烈提示 opioid 戒断；**体检发现缺失不能否定**诊断。USMLE 高阶题（如 [[mistakes/uworld-mistakes#^Q3189]]）故意只给症状不给典型体检 → 考"排除法"思维（vital signs 正常 → 排除 GABA 类；HR 不慢 + 黏膜干 → 排除 cholinergic；剩 opioid）。
>
> 痛苦但**通常不致死**（成人）。

#### UW Opioid Withdrawal 4 维度完整表

![[{04B719AC-9897-4F69-9622-6F37F3CDB781}.png]]
*↑ UW 原图：Opioid Withdrawal 4 维度对照（Time course / Clinical / Diagnosis / Management）*

**关键补充信息（图独有，前述文本未明示）**：
- **Time course 警示** ⚠️：给 **opioid antagonist**（Naloxone / Naltrexone）后**立即**发作 = 医源性 precipitated withdrawal（life-threatening！见 §3.5）
- **Diagnosis = History & examination alone** —— **纯临床诊断**，不需要 tox screen / 血检
- **Cardiac vital signs 调和**：UW 此图列 "↑ pulse / ↑ BP / diaphoresis"，需与下方 "vital signs OFTEN NORMAL" 调和 → 阿片戒断 vital signs **可轻度升高（mild），但不会 storm**（与 GABA 类戒断的 autonomic storm 严重度差很多）

→ 来源：[[mistakes/uworld-mistakes#^Q3189]] 图 2（双地点 Obsidian 反向链接调取）

> [!danger] 关键鉴别：vital signs 是决定性证据 ⭐⭐⭐（Q3189 触发）
> **Alcohol / BZD 戒断 = autonomic STORM**（HR/BP/T 全飙 + AMS + 可 seizure 致死）
> **Opioid 戒断 = 痛苦但 vital signs OFTEN NORMAL**（清醒 + 想活下来 + 不会死）
> **题干特意写 "vital signs are normal"** + diaphoresis + 胃肠症状（吐/泻/痛）+ 肌痛 + 失眠 → **Opioid withdrawal**
> 戒断鉴别 3 大类速记口诀："**GABA 飙 / 阿片平 / 兴奋剂沉**"

#### 阿片中毒 vs 戒断（"反向阿片"对照表）

| 系统 | 中毒（Intoxication）| 戒断（Withdrawal）|
|---|---|---|
| **瞳孔** | **针尖 miosis** | **散瞳 mydriasis** |
| **肠** | 便秘 | **腹泻 + 肠鸣音 ↑** |
| **CNS** | 镇静 / 昏迷 | 失眠 / 焦虑 / 烦躁 |
| **呼吸** | 抑制（致死）| 正常或略快 |
| **皮肤** | — | 出汗 + **piloerection（goosebumps）** |
| **分泌** | — | **流泪 + 流鼻涕 + 打哈欠 + 流口水** |
| **肌肉** | — | **肌痛 myalgia + 肌阵挛轻** |

"Cold turkey" 形象 = piloerection + 寒战 + 苍白 → 像冷的火鸡皮。

> [!tip] 起病时间窗
> - 短效阿片（**海洛因**）：last dose 后 **4-12h** 起；24-48h 高峰
> - 长效阿片（**美沙酮**）：last dose 后 **24-48h** 起；72-96h 高峰

### 3.4 【维持期 长期】三药对比 ⭐⭐⭐

| 维度 | **Methadone** | **Buprenorphine** | **Naltrexone** |
|---|---|---|---|
| **机制** | μ **完全激动剂** | μ **部分激动剂** + κ 拮抗 | μ **拮抗剂** |
| **患者状态** | 在用阿片 / 戒断中均可 | 在用阿片 / 戒断中均可（但要等轻度戒断出现再给）| **必须已脱毒** |
| **启动前提** | 可立即启动 | 等 COWS 评分提示轻度戒断（避免 precipitated withdrawal）| 末次短效阿片 ≥ 7 天；末次长效（美沙酮）≥ 10-14 天 |
| **滥用风险** | 高（黑市流通）| 低（部分激动 + 含 naloxone 复方）| 无（拮抗剂）|
| **处方限制** | 仅限注册诊所（OTP）| 门诊医生可开（DATA 2000 / X-waiver 已取消）| 任何医生可开 |
| **过量风险** | 可致死（呼吸抑制）| 低（部分激动有"天花板效应"）| 无 |
| **孕妇** | ✅ 推荐 | ✅ 推荐 | ❌ 不推荐 |

### 3.5 Precipitated Withdrawal（医源性戒断）⚠️

> [!danger] 患者体内有阿片时，给 Buprenorphine 或 Naltrexone → 把强效阿片踢下 μ 受体 → 急性剧烈戒断
> - **Buprenorphine**：等 COWS ≥ 12 再给
> - **Naltrexone**：等完全脱毒 ≥ 7 天（短效阿片）/ ≥ 10-14 天（美沙酮等长效）

### 3.6 三阶段绑死 — Naltrexone / Naloxone / 戒断管理药 三角关系 ⭐

> [!warning] 高频误区纠正
> 学生常说"Naltrexone 用于酒精和阿片**戒断**，Naloxone 只用于阿片**戒断**" —— **这句话两个错误**。
> 
> **"过量（overdose）" ≠ "戒断（withdrawal）" ≠ "维持（maintenance）"** —— 三个完全不同的临床阶段，对应三类完全不同的药。

| 阶段 | 临床场景 | Alcohol | Opioid |
|---|---|---|---|
| **急性过量**（overdose）| 救命 | 支持治疗（无特效解毒剂）| **Naloxone** |
| **急性戒断**（withdrawal）| 停药后症状管理（震颤/癫痫/痛苦）| **BZD** | **Methadone / Buprenorphine / Clonidine** |
| **维持/防复发**（maintenance）| 长期不让复用 | **Naltrexone / Acamprosate / Disulfiram** | **Naltrexone**（脱毒后）/ Methadone / Buprenorphine |

> [!danger] 两条否定句必背
> - **Naltrexone 不治戒断症状** —— 它治"防复发"。AUD 急性戒断仍要用 BZD；阿片急性戒断仍用 Methadone/Buprenorphine/Clonidine。
> - **Naloxone 不治阿片戒断** —— 它逆转"急性过量"。给戒断中的患者用 Naloxone = 雪上加霜（加重戒断），临床绝不这么做。
> 
> **反向陷阱**：Naltrexone 给正在用阿片的患者 → 诱发严重 precipitated withdrawal（见 §3.5）；Naloxone 给阿片过量患者 → 救命但**会突然把患者推入急性戒断**（短暂、可控，但要预期）。

> [!tip] 一句话锁定三角关系
> - 救命 = **Nalox**one（**N**ow，鼻喷/IV，30 分钟代谢完）
> - 戒断管理 = **BZD（酒）/ Methadone-Buprenorphine（阿片）**
> - 防复发 = **Naltrex**one（**L**ong-term，口服/IM 月剂）

---

## 4. Acute Withdrawal — 对症急救药（按物质分）

| 物质戒断 | First-line | 关键机制 | 危险信号 |
|---|---|---|---|
| **Alcohol** | **Benzodiazepines** | 替代 GABA-A 兴奋抑制 | DT（震颤谵妄）、戒断性癫痫 — 可致死 |
| **Benzodiazepines** | **长效 BZD 缓慢递减**（Diazepam / Chlordiazepoxide）| 同上 | 戒断性癫痫 — 可致死 |
| **Opioids** | **Methadone / Buprenorphine**（最佳）或 **Clonidine** 对症 | 替代 μ 激动 / 抑制蓝斑交感 | 痛苦但**通常不致死**（成人）|
| **Nicotine** | **NRT** | 替代尼古丁 | 不致死 |
| **Stimulants**（cocaine, amphetamine）| **支持治疗**（无 FDA 药）| — | 抑郁 / 自杀念头 — 心理监测 |
| **Cannabis** | **支持治疗** | — | 不致死 |

> [!danger] 戒断会致死的只有 3 类
> **Alcohol / Benzodiazepines / Barbiturates**（共同点：GABA-A 系统依赖）
> 其它戒断（阿片、可卡因、大麻、尼古丁）"痛苦但不致死"。

#### UW 6 物质戒断对照表（症状 + 体检发现）

![[{B47FDB4C-F732-4698-850A-687DA01673C8}.png]]
*↑ UW 原图：6 物质戒断症状 + 体检发现完整对照（与上方"治疗对照表"互补）*

**关键对比要点**：
- **Alcohol / BZD** 体检 = **seizures + tachycardia + palpitations**（GABA 类自主神经风暴）
- **Opioids** 体检 = **dilated pupils + yawning + piloerection + lacrimation + hyperactive bowel sounds**（"反向阿片"指纹，区别于 §3.3 中毒针尖瞳 / 便秘）
- **Stimulants / Nicotine / Cannabis** 体检 = **no significant findings**（这就是为什么 "GABA 飙 / 阿片平 / 兴奋剂沉" 口诀成立）

→ 来源：[[mistakes/uworld-mistakes#^Q3189]]（Heroin 戒断 vs BZD 戒断错题，2026-05-19 入库；图同时存于错题卡 + 本章节，**双地点 Obsidian 反向链接调取**）

---

## 5. 大一统决策树

```
患者来就诊：

成瘾物质？
├─ Alcohol
│   ├─ 急性戒断（< 72h，震颤/谵妄/癫痫风险）
│   │   └─► BZD（chlordiazepoxide / lorazepam if 肝病）
│   └─ 维持期
│       ├─ 还在喝 + cravings 强 ──► Naltrexone
│       ├─ 已戒断 + 防复饮 ───────► Acamprosate（肝病也能用）
│       └─ first-line 失败 + 高动机 + 已戒断 + 监督─► Disulfiram（second-line）
│
├─ Nicotine
│   ├─ 想戒（Quit Day 设定）
│   │   ├─ 一线：NRT / Bupropion / Varenicline
│   │   └─ Bupropion 禁忌：癫痫、饮食障碍
│   └─ 急性戒断（不致死，按需 NRT）
│
├─ Opioid
│   ├─ 急性过量（呼吸抑制）─────► Naloxone
│   ├─ 急性戒断（痛苦不致死）──► Methadone / Buprenorphine（最佳）或 Clonidine
│   ├─ 维持期 — 还在用
│   │   ├─► Methadone（OTP 诊所）
│   │   └─► Buprenorphine（门诊，等 COWS ≥ 12）
│   └─ 维持期 — 已脱毒 ≥ 7 天
│       └─► Naltrexone（任意医生可开，月剂 IM 最佳依从性）
│
└─ Benzodiazepine
    └─ 急性戒断 ──► 长效 BZD 缓慢递减（不能突然停！会癫痫）
```

---

## 6. USMLE 高频陷阱（一句话总结）

| 陷阱 | 正解 |
|---|---|
| Stem 提 smoking 12 年 + 问 AUD 用药 → 选 Bupropion ❌ | Bupropion 是**戒烟**药，不治 AUD（Q12541 触发本笔记）|
| Stem 患者 still drinking → 选 Disulfiram ❌ | Disulfiram 要**先戒酒** |
| AUD 有 craving / 怕复发 → 选 Disulfiram ❌（Q15104）| Disulfiram **不降 craving**；有 craving 用 **anti-craving 药**（Acamprosate / Naltrexone）|
| 戒酒一段时间 / 患者 motivated → 直接上 Disulfiram ❌（Q15104）| Disulfiram 是 **second-line**，"三必备" = first-line 失败 + motivated + supervised，缺一不选 |
| AUD + 肝衰 → Naltrexone ❌ | 肝衰用 **Acamprosate**（肾排，肝病安全）|
| OUD 患者还在用海洛因 → Naltrexone ❌ | 必须**脱毒 7 天**才能用 Naltrexone |
| 阿片过量 → Naltrexone ❌ | 救命用 **Naloxone**（短效 IV/IM/IN）|
| 急性阿片戒断症状管理 → Naloxone / Naltrexone ❌ | 戒断用 **Methadone / Buprenorphine / Clonidine**；Naloxone 会**加重**戒断（见 §3.4）|
| "Naltrexone 是戒断药" ❌ | Naltrexone 是**防复发**药（维持期），不是戒断症状管理药；AUD 戒断仍用 BZD |
| 老年/肝病 alcohol withdrawal → Chlordiazepoxide ❌ | 用 **Lorazepam**（LOT 法则）|
| AWS seizure → Phenytoin ❌（Q3187 高频干扰项）| AWS seizure 用 **BZD**（GABA-A）；status epilepticus 加 **Phenobarbital**；Phenytoin 是 Na 通道，作用点错 |
| 术后 24-72h 突发 seizure → sepsis / 头外伤 ❌ | 长期酗酒者首想 **AWS**（住院常 underreport alcohol use）|
| 戒断 + vital signs 正常 → 选 alcohol/BZD 戒断 ❌（Q3189 触发）| Opioid 戒断 vital signs **正常**；vitals 飙 = **alcohol/BZD 戒断**（GABA 类）— "GABA 飙 / 阿片平 / 兴奋剂沉" |
| 派对后 seizure + 高热 + myoclonus + SSRI 用户 → 选 cannabis ❌（Q11853 触发）| **MDMA + Serotonin Syndrome**：高热 + 肌阵挛 + 反射亢进 + 低钠 + SSRI 用户 = 指纹（MDMA 不在本笔记，见 [[mistakes/uworld-mistakes#^Q11853]]）|
| 看不到 dilated pupils + yawning + piloerection → 不诊断 opioid 戒断 ❌（Q3189 反思）| 这些是 **"may also be evident"**（体检发现，可有可无）；**症状 4-5 联**（吐/泻/痛/失眠/酸痛）才是 **"primarily include"**（指纹必现）。体检缺失**不能否定**诊断，必须用**排除法**（详见 §3.3 + 错题 [[mistakes/uworld-mistakes#^Q3189]]）|
| 戒烟选 Bupropion + 患者有癫痫 / 神经性贪食 ❌ | Bupropion **禁忌**：癫痫、饮食障碍 |
| BZD 戒断突然停药 ❌ | 必须**缓慢递减**，否则癫痫致死 |

---

## 7. 记忆挂钩

> [!success] 成瘾科 4 兄弟门诊分工
> ```
> ┌─────────────────────────────────────────┐
> │  门诊大厅                                │
> ├─────────────────────────────────────────┤
> │  Naltrexone   "管酒 + 管阿片"            │
> │               拔掉快乐键的人              │
> │                                          │
> │  Acamprosate  "只管酒"                   │
> │               让大脑安静下来的人          │
> │                                          │
> │  Disulfiram   "吓唬已经戒酒的人"         │
> │               让你害怕喝酒的人            │
> │                                          │
> │  Methadone    "管阿片"                   │
> │               OTP 诊所专员                │
> │                                          │
> │  Buprenorphine "管阿片"                  │
> │               门诊也能开的轻骑兵          │
> │                                          │
> │  Bupropion    "管烟 + 抗抑郁"            │
> │               双修选手                    │
> │                                          │
> │  Varenicline  "只管烟"                   │
> │               尼古丁受体冒牌货            │
> │                                          │
> │  Naloxone     "急诊救命"                 │
> │               不在门诊                    │
> └─────────────────────────────────────────┘
> ```

> [!tip] Nalox vs Naltrex 一秒区分
> - **Nalox**one = "Now! 救命！" → 短效，急救
> - **Naltrex**one = "Next 几个月" → 长效，维持

---

## 8. 自测题（建议 3 天后做，看自己能否盲答）

> [!question]- Q1：45 yo 男性，alcohol use disorder，每日饮 8 罐啤酒，想戒但 cravings 强。无肝病。最佳药物？
> **Naltrexone**（still drinking 也能启动；cravings 强是 Naltrexone 的靶适应症）

> [!question]- Q2：同上患者，但 AST 800 / ALT 600 + bilirubin 5。最佳药物？
> **Acamprosate**（Naltrexone 急性肝炎禁忌；Acamprosate 经肾排，肝病安全）

> [!question]- Q3：38 yo 阿片成瘾者，正在使用海洛因，要求戒毒。可否立即给 Naltrexone？
> ❌ 不可。会诱发 precipitated withdrawal。必须**先脱毒 7-10 天**。可改用 Buprenorphine（等 COWS ≥ 12 后）或 Methadone。

> [!question]- Q4：72 yo 老年男性，alcohol withdrawal 第 1 天，肝硬化 Child B。BZD 怎么选？
> **Lorazepam**（LOT 法则：经肾排，无活性代谢产物，肝病/老年首选）

> [!question]- Q5：30 yo 女性，想戒烟（1 PPD × 10 年），有 bulimia 病史。能选 Bupropion 吗？
> ❌ 不能。Bupropion **禁忌**：饮食障碍 + 癫痫。改用 NRT 或 Varenicline。

> [!question]- Q6：阿片过量呼吸 4 次/分，瞳孔针尖。给哪个药？
> **Naloxone**（不是 Naltrexone！短效救命药）

> [!question]- Q7：35yo 男性术后 30h 出现 tonic-clonic seizure + 震颤 + 出汗 + 反射亢进，长期酗酒史。下一步？给 Phenytoin 行吗？
> **IV BZD**（lorazepam / diazepam）。**Phenytoin ❌ 无效**：AWS seizure 是 GABA-A 脱敏 + rebound overexcitation，Phenytoin 是 Na 通道阻断 → 作用点错。Status epilepticus 时可加 **Phenobarbital**（也是 GABA-A）。

> [!question]- Q8：17yo 男孩 24h 呕吐 / 水样腹泻 / 失眠 / 全身酸痛 + 出汗 + 干黏膜 + **vital signs 全正常**（T 36.6 / HR 88 / BP 110/74）。诊断？为什么不是 BZD 戒断？
> **Heroin (Opioid) Withdrawal**。BZD / Alcohol 戒断**必有 autonomic storm**（HR/BP/T 全飙 + AMS + 可 seizure），本题 vital signs 全正常 → 直接排除 GABA 类戒断。Opioid 戒断 = "痛苦但不死"，vital signs 通常正常。口诀 "GABA 飙 / 阿片平 / 兴奋剂沉"。

> [!question]- Q9：21yo 大学男生派对后 seizure，PMH MDD on sertraline。T 40°C / HR 120 / BP 170/96 / diaphoretic + 肠鸣音↑ + DTR 3+ + myoclonus + Na 122。诊断？为什么不是 cannabis？
> **MDMA (Ecstasy) intoxication + Serotonin Syndrome**。Cannabis 没有 hyperthermia / myoclonus / hyperreflexia / 低钠。MDMA = synthetic amphetamine（推 NE/DA/5-HT），与 SSRI 合用 → 严重 SS。低钠机制：SIADH + 过度饮水降温。"干 vs 湿" 鉴别：anticholinergic（DPH）= 干（皮肤干 + 肠鸣音↓）；MDMA/SS = 湿（diaphoresis + 肠鸣音↑）。

> [!question]- Q10：中年女性 AUD 戒酒 2 周，occasional cravings + 怕复发，无 withdrawal 症状、无肝病、无阿片药。最佳药物？为什么不是 Disulfiram？
> **Acamprosate 或 Naltrexone**（first-line anti-craving 药）。**不选 Disulfiram**：① 是 second-line，需 first-line 失败才考虑 ② Disulfiram 不降 craving，只靠"喝了难受"威慑 ③ "三必备"= failed first-line + highly motivated + supervised，本题一条都不满足。有 craving = 需 anti-craving 药主动降冲动，不靠意志力。

---

## 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes#^Q12541]] AUD 一线药 — Bupropion 误选 → 正解 Naltrexone（触发本笔记，2026-05-19 入库）
  - [[mistakes/uworld-mistakes#^Q3187]] ✅ AWS withdrawal seizure / Phenytoin 陷阱（2026-05-19 入库，触发 §1.1 AWS 4 阶段表 + §1.2 Phenytoin 陷阱扩展）
  - [[mistakes/uworld-mistakes#^Q3189]] Heroin 戒断 vs BZD 戒断（vital signs 鉴别）（2026-05-19 入库，触发 §3.3 vital signs callout + 反向阿片表 + §6 陷阱表）
  - [[mistakes/uworld-mistakes#^Q11853]] MDMA + Serotonin Syndrome（SSRI 陷阱）（2026-05-19 入库，跨链 — MDMA 不在本笔记定位，触发 §6 陷阱表 + 跨链建议新建中毒鉴别专题）
  - [[mistakes/uworld-mistakes#^Q12432]] AUD vs AD 鉴别做对（实验室指纹 MCV+AST/ALT 定胜负 — 见 USMLE_实验室指纹大全 §5.5.x）
  - [[mistakes/uworld-mistakes#^Q3382]] AD vs MDD 鉴别 + psychotherapy 一线（精神科治疗"诊断对≠治疗对"同源）
  - [[mistakes/uworld-mistakes#^Q15104]] AUD 药物治疗 — Acamprosate vs Disulfiram（2026-05-19 入库，触发 §1.3 Disulfiram 三必备 callout + AUD 决策树 + §6 陷阱表 2 行 + §8 Q10）
  - 等积累更多 OUD / Smoking Cessation / AUD 错题后横向连接
- 📚 主笔记：
  - [[完整笔记/Peixuan分科笔记/psych]]（成瘾医学章节）
- 🏥 跨学科：
  - [[完整笔记/专题笔记/psych_物质急性中毒鉴别表]] ⭐ **互补专题**（v1 = 2026-05-19，Q11853 触发新建；本笔记 = 戒断 / 维持 / 急救药，对方 = 中毒急性表现 + SS/NMS/MH）
  - [[完整笔记/专题笔记/USMLE_实验室指纹诊断大全]] §5.5 慢性酒精性多系统指纹（MCV↑ + AST/ALT≥2:1 = AUD 指纹）+ §5.5.x AUD vs AD 鉴别
  - [[完整笔记/Peixuan分科笔记/消化腺]]（肝衰影响 Naltrexone 选择；AUD 共病肝硬化）
  - [[完整笔记/Peixuan分科笔记/肾脏]]（CrCl<30 → Acamprosate 禁）
  - [[完整笔记/Peixuan分科笔记/感染]]（IVDU → HCV / HIV，影响 OUD 药物选择）
  - [[完整笔记/Peixuan分科笔记/OB]]（孕妇 OUD → Methadone / Buprenorphine，禁 Naltrexone）
  - [[完整笔记/专题笔记/心内_老年多药患者诊断思维]] §2.3 Cirrhosis 用药陷阱（benzo/opioid 蓄积诱发 HE）
- 🌱 TODO（后续整合）：
  - 累积更多 OUD / Smoking Cessation 错题后 → 补充本笔记的"易混表"
  - 累积更多 BZD 戒断 / DT 错题后 → 强化 §1.4 急性戒断章节
  - 考虑生成 [[完整笔记/专题笔记/psych_神经递质_成瘾环路]]（μ-opioid / NMDA / GABA / DA 通路与药物对应）
  - ✅ Q12541 错题卡已于 2026-05-19 入库（^Q12541），anchor 反链已激活

---

## 版本记录

- **v1（2026-05-19）**：基于 Q12541 错题首次成稿，覆盖 4 大成瘾领域全景对照
- **v1.1 正式整合（2026-05-19）**：从草稿升级为专题笔记
  - frontmatter 标准化（USMLE-Step2 / psych / 神经 / 专题笔记）
  - 修复 wikilink：`_衍生_神经递质_成瘾环路` → `psych_神经递质_成瘾环路`；Q12541 `#` → `#^`
  - 关联补充 USMLE_实验室指纹大全 §5.5 / Q3382 AD 同源（治本原则）/ 心内_老年多药 §2.3
- **v1.2（2026-05-19）**：补 §3.4 "三阶段绑死" 章节 + §6 陷阱表 2 行
  - 触发：对话中用户问"Naltrexone 用于酒精和 opioid 戒断、Naloxone 只用于 opioid 戒断" → 揭示原笔记**缺少否定型陈述**（"Naltrexone/Naloxone 都不是戒断管理药"）
  - 新增内容：戒断 vs 维持 vs 过量 三阶段表 + 两条否定句必背 + 反向陷阱（Naloxone 给戒断患者会加重）
- **v1.3（2026-05-19）按用药时间重组**：用户反馈"太乱了"——指出每个物质章节内部时间顺序混乱
  - **§1 Alcohol** 内部按"急性戒断 → 维持期"重排（原 §1.2 维持期 3 药在前 / §1.4 BZD 在后 → 倒置为：§1.2 BZD 急性救命在前 / §1.3 维持期 3 药在后）
  - **§3 Opioid** 内部按"过量 → 戒断 → 维持期"重排（拆开原 §3.3 过量 vs 戒断混合表，明确为：§3.2 急性过量 Naloxone / §3.3 急性戒断 Methadone-Bup-Clonidine / §3.4 维持期三药 / §3.5 Precipitated Withdrawal / §3.6 三阶段绑死）
  - 每章新增"本章按用药时间从早到晚组织"info callout + 时间轴速览
  - §2 Nicotine 不动（原"启动时机"列已覆盖时间维度）
- **v1.4（2026-05-19）Q3187 触发增量**：做对题反向贡献新知识点
  - **§1.1** 时间轴细化（6h/12h/12h/48h 4 阶段窗口纠正 — 原"24-72h DT/癫痫高峰"是混淆）+ 新增 AWS 4 阶段完整表（mild / seizure / hallucinosis / DT）+ alcoholic hallucinosis vs DT 鉴别 callout + "6-12-12-48"口诀
  - **§1.2** 章节标题"0-72h" → "6-96h"（覆盖 DT 窗口）+ 新增 AWS seizure 用药对比表（BZD / Phenobarbital / Phenytoin）+ Phenytoin 陷阱 danger callout + 术后 underreport alcohol use 高频场景 callout
  - **§6** 陷阱表 +2 行（Phenytoin 治 AWS seizure / 术后突发 seizure 想 sepsis）
  - **§8** 自测题 +Q7（AWS seizure + Phenytoin 陷阱）
  - 错题反链：[[mistakes/uworld-mistakes#^Q3187]]
- **v1.5（2026-05-19）分科同步 + Pentobarbital 澄清**：Q3187 触发的衍生扩展后，扫 3 个分科笔记找增量并整合
  - **§1.2** 新增 "Phenobarbital vs Pentobarbital 别混" info callout（Pheno=AED / Pento=麻醉重症；neuro 笔记 SE 难治期用的是后者）
  - **外科分科** `外科.md` "Postoperative Confusion" 节加 AWS / Withdrawal Seizure 项（4 阶段时间窗 + Phenytoin 陷阱 + 反链）
  - **neuro 分科** `neuro.md` Alcohol withdrawal 节加 "AWS seizure 用药陷阱" 警告（Phenytoin 无效）+ 反链
  - **psych 分科** `psych.md` 加 2 处反链（Alcohol Withdrawal Timeline 前 + SUD 表后），指向本笔记 §1.3 / §3.4 / §2
- **v1.6（2026-05-19）Q3189 + Q11853 双错题触发增量**：
  - **§3.3** 新增 **vital signs 关键鉴别 danger callout**（"GABA 飙 / 阿片平 / 兴奋剂沉"口诀）+ **阿片中毒 vs 戒断"反向阿片"对照表**（瞳孔/肠/CNS/呼吸/皮肤/分泌/肌肉 7 维度）+ 起病时间窗（短效 4-12h / 长效 24-48h）
  - **§6** 陷阱表 +2 行（vital signs 正常 → opioid 戒断 / 派对后 seizure + SSRI → MDMA + SS）
  - **§8** 自测题 +Q8（opioid 戒断 vs BZD 戒断）+ Q9（MDMA + SS）
  - **关联** 加 Q3189 + Q11853 反链
  - MDMA 不在本笔记定位（戒/维持/急救），仅跨链；TODO 累积 3-5 道中毒/SS/NMS/MH 错题后考虑新建 [[完整笔记/专题笔记/psych_物质急性中毒鉴别表]]
- **v1.7（2026-05-19）大规模分科同步 + 互补专题新建**（用户审阅 9 项增量清单后选"都做"）
  - ⭐ **新建** [[完整笔记/专题笔记/psych_物质急性中毒鉴别表]] **v1**（Q11853 触发；6 大物质中毒 + SS/NMS/MH 三联鉴别 + Anticholinergic vs Cholinergic 干湿对照；与本笔记**互补定位**）
  - **psych.md**：① L1118-1124 中毒表加 **MDMA + 抗胆碱 + PCP** 3 行 ② L476 SS vs NMS 一句话升级反链 ③ L1124 后加 **4 大戒断 vital signs 对比表** + MDMA 简短小节
  - **neuro.md**：① L7490 MH vs NMS 表升级为 **SS vs NMS vs MH 三联鉴别**（USMLE 高频空白补齐）+ 三药角色（Dantrolene / Bromocriptine / Cyproheptadine）+ 速记决策 callout ② L12023 NMS 加 SS 鉴别反链 ③ L6401 Myoclonus 加 **6 大成因鉴别**（SS / 缺氧 / 代谢 / 感染 / 退行 / 抗胆碱）
  - **uworld-mistakes** Q11853 + Q3189 TODO 全部 ✅ + 跨链补强
  - **关联** 加新专题反链（**互补定位** 明示）
- **v1.8（2026-05-19）Q3189 二次反思 — "症状指纹 vs 体检发现" 用词分层**：用户洞察"经典 opioid 体检几乎全缺，stem 怎么诊断 opioid" → 揭示 UW 教学文本用词差异是关键诊断分层
  - **§3.3** 阿片戒断 info callout 重写为两层结构（**Symptoms "primarily include" = 必现指纹** vs **Examination findings "may also be evident" = 可有可无补充**）+ 排除法 4 步诊断思维
  - **§6** 陷阱表 +1 行（体检缺失不能否定 opioid 戒断诊断 — 必须排除法）
  - **错题卡 Q3189** 加 "实际诊断路径 — 排除法" 段（含 USMLE Step 2 高阶技能 callout：pattern recognition → 排除法）+ 更新 "我为什么错" 加深一层教训
- **v1.9（2026-05-19）Q3189 图归位 ×3**：错题卡 Q3189 用户追加 2 张新图（共 3 张）→ 按双地点工作流归位
  - **图 1**（UW Common Withdrawal Syndromes）→ 主笔记 §4 已归位（v1.7）
  - **图 2**（UW Opioid Withdrawal 4 维度完整表）→ 主笔记 **§3.3** 归位 + 补充图独有 3 点（**time course 警示 / 纯临床诊断 / vital signs 调和**：mild ≠ storm）
  - **图 3**（UW Cholinergic Toxicity DUMBELS）→ [[完整笔记/专题笔记/psych_物质急性中毒鉴别表]] **§6.2** 归位 + 补充 nicotinic effects
  - **错题卡 Q3189** 3 张图说明拆分（每图独立说明 + 各自归位反链）
- **v1.10（2026-05-19）Q15104 触发 — Disulfiram "三必备" + AUD 决策树**：
  - **§1.3** 新增 "Disulfiram = second-line 三必备" warning callout（first-line 失败 + motivated + supervised，缺一不选）+ "Disulfiram 不降 craving"机制澄清 + AUD 药物决策树 tip callout
  - **§5** 大一统决策树 alcohol 维持期 Disulfiram 行加 "first-line 失败" 前提
  - **§6** 陷阱表 +2 行（有 craving 选 Disulfiram ❌ / 戒酒一段时间就上 Disulfiram ❌）
  - **§8** 自测题 +Q10（AUD 药物选择 — 为什么不是 Disulfiram）
  - **关联** 加 Q15104 反链
- **v1.11（2026-05-19）Q23098 触发 — §2 戒烟分阶段行为干预**：
  - **§2** 新增 §2.3 "分阶段行为干预（Stage of Change）"：烟草成瘾三层面（生理 / 心理 / 习惯）+ 4 阶段（未准备 / 准备 / 吃力 / 刚戒）干预对照表 + trigger-linking 核心行为策略 callout + 阶段匹配陷阱 warning callout
  - 触发题 Q23098（做对，未入错题本）—— 知识补充，非错题同步
- 待补充：随后续错题积累，逐步增补具体陷阱场景与临床决策细节
