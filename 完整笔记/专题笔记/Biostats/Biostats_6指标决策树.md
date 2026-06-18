# Biostats 6 指标决策树（2 × 3 框架）

> [!success] 🚀 超简版入口（绕的时候先看这个）— 一个例子 + 3 个动作
> **别背 6 个公式。** 记住一个例子：**吸烟者得病 40%，不吸烟 10%**。对这两个数只做 3 个动作：
>
> | 动作 | 算 | 叫什么（全称） | 人话 |
> |---|---|---|---|
> | **① 减** | 40 − 10 = **30%** | **ARI** = Attributable Risk / Absolute Risk Increase（归因危险度 / 绝对风险增加） | 吸烟**多加** 30% 风险（绝对差） |
> | **② 除（比）** | 40 ÷ 10 = **4 倍** | **RR** = Relative Risk / Risk Ratio（相对危险度） | 吸烟者是 **4 倍**（强度） |
> | **③ 除（占比）** | 30 ÷ **40** = **75%** | **ARP** = Attributable Risk Percent（暴露组归因危险度百分比） | 病里 **75%** 赖吸烟（除以暴露组！） |
> | **④ 取倒数** | 1 ÷ 0.30 ≈ **3.3 人** | **NNH** = Number Needed to Harm（需暴露致害人数） | 3.3 个吸烟多害 1 个 |
>
> **唯一易混点**：②③ 都是"除"——**RR 除以"另一组"（10）；ARP 减完除以"暴露组自己"（40）**。
> **死记一条**：问"**百分比 / 几成赖暴露**" → **减完一定再除以暴露组（大的那个）**，别停在 30%（那是 ARI）。
>
> **救人侧 = 同一套动作换皮**（吃药 16%→10%）：减=**ARR**(6%) / 占比=**RRR**(37%) / 倒数=**NNT**(17人)。
> → **ARR↔ARI、RRR↔ARP、NNT↔NNH**；逻辑一套，名字两套（救人"降低/防" vs 害人"增加/害"）。

## 📐 核心决策树

```
                       2 × 3 = 6 指标
                              │
                ┌─────────────┴─────────────┐
                │                           │
          "救人"场景                   "害人"场景
        (干预降低风险)                 (暴露增加风险)
                │                           │
      ┌─────────┼─────────┐       ┌─────────┼─────────┐
      │         │         │       │         │         │
     ARR       RRR       NNT      ARI      RRI       NNH
   绝对值     相对%      人数    绝对值    相对%      人数
      │         │         │       │         │         │
      ▼         ▼         ▼       ▼         ▼         ▼
  Risk_ctrl  ARR/      1/ARR   Risk_exp   ARI/      1/ARI
  −Risk_tx   Risk_ctrl         −Risk_un   Risk_un
                                exp       exp
```

---

## 📋 表格速查版

| 维度 | 救人场景 | 害人场景 |
|---|---|---|
| **绝对差**（百分点）| ARR = Risk_ctrl − Risk_tx | **ARI** = Risk_exp − Risk_unexp |
| **相对比**（%）| RRR = ARR / Risk_ctrl | RRI = ARI / Risk_unexp |
| **人数** | NNT = 1 / ARR | NNH = 1 / ARI |
| **归因占比**（%，**分母 = 暴露组 Re**）| （救人侧对应 RRR，见上行） | **ARP =（Re − Ru）/ Re =（RR − 1）/ RR** |

