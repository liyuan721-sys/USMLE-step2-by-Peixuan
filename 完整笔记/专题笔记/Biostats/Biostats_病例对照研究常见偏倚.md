---
tags:
  - USMLE-Step2
  - Biostats
created: 2026-07-06
type: 专题笔记
---

# 病例对照研究常见偏倚（Biases in case-control studies）

> [!info] 一句话定位
> **病例对照研究（case-control study）是回顾性的**：先按「有病 / 无病」分组，再回头问既往暴露。凡是"回头看 + 靠受试者回忆暴露"，第一警惕就是 **回忆偏倚（recall bias）**。

---

## 一、为什么 case-control 天生易偏

```
先确定 disease status（病例 vs 对照）
  ↓
再回顾性追问 past exposure（既往暴露）
  ↓
病例已知自己得病 → 更用力回想 / 夸大 / 错误归因
  ↓
= recall bias（回忆偏倚）→ 暴露被错误分类
  ↓
主研究问题（如"哪种剂型风险高"）被污染
```

> [!warning] 本题情境
> 病例对照研究比较乳腺癌患者 vs 对照的 **雌激素替代治疗（estrogen replacement therapy, ERT）剂型**，暴露数据**来自受试者自报**。患者更可能仔细回想激素史，对照回想得没那么细 → **recall bias** 直接动摇"不同剂型风险无差别"这个结论的**内部效度（internal validity）**。

---

## 二、Case-control 高频偏倚速查

| 偏倚 (英) | 中文 | 触发场景 | 关键钥匙 |
|---|---|---|---|
| Recall bias | 回忆偏倚 | 病例 vs 对照回忆既往暴露的准确度不同 | **回顾性 + 自报暴露** |
| Selection bias | 选择偏倚 | 病例/对照抽样不代表源人群 | 对照来源与病例不可比 |
| Interviewer bias | 访谈者偏倚 | 访谈者知道分组、追问深度不同 | 未设盲的访谈 |
| Berkson bias | 入院率偏倚 | 病例与对照都取自住院人群 | 医院对照 |
| Misclassification | 错分偏倚 | 暴露/结局归类错误 | recall bias 是其常见来源 |

> [!tip] 快速反射
> **"case-control + 靠病人回忆 = recall bias"**。这是配对反射，先答它，再看题干有没有更强线索指向别的偏倚。

---

## 三、干扰项如何排除（本题）

> [!danger] 为什么别的选项弱
> | 干扰项 | 为什么不是首选 |
> |---|---|
> | Selection bias 选择偏倚 | 题目已给 **age-matched controls**、样本量相近 → 抽样端相对可控 |
> | Sampling / sample size 样本量 | 样本量相近，不是核心缺陷 |
> | Confounding 混杂 | 年龄已匹配；且问的是"剂型自报"这个测量端问题 |
> | 核心焦点 | 暴露信息**来自患者回忆而非处方数据库** → 直指 recall bias |

> [!info] 内部效度视角
> 本题不是问"哪种偏倚最常见"这种死记题，而是问 **什么最会动摇该研究结论**。暴露测量端不可靠 → 结论"剂型间无差别"不可信 → 选 recall bias。

---

## 四、复习题

> [!question]- 病例对照研究里，暴露信息靠受试者自报，最该警惕哪种偏倚？
> **Recall bias（回忆偏倚）**。病例因已知患病更用力/更偏差地回忆既往暴露，导致暴露错分。

> [!question]- 如何在设计上减少 recall bias？
> 用**客观暴露记录**（如处方数据库、病历、生物标志物）替代自报；对访谈者与受试者尽量**设盲**分组信息；或选用暴露记录早于发病的**前瞻性/巢式设计**。

> [!question]- 题干给了 age-matched controls，这排除了哪种偏倚、不排除哪种？
> 年龄匹配主要控制**年龄这一混杂（confounding）**，但**不能**修正靠回忆得来的暴露错分——recall bias 仍在。

---

## 🔗 关联

- 🔁 错题：待补
- 📚 主笔记：[[完整笔记/Peixuan分科笔记/Biostats_Master]]
- 🏥 跨学科：任何"回顾性问既往用药/暴露"的流行病学题（药物流行病、致畸暴露史）都先排 recall bias。
- 🌱 反链：[[NBME/nbme-records/NBME 11/NBME11A_S2_breakdown#^Q091]]
  - 相关专题：[[完整笔记/专题笔记/Biostats/Biostats_OR_CI_因果三连陷阱]]（case-control 只能算 OR、不能算 risk）
