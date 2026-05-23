---
title: 📚 复习入口（Dashboard）
date: 2026-05-10
tags:
  - dashboard
  - 学习工具
aliases:
  - Dashboard
  - 复习仪表盘
status: 常驻
---

# 📚 复习入口

> [!info] 极简标签体系（v4）
> 笔记**不预设客观标签** — 标签完全由你刷题/学习时**手动添加**
> 只用 5 个核心标签，每个都对应明确行动：

| 标签 | 含义 | 行动 |
|------|------|------|
| `#薄弱点` | 反复错的概念 | 每天复习 |
| `#难记` | 死记硬背的内容（口诀/数字/列表） | 间隔重复 |
| `#考前必看` | 考前 24h 冲刺 | 考前 1 天看 |

---

## 🎯 当前焦点 — 2026-05-23 Psych 治疗 4 连击 + Q15088 反复错 🔴

> [!danger] 反复错 — 最高优先级
> [[mistakes/uworld-mistakes#^Q15088-redo|Q15088 MDD-psychotic]] 2 天间隔重做仍选 C（Fluoxetine + Lithium）→ **🔴 反复错**。根错因 = 治疗哲学误区（不急 ≠ 不治妄想 / Lithium 误当温和版 AP / 精神运动迟滞误读为稳定）。**3 天内必须重做验证**。

| 优先级 | 薄弱点 | 复习入口 |
|---|---|---|
| ⭐⭐⭐🔴 | **MDD with psychotic features 治疗**（妄想必须有 AP / Lithium 不治妄想）| [[完整笔记/专题笔记/psych/_衍生_精神障碍选对治疗SOP#3.4 MDD 治疗按「有无精神病性」分流 ⭐⭐⭐\|SOP §3.4]] · [[mistakes/uworld-mistakes#^Q15088-redo\|Q15088 重做卡]] · [[mistakes/uworld-mistakes#^Q15088\|Q15088 首次卡]] · [[mistakes/uworld-mistakes#^Q15811\|Q15811 → ECT]] |
| ⭐⭐⭐ | **成人 ADHD + 物质滥用 → Atomoxetine**（Clonidine 是儿童款）| [[完整笔记/专题笔记/psych/_衍生_精神障碍选对治疗SOP#3.1 ADHD 用药决策\|SOP §3.1]] · [[mistakes/uworld-mistakes#^Q14348\|Q14348]] |
| ⭐⭐⭐ | **儿童 GAD vs Social Anxiety**（先数担忧靶点）| [[完整笔记/专题笔记/psych/_衍生_精神障碍选对治疗SOP#3.2 焦虑谱系（先数靶点 → 再分配药）\|SOP §3.2]] · [[mistakes/uworld-mistakes#^Q16153\|Q16153]] |
| ⭐⭐⭐ | **BED 一线 = SSRI**（减肥药 ≠ BED 药 / Bupropion 进食障碍禁忌）| [[完整笔记/专题笔记/psych/_衍生_精神障碍选对治疗SOP#3.3 进食障碍三兄弟\|SOP §3.3]] · [[mistakes/uworld-mistakes#^Q16490\|Q16490]] |
| ⭐⭐⭐ | **儿童 OCD = SSRI + CBT-ERP**（Psychodynamic 是诱饵）| [[完整笔记/专题笔记/psych/_衍生_精神障碍选对治疗SOP#3.5 心理治疗对号入座\|SOP §3.5]] · [[mistakes/uworld-mistakes#^Q8923\|Q8923]] |

> [!tip] 本周行动节奏
> - **每天先扫 5 句口诀**：[[完整笔记/专题笔记/psych/_衍生_精神障碍选对治疗SOP#四、5 大反陷阱口诀（Memory Hook）\|SOP §四 5 句口诀]]（覆盖今日 4 题 + 历史 5 题）
> - **3 天内重做 Q15088** 验证底层修复（治疗哲学误区，不是关键词漏看）
> - **背 5 张对号入座表**到反射弧（ADHD / 焦虑 / 进食 / MDD / 心理治疗）
> - 历史前置题串联复习：[[mistakes/uworld-mistakes#^Q2496\|Q2496 Panic]] / [[mistakes/uworld-mistakes#^Q21090\|Q21090 围产期 GAD]] / [[mistakes/uworld-mistakes#^Q2353\|Q2353 AN]] / [[mistakes/uworld-mistakes#^Q12541\|Q12541 AUD]]
> - 主笔记 4 个章节已挂「考前必看」「薄弱点」：MDD / OCD / Eating Disorders / GAD

### 📌 历史焦点存档
- [[复盘/2026-05-14_早晨复盘清单]]（抗凝药拮抗剂 / 抗凝特殊人群 / 5 急症 / 三大束）— 1 周重做已过期，待验证状态

---

## 📥 如何添加标签

### 方法 1: 行内（推荐）
```markdown
**Critical coarctation 的"上肢血压高"是相对的** #薄弱点
```

### 方法 2: Callout 标题后
```markdown
> [!warning] 妊娠绝对禁忌 #难记
> PPHM-CASC...
```

---

## 🔴 反复错（最高优先级 — 每天看）

```query
tag:#薄弱点 -file:"_考前必看" -file:"复习入口_Dashboard" -file:"CLAUDE" -path:"常用prompts" -path:"mistakes" -path:"复盘"
```

---

## 📝 难记内容（间隔重复）

```query
tag:#难记 -file:"_考前必看" -file:"复习入口_Dashboard" -file:"CLAUDE" -path:"常用prompts" -path:"mistakes" -path:"复盘"
```

---

## 🚨 考前必看（24h 冲刺）

```query
tag:#考前必看 -file:"_考前必看" -file:"复习入口_Dashboard" -file:"CLAUDE" -path:"常用prompts" -path:"mistakes" -path:"复盘"
```

---

## 🎯 组合查询

### 最紧急复习（薄弱点 + 考前必看）
```query
tag:#薄弱点 tag:#考前必看 -file:"_考前必看" -file:"复习入口_Dashboard" -file:"CLAUDE" -path:"常用prompts" -path:"mistakes" -path:"复盘"
```

---

## ⚠️ 重要：必须切换到阅读模式

> [!danger] Embedded Search 只在**阅读模式**显示
> 编辑模式只显示原始代码框
>
> **切换方法**：`Ctrl+E` 或右上角"切换为阅读模式"图标

---

## 🔍 替代：用 Obsidian 全局搜索

按 `Ctrl+Shift+F` → 输入：

| 搜索 | 效果 |
|------|------|
| `tag:#薄弱点` | 所有薄弱点位置（含上下文） |
| `tag:#薄弱点 tag:#考前必看` | 两个标签都有的 |
| `tag:#薄弱点 -tag:#已掌握` | 排除已掌握的 |
| `tag:#薄弱点 path:小组讲课笔记` | 限定路径 |

**搜索可保存为收藏**：右上角 ⭐

---

## 📚 复习节奏建议

### 每日
- 打开 Dashboard → 看 `#薄弱点` 列表
- 点击具体段落跳转复习

### 每周
- 通读所有 `#难记` 内容
- 把本周新错点加 `#薄弱点`

### 错题流程
- 刷错 UWorld 题 → 找到对应笔记段落 → 加 `#薄弱点`
- 反复错 3 次以上 → 加 `#考前必看`

### 考前 2 周
- 通读 `#难记` + `#薄弱点`
- 把所有还不熟的加 `#考前必看`

### 考前 1 天
- 只看 `#考前必看`

---

## 🔗 vault 主要笔记入口

### 主战场（完整笔记/）
- [[心内]]
- [[OB]]
- [[GYN]]
- [[儿科]]
- [[完整笔记/Peixuan分科笔记/pulmonary]]
- [[newborn care and screening]]
- [[完整笔记/专题笔记/OB_GYN/OB_GYN_孕期致畸药]]

### 衍生工具
- [[完整笔记/专题笔记/USMLE/USMLE_高频陷阱]]
- [[完整笔记/专题笔记/USMLE/USMLE_鉴别诊断速查]]
- [[完整笔记/专题笔记/USMLE/USMLE_高频评分_公式]]
- [[完整笔记/专题笔记/USMLE/USMLE_易混药物对照]]
- [[完整笔记/_衍生_Screening_Guidelines]]
- [[完整笔记/专题笔记/心内/心内_CHD_总索引]]（心内 × 4 衍生 × 综合征 三轴导航）
- [[完整笔记/专题笔记/psych/psych_医患沟通对话术SOP]]（MI 对话术题统一解题框架）
- [[完整笔记/专题笔记/psych/psych_精神科药物副作用速查]]（抗抑郁药 / 抗精神病药 / 锂盐 / EPS 副作用）

### 错题与记录
- [[错题本]]
- [[薄弱点]]
- [[mistakes/uworld-mistakes]]
- [[NBME/nbme-records]]

### 小组讲课笔记
- [[2026-05-10_心血管_妊娠与先心病_详细学习版]]
- [[2026-05-10_心血管_妊娠与先心病_速查版]]

### 工具
- [[工作流]]
- [[常用prompts]]
- [[诊断报告]]

---

## 💡 标签设计哲学

> [!success] 为什么只用 5 个标签？
>
> 1. **每个标签必须对应一个具体的复习动作**
>    - 模糊的标签 = 复习时不知道怎么用
>    - "高频" 标签 → 知道但不知道怎么办
>    - "薄弱点" 标签 → **每天看一遍**（具体动作）
>
> 2. **主动标注 > 被动接受**
>    - 自己标的会记住
>    - 别人贴的标签 = 视觉噪音
>
> 3. **少而精 > 多而杂**
>    - 100 个标签 = 没标签
>    - 5 个标签 = 真正的筛选工具

---

## ⚙️ 故障排查

> [!warning] Embedded Search 不显示？

**检查 1：阅读模式**
- 必须在阅读模式（Reading View）才显示
- `Ctrl+E` 切换

**检查 2：标签真的存在？**
- `Ctrl+Shift+F` → `tag:#薄弱点`
- 有结果 → 标签存在
- 无结果 → 还没加

**检查 3：搜索语法**
- ✅ `tag:#薄弱点`（冒号后无空格）
- ❌ `tag: #薄弱点`

**检查 4：手动刷新**
- `Ctrl+R` 重新加载 vault
