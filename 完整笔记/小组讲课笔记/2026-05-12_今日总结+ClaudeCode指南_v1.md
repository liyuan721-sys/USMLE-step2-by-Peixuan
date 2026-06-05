---
tags:
  - USMLE-Step2
  - 学习日志
  - Claude-Code-Brief
created: 2026-05-12
session: AMBOSS_Neuro_HY200
status: 日总结-v1
---

# 2026-05-12 Neuro HY200 — 今日总结 + 行动清单

> [!info] 文件用途
> - **第一部分**：今日学习数据 + 产出清单（给 Peixuan 自己看）
> - **第二部分**：Claude Code 执行指南（按优先级排序的整合任务）
> - **第三部分**：本周复习日程

---

## 第一部分：今日产出全景

### 📊 数据
- **学习时长**：~3.5 小时（AMBOSS HY 200 Neuro 课）
- **课件张数**：~12 张
- **题目**：~10 道 UWorld 关联题（**4 道错**）
- **生成文件数**：4 个（详细 breakdown / 听课草稿 / 训练手册 / 本总结）
- **知识点总数**：~242 条
- **元技能**：6 条（新建）
- **交互式训练 widget**：2 个（Day 1 痴呆 + Day 3 头痛）

### 📁 4 个产出文件

| # | 文件 | 用途 | 状态 |
|---|---|---|---|
| 1 | **`2026-05-12_Neuro_HY200_错题详细breakdown_v1.md`** | 4 道错题 9 部分详细 + 元学习反思 | ✅ 已生成 |
| 2 | **`2026-05-12_Neuro_HY200_听课笔记草稿_v1.md`** | 按器官/疾病重组的知识结构 | ✅ 已生成 |
| 3 | **`2026-05-12_USMLE扫描算法_Buzzword训练手册_v1.md`** | 跨学科答题元技能 + Day 1-30 训练 | ✅ 已生成（含 Day 1/Day 3）|
| 4 | **`2026-05-12_今日总结+ClaudeCode指南_v1.md`** | 本文件 | ✅ 当前 |

### 🎯 6 大模块覆盖

```
✅ 模块 1：PAD / Leriche / 下肢溃疡（含 vascular vs neurogenic claudication）
✅ 模块 2：脊髓不全损伤综合征（4 大综合征 + 三大束交叉 + Syringomyelia 5 幕剧）
✅ 模块 3：痴呆完整谱系（13 种痴呆 + 病理蛋白 + 治疗 + Beers criteria）
✅ 模块 4：头痛 5 大类型 + 5 个进阶头痛
✅ 模块 5：跨学科 Schema（Horner / 不自主运动 / ADL/IADL / Tauopathy / EPS / 小大纤维）
✅ 模块 6：USMLE 答题元技能（6 条）
```

### 🌱 4 道错题分类

| 错题 | 类型 | 修复优先级 |
|---|---|---|
| 1. Pseudodementia 误选 Donepezil | **答题方法**（反射诊断 + 抑郁标志全漏）| 🔴 高（系统性模式典型） |
| 2. CJD 误选 FTD | **答题方法**（症状词 + 单一症状导向）| 🔴 高（与错题 1 同模式）|
| 3. Syringomyelia + Horner | **知识缺口**（病程演变 + Horner 关联）| 🟡 中（建主笔记修复）|
| 4. Leriche | **Schema 缺失**（PAD 三联征不认识）| 🟢 低（背三联征 + 解剖图）|

---

## 第二部分：Claude Code 执行指南

> [!warning] 给 Claude Code 的 6 个整合任务（按优先级）
> 
> Claude Code 在以下时机执行：
> - 立即执行：优先级 1 任务
> - 错题积累达到阈值时：优先级 2-7 任务

### 🔴 优先级 1（立即建，跨多疾病 schema）

**任务**：建立 [[完整笔记/专题笔记/神经/神经_Horner综合征]]

**输入**：
- `2026-05-12_Neuro_HY200_错题详细breakdown_v1.md` → 错题 3 章节
- `2026-05-12_Neuro_HY200_听课笔记草稿_v1.md` → 模块 5.1

**输出**：正式主笔记，含：
1. Horner 综合征基础（解剖通路 + 三级神经元）
2. 3 级定位与病因对照表
3. 各级标志性 stem 钩子
4. Horner ptosis vs CN III ptosis 鉴别
5. 跨学科关联（Neuro/眼科/胸外/心内）

---

### 🟡 优先级 2（≥ 6 道痴呆错题后建）

**任务**：建立 [[完整笔记/专题笔记/神经/神经_老年痴呆鉴别]]

