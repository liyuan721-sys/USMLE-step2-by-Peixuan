# UWorld 错题整理
###  [2026-05-10] Hill's criteria:看到剂量分层 + RR 单调递增 = 选 dose-response
#biostats #causality #dose-response 🟡
- **来源**:UW Q20787
- **题干要点**:RCT 比较运动 vs 标准护理对糖尿病停药率影响,运动组按剂量分 T1/T2/T3 三组,RR 随剂量从 12.1→25.2→38.9 单调递增
- **正确答案**:B — 更大运动量与更高停药率显著相关(= biological gradient / dose-response)
- **我选了**:B(做对但 Mark)— 纠结点:B vs D
- **关键 buzzword / 识别公式**:
  - "**剂量分层 + 结果单调** → dose-response" 
  - "**additional support**" → 排除已在题干主结果里的信息(D 是 RCT 主结果,不算 additional)
  - **Hill's 三大金刚**:dose-response / temporality / strength of association
- **关联笔记**:[[Biostats_Master#Causality / Hill's criteria]]
- **重做次数**:☐ 1st
- **状态**:🟡 不熟(Mark)

**干扰项分析**:
- A. "Bias completely eliminated" — 错。"completely" 是 USMLE 经典绝对化陷阱,RCT 也不可能完全消除 bias
- C. 12 个月随访时长 — 错。follow-up 时长是研究设计要素,但**不是 Hill's criteria**
- D. RCT 主结果(intensive vs standard 有显著关联)— 错。这是题干已给的信息,不是 "additional" 支持

### [2026-05-10] OR 方向陷阱 + case-control 不能算 risk

#biostats #odds-ratio #case-control #方向陷阱 🔴

- **来源**: UW Q20227
- **题干要点**: Case-control 研究,Black vs Non-Hispanic White 女性的 pregnancy-related death,未调整 OR = 3.07 (95% CI 2.78-4.20),调整后 OR = 2.65 (95% CI 2.12-3.45) 仍显著
- **正确答案**: B — 调整后关联仍显著,提示有**未被研究纳入的外部因素**(如结构性歧视)在起作用
- **我选了**: D — 错因:**方向陷阱 + risk/odds 混淆**(双重陷阱)
- **关键 buzzword / 识别公式**:
  - **OR > 1 → 暴露组 odds 高于 reference 组**(谁是暴露谁是 reference,看题干"X compared to Y" — X 是暴露)
  - **Case-control 只能算 OR,不能算 risk/RR**(因为不是从暴露追到结局,是从结局倒推暴露)
  - "**adjusted OR 仍显著**" → 残留关联 → 暗示有**未测量的混杂**(unmeasured confounders / external factors)
- **关联笔记**: [[Biostats_Master#Odds Ratio]] / [[Biostats_Master#Study Design - Case-Control]]
- **重做次数**: ☐ 1st
- **状态**: 🔴 反复错

**干扰项分析**:
- A. "primarily due to poverty / low prenatal care" — 错。这些因素已经在 adjusted model 里 controlled 了,关联仍显著说明这些**不是主因** 
- C. "case-control design 不能得出 statistically significant conclusions" — 错。case-control **可以**做 OR + CI,这是其核心用途(尤其对罕见结局)
- **D. "NHW 是 Black 的 3 倍"** — 错。**方向反了**。题干 "Black compared to NHW" 意思是 Black 是暴露组,OR 3.07 = Black 的 odds 是 NHW 的 3 倍。USMLE 经典反向陷阱
- E. "调整 contraception use → advanced maternal age contributes" — 错。研究**没有**调整 contraception use,而且 maternal age >35 的 p = 0.12 不显著

**⚠️ CK 高频陷阱**:
1. **OR 方向永远看"X compared to Y" — X 是暴露,Y 是 reference**
2. **Case-control 永远算 OR,不算 RR/risk**(选项里说 "risk" 还涉及 case-control → 警惕)
3. **Adjusted OR 仍显著 → 有 unmeasured confounders**(经典考点,常考"种族健康差异"vignette)