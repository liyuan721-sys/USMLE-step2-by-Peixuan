---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-06-24
type: 专题笔记
---

# 广告题套路 — 相对 vs 绝对 measures（"相对放大"骗局）

> [!info] 这张卡解决什么
> UWorld / NBME 的**药品广告题（drug ad / promotional material）**反复用**同一组数据**报出"看起来很大"的相对数字（relative measures）来夸大疗效，而**绝对获益（absolute measures）其实很小**。本卡把 4 道源题（[[mistakes/uworld-mistakes_2026-06#^Q22326]] / [[mistakes/uworld-mistakes_2026-06#^Q22327]] / [[mistakes/uworld-mistakes_2026-06#^Q21323]] / [[mistakes/uworld-mistakes_2026-06#^Q20561]]）串成一个反射：**看到广告强调大百分比 → 立刻换算绝对差**。

---

## 一、一句话核心

> [!danger] 铁律
> **相对 measures（RRR / OR / HR 降幅 / "X% greater odds"）放大效应；绝对 measures（ARR / absolute difference 绝对差）才反映真实获益。**
> 广告与论文摘要**偏爱相对**（数字大、好看）；考点 = 你能不能识破并算出绝对差。

---

## 二、同一组数据的"三张脸"（Q22326 + Q22327 实例）⭐

LupMAB + 标准治疗 vs 标准治疗，肾应答率 **43% vs 32%**（p < 0.05）。同一组数字可以报成三个完全不同的"大小"：

> [!info]- 📊 LupMAB 广告原图（Q22326 / Q22327 源 vignette）
> ![[{AEAB3965-BBD1-4B73-97FF-15D25AD9335F} 1.png]]
> 
> 广告醒目大字 **"55% greater odds"**（odds 相对，最唬人）；细看肾应答 **43 vs 32**（绝对差仅 11pp）；不良事件表两组接近。典型"相对放大"排版。

```
治疗组应答 43%        对照组应答 32%
──────────────────────────────────────────────
① 绝对差 (absolute difference / ARR)
     43% − 32% = 11 个百分点          ← 真实获益（最小、最诚实）
② 相对差 (relative difference / RRR-型)
     (43 − 32) / 32 = 34%             ← 中等放大
③ odds 相对 ("55% greater odds" → OR≈1.55)
     odds_tx=43/57=0.75
     odds_ctrl=32/68=0.47
     OR = 0.75 / 0.47 ≈ 1.6          ← 最大放大（广告选这个登广告）
──────────────────────────────────────────────
同一份数据 → 11% / 34% / 55%，广告永远挑最大的那张脸。
```

> [!warning] odds ≠ probability（这正是 odds 被放大的根源）⭐
> - **Probability（概率/率）= 应答 / 总人数** = 43/100 = 43%。
> - **Odds（比值）= 应答 / 未应答** = 43/57 = 0.75（**57 = 100 − 43 = 未应答率**）。
> - 分母从"总数 100"换成"未应答（100 − 它自己）"→ 数字被抬高 → **OR 永远比 RR 更夸张**（结局越常见放大越狠）。
> - 一句话：**「概率除以总数，odds 除以'剩下没发生的'。」** 看到广告报 odds/OR，先换回绝对率（43% vs 32%，真实差就 11pp）。

> [!warning] 两道题的考法
> - **Q22326（Item 1，做错）**：广告说 "55% greater odds" → 要你反推 **OR = 1 + 55% = 1.55**（不是 1.22），再用 p=0.031 卡掉含 1 的 CI。
> - **Q22327（Item 2，做对）**：要你识破 **真实绝对获益(11%)远小于宣传的 55%**（C 选项）；不能据此推单药、不能据小亚组、p<0.05 已足够不必 CI。

---

## 三、relative vs absolute 速查表

| 指标 | 类型 | 公式 | null value | 性格 |
|---|---|---|---|---|
| **ARR**（absolute risk reduction 绝对风险降低）| **绝对** | Risk_ctrl − Risk_tx | 0 | 真实、最小、最诚实 |
| **绝对差**（mean / % difference）| **绝对** | 直接相减 | 0 | 同上 |
| **RRR**（relative risk reduction 相对风险降低）| **相对** | ARR ÷ Risk_ctrl = **1 − RR** | 0 | 放大 |
| **RR**（risk ratio 风险比）| 比值 | Risk_tx ÷ Risk_ctrl | 1 | — |
| **OR**（odds ratio 比值比）| 比值（相对）| odds_tx ÷ odds_ctrl | 1 | 比 RR 更夸张（尤其结局常见时）|
| **HR**（hazard ratio 风险比，时间-事件）| 比值（相对）| 瞬时风险比 | 1 | 降幅 = **1 − HR** |
| **NNT**（number needed to treat）| 绝对衍生 | **1 / ARR**（向上取整）| ∞ | ARR 越小 NNT 越大 = 获益越虚 |

> [!tip] 一眼分辨
> - 字面带 **"relative" / "greater odds" / "% reduction in risk"** → **相对**（要警惕放大）。
> - 字面带 **"absolute" / "percentage points 个百分点" / "ARR" / "NNT"** → **绝对**（真实）。
> - **比值 null = 1（RR/OR/HR）；差值 null = 0（ARR/绝对差）**。

---

## 四、HR 降幅 + 复合终点（Q21323）⭐

广告：Toraflozin vs 安慰剂，复合终点（CV 死亡/住院/急诊）**480 vs 640** 事件（各 N=8000），**HR = 0.75（95% CI 0.63–0.88）**。

```
相对脸：HR 0.75 → 降幅 = 1 − 0.75 = 25%        ← 广告/正确选项的"25%"
绝对脸：480/8000 = 6%  vs  640/8000 = 8%
        ARR = 8% − 6% = 2 个百分点              ← 真实获益其实只有 2pp
诱饵   ："降低 75%"(把 HR 值当降幅) / "160 例 CV 死亡"(复合终点不可拆)
```

> [!danger] 三个高频坑
> - **HR 值 ≠ 降幅**：HR 0.75 是降 **25%**（1−HR），不是 75%。
> - **复合终点（composite endpoint）不可拆**：640−480=160 是复合事件差，**不能**说成"多 160 例 CV 死亡"。
> - **HR ≈ RRR（当事件不常见时）**：本题 HR 0.75 ↔ 相对降 25%（2/8）对得上。

---

## 五、RRR vs ARR 半步陷阱（Q20561）⭐

题问 **RRR**，很多人算到 **ARR（绝对差）就交卷** → 漏了"÷ Risk_ctrl"那半步。

```
① Risk_ctrl = 事件/样本（对照）   ② Risk_tx = 事件/样本（治疗）
③ ARR = Risk_ctrl − Risk_tx       ← 半步（绝对，干扰项塞这个值）
④ RRR = ARR ÷ Risk_ctrl = 1 − RR  ← 到站（相对）
   NNT = 1 / ARR
```

> [!warning] 反射
> 见 **"RRR"（R = Relative）→ 必须除基线风险**；交 ARR 的值 = 中钓饵。也可直接 **1 − RR**。

---

## 六、USMLE stem 信号 + 答题反射

| Stem 信号 | 反射 |
|---|---|
| 广告/promotional material **强调一个大百分比** | 警惕**相对放大** → 自己算**绝对差** |
| "X% greater odds" | OR = **1 + X%**；再 p/CI 判显著 |
| "X% reduction in risk" / RRR | 相对 → 真实获益可能很小，找 ARR |
| HR / RR / OR = 某值 | 降幅 = **1 − 比值**（别把比值当降幅）|
| 选项里有"绝对差/真实获益较小" | 常是**正确**的诚实选项 |
| 复合终点 composite | **不可拆**到单一组分 |

> [!success] 黄金套路
> **广告题问"最恰当结论/推荐" → 选最诚实、最不越界的那句**（通常点明"绝对获益较小"或"只能下保守结论"），**远离夸大相对数字 / 拆复合终点 / 推单药 / 据小亚组**的选项。

---

## 七、Memory Hook

> [!success] 记忆挂钩
> - **"相对放大、绝对真实"**——RRR/OR/HR 降幅好看，ARR 才是真获益。
> - **"同一组数据三张脸：11% / 34% / 55%，广告挑最大。"**
> - **"降幅 = 1 − 比值"**（HR 0.75 = 降 25%，不是 75%）。
> - **"RRR 带 R=Relative，必须除基线；ARR 是半步。"**
> - **"比值 null=1，差值 null=0；复合终点不可拆。"**

---

## 八、🔗 关联

- 🔁 同主题错题/做对题：
  - [[mistakes/uworld-mistakes_2026-06#^Q22326]] "55% greater odds" → OR 1.55 + CI（Item 1，做错 🔴 计算）
  - [[mistakes/uworld-mistakes_2026-06#^Q22327]] 绝对差 11% ≪ 宣传 55%（Item 2，做对）
  - [[mistakes/uworld-mistakes_2026-06#^Q21323]] HR 0.75 = 降 25% + 复合终点不可拆（做对）
  - [[mistakes/uworld-mistakes_2026-06#^Q20561]] RRR vs ARR 半步陷阱（做错 计算）
  - [[mistakes/uworld-mistakes_2026-05#^Q20057]] ARR 反推样本量
  - [[mistakes/uworld-mistakes_2026-06#^Q12673]] NNT=1/ARR（ARR=7.2%→NNT 14；做对 🟢）
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
- 📋 邻近专题：
  - [[完整笔记/专题笔记/Biostats/Biostats_6指标决策树]]（救人/害人 6 指标 + 半步陷阱完整版）
  - [[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]（OR 方向/换算 + CI 判读）
  - [[完整笔记/专题笔记/Biostats/Biostats_统计显著vs临床显著]]（绝对差 vs 阈值 = 临床显著）
- 🏥 跨学科：[[完整笔记/Peixuan分科笔记/心内]]（降压/心血管复合终点解读）/ [[完整笔记/Peixuan分科笔记/肾脏]]（狼疮肾炎 RCT）
- 🌱 TODO：再遇广告题/相对绝对题 → 增量补例

---

## 九、✅ 默写测试

> [!question]- 默写题 1
> 同一组数据 43% vs 32%，写出绝对差、相对差、odds 三种"脸"的算法与数值，并说明广告为何选 55%。

> [!question]- 默写题 2
> HR = 0.75 代表风险降低多少？为什么不是 75%？复合终点的总事件差能不能拆成单一组分？

> [!question]- 默写题 3
> RRR 和 ARR 的公式各是什么？"半步陷阱"指什么？RRR 还能用什么一步式算出？

> [!question]- 默写题 4
> 看到药品广告强调"55% greater odds / 降低风险 40%"，你的第一反射动作是什么？答题时倾向选哪一类选项、远离哪一类？
