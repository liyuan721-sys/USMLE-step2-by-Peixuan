---
tags:
  - USMLE-Step2
  - 心血管
  - 急诊
  - 专题笔记
created: 2026-05-14
type: 专题笔记
parent_topic: ACLS 心脏骤停急救决策树 + 4 节律 + 5H5T + 三种电击
source_错题: Q4725
---

# _衍生_ACLS 急救决策树（Advanced Cardiac Life Support）

> [!info] 本笔记定位
> **心脏骤停 + 不稳定心律失常的急救决策枢纽**。
> - USMLE Step 2 CK 急救场景高频考点
> - 核心思维：**"先看脉搏，后看节律"** — 脉搏决定治疗，节律决定诊断
> - 与 [[完整笔记/专题笔记/心内/心内_Vaughan_Williams抗心律失常药]] 互补：本笔记讲**急救流程**，Vaughan 讲**药物对照**
> 
> **来源**：错题 Q4725（PEA 房颤）+ 后续 VF / Asystole / 不稳定心律失常 / ROSC 题积累

---

## Part 0. 核心方法论

### 0.1 "V 除颤，P/A 按压" 二分铁律 ⭐⭐⭐

> [!success] 4 字诀
> **"V 除颤（VF + 无脉 VT），P/A 按压（PEA + Asystole）"**
> - V = **V**entricular（VF + 无脉 VT）→ 电击有效
> - P/A = **P**ulseless / **A**systole → 电击无用，按压 + Epi + 找原因

### 0.2 "先脉搏，后节律" ⭐⭐⭐

> [!danger] 关键反陷阱
> 看到 stem 给节律（房颤 / 窦律 / 缓慢律），**先停下来**问：**有脉吗？**
> - **节律决定诊断**（VF / PEA / Asystole）
> - **脉搏决定治疗**（电击 vs CPR + Epi）

### 0.3 PEA 经典比喻

> [!tip] PEA = 电话有铃声但没人接
> - 监护仪显示节律 = 铃声
> - 心肌不收缩 = 没人接
> - **电击没用**（电铃声的电话没意义）
> - 治疗 = 找"为什么没人接"（5H5T）+ 持续敲门（CPR）+ 唤醒剂（Epi）

---

## Part 1. 心脏骤停 4 种节律对照表 ⭐⭐⭐

### 1.1 完整对比

| 节律 | ECG 特征 | 脉搏 | 处理 | 是否除颤？|
|---|---|---|---|---|
| **VF**（Ventricular Fibrillation 室颤）| 完全混乱波形，**无 QRS** | 无 | CPR + **除颤** + Epi | ✓ **是** |
| **Pulseless VT**（无脉室速）| 宽 QRS 规整 / 多形 | 无 | CPR + **除颤** + Epi | ✓ **是** |
| **PEA**（Pulseless Electrical Activity）| **任何有形节律**（窦律 / 房颤 / 缓慢 / etc）| **无** ★ | CPR + Epi + 5H5T | ❌ **否** |
| **Asystole**（停搏）| **直线**（必须确认 2 导联避免误判）| 无 | CPR + Epi + 5H5T | ❌ **否** |

### 1.2 ECG 识别细节

> [!info] Asystole 确认要点
> 真 asystole **必须 2 导联确认** — 单导联直线可能是导联脱落 / 电极接触不良 / fine VF 被误判。

> [!info] PEA 范围
> PEA = "电活动 + 无脉" 的统称，**包括所有非 VF / 非 VT 的节律**：窦律 / 房颤 / 房扑 / 缓慢律 / 不规则律 / agonal rhythm 全算。

---

## Part 2. 完整 ACLS 算法

**UWorld 官方流程图**（本地截屏）：

![[{D20DE2F4-B2B2-475A-8530-4F4B105CE8BD}.png]]

