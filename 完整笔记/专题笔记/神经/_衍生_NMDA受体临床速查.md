---
tags:
  - USMLE-Step2
  - 神经
  - 精神科
created: 2026-05-22
type: 专题笔记
---

# NMDA 受体临床速查

> [!info] 用途
> NMDA 受体是 USMLE Step 1 神药基础 + Step 2 多个高频考点（ketamine / esketamine / memantine / anti-NMDA 脑炎 / 酒精-BZD 戒断 / Mg in eclampsia / 兴奋毒性）的共同机制锚。一张图把基础 + 临床打通。

---

## 一、本质：谷氨酸（CNS 主要兴奋递质）的一种受体

| 谷氨酸受体亚型 | 速度 | 通透 | 主要作用 |
|---|---|---|---|
| **AMPA** | 快 | Na⁺ / K⁺ | 大部分日常兴奋传导 |
| **Kainate** | 中 | Na⁺ / K⁺ | 调节 |
| **NMDA** ⭐ | 慢 | **Na⁺ / K⁺ / Ca²⁺** ⭐ | **学习记忆 / 突触可塑性（LTP）** |

> NMDA = N-Methyl-D-Aspartate（合成激动剂名字，不是天然配体；天然配体是 **glutamate**，需共激动剂 glycine / D-serine）。
>
> NMDA 的两大独特点：① 让 **Ca²⁺ 进细胞** ② **双锁门控**。

---

## 二、双锁机制 ⭐（核心理解）

```
锁 ① 配体绑定（glutamate + glycine 或 D-serine）
锁 ② 突触后膜先去极化（把堵在通道里的 Mg²⁺ 推出去）
        ↓ 两把锁都开
通道打开 → Ca²⁺ 涌入 → 启动胞内信号（CaMKII 等）
        ↓
LTP（长时程增强）= 学习记忆的细胞基础
```

> [!tip] 为什么这设计聪明
> 双锁保证只有"既有谷氨酸释放、又之前已经被激活过"的突触才进 Ca²⁺ —— 即 **"用进废退"** 的分子基础。Hebbian rule：**"cells that fire together, wire together"**。

**Mg²⁺ 是天然守门员** —— 静息状态下堵在通道里；去极化把它推出去。这条机制衍生出多个临床关联（Mg in eclampsia、低 Mg 神经兴奋等）。

---

## 三、临床应用速查表（USMLE 高频，按主题分）

### 3.1 NMDA 拮抗剂 = 解离 / 麻醉 / 抗抑郁

