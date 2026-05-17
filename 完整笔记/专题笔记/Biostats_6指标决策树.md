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