> [!info] 图示读法
> - **左路 VF / 无脉 VT**：CPR → **除颤** → 继续 CPR + IV/IO + Epi q3-5 min → rhythm check → 仍 shockable → 再除颤（第 3 次后加 **Amiodarone**）→ ROSC
> - **右路 PEA / Asystole**：CPR → 不除颤 → IV/IO + Epi q3-5 min + **找 5H5T** → rhythm check → 若变 shockable rhythm → 走左路
> - **两路汇合**：每 2 min check pulse & rhythm + treat reversible causes → 直到 ROSC
> - **★ Amiodarone 注脚**：仅在 **第 3 次除颤后** 给（300 mg → 150 mg）
> 
> 🔗 详见 [[mistakes/uworld-mistakes_2026-05#^Q4725]]

### 2.1 文字版总流程

```
心脏骤停（无意识 + 无脉 + 无呼吸 / agonal）
        │
        ▼
   立即 CPR + 给氧 + 连监护
   30:2（按压 : 通气）
   100-120 次/分，深度 5-6 cm
        │
        ▼
   评估节律（每 2 min）
        │
   ┌────┴────────────────────┐
   ▼                          ▼
可除颤 (VF / pulseless VT)  不可除颤 (PEA / Asystole)
   │                          │
   ▼                          ▼
1. Defibrillation 200J 双相  1. CPR x 2 min
2. CPR x 2 min                2. IV / IO access
3. IV / IO access             3. **Epi 1 mg q3-5 min**
4. **Epi 1 mg q3-5 min**      4. Treat reversible (5H5T)
   │                          │
   ▼                          ▼
重新评估节律                重新评估节律
   │                       （ROSC? 或继续 CPR？）
   ▼
仍 VF? → 再除颤
+ Amiodarone 300 mg（第 3 次除颤后）
+ Lidocaine（替代）
   │
   ▼
ROSC → 复苏后管理（targeted temp / 心导管 / ICU）
```

### 2.2 高质量 CPR 关键参数

| 参数 | 标准 |
|---|---|
| **按压频率** | 100-120 次 / min |
| **按压深度** | 5-6 cm（成人）|
| **按压：通气** | **30 : 2**（未插管）;  插管后持续按压，10 次/min 通气 |
| **rhythm check 频率** | **每 2 min** 一次（不超过 10 秒）|
| **switch compressor** | 每 2 min 换人（避免疲劳） |
| **ETCO2 监测** | > 10 mmHg 提示有效；ROSC 时突增 |

### 2.3 "见骤停先做什么"决策序列

```
1. 确认无反应 → 喊救命 + 启动 code blue
2. 检查 pulse + breathing（≤ 10 秒）
3. 启动 CPR（30:2）
4. 接 AED / 监护仪 → 评估节律
5. 评估节律后按 2.1 流程
```

---

## Part 3. 5H5T 可逆因（PEA / Asystole 必找） ⭐⭐⭐

### 3.1 完整清单

| H（5 个）| T（5 个）|
|---|---|
| **H**ypovolemia 低血容量 | **T**ension pneumothorax 张力气胸 |
| **H**ypoxia 低氧 | **T**amponade (cardiac) 心包填塞 |
| **H**ydrogen ion 酸中毒 | **T**oxins 毒物（CCB / β-B / TCA / 阿片 / 可卡因）|
| **H**ypo / Hyperkalemia 钾异常 | **T**hrombosis (Pulmonary) 肺栓塞 |
| **H**ypothermia 低温 | **T**hrombosis (Coronary) 冠脉栓塞（MI）|

### 3.2 每个可逆因的针对性处理

| 可逆因 | 识别 stem 关键词 | 处理 |
|---|---|---|
| **Hypovolemia** | 出血史 / 烧伤 / 严重脱水 / 低 CVP | **IV 补液**（晶体 + 血制品如失血）|
| **Hypoxia** | COPD / 哮喘急性 / 窒息 / 溺水 | 高流量氧 + 气道管理 |
| **H+ 酸中毒** | DKA / 肾衰 / 严重休克 / pH < 7.1 | **NaHCO3** + 治原因 |
| **高 K** | 透析患者 / CKD / 横纹肌溶解 / TLS | **Ca + insulin + glucose + Kayexalate + 透析** |
| **低 K** | 利尿剂 / 呕吐腹泻 | 补 K + Mg |
| **Hypothermia** | 暴露史 / 溺水 / 老人 | **复温**（"不死直到温暖死"）|
| **Tension pneumo** | 创伤 / 机械通气 / 气管偏 / 一侧呼吸音消失 + 鼓音 | **针刺减压**（详 3.2.1）→ 立即胸管 |
| **Tamponade** | 尿毒症 / 创伤 / 抗凝 / 主动脉夹层 / Beck 三联 | **心包穿刺** subxiphoid（详 3.2.2）|
| **Toxins** | 中毒史 / 用药史 | 解毒剂逐药对照（详 3.2.3）|
| **PE** | DVT / 长期卧床 / 高凝 | **tPA 溶栓** |
| **MI** | 胸痛先发 / CAD 史 | **心导管 / PCI** |

### 3.2.1 张力性气胸针刺减压（Needle Thoracostomy）⭐

> [!danger] 临床诊断，不等 CXR
> 张力性气胸 = **临床诊断**：一侧呼吸音消失 + 同侧叩诊鼓音 + 气管向对侧偏 + JVD + 低血压。**立即针刺减压，不等影像**。

#### 穿刺点选择（新旧对照，USMLE 都考）

| 路径 | 位点 | 适用 |
|---|---|---|
| **经典路径**（ATLS 旧版 + 多数教科书）| **2nd ICS, midclavicular line**（第 2 肋间，锁骨中线）| 儿童 + 体型瘦小成人 |
| **更新路径**（ATLS 第 10 版 / 2018 起推荐）| **4th-5th ICS, anterior axillary line**（第 4-5 肋间，腋前线，乳头水平）| **成人首选**（胸壁更薄、命中率↑、避开内乳动脉）|

> [!info] 为什么改路径？
> 多项 CT 研究显示成人前胸壁在 2nd ICS 厚度常 > 5 cm（特别是肥胖 / 肌肉发达者），标准 5 cm 针可能**够不到胸膜腔**。腋前线第 4-5 肋间胸壁薄、解剖标志清晰，命中率从 ~50% 升到 ~95%。

#### 操作要点

```
1. 器材：14-16 gauge 留置针，长度 ≥ 5 cm（成人）
2. 标志：
   - 经典：锁骨中点正下方，第 2 肋间隙
   - 更新：胸大肌外侧缘 + 乳头水平 + 第 4-5 肋间
3. 进针：沿肋骨上缘垂直胸壁刺入
   （避开下缘的肋间神经血管束 V-A-N，由上到下排列）
4. 听到"嘶嘶"气流 + 患者血流动力学迅速改善 = 成功
5. 留置外鞘 + 拔出针芯 → 临时减压
6. 立即放胸管（28-32 Fr）于第 4-5 ICS, midaxillary line
   ★ 针刺减压是临时桥接，不是终点
```

#### 高频陷阱

| 陷阱 | 正确做法 |
|---|---|
| ❌ 等 CXR 再穿刺 | ✓ 临床诊断立即穿，CXR 用于穿后确认 |
| ❌ 穿在下缘 | ✓ 沿肋骨**上缘**进针 |
| ❌ 5 cm 针穿肥胖成人 2nd ICS | ✓ 改腋前线 4-5 ICS 或用更长针 |
| ❌ 针刺后不放胸管 | ✓ 必须随后放胸管确证持续引流 |
| ❌ 双侧同时减压（无确凿双侧征）| ✓ 单侧确诊先做单侧 |

### 3.2.2 心包穿刺（Pericardiocentesis）⭐

> [!danger] 急救指征
> Beck 三联（hypotension + JVD + muffled heart sounds）+ 床旁 echo 显示**心包积液 + RV diastolic collapse** = 立即心包穿刺。不等 CT。

#### 三种入路对照

| 路径 | 位点 | 进针方向 | 优缺点 |
|---|---|---|---|
| **Subxiphoid**（剑突下）⭐ 急救首选 | 剑突左下方 1-2 cm | 向**左肩**方向，与皮肤 30-45° | ✓ 远离冠脉 / 内乳动脉；✓ 不需特殊体位；✗ 路径较长 |
| **Apical**（心尖） | 心尖搏动外侧（第 5-6 肋间，腋前线内）| 向**右肩**方向 | ✓ 路径短；✗ 易伤肺 / LAD |
| **Parasternal**（胸骨旁）| 第 5 肋间，胸骨左缘旁开 1-2 cm | 垂直 | ✗ **易伤内乳动脉**，少用 |

#### 操作要点（subxiphoid 标准流程）

```
1. 器材：18 G spinal needle 或 pericardiocentesis kit，
        长 7-10 cm，连接 20 mL 注射器 + 三通
2. 体位：仰卧 30-45° 抬头位（积液重力下沉到心包下部 → 易抽）
3. 进针点：剑突左下方约 1-2 cm
4. 方向：朝**左肩尖**方向，与皮肤成 30-45°
   （而不是垂直 — 垂直会刺向腹腔）
5. 监测：
   - 持续 ECG → 触到心外膜会出现 ST↑ / PVC → 立即回撤
   - 床旁 echo 引导 ⭐ 首选（可识别最安全窗口 + 实时看针尖）
6. 抽吸：边进针边轻负压抽吸
7. 抽出液体：
   - 心包腔血液 ★ "不凝固"（纤维素被剥离）
   - 心室血液 → "立即凝固" → 撤针重定位
8. 完成：留置 pigtail catheter 连接负压引流 24-72 h
```

#### USMLE 高频陷阱

| 陷阱 | 正确做法 |
|---|---|
| ❌ 不稳定 tamponade 先做 CT | ✓ 床旁 echo + 立即穿刺 |
| ❌ 抽出血就放弃（以为穿到心室）| ✓ 看是否凝固，不凝 = 心包腔出血 |
| ❌ 慢性大量积液 + 稳定 + 立即穿刺 | ✓ 慢性积液 → 心包窗手术（pericardial window），更持久 |
| ❌ 单纯 IV 补液处理 tamponade | ✓ 补液仅作桥接（提高 right-sided preload），定性治疗仍是引流 |
| ❌ 抗凝相关大量积液 → 继续抗凝 | ✓ 立即停 + 凝血纠正 + 引流 |

### 3.2.3 解毒剂详解（Toxins 5T 核心）⭐⭐⭐

> [!info] 框架
> 表型识别 → 一线解毒剂 → 二线 / 联合。**ACLS 场景下最高频 5 类**：Opioid / BZD / β-B / CCB / TCA。其他（CO / cyanide / dig / 醇类 / methemoglobin / APAP / ASA）作扩展记忆。

#### A. Opioid（阿片类）— 心搏 / 呼吸骤停常因

| 项目 | 详情 |
|---|---|
| **常见药** | Heroin / Morphine / Fentanyl / Oxycodone / Methadone |
| **表现** | **针尖瞳孔 (miosis)** + 呼吸抑制（< 12/min）+ 意识抑制 + 心动过缓 + 低血压 |
| **解毒剂** | **Naloxone**（μ 受体竞争性拮抗）|
| **剂量** | **0.04-0.4 mg IV/IM/IN q2-3 min** titrate；持续输注 = 2/3 of effective bolus dose/h |
| **起效** | IV 1-2 min；IM/IN 2-5 min |
| **半衰期** | **30-90 min**（短于多数阿片，特别是 methadone / fentanyl）→ 监护下需重复或输注 |
| **戒断风险** | 突然全量逆转 → 剧烈戒断（HTN / 心动过速 / N/V / 焦虑 / 肺水肿）→ 起始低剂量 |
| **USMLE 陷阱** | "Fentanyl OD 后 naloxone 一次见效又再昏迷" → 长效阿片 + 短效拮抗 → 持续输注 |

#### B. Benzodiazepine（苯二氮䓬）

| 项目 | 详情 |
|---|---|
| **常见药** | Midazolam / Lorazepam / Diazepam / Alprazolam |
| **表现** | 意识抑制 + 共济失调 + 呼吸抑制（**单纯 BZD 罕单独致死**）|
| **解毒剂** | **Flumazenil 0.2 mg IV q1min，max 1 mg** |
| **关键警示** | **ACLS 中极少用 Flumazenil** ⭐ |
| **禁忌** | ① 长期 BZD 使用者（撤药致**难治性癫痫**）② TCA 共服（BZD 在保护其癫痫，撤掉则惊厥）③ 未知共服药物 ④ 癫痫病史 |
| **USMLE 陷阱** | 不明中毒 + 昏迷 → **首选 Naloxone + 支持通气**，**不**给 Flumazenil |

#### C. β-blocker（β 受体阻滞剂）中毒

| 项目 | 详情 |
|---|---|
| **常见药** | Propranolol（最毒，过血脑屏障 + Na 阻）/ Metoprolol / Atenolol |
| **表现** | 心动过缓 + 低血压 + AV block + **低血糖**（β 阻 → 糖原分解↓）+ 支气管痉挛 + 意识抑制 |
| **一线解毒** | **Glucagon 3-10 mg IV bolus → 1-5 mg/h 输注** |
| **机制** | 旁路 β 受体 → 直接激活心肌 Gs → ↑ cAMP → ↑ HR + 收缩力 |
| **副作用** | 严重 N/V（常）→ 必备防误吸 |
| **二线** | High-dose insulin / glucose（同 CCB 中毒）/ IV 钙 / Atropine / 经皮起搏 / Lipid emulsion（脂溶性如 propranolol）|

#### D. Calcium Channel Blocker（CCB，非 DHP）中毒 ⭐ 最致命

| 项目 | 详情 |
|---|---|
| **常见药** | **Verapamil**（最致命）/ Diltiazem（非 DHP）；DHP 类（amlodipine 高剂量）也可 |
| **表现** | 心动过缓 + 低血压 + AV block + 意识抑制 + **高血糖**（β 细胞 Ca 通道阻 → 胰岛素分泌↓）⭐ 与 β-B 鉴别点 |
| **解毒阶梯** | 见下表 |

```
CCB 中毒 5 步阶梯：
Step 1: IV calcium
   - Calcium gluconate 3-6 g IV 或 Calcium chloride 1-3 g IV
   - 机制：提高细胞外 Ca → 推动残余通道开放
   - 中重度需重复给

Step 2: High-dose Insulin-Euglycemia (HIE) ★ 一线（中-重度）
   - Regular insulin 1 U/kg IV bolus → 0.5-1 U/kg/h 输注
   - 同时 D50 维持血糖正常
   - 机制：CCB 中毒时心肌从游离脂肪酸代谢转向依赖葡萄糖 →
     大量胰岛素 = 心肌"代谢支持"，改善 inotropy

Step 3: Vasopressors
   - Norepinephrine 首选（α 收缩 + 弱 β1）
   - 严重时 Epi

Step 4: Glucagon（同 β-B）— 效果弱于 β-B 中毒

Step 5: Lipid emulsion 20%
   - 1.5 mL/kg IV bolus → 0.25 mL/kg/min × 10 min
   - "脂质池"捕获脂溶性药物（verapamil 脂溶性高）

Step 6 (refractory): VA-ECMO
```

> [!warning] β-B vs CCB 鉴别（高频陷阱）
> 表现高度重叠，关键鉴别 = **血糖**：
> - β-B 中毒 → **低**血糖（糖原分解↓）
> - CCB 中毒 → **高**血糖（胰岛素分泌↓）

#### E. TCA（三环类抗抑郁药）中毒 ⭐⭐⭐ 高频

| 项目 | 详情 |
|---|---|
| **常见药** | Amitriptyline / Nortriptyline / Imipramine / Doxepin / Clomipramine / Desipramine |
| **表现 — "3 C's"** | **C**ardiotoxicity（QRS > 100 ms + QT 长 → VT / VF / 心搏停）+ **C**onvulsions（癫痫）+ **C**oma（昏迷）+ 抗胆碱（口干 / 视力模糊 / 尿潴留 / 肠麻 / 高热 / 谵妄）+ α1 阻（直立低血压）|
| **诊断 ECG** | **Terminal R wave in aVR > 3 mm** 或 **R/S ratio in aVR > 0.7** ⭐ 经典指纹 |
| **一线解毒** | **NaHCO₃ 1-2 mEq/kg IV bolus → 持续输注** |
| **目标** | 血 pH **7.45-7.55** + QRS **< 100 ms** |
| **机制（双效）** | ① **碱化** → ↑ TCA 与白蛋白结合 → ↓ 游离活性药；② **Na 负荷** → 克服 TCA 对心肌 Na 通道阻滞 |
| **指征** | QRS > 100 ms / 室性心律失常 / 低血压 / 癫痫 / 任何意识改变 + 已知 TCA 摄入 |
| **禁忌药** | ❌ Class IA / IC（同样阻 Na，加重传导阻滞）❌ Flumazenil（即使共服 BZD，会去除癫痫保护）❌ Physostigmine（虽然抗胆碱症状 — 但 TCA 中毒不用，加重心毒）|
| **癫痫处理** | **Benzodiazepines**（首选）→ phenobarbital；**避免 phenytoin**（Na 通道阻，加重 TCA 心毒）|

#### F. 其他必背解毒剂（扩展）#薄弱点

| 中毒 | 表型指纹 | 解毒剂 |
|---|---|---|
| **CO 中毒** | 头痛 + 群发 + 樱桃红肤 + SaO₂ 假正常（pulse ox）+ 真低 SaO₂（co-oximetry）| **100% O₂ via NRB**；HBO（妊娠 / COHb > 25% / 神经症状 / 意识丧失）|
| **Cyanide** | 烟雾吸入 / 硝普钠长用 + "almond breath" + 静脉血氧↑（细胞用不了 O₂）+ 严重乳酸酸中毒 | **Hydroxocobalamin 5 g IV**（首选，尿变红）或 Na thiosulfate + nitrites |
| **Methemoglobinemia** | 苯佐卡因 / dapsone / 亚硝酸盐 + **chocolate-brown blood** + 紫绀不响应 O₂ + SaO₂ ~85% | **Methylene blue 1-2 mg/kg IV**（G6PD 缺陷禁用） |
| **Digoxin** | 黄绿视 + N/V + 任何心律（双向 VT 经典）+ 高 K | **Digoxin-specific Fab (Digibind)** |
| **Acetaminophen** | 24h 无症状 → 24-72h 肝损 → 暴肝衰 | **N-acetylcysteine (NAC)** PO 140 mg/kg load → 70 mg/kg q4h × 17，或 IV 21h 方案 |
| **Salicylate** | 早期呼吸碱 + 后期 AG 代酸 + 高热 + 耳鸣 | **NaHCO₃ 尿液碱化**（目标尿 pH 7.5-8）+ 透析（重）|
| **Methanol / Ethylene glycol** | AG 代酸 + 渗透 gap↑（甲醇 → 视神经；乙二醇 → 草酸钙肾结石）| **Fomepizole**（首选）或乙醇 + 透析 |
| **Iron** | 5 期（GI → quiescent → 休克 → 肝衰 → 肠瘢痕）+ 影像见铁丸 | **Deferoxamine** IV |
| **有机磷 / 神经毒**| SLUDGE-M + 烟碱 + CNS | **Atropine**（抗 M，先大剂量）+ **Pralidoxime (2-PAM)**（再生 AChE）|
| **β-agonist / 茶碱**| 心动过速 + 低 K + 震颤 | 支持 + 严重时 β-blocker（仅特定情况）|

> [!success] 一句话锁定 5T 解毒剂顺序
> **"阿片 Naloxone，BZD 别用 Flumazenil（ACLS 中），β-B Glucagon，CCB 钙 + 高胰岛素，TCA NaHCO₃ 看 QRS"**

### 3.3 高频考点：哪些可逆因有特异治疗

> [!success] 4 个"想到立刻做"特异处理
> - **张力气胸** → 针刺减压（不等 CXR）
> - **心包填塞** → 床旁 echo → 心包穿刺
> - **PE 不稳** → 床旁 TTE → tPA
> - **高 K** → Ca + insulin + glucose

---

## Part 4. ACLS 用药速查 ⭐⭐⭐

### 4.1 主要用药

| 药 | 剂量 | 用途 | 时机 |
|---|---|---|---|
| **Epinephrine** | **1 mg IV / IO q3-5 min** | **所有 4 种骤停节律** ⭐ | 越早越好（不可除颤节律立即给；可除颤节律首次除颤后给）|
| **Amiodarone** | 300 mg IV bolus → 150 mg | VF / 无脉 VT | **第 3 次除颤后** |
| **Lidocaine** | 1-1.5 mg/kg | VF / 无脉 VT 替代 | Amio 替代（资源 / 过敏）|
| **Magnesium** | 1-2 g | **Torsades de Pointes** | 任何时间，不论血 Mg |
| **Atropine** | 1 mg q3-5 min（max 3 mg）| **症状性窦缓 / AV 阻滞**（**有脉**）| ❌ **不用于 asystole**（2010 AHA 移除） |
| **NaHCO3** | 1 mEq/kg | 严重酸中毒 / 高 K / TCA 中毒 | 选择性，不常规 |
| **Calcium** | 1 g IV | 高 K / CCB 中毒 / 低 Ca | 选择性 |

### 4.2 复苏后管理用药（ROSC 后）

| 药 | 用途 |
|---|---|
| **Norepinephrine / Epi 输注** | 维持 MAP ≥ 65 mmHg |
| **Amiodarone 维持** | 预防 VF 复发 |
| **Targeted Temperature Management** | 32-36°C × 24h（昏迷患者，防神经损伤）|

### 4.3 反陷阱：什么药 USMLE 不要选

> [!danger] ACLS 常见错误选项
> - ❌ **Atropine for asystole**（2010 移除）
> - ❌ **Lidocaine for PEA**（Lidocaine 只用于 VF / 无脉 VT）
> - ❌ **NaHCO3 常规**（除非证据明确：高 K / 严重酸 / TCA）
> - ❌ **Amio 第一次除颤就给**（必须第 3 次除颤后）
> - ❌ **Procainamide 急性 VF**（IA 类，复苏中不用）

---

## Part 5. 三种"电击方式"对比 ⭐⭐⭐

> [!warning] USMLE 最易混
> Defibrillation / Synchronized Cardioversion / Pacing 完全不同，混了 = 致命。

| 维度 | **Defibrillation**（除颤）| **Synchronized Cardioversion**（同步复律）| **Pacing**（起搏）|
|---|---|---|---|
| 同步 R 波？| **否** | **是** | — |
| 能量 | 高（200J 双相 / 360J 单相）| 低（50-200J 递增）| 低脉冲 |
| **脉搏要求** | 必须**无脉** | 必须**有脉** | 有脉（缓慢）|
| **意识** | 无 | 通常需镇静 | 清醒 |
| **适应症** | **VF / 无脉 VT** | **有脉**的不稳定 SVT / 房颤 / 房扑 / 单形 VT | 症状性窦缓 / 高度 AV 阻滞 |
| 危险性 | 必须，不电就死 | 不同步 + 有脉 → 误击在 T 波 → **VF** | 一般安全 |

### 5.1 "同步"的意义

> [!info] 为什么同步那么重要？
> 心动周期里有个**易损期**（T 波）— 电击落在这里会诱发 VF。
> - **VF / 无脉 VT 已经没节律可同步** → 直接除颤
> - **有脉患者**有节律 → 必须同步到 R 波避开 T 波 → 用 Synchronized Cardioversion

### 5.2 起搏（Pacing）适应症

| 类型 | 适应症 |
|---|---|
| **Transcutaneous Pacing (TCP)** | 急救：症状性窦缓 / Mobitz II / 完全 AVB / Atropine 失败 |
| **Transvenous Pacing (TVP)** | 短期过渡：TCP 后维持，等永久起搏器 |
| **Permanent Pacemaker (PPM)** | 永久：症状性窦缓 / 完全 AVB / 双束支 + 晕厥 |

---

## Part 6. 心律失常急救三分类决策树

```
Step 1: 患者有脉吗？
   │
   ┌────┴────┐
   无脉      有脉
   │         │
   ▼         ▼
Step 2a:   Step 2b: 血流动力学稳定？
评估节律     │
   │      ┌──┴──┐
   ▼     稳定   不稳定
┌──┴──┐   │       │
VF/VT  PEA/  ▼       ▼
除颤   Asys 抗心律失常  Synchronized
       CPR  药         Cardioversion
            (按节律类型)  （任何不稳的房颤 / SVT /
                          单形 VT 都用同步）
```

### 6.1 "稳定 / 不稳定"判定（高频）

> [!warning] 任 1 条即"不稳定"
> - **SBP < 90** 或灌注差
> - **意识改变**
> - **持续胸痛 / 缺血表现**
> - **急性心衰**
> - 任 1 条满足 → **不稳定** → 立即同步复律（不再药物）

### 6.2 稳定患者的抗心律失常药选择

| 节律 | 一线 |
|---|---|
| SVT（窄 QRS 规整）| Vagal → **Adenosine IV push** |
| 房颤 / 房扑 控率 | β-blocker / Diltiazem |
| 房颤 / 房扑 律转 | **Amiodarone** / 电复律（择期） |
| 单形 VT 稳定 | **Amiodarone** / Lidocaine |
| 多形 VT（TdP）| **Magnesium** |
| WPW + AFib | **Procainamide / Ibutilide**（**禁** AV 结阻滞剂）|

---

## Part 7. "看到房颤" 答题决策树 ⭐⭐⭐

```
看到 stem 提到房颤 → 必须先问：

1. 有脉吗？
   - 无脉 → PEA → CPR + Epi（不电击！）★ Q4725 陷阱
   - 有脉 → 继续

2. 血流动力学稳定吗？
   - 不稳定（低 BP / 意识 / 胸痛 / 心衰）→ Synchronized Cardioversion
   - 稳定 → 继续

3. WPW 患者？
   - 是 → Procainamide / Ibutilide / 电复律
       **禁用 AV 结阻滞剂**（β / CCB / Adenosine / Digoxin → VF）
   - 否 → 率控（β / Diltiazem）或律转（amiodarone / 择期 cardio）

4. 长期管理：
   - CHA2DS2-VASc 评分 → 抗凝（Apixaban / Warfarin 机械瓣）
```

---

## Part 7.5. STEMI 初始稳定化 ⭐⭐⭐（与 ACLS 协同）

> [!info] 与 ACLS 的关系
> ACLS 处理**已经骤停**的患者（4 节律）。STEMI 是**急性 MI 未骤停但随时可能骤停**的场景 —— 处理目标是 **稳定 + 限制梗死 + 再灌注**，防止演变为 VF / 心源性休克 / 完全 AV block → ACLS。
> - STEMI 是 ACLS 的"前置场景" + 5T 的 **T**hrombosis (Coronary) 病因
> - ROSC 后高度怀疑 STEMI → 立即 cath lab（详见 Part 8.2）

### 7.5.1 UWorld 流程图

![[{B655FC07-FC74-4035-A262-B32E35C10996}.png]]

### 7.5.2 初始稳定化 7 项核心用药 ⭐

> [!success] 所有 STEMI 入院 6 项必给（除非禁忌）
> 
> | 药 | 剂量 | 机制 | 禁忌 / 注意 |
> |---|---|---|---|
> | **Supplemental O₂** | 维持 SaO₂ ≥ 90% | 改善缺血心肌氧合 | **SaO₂ ≥ 90% 不必给**（高氧 → 冠脉收缩 + 自由基损伤）|
> | **Aspirin** | **325 mg 嚼服** | 不可逆 COX-1 抑制 → ↓TXA2 → ↓血小板聚集 | 活动性出血 / 过敏 |
> | **P2Y12 inhibitor** | Clopidogrel 600 mg / Ticagrelor 180 mg / Prasugrel 60 mg | ADP 受体阻断 → DAPT 双抗 | Prasugrel 禁用于卒中史 |
> | **Nitrates** | 舌下 NTG q5min × 3，必要时 IV | ↓preload + 冠脉扩张 → 缓解胸痛 | **禁忌**：SBP < 90 / RV 梗死 / 24h 内 PDE-5 抑制剂 (sildenafil) |
> | **β-blocker** | 口服 metoprolol 25-50 mg q6-12h | ↓HR + ↓收缩力 → ↓心肌耗氧 + 防 VF | **禁忌 4 条**：低血压 / 心动过缓 / **急性心衰** / heart block ⭐ |
> | **High-dose statin** | **Atorvastatin 80 mg** | 斑块稳定 + 抗炎 + ↑NO | 无急性禁忌（即使 LDL 已达标也给）|
> | **Anticoagulation** | UFH / Enoxaparin / Bivalirudin / Fondaparinux | 防血栓蔓延 / catheter thrombosis | 选药取决于 reperfusion 策略（PCI 偏 UFH / bivalirudin；fibrinolysis 偏 enoxaparin）|

### 7.5.3 症状触发 → 二线药决策树 ⭐

> [!warning] 4 个症状 → 4 个对应二线药（独立通路，不冲突）
> 
> | 症状 | 二线药 | 禁忌 / 注意 |
> |---|---|---|
> | **持续胸痛 + HTN / HF** | **IV nitroglycerin** | 禁忌：低血压 / **RV 梗死** / 重度 AS（前后负荷依赖）|
> | **持续严重疼痛** | **IV morphine** | 慎用：低血压 / 呼吸抑制；新证据示 morphine 可能 ↓ P2Y12 吸收（不再常规一线） |
> | **不稳定窦缓** | **IV atropine** 0.5-1 mg | **仅** sinus brady + 症状有效；对 Mobitz II / 3° AVB 无效（infranodal）|
> | **肺水肿** | **IV furosemide** | 禁忌：**低血压 / 低血容量**（会加重休克）；先确认容量过载 |

### 7.5.4 Reperfusion 决策（核心）

```
所有 STEMI 患者：
    │
    ▼
评估 PCI 可及性
    │
   ┌┴─────────────────────────────────┐
   ▼                                   ▼
PCI 90 min 内可达                   PCI > 120 min 不可达
   │                                   │
   ▼                                   ▼
Primary PCI ⭐                     Fibrinolysis (tPA / TNK)
（door-to-balloon ≤ 90 min）       （door-to-needle ≤ 30 min）
   │                                   │
   │                                   ▼
   │                              ★ 必须 3-24h 内转 PCI 中心
   │                                   │
   └────────────┬──────────────────────┘
                ▼
         Post-PCI 管理：
         - DAPT × 12 月
         - β-B + ACEi + statin + 醛固酮拮抗剂（如 EF<40）
         - 心脏康复
```

> [!danger] Fibrinolysis 绝对禁忌（必记 ⭐）
> - 既往任何颅内出血 / 缺血性卒中（3 月内）
> - 已知颅内血管畸形 / 恶性肿瘤
> - 活动性出血（不含月经）
> - 主动脉夹层疑似
> - 3 月内严重头部 / 面部外伤
> - 2 月内颅内 / 脊髓手术

### 7.5.5 高频陷阱

| 陷阱 | 正确认知 |
|---|---|
| ❌ 所有 STEMI 都给 β-blocker | ✓ 4 禁忌：低血压 / 心动过缓 / 急性心衰 / heart block |
| ❌ STEMI + RV 梗死 给 NTG | ✓ RV 梗死前负荷依赖，NTG → 灾难性低血压 → 给液体 + dobutamine |
| ❌ SaO₂ 95% 也常规吸氧 | ✓ SaO₂ ≥ 90% 不必给（高氧反致害） |
| ❌ PCI 不可及就先观察 | ✓ 必须 fibrinolysis（除非禁忌），再转 PCI 中心 |
| ❌ Fibrinolysis 后稳定就不转 PCI | ✓ 3-24h 内必须转（rescue / routine PCI） |
| ❌ 急性心衰患者给 β-blocker 控率 | ✓ 急性失代偿期暂停 β-B（等稳定后再起） |
| ❌ STEMI + sinus brady 直接 PPM | ✓ Atropine 一线（inferior MI 后窦缓多迷走介导，可逆） |

### 7.5.6 与 5H5T 的联动

STEMI 在 ACLS 框架中 = **5T 之 Thrombosis (Coronary)**：
- STEMI → VF / 无脉 VT → ACLS 左路 → ROSC → cath lab
- STEMI → 完全 AV block（inferior MI / RCA 闭塞）→ 不稳定 → Atropine → TCP → cath lab
- STEMI → 心源性休克 → IABP / Impella + 紧急 PCI
- STEMI → 机械并发症（free wall rupture / VSD / papillary muscle rupture，3-5 天）→ 急诊外科

> [!tip] STEMI 5 字记忆
> **"O-A-P-N-B-S-A"** = O₂ / Aspirin / P2Y12 / Nitrates / β-Blocker / Statin / Anticoag（6 + 1）
> 二线 4 触发：**"痛 HTN → 硝；剧痛 → 吗；缓 → 阿；水 → 速"**

---

## Part 8. ROSC 后管理（Post-Cardiac Arrest Care）

### 8.1 立即处理 4 步

```
1. 优化氧合 + 通气
   - SpO2 目标 92-98%（避免高氧 → 神经损伤）
   - ETCO2 目标 35-45 mmHg

2. 血流动力学支持
   - MAP ≥ 65 mmHg
   - IV fluid + Norepinephrine / Epi 输注

3. 找诱因 + 治原因
   - 12 导联 ECG（找 STEMI → 心导管）
   - 5H5T 评估
   - 实验室全套 + ABG

4. 神经保护
   - Targeted Temperature Management (TTM)
     32-36°C × 24h（昏迷患者）
   - 控癫痫（EEG 监测）
   - 神经预后评估 ≥ 72h 后
```

### 8.2 复苏后心导管指征

> [!success] 复苏后立即做心导管的指征
> - **STEMI 表现** → 立即去 cath lab（< 90 min）
> - **不稳定 + 怀疑 ACS** → 紧急
> - **VF / 无脉 VT 骤停** + 高度怀疑 ACS → 即使无明显 STEMI，也考虑早期心导管

---

## Part 9. PALS 速查（儿童 ACLS 简短对比）

| 项 | 成人 ACLS | 儿童 PALS |
|---|---|---|
| **CPR 按压：通气** | 30 : 2（单人）| 30 : 2（单人）/ **15 : 2**（双人 + 儿童）|
| **按压深度** | 5-6 cm | **胸廓深度 1/3** |
| **按压频率** | 100-120 / min | 同 |
| **Epi 剂量** | 1 mg | **0.01 mg/kg** |
| **除颤能量** | 200J | **2 J/kg**（首次）→ 4 J/kg |
| **可逆因** | 5H5T | 同 |

---

## Part 10. Memory Hook 集合

### 10.1 核心口诀

> [!success] 5 个核心口诀
> 1. **"V 除颤（VF + 无脉 VT），P/A 按压（PEA + Asystole）"**
> 2. **"先看脉搏，后看节律"** — 脉搏决定治疗，节律决定诊断
> 3. **"PEA = 电话有铃声但没人接"** — 节律 ≠ 循环
> 4. **"V 字开头要除颤；P/A 开头要按压"**
> 5. **"flatline shock 是电视剧；真临床绝不电 asystole"**

### 10.2 时间窗 3 个数字

> [!tip] ACLS 三个时间数字
> - **30 : 2** = CPR 按压 : 通气比
> - **2 min** = 每周期 + rhythm check
> - **3-5 min** = Epi 间隔

### 10.3 5H5T 速记

> H = "**5 个 Hypo-**"（Hypovolemia / Hypoxia / Hypothermia / Hypo-Hyperkalemia）+ **H 离子**（酸）
> T = "**5 个 T**"（Tension pneumo / Tamponade / Toxins / Thrombosis × 2: **P**E + **M**I）

### 10.4 用药记忆

> [!tip] Epi vs Amio 记忆
> - **Epinephrine** = "**E**arly + **E**veryone" — 越早越好 + 4 种节律都用
> - **Amiodarone** = "**A**fter 3rd shock" — 第 3 次除颤后才给

### 10.5 三种"电"方式速记

> **"无脉无 R = Defib，有脉同 R = Sync，缓慢起搏 = Pacing"**

---

## Part 11. 跨学科陷阱

| 学科 | 陷阱 | 关键点 |
|---|---|---|
| **外科** | 创伤性心包填塞 → PEA | 5T 之 Tamponade，**穿刺急救** |
| **外科** | 张力气胸 → PEA | 5T 之 Tension pneumo，**针刺减压不等 CXR** |
| **肺** | 大块 PE → 不稳定 → PEA | 5T 之 PE，**tPA 溶栓** |
| **感染** | 脓毒症 → 持续低血容量 → PEA | 5H 之 Hypovolemia，**大量补液 + 升压药** |
| **内分泌** | DKA / Adrenal crisis → PEA | 5H 之 Hypovolemia + H+ 酸中毒 |
| **肾 / Heme** | 高 K（CKD / TLS / 溶血）→ VF | 5H 之 Hyperkalemia，**Ca + insulin** |
| **中毒** | TCA → VT/VF；β-B/CCB → bradycardia → PEA | 5T 之 Toxins，**特异解毒**（NaHCO3 / Glucagon / Insulin）|
| **低温**（户外 / 老人）| Hypothermia → VF | 5H 之 Hypothermia，**复温**（"不死直到温暖死"）|
| **儿科** | 溺水 → Hypoxia → 骤停 | PALS 流程 + 5H 之 Hypoxia |
| **神经** | 重型卒中 → herniation → 骤停 | 不可逆，但仍按 ACLS 跑 |

---

## Part 12. 高频陷阱总结

| 陷阱 | 正确认知 |
|---|---|
| ❌ 看到房颤 = 复律 | ✓ 必须先看脉搏；**无脉房颤 = PEA = 不电击** |
| ❌ PEA 可以除颤 | ✓ 错！PEA = 电活动正常但心肌不收缩，电击对"机械停跳"无效 |
| ❌ Asystole 给 atropine | ✓ 错！2010 AHA 已移除；asystole = CPR + Epi |
| ❌ "有节律 = 有循环" | ✓ 错！PEA 关键就是节律和循环脱钩 |
| ❌ 见骤停先评估 ABG / 实验室 | ✓ 错！先 CPR；评估同步做 |
| ❌ 第一次除颤就给 amiodarone | ✓ 错！第 3 次除颤后才给 |
| ❌ Defibrillation 和 Cardioversion 一样 | ✓ 错！同步与否 + 脉搏要求完全不同 |
| ❌ Lidocaine 是 PEA 一线药 | ✓ 错！Lidocaine 仅用于 VF / 无脉 VT |
| ❌ "flatline shock" | ✓ 电视剧才有；真临床绝不电击 asystole |
| ❌ PEA 不需要找原因 | ✓ 错！**5H5T 必找**；不像 VF 单纯电击就行 |
| ❌ ROSC 后高流量氧最好 | ✓ 错！避免高氧（神经损伤）→ SpO2 92-98% |
| ❌ ROSC 后立即唤醒患者 | ✓ 错！昏迷患者需 TTM 32-36°C × 24h |

---

## 🔗 关联

- 🔁 **同主题错题**：
  - [[mistakes/uworld-mistakes_2026-05#^Q4725]] PEA 房颤陷阱（首张 ACLS 卡）
  - 等后续 VF / Asystole / 同步复律 / 5H5T 各因 / ROSC 后管理题积累
- 📚 **主笔记**：
  - [[完整笔记/Peixuan分科笔记/心内]]（ACLS + 心律失常急救）
  - [[完整笔记/专题笔记/心内/心内_Vaughan_Williams抗心律失常药]] ⭐（**姊妹笔记** — Vaughan 讲药物对照，本笔记讲急救流程；两者互补）
- 🏥 **跨学科**：
  - [[完整笔记/Peixuan分科笔记/外科]]（创伤性心包填塞 / 张力气胸 → PEA → 特异处理）
  - [[完整笔记/Peixuan分科笔记/pulmonary]]（大块 PE → 不稳 → PEA → tPA）
  - [[完整笔记/Peixuan分科笔记/感染]]（脓毒症休克 → 持续低血容量 → PEA）
  - [[完整笔记/Peixuan分科笔记/endocrine]]（Adrenal crisis / DKA → PEA）
  - [[完整笔记/专题笔记/心内/心内_主动脉急症决策树]]（心包填塞共享 + 难治性休克 / PEA 系列）
  - [[完整笔记/专题笔记/内分泌/内分泌_肾上腺皮质功能不全]]（Adrenal crisis → 持续低 BP → PEA 病因）
  - [[完整笔记/专题笔记/USMLE/USMLE_读题策略]]（"看到节律就电"反射 = 模式识别错位）
- 🌱 **TODO（持续扩充）**：
  - 累计 3+ 道 PEA 病因题（5H5T 各场景）→ 拆出 [[完整笔记/专题笔记/_衍生_PEA可逆因鉴别]]
  - 累计 3+ 道 ROSC 后管理题（TTM / 心导管时机 / 神经预后）→ 补 Part 8
  - 累计 3+ 道 PALS 儿童急救题 → 扩 Part 9
  - 累计 3+ 道"同步 vs 不同步电复律"陷阱题 → 补 Part 5

---

## 📋 文件元信息

- **建立**：2026-05-14（由 Q4725 PEA 房颤陷阱触发）
- **状态**：v1.1（2026-05-15 扩展 Part 3.2 — 新增 3.2.1 张力性气胸穿刺点新旧路径 + 3.2.2 心包穿刺三入路 + subxiphoid 标准流程 + 3.2.3 解毒剂详解 5T 核心 + 扩展）
- **应试目标**：USMLE Step 2 CK 急救 + ICU + 围手术期 ACLS 模块
- **复习节奏**：
  - 考前每周扫 Part 0 + Part 10（Memory Hook）+ Part 12（陷阱）
  - 考前 1 月精读 Part 1-7（4 节律 / ACLS 算法 / 5H5T / 用药 / 三种电击 / 急救分类 / 房颤决策）
- **5 天 ACLS 巩固计划**（Peixuan 推荐）：
  - Day 1：4 节律对照（Part 1） + "V 除颤 P/A 按压"
  - Day 2：5H5T + 针对处理（Part 3）
  - Day 3：用药速查（Part 4）+ Epi q3-5 / Amio 第 3 次
  - Day 4：三种"电"方式（Part 5） + 房颤决策（Part 7）
  - Day 5：全套默写 + ROSC 管理（Part 8）

**Last updated**: 2026-05-17 v1.2（新增 Part 7.5 STEMI 初始稳定化：UWorld 流程图 + 7 项核心用药 + 4 触发二线药 + Reperfusion 决策 + fibrinolysis 禁忌 + 与 5H5T 联动；修正首页裸图位置）