**触发条件**：错题本累计 6+ 道痴呆相关错题
**当前进度**：4/6（今天 3 道：Pseudo + CJD + Syringomyelia 部分相关；含一道 Memantine 题，需再积累 2 道）

**输入**：
- 错题本中所有痴呆相关 Q#####
- `听课笔记草稿_v1.md` 模块 3（痴呆完整谱系）

**输出**：决策树形主笔记，含：
1. AD vs VaD vs LBD vs FTD vs Pseudo vs NPH 三相鉴别
2. Stem 关键词 → 诊断映射表
3. NBME 高频应试陷阱集合
4. 治疗对照（含 Beers Criteria）

---

### 🔴 优先级 3（≥ 8 道方法类错题后建）⭐ 最高个性化价值

**任务**：建立 [[完整笔记/专题笔记/_衍生_Peixuan答题习惯陷阱]]

**触发条件**：错题本累计 8+ 道"反射性诊断 / 单一症状导向 / 没扫全 stem"类错题
**当前进度**：3/8（今天 3 道：Pseudo + CJD + 部分相关）

**输入**：
- `错题详细breakdown_v1.md` → "元学习反思"章节
- 后续 5 道同类错题（按"我为什么错"分类）
- `训练手册_v1.md` → 第一部分（扫描算法）

**输出**：个性化反思笔记，含：
1. 系统性错误模式归纳（基于 8+ 道错题）
2. 每种模式的"trigger 场景 + 修复方法"
3. 6 条元技能应用案例
4. 月度复盘表模板

---

### 🟡 优先级 4-7（≥ 3-4 道相关错题后建）

| # | 衍生笔记 | 触发阈值 | 当前进度 |
|---|---|---|---|
| 4 | [[完整笔记/专题笔记/_衍生_脊髓不全损伤综合征鉴别]] | ≥ 4 道脊髓错题 | 1/4 |
| 5 | [[完整笔记/专题笔记/_衍生_不自主运动5种鉴别]] | ≥ 3 道运动障碍错题 | 1/3 |
| 6 | [[完整笔记/专题笔记/_衍生_下肢缺血鉴别]] | ≥ 3 道 PAD/外周血管错题 | 1/3 |
| 7 | [[完整笔记/专题笔记/_衍生_5大头痛速查]] | ≥ 3 道头痛错题 | 0/3（今天选对了）|

---

### 📝 Claude Code 命令模板

```
> 任务：根据触发条件建立 [[完整笔记/专题笔记/XXX]]
> 输入文件：
>   - /mnt/user-data/outputs/2026-05-12_Neuro_HY200_错题详细breakdown_v1.md
>   - /mnt/user-data/outputs/2026-05-12_Neuro_HY200_听课笔记草稿_v1.md
>   - mistakes/uworld-mistakes_2026-05.md (筛选相关 Q#####)
> 要求：
>   - 严格按 Peixuan 双链路径 v2 规则
>   - 中英双语 + callout + ASCII 树
>   - 关联 4 类齐全（🔁 同主题 / 📚 主笔记 / 🏥 跨学科 / 🌱 TODO）
>   - 内容标签留给 Peixuan 手动加
```

---

## 第三部分：本周复习日程（每日具体动作）

### 📅 Day 1（今晚，2026-05-12）

> [!success] 今晚必做（30-45 分钟）
> - [ ] 读 **元学习反思** 3 遍（错题 breakdown 文件开头）
> - [ ] 用 **Day 1 痴呆 Buzzword 交互卡** 刷 5 分钟（已生成 widget）
> - [ ] 用 **Day 3 头痛 Buzzword 交互卡** 刷 5 分钟（已生成 widget）
> - [ ] 4 个文件**同步到 Obsidian vault**：
>   - 错题详细 breakdown → `mistakes/` 文件夹（参考）
>   - 听课草稿 → `小组讲课笔记/` 或单独文件夹
>   - 训练手册 → `完整笔记/专题笔记/`
>   - 总结 → `小组讲课笔记/`

### 📅 Day 2（明天，2026-05-13）

> [!tip] 训练计划
> 
> **早晨 10 分钟**：
> - 重温 Day 1 痴呆 10 个 buzzword（间隔重复）
> 
> **听课时**：
> - 重点关注脊髓 / 神经外科模块（Day 2 buzzword 待填）
> - 实时记录 buzzword 给 Claude（继续填手册 Day 2）
> 
> **晚上 20 分钟**：
> - 做 5 道 UWorld 痴呆 / 脊髓相关题
> - **强制计时 60 秒/题**
> - **强制用扫描 4 步算法**
> - 写反思（用训练手册第三部分模板）
> 
> **临睡前 5 分钟**：
> - 检查"分母重设词"反射库是否新增触发词

