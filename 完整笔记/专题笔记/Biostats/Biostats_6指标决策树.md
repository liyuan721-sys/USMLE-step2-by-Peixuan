# Biostats 6 指标决策树（2 × 3 框架）

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
     ARR       RRR       NNT     ARI/ARP   RRI       NNH
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
| **绝对差**（百分点）| ARR = Risk_ctrl − Risk_tx | ARI/ARP = Risk_exp − Risk_unexp |
| **相对比**（%）| RRR = ARR / Risk_ctrl | RRI = ARI / Risk_unexp |
| **人数** | NNT = 1 / ARR | NNH = 1 / ARI |

---

## 🧮 RRR 的两个等价公式 ⭐

> [!tip] 给 RR 时走捷径
> - **法 1（先减后除）**：RRR = ARR / Risk_ctrl =（Risk_ctrl − Risk_tx）/ Risk_ctrl
> - **法 2（用 RR）**：**RRR = 1 − RR**，其中 **RR = Risk_tx / Risk_ctrl**
>
> 两者完全等价（把 RR 代入即得：1 − Risk_tx/Risk_ctrl =（Risk_ctrl − Risk_tx）/ Risk_ctrl）。
> **stem 直接给 RR 就用法 2 最快**：如 RR = 0.83 → RRR = 1 − 0.83 = **0.17**（[[mistakes/uworld-mistakes_2026-06#^Q20561]]）。

> 同理害人场景：**RRI = RR − 1**（RR > 1 时），与 RRI = ARI / Risk_unexp 等价。

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
