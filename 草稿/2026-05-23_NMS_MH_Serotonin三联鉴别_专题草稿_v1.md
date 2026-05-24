---
tags:
  - USMLE-Step2
  - 精神
  - 神经
created: 2026-05-23
updated: 2026-05-23
type: 专题笔记草稿
---

# 三大"高热 + 精神状态改变"综合征鉴别（NMS / MH / Serotonin Syndrome）+ MAOI HTN crisis 第 4 列

> [!info] 一句话定位
> NMS / MH / Serotonin Syndrome 三者都可表现为 **高热 + 意识改变 + 肌肉异常 + 自主神经紊乱**，临床极易混；本草稿 v1.1 加入第 4 列 **MAOI Tyramine HTN crisis**（adrenergic 通路，体征是血压飙升而非神经肌肉兴奋）。**区分核心 = 触发药/食物 + 起病时间 + 肌张力/反射模式 + 递质通路**。

> [!info] 草稿状态
> 草稿 **v1.1**（2026-05-23 升级）。
> - **源头错题**：[[mistakes/uworld-mistakes#^Q12203]] NMS（haloperidol 触发，问机制选"多巴胺活性↓"）
> - **v1.1 新增触发题**：[[mistakes/uworld-mistakes#^Q4879]] MAOI tyramine HTN crisis（与 SS 鉴别 — adrenergic vs serotonergic 通路完全分开）
> - 等 psych / neuro 章节复习完后由 Claude Code 整合 MH + Serotonin Syndrome + MAOI HTN crisis + 抗胆碱能毒性 类错题 → 升级为正式专题笔记 [[完整笔记/专题笔记/_衍生_高热肌强直急症鉴别]]（凑齐"高热+谵妄+血压"五鉴别）。

---

## MAOI 两条祸（决策分流）⭐ v1.1 新增

[[mistakes/uworld-mistakes#^Q4879]] 触发增量：MAOI 是**两条祸的开关**，必须看"配什么"决定走哪条 — **食物 → HTN crisis（adrenergic）；联用 5-HT 能药 → SS（serotonergic）**。两条祸通路完全分开，体征也完全不同。

```
MAOI 患者出问题
  ├─ 配 tyramine 食物（陈年奶酪 / 腌肉 / 红酒 / 发酵豆制品 / 熟透水果 / 啤酒 / 酱料）
  │     → HYPERTENSIVE CRISIS（adrenergic）
  │       机制：tyramine = 间接拟交感胺 → 挤出储存的 NE/Epi → α1+β1 双激动
  │       体征：血压飙升 / 剧烈头痛 / 心动过速 / 焦虑震颤 / 卒中
  │       解药：phentolamine（α 阻断）/ nitroprusside / labetalol（α+β 双阻必须）
  │
  └─ 配 serotonergic 药（SSRI / SNRI / meperidine / tramadol / 曲坦 / linezolid / DXM / MDMA）
        → SEROTONIN SYNDROME（5-HT↑）
          机制：5-HT 在突触间隙堆积
          体征：hyperreflexia / clonus / myoclonus / 体温↑ / 散瞳 / 躁动
          解药：cyproheptadine + 停药 + 支持
```

> [!warning] 看体征前先问触发
> "是吃了**食物**，还是吃了**药**出的事？" — 食物路 → HTN crisis；药路 → SS。两套递质、两套体征、两套解药，**不要因为"都是 MAOI 引起"就混为一谈**。

### Tyramine 高含量食物清单（USMLE 高频）

| 食物类 | 典型例子 | 备注 |
|---|---|---|
| **陈年发酵奶酪** | Aged cheese（cheddar / blue / Swiss） | 越陈越多；新鲜奶酪 OK |
| **腌制肉类** | Cured meat / 萨拉米 / 烟熏鱼 / 鸡肝 | "腌"= tyramine |
| **发酵酒** | **红酒** / 啤酒 / vermouth / sherry | 蒸馏酒（伏特加 / 威士忌）通常 OK |
| **发酵豆制品** | 酱油 / 味噌 / tempeh / fava beans（蚕豆） | 蚕豆含 dopa → 同样升 NE |
| **熟透/过熟水果** | 香蕉皮（果肉 OK）/ 牛油果 / 无花果 | 储存太久也会↑ |
| **腌渍/酱料** | 泡菜 / 酸菜 / 酱油 / Marmite | |

### 隐藏 MAOI 三剑客（USMLE 高频陷阱）

| 药物 | 真实身份 | 临床场景 | MAOI 风险点 |
|---|---|---|---|
| **Linezolid** | 抗 G+ 抗生素 | 治 VRE / MRSA / 复杂 SSTI | 弱可逆 MAOI → 与 SSRI / tramadol 联用 → **SS**；用前需停 SSRI ≥2 周（fluoxetine ≥5 周） |
| **Selegiline**（高剂量） | 抗 PD MAO-B 抑制剂 | PD 增效 / DA 保留 | **低剂量**选择性 MAO-B → tyramine 风险小；**高剂量失选择性** → 同样需忌口 + 与 SSRI 禁联用 |
| **Methylene blue** | 治 methemoglobinemia | 急救解毒 | 强 MAOI → 5-HT 能药联用禁忌（SS 风险） |

---

## High-Yield Summary Table（核心对比 — 加入 HTN crisis 第 4 列）

| 指标 | **NMS** | **Malignant Hyperthermia (MH)** | **Serotonin Syndrome** | **MAOI Tyramine HTN crisis** ⭐v1.1 |
|---|---|---|---|---|
| **机制** | 中枢**多巴胺↓**（D2 阻断） | 骨骼肌 **RyR1 钙失控** | 中枢/外周 **5-HT↑** | **NE/Epi 爆发**（tyramine 挤出储存儿茶酚胺） |
| **递质通路** | DA | 钙（细胞内） | 5-HT | **Adrenergic（NE/Epi）** |
| **触发** | 抗精神病药（haloperidol / 起始/加量）、止吐药（metoclopramide）、**撤帕金森药** | **吸入麻醉 + 琥珀胆碱** | SSRI/SNRI、MAOI、曲马多、linezolid、MDMA、DXM、曲坦 | **MAOI + tyramine 食物**（陈年奶酪/红酒/腌肉） |
| **起病** | **数天**（1–3 天）缓 | **数分钟–数小时**（麻醉中/后） | **数小时（<24h）** | **数分钟–小时**（餐后急起） |
| **肌张力/反射** | **铅管样强直**（lead-pipe）+ 反射正常/减弱 | 全身僵硬 + **咬肌痉挛** | **clonus + hyperreflexia**（下肢为主） | **无肌强直 / 无反射异常** |
| **特征体征** | 流涎、自主紊乱、AMS | **ETCO₂↑**（早期最敏感）、酸中毒 | **clonus / hyperreflexia / 散瞳** | **血压飙升 + 剧烈头痛**（出血/卒中风险） |
| **CK / 肌溶解** | ↑↑（myoglobinuria） | ↑↑ | 轻度↑ | 一般正常 |
| **解药** | 停药 / 恢复 DA；BZD；难治 **bromocriptine** 或 dantrolene | **dantrolene** + 停麻醉药 + 降温 | 停药 + 支持 + **cyproheptadine** | **phentolamine**（α 阻断）/ nitroprusside / labetalol（α+β）|
| **一句话区分** | "**脑里多巴胺不够**" | "**肌肉钙太多**" | "**5-HT 太多 + 反射亢进/阵挛**" | "**NE 太多 + 血压爆**" |

---

## 三秒决策树（考试最快区分法 — v1.1 四联版）

```
              急性高热 / 精神改变 / 肌肉异常 / 血压异常
                              |
   ┌──────────────────┬───────┴────────┬──────────────────┐
   ▼                  ▼                ▼                  ▼
给了抗精神病药      给了麻醉/         给了 5-HT 能药      给了 MAOI
+ 铅管样强直       琥珀胆碱         (SSRI/MAOI/曲马多…) + 吃了 tyramine
+ 反射正常        + 起病数小时       + 阵挛 clonus       食物（奶酪/红酒/
+ 起病数天       + ETCO₂↑          + 反射亢进/散瞳     腌肉/酱料）
    |                  |                |                  |
    ▼                  ▼                ▼                  ▼
   NMS                MH         Serotonin Syndrome    HTN crisis
 多巴胺↓             钙失控           5-HT↑              NE/Epi↑
bromocriptine     dantrolene      cyproheptadine      phentolamine
```

> [!tip] 四个"急症"最快区分法（v1.1）
> - 给了**抗精神病药** + **铅管样强直 + 反射正常** → **NMS**（数天起病）
> - 给了**麻醉 / 琥珀胆碱** + 起病**数小时** + 呼气末 CO₂↑ → **MH**
> - 给了**5-HT 能药** + **阵挛 / 反射亢进 / 散瞳** → **Serotonin Syndrome**（数小时）
> - 给了 **MAOI + tyramine 食物** + **血压飙升 + 剧烈头痛** → **HTN crisis**（adrenergic，餐后急起）

---

## 关键鉴别维度（深度理解）

> [!warning] 区分的"金钥匙"是反射
> - **NMS**：反射**正常或减弱**，肌肉是"铅管样"被动僵硬（全程等阻力）。
> - **Serotonin Syndrome**：反射**亢进 + 阵挛(clonus)**，**下肢更明显**，常伴**散瞳**——这是与 NMS 最关键的区别。
> - **MH**：靠**触发场景（麻醉中）+ ETCO₂↑** 直接锁定，不靠反射。

> [!danger] 三个"本质机制" + 对应解药
> - **NMS = 多巴胺不够** → 补多巴胺：**bromocriptine**（多巴胺激动剂，踩油门）
> - **MH = 钙太多** → 关钙闸：**dantrolene**（抑制肌浆网 RyR1 钙释放）
> - **Serotonin Syndrome = 5-HT 太多** → 抗 5-HT：**cyproheptadine**（赛庚啶）

---

## 易混点 & 陷阱

> [!warning] 高频陷阱
> - **dantrolene 在 NMS 和 MH 都能用，但角色不同**：MH 是一线治本（直接抗 RyR1）；NMS 只是重症/难治时对症（治本应恢复多巴胺）。
> - **尿潜血陷阱**（NMS / MH 共有）：尿试纸潜血(+) 但镜下 RBC 少/无 = **肌红蛋白尿(myoglobinuria)**，因 heme 蛋白让试纸阳性，但非完整红细胞。
> - **起病时间是 NMS vs MH 的快速分水岭**：NMS 数天缓起，MH 麻醉中/后数小时急起。
> - **Serotonin Syndrome 与 NMS 最易混**：两者都有高热+肌张力高+自主神经紊乱，**靠"反射亢进+阵挛+散瞳"区分 Serotonin Syndrome**；NMS 反射不亢进、是铅管样。
> - **MAOI HTN crisis vs SS 最易混**（v1.1 新增）：两者都"MAOI 引起" + 都急性起病，但 **HTN crisis 走 adrenergic（NE/Epi → 血压↑头痛），SS 走 serotonergic（5-HT → 反射亢进/阵挛/散瞳）**。看**触发分流**：食物→HTN，药→SS。
> - **β 阻断单用禁忌于 MAOI HTN crisis**（v1.1 新增）：单纯 β 阻断会让 α1 失对抗 → 血压反而进一步升高。必须用 **phentolamine（纯 α 阻断）/ nitroprusside / labetalol（α+β 双阻）**。
> - **抗胆碱能毒性(anticholinergic toxicity)** 也表现高热+谵妄，但**皮肤干热（无汗）、肠鸣音消失、散瞳**——与上述四者"出汗/自主神经活跃"不同（"red as a beet, dry as a bone, hot as a hare, mad as a hatter"）。

---

## Memory Hook（记忆挂钩）

> [!success] 锁定记忆（v1.1 四联版）
> - **NMS = N→脑(Neuro)**：多巴胺被关 → 慢(数天) → 救脑用 **bromocriptine**
> - **MH = M→肌(Muscle)**：钙失控 → 麻醉中急起 → 救肌用 **dantrolene**
> - **Serotonin = S→反射 Sky-high(亢进)**：阵挛+反射亢进+散瞳 → 救用 **cyproheptadine**
> - **HTN crisis = H→血压 (Hypertension)**：tyramine 食物 → NE 爆发 → 救压用 **phentolamine**
> - 四个解药口诀："**多巴胺 bromo / 钙 dantro / 五羟色胺 cypro / 肾上腺 phento**"
> - **MAOI 两条祸记忆钩**："**红酒配奶酪，血压爆（HTN）；MAOI 配新药（5-HT），反射跳（SS）。**"

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes#^Q12203]] NMS（haloperidol 触发，问机制选"多巴胺活性↓"；本草稿源头题）
  - [[mistakes/uworld-mistakes#^Q4879]] MAOI tyramine HTN crisis（v1.1 触发题；MAOI 两条祸 — adrenergic vs serotonergic 通路分流）
  - [[mistakes/uworld-mistakes#^Q11853]] MDMA + Serotonin Syndrome（SS 实例 — MDMA 是强 5-HT 释放剂；与本表 SS 列互证）
  - [[mistakes/uworld-mistakes#^Q2501]] NMS vs EPS 鉴别 + NMS 用药（NMS 实例 — bromocriptine / dantrolene 选择；与本表 NMS 列互证）
  - [[mistakes/uworld-mistakes#^Q20497]] Venlafaxine 剂量依赖性高血压（与 HTN crisis 同 adrenergic 通路 — SNRI 高剂量 NE↑；与 MAOI+tyramine 机制同源）
  - （MH 待后续错题积累后回连）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/psych]] / [[完整笔记/Peixuan分科笔记/neuro]] / [[完整笔记/Peixuan分科笔记/心内]]（v1.1 — hypertensive crisis 鉴别与处理 phentolamine/nitroprusside/labetalol）
- 🏥 跨学科：
  - [[完整笔记/Peixuan分科笔记/外科]]（MH = 围术期麻醉急症）
  - [[完整笔记/Peixuan分科笔记/肾脏]]（NMS/MH 横纹肌溶解 → 肌红蛋白尿 → AKI）
  - [[完整笔记/Peixuan分科笔记/感染]]（v1.1 — **Linezolid 是隐藏 MAOI**：治 VRE/MRSA 时与 SSRI/tramadol 联用诱发 SS；用前需停 SSRI ≥2 周，fluoxetine ≥5 周）
- 🌱 TODO（待生成衍生）：等 psych / neuro 章节复习完，请 Claude Code 把本表 + [[mistakes/uworld-mistakes#^Q12203]] NMS + [[mistakes/uworld-mistakes#^Q4879]] HTN crisis + 后续 MH / Serotonin Syndrome / 抗胆碱能错题整合升级为正式专题笔记 [[完整笔记/专题笔记/_衍生_高热肌强直急症鉴别]]（凑齐 NMS / MH / SS / HTN crisis / 抗胆碱能毒性 **五鉴别** + 各自实验室指纹 + 治疗 + ECT 是否适用）

---

## 版本记录

| 版本 | 日期 | 关键变更 |
|---|---|---|
| v1 | 2026-05-23 | 初版三联鉴别表（NMS / MH / SS）+ 三秒决策树 + 反射"金钥匙" + 三机制三解药 Memory Hook + 抗胆碱能毒性对照（第 4 列待整合） |
| **v1.1** | **2026-05-23** | **触发：[[mistakes/uworld-mistakes#^Q4879]] MAOI tyramine HTN crisis 错题入库**。新增：① MAOI 两条祸（决策分流）章节（食物→HTN / 药→SS）② Tyramine 高含量食物清单 6 类 ③ 隐藏 MAOI 三剑客（linezolid / selegiline 高剂量 / methylene blue）④ High-Yield Summary Table 加入 HTN crisis 第 4 列 ⑤ 三秒决策树升 v1.1 四联版 ⑥ 高频陷阱新增 SS vs HTN crisis 鉴别 + β 阻断单用禁忌 ⑦ Memory Hook 加 H→Hypertension/phento + 红酒配奶酪记忆钩 ⑧ 关联追加 Q4879 / Q11853 / Q2501 / Q20497 + 心内主笔记 + 感染跨学科 linezolid 链 |