| 药 | NMDA 作用 | 临床用途 | 重点 |
|---|---|---|---|
| **Ketamine** | 强拮抗 | 分离麻醉（急诊 / 儿科 / 战地）；街头滥用 "Special K" | DEA Schedule III；致解离 / 幻觉 |
| **Esketamine** (Spravato) | 强拮抗（S 对映体）| **TRD + MDD with acute SI** | 鼻喷剂；详见 [[完整笔记/专题笔记/psych/_衍生_快速抗抑郁药_Esketamine]] |
| **PCP** | 强拮抗 | 街头滥用（"天使尘"）| 暴力 + 解离 + 眼球震颤 + 眼震；急救 BZD（详见 [[mistakes/uworld-mistakes#^Q3191]]）|
| **Memantine** | **弱**拮抗 | **中-重度 Alzheimer**（不是 mild）| 拮抗病理性谷氨酸过度兴奋，但不灭正常信号 —— "调音不灭音" |
| **Dextromethorphan** | 弱拮抗 | 止咳；高剂量滥用致解离 / 幻觉 | 配 ondansetron / promethazine 增强滥用风险 |
| **Tramadol** / **Methadone** | 部分拮抗 | 止痛 / OUD 治疗 | 5-HT 综合征 + 癫痫风险（你 Q3762 卡 Bupropion-Tramadol 并列降阈值药）|

### 3.2 NMDA 自身免疫 — Anti-NMDA Receptor Encephalitis ⭐

| 维度 | 内容 |
|---|---|
| **谁** | **年轻女性**（典型）/ 男性 / 儿童 |
| **何时** | 急性-亚急性起病（数周）|
| **副肿瘤背景** | **卵巢畸胎瘤**（女性 ~50% 检出）/ 男性可有睾丸生殖细胞瘤；查 pelvic US + 全身影像 |
| **典型四联** | ① **精神病性症状**（幻觉 / 妄想 / 紧张症样）② **癫痫**（多型）③ **运动障碍**（口面部不自主、舞蹈样、自主神经风暴）④ **自主神经不稳 + 意识波动**（与 catatonia / NMS 重叠）|
| **诊断** | 脑脊液 **anti-NMDA receptor antibody** 阳性 ⭐；MRI 常正常或非特异；EEG 非特异慢波 |
| **治疗** | ① **切肿瘤**（如有）② **一线**：IV 类固醇 + IVIG / 血浆置换 ③ **二线**：rituximab / cyclophosphamide |
| **预后** | 早诊 + 治疗 ~80% 显著恢复；可复发 |

> [!danger] 题干红旗
> "**年轻女性 + 急性精神病性症状 + 癫痫 + 不自主运动 + 自主神经不稳**" → **首先想 anti-NMDA 脑炎 + 查盆腔肿瘤**。不要套 "primary psych disorder"（你的 Q15017 / Q11967「新发精神病先排器质」原则的极致版）。

### 3.3 Mg²⁺ — 天然 NMDA 拮抗剂

| 临床 | 机制 |
|---|---|
| **Eclampsia / preeclampsia 抗惊厥** | MgSO4 IV → 堵 NMDA → 神经兴奋性↓ → 防抽搐 |
| **TdP 急救** | Mg 稳定膜电位（多机制，含 NMDA 部分）|
| **低 Mg → 神经兴奋 / TdP** | NMDA"守门员"消失 → 过度兴奋 |
| **Mg 中毒** | DTR↓ → 嗜睡 → 呼吸抑制 → 心搏停；解毒 = IV Ca |

### 3.4 酒精 / BZD 戒断 — NMDA 上调代偿

```
慢性酒精 / BZD = GABA(刹车)↑ + NMDA(油门)抑制
              ↓ 大脑长期代偿
       GABA↓（拆刹车）+ NMDA↑（加油门）
              ↓ 突然戒断
        刹车没了 + 油门最大 = 戒断性癫痫 / DTs
```

- 治疗：长效 BZD（chlordiazepoxide / diazepam）—— 重新踩刹车 + 慢慢撤
- 阿片戒断**不致命**：因为不动 GABA / NMDA 轴
- 详见 [[mistakes/uworld-mistakes#^Q3762]] Alprazolam withdrawal seizure

### 3.5 Excitotoxicity（兴奋毒性）— 卒中 / TBI 的细胞死亡机制

```
卒中 / TBI → 神经元缺氧 → 大量谷氨酸释放
            ↓
       NMDA 过度激活
            ↓
       Ca²⁺ 过载（mitochondrial damage）
            ↓
       凋亡 / 坏死
```

- 临床意义：解释为什么早期再灌注 + 神经保护是关键
- Memantine 的"调音"作用基于这条机制

---

## 四、GABA ↔ NMDA 镜像（理解戒断综合征关键）

| 系统 | 主要递质 | 主要受体 | 临床钩 |
|---|---|---|---|
| **抑制系统**（"刹车"）| GABA | GABA-A / B | 酒精 / BZD / 巴比妥增强 → 镇静 / 抗惊厥；急性戒断 = 拆刹车 → 兴奋失控 |
| **兴奋系统**（"油门"）| Glutamate | NMDA / AMPA / kainate | NMDA 拮抗 → 解离 / 麻醉 / TRD；NMDA 过度激活 → 兴奋毒性 / 戒断癫痫 |

> [!tip] 一句话理解
> **酒精 / BZD 戒断致命 = 大脑同时拆刹车（GABA↓）+ 加油门（NMDA↑）→ 神经元过度兴奋 → 癫痫 / DTs**。
> 阿片戒断不致命 = 不动这两个轴。

---

## 五、Memory Hook

- **NMDA = "Need More Depolarization Always"** → 双锁机制（光有配体不够，要先去极化把 Mg²⁺ 推走）
- **N-M-D-A 四字母拆**：**N**eeds memory(LTP) / **M**g 守门员 / **D**epolarization-gated / **A**nimal **K**etamine 拮抗
- **NMDA 拮抗剂 KMD 三兄弟**：**K**etamine（rapid antidepressant + 解离麻醉）/ **M**emantine（Alzheimer）/ **D**extromethorphan（止咳）
- **Anti-NMDA 脑炎红旗**：**"年轻女 + 精神病 + 癫痫 + 不自主 + 查盆腔（卵巢畸胎瘤）"**
- **酒精戒断 NMDA 机制**：**"拆刹车 + 加油门 = 命悬一线"**

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes#^Q3762]] Alprazolam withdrawal seizure（NMDA 上调 + GABA 下调 → 戒断癫痫）
  - [[mistakes/uworld-mistakes#^Q3191]] PCP 中毒首选 BZD（NMDA 拮抗剂中毒处理）
  - [[mistakes/uworld-mistakes#^Q15791]] Catatonia（NMDA hypofunction 假说之一 — lorazepam 一线）
  - [[mistakes/uworld-mistakes#^Q15017]] 新发精神病 workup 顺序（anti-NMDA 脑炎是必排器质病因之一）
  - [[mistakes/uworld-mistakes#^Q11967]] 儿童急性精神病→SLE（多系统拼图思路 — anti-NMDA 脑炎是同范式）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/neuro]] / [[完整笔记/Peixuan分科笔记/psych]] / [[完整笔记/Peixuan分科笔记/免疫疫苗]]
- 🏥 跨学科：
  - [[完整笔记/专题笔记/psych/_衍生_快速抗抑郁药_Esketamine]]（Esketamine 详细，NMDA 拮抗剂代表）
  - [[完整笔记/Peixuan分科笔记/OB]]（MgSO4 in eclampsia — Mg 是天然 NMDA 拮抗剂）
  - [[完整笔记/Peixuan分科笔记/GYN]] / [[完整笔记/Peixuan分科笔记/hematology oncology]]（anti-NMDA 脑炎与卵巢畸胎瘤 / 副肿瘤综合征）
  - [[完整笔记/专题笔记/psych/psych_物质急诊速查]]（PCP / ketamine / dextromethorphan 滥用）
- 🌱 TODO（待积累）：
  - 等积累 anti-NMDA 脑炎错题 → 单独建条目
  - 等积累副肿瘤综合征错题 → 生成衍生（含 anti-NMDA / anti-Hu / anti-Yo / Lambert-Eaton 等）
  - 等积累兴奋毒性 / 神经保护错题 → 衍生

## ✅ 学习行动

- [ ] 默写谷氨酸三受体对比表（AMPA / kainate / NMDA）
- [ ] 默写 NMDA 双锁机制 + Mg²⁺ 守门员
- [ ] 默写 NMDA 拮抗剂 KMD 三兄弟（Ketamine / Memantine / Dextromethorphan）+ esketamine
- [ ] 默写 anti-NMDA 脑炎四联 + 卵巢畸胎瘤背景 + 治疗阶梯
- [ ] 默写酒精 / BZD 戒断的 GABA-NMDA 跷跷板机制
- [ ] 找 3 道类似题：① Mg in eclampsia ② anti-NMDA 脑炎 ③ Memantine in Alzheimer