### 📅 Day 3-7（本周后续）

| 日 | 重点 |
|---|---|
| Day 3 | 重温 Day 3 头痛卡 + 听课卒中模块 + 5 题计时 |
| Day 4 | 重温 Day 1+3 综合 + 听课癫痫 / 运动障碍 + 5 题 |
| Day 5 | 重温累计 buzzword + 听课 MS / Demyelinating + 5 题 |
| Day 6 | Day 1-5 综合自测 + 5 题 |
| Day 7 | **本周周报** + 抽 20 个 buzzword 自测 + 错的进入下周 |

### 📅 1 周后（2026-05-19）

> [!warning] 验证修复效果
> - [ ] **重做今天 4 道错题**（盲做，不看 breakdown）
> - [ ] 验证扫描算法是否内化（用时 + 错因分析）
> - [ ] 决定哪些衍生笔记可以触发生成

---

## 第四部分：今天的 7 个高价值 takeaway

> [!success] 不管别的都忘了，这 7 条必须记住
> 
> 1. **MMSE 18 是 Donepezil vs Memantine 分水岭**
> 2. **"Painless burns on hands" = Syringomyelia → 想 Horner 5 幕剧**
> 3. **"Stepwise decline + 局灶征" = VaD → 治疗是二级预防（Aspirin + 控 CV 风险），不是 Donepezil**
> 4. **"Concerned about memory + lost interest" = Pseudodementia → SSRI**
> 5. **"Startle myoclonus + EEG 周期性尖波" = CJD（不是 FTD）**
> 6. **GCA 黄金规则**：怀疑就 IV 类固醇，不等 biopsy（防失明）
> 7. **Cluster headache 急性首选 = 100% O₂ 12-15 L/min**（不是 Triptan）
> 
> ⭐ 加 USMLE 元技能 #5：**看到主线不要反射诊断 → 强制扫全 stem**

---

## 第五部分：未尽事项（明天接着学）

> [!todo] 本课件还未讲完的 Neuro topic（预期接下来）
> 
> - [ ] **卒中 (Stroke)**：MCA / ACA / PCA / 腔隙 / Wallenberg / Watershed / tPA
> - [ ] **癫痫 (Epilepsy)**：分类 / status epilepticus / 抗癫痫药
> - [ ] **运动障碍 (Movement disorders)**：PD / ET / Dystonia / Tic / Tourette
> - [ ] **MS / Demyelinating**：MS / NMO / ADEM
> - [ ] **神经肌肉 (Neuromuscular)**：MG / ALS / GBS / 周围神经病
> - [ ] **昏迷 / 意识障碍**：GCS / 脑死亡 / 谵妄
> - [ ] **CN palsies**：CN III/IV/VI/VII 各家鉴别
> - [ ] **儿童神经发育**

---

## 📋 文件结构总览（给 Peixuan 看的全景）

```
2026-05-12 Neuro HY200 学习产出
│
├── 错题层（个性化）
│   └── 错题详细 breakdown_v1.md
│       ├── 元学习反思 ⭐
│       ├── 错题 1: Pseudodementia
│       ├── 错题 2: CJD
│       ├── 错题 3: Syringomyelia + Horner
│       └── 错题 4: Leriche
│
├── 知识层（按器官/疾病重组）
│   └── 听课笔记草稿_v1.md
│       ├── 模块 1: 下肢血管缺血
│       ├── 模块 2: 脊髓不全损伤综合征
│       ├── 模块 3: 痴呆完整谱系（13 种）
│       ├── 模块 4: 头痛 5 大 + 5 进阶
│       └── 模块 5: 跨学科 Schema
│
├── 元层（跨学科通用）
│   └── 扫描算法 + Buzzword 训练手册_v1.md
│       ├── 扫描 4 步算法
│       ├── Day 1 痴呆（✅ 完整 + 交互卡）
│       ├── Day 3 头痛（✅ 完整 + 交互卡）
│       ├── Day 2/4-30（占位）
│       ├── 单题反思模板
│       ├── 周报模板
│       └── 附录：6 条元技能 + 错误模式
│
└── 总结层
    └── 今日总结 + Claude Code 指南_v1.md（本文件）
```

⭐ **层级关系**：元层 > 知识层 > 错题层 — 越上层越通用

---

**Last updated**: 2026-05-12 课程结束
**Next session**: 待定（明天继续 AMBOSS HY 200 Neuro 剩余内容）
**Status**: ✅ 完整闭环