> [!danger] ⚠️ ARI ≠ ARP（你反复栽的就是这一步）
> | | 含义 | 公式 | 单位 | 例（Re=20%, Ru=5%） |
> |---|---|---|---|---|
> | **ARI**（绝对风险增加 Absolute Risk Increase；= 归因危险度 attributable risk, AR）| 暴露**多加**的绝对风险 | **Re − Ru** | 百分点 | **15%** |
> | **ARP**（归因危险度百分比 Attributable Risk Percent；= 归因分数 AF）| 暴露者发病中**赖暴露的占比** | **(Re − Ru) / Re** | 占比% | **75%** |
>
> **ARP 必须再除以 Re（暴露组风险）** —— 别减完就停（那是 ARI）。
> **直觉**：暴露者 20% 得病，其中 15% 是暴露害的 → 15 占 20 的 **75%** = ARP。
> **口诀**：题问 "**percentage** attributed to" → **减完除以暴露组**；选项里**带 % 且最大的 = ARP**（≥ ARI）。错题 [[mistakes/uworld-mistakes_2026-05#^Q20430]]（反复错×3：先选 NNH 13，后选 ARI 15）。

---

## 🧮 给 RR 时的速算捷径（RRR / RRI / ARP）⭐

> [!tip] 给 RR 时走捷径
> - **法 1（先减后除）**：RRR = ARR / Risk_ctrl =（Risk_ctrl − Risk_tx）/ Risk_ctrl
> - **法 2（用 RR）**：**RRR = 1 − RR**，其中 **RR = Risk_tx / Risk_ctrl**
>
> 两者完全等价（把 RR 代入即得：1 − Risk_tx/Risk_ctrl =（Risk_ctrl − Risk_tx）/ Risk_ctrl）。
> **stem 直接给 RR 就用法 2 最快**：如 RR = 0.83 → RRR = 1 − 0.83 = **0.17**（[[mistakes/uworld-mistakes_2026-06#^Q20561]]）。

> 同理害人场景：**RRI = RR − 1**（RR > 1 时），与 RRI = ARI / Risk_unexp 等价。

> [!tip] 害人侧"归因占比"捷径：**ARP =（RR − 1）/ RR** ⭐（你反复错的那个）
> - **给 RR 直接套**：ARP =（RR − 1）/ RR。如 **RR = 4 → (4−1)/4 = 75%**（与具体风险值无关，RR 一样 ARP 就一样）。
> - **与 RRR 完美镜像**（都是"占比%"家族、分母都是**大的那个风险**）：
>   - 救人 **RRR = 1 − RR**（RR<1）
>   - 害人 **ARP =（RR − 1）/ RR**（RR>1）
> - **等价证明**：ARP =（Re − Ru）/ Re = 1 − Ru/Re = 1 − 1/RR =（RR − 1）/ RR。
> - ⚠️ **别和 ARI 混**：ARI = Re − Ru（减法，绝对差）；**ARP 要除以 Re**（占比）。错题 [[mistakes/uworld-mistakes_2026-05#^Q20430]]。

---

## 🔬 RR vs ARP：算法 + 临床意义 ⭐⭐

| | **RR**（相对危险度 Risk Ratio） | **ARP**（归因危险度百分比 Attributable Risk Percent） |
|---|---|---|
| 公式 | Re / Ru | (Re − Ru) / Re =（RR − 1）/ RR |
| 单位 | 倍（比值） | 占比 % |
| 临床意义 | 暴露让发病风险**变成几倍** = **关联强度** | 暴露者的病里**几成赖暴露**（= 戒掉暴露可预防的比例） |
| 回答 | "关系**多强**?"（病因学） | "暴露者的病能**防掉多少**?"（公共卫生/可预防性） |
| 解读例 | RR=4 → 暴露者发病率是 4 倍 | ARP=75% → 暴露者的病 75% 是暴露害的，剩 25% 是基线 |

### RR → ARP 阶梯（背下来秒答）

| RR | 1 | 2 | **4** | 5 | 10 | ∞ |
|---|---|---|---|---|---|---|
| **ARP =(RR−1)/RR** | 0% | 50% | **75%** | 80% | 90% | →100%（永不到） |

**RR 越大 → ARP 越接近 100%**（暴露解释的病越多），但永远 <100%。**ARP 只取决于 RR**（绝对风险约掉了）。

### 相对 vs 绝对：同一对数据两个故事 ⭐

> [!warning] 高 RR/ARP ≠ 大绝对影响（基线低时绝对获益可能很小）
> | | R1（40% vs 10%） | R2（8% vs 2%） |
> |---|---|---|
> | RR | 4 | 4 |
> | **ARP** | **75%** | **75%** |
> | ARI（Re−Ru） | **30%** | **6%** |
> | NNH（1/ARI） | ~3.3 人 | ~17 人 |
>
> 两组暴露"同样恶"（RR/ARP 一样），但 **R1 绝对危害大得多**（基线高 → ARI 30% vs 6%）。
> **RR/ARP = 相对故事（强度 + 暴露者中可预防比例）；ARI/NNH = 绝对故事（实际波及多少人）。**

### stem 钩子

| 看到… | 要的指标 |
|---|---|
| "X 倍 / how many times more likely / 关联强度" | **RR** |
| "**percentage** of disease in exposed **attributable to** / **could be prevented** by eliminating exposure" | **ARP** |
| "绝对增加多少风险 / 多少人受害（NNH）" | ARI / NNH |

---

## 🔑 三大配套法则

1. **分母法则**：分母总是"大的那个"
   - 救人：Risk_ctrl（大）
   - 害人：Risk_unexp（基线）

2. **按意义算 > 死记公式**：看到指标先问 3 个问题
   - 救人还是害人？
   - 绝对还是相对？
   - 要不要倒数？

3. **先减后除**：算到 ARR/ARI 不算完，看 stem 要哪个指标继续算

---

## ⚠️ 易混陷阱

- **"半步陷阱"**：算出 ARR 就停 → 但 stem 要的是 RRR
- **RRR 字面提示**：R = Relative → 想到"相对" → 必须除参照基线
- **算出负数**：可能用错了场景（救人/害人搞反了）

---

## 🔗 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes_2026-06#^Q20561]] RRR vs ARR 半步陷阱（算到 ARR 就停，漏 ÷Risk_ctrl）
  - [[mistakes/uworld-mistakes_2026-06#^Q20711]] RR 计算 — 多结局图锁定正确结局行
  - [[mistakes/uworld-mistakes_2026-05#^Q20057]] ARR 反推样本量
  - [[mistakes/uworld-mistakes_2026-05#^Q20430]] ARP 阳性归因比（害人场景）
  - [[mistakes/uworld-mistakes_2026-05#^Q7708]] / [[mistakes/uworld-mistakes_2026-05#^Q7709]] 复合终点 + NNT
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
- 📋 邻近笔记：[[完整笔记/专题笔记/Biostats/Biostats_诊断4指标动态_PPV陷阱]]（Sn/Sp/PPV/NPV 诊断指标家族 — 与本卡风险指标家族区分）/ [[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]
- 🌱 TODO：连对 2 道 ARR/RRR/RR/NNT 计算题 → 可降级相关错题状态
