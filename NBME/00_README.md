# NBME 学习系统 — 最终交付包

> 共 7 个文件。其他迭代版本全部废弃。

---

## 📦 文件清单

| 文件名 | 用途 | 使用频率 |
|---|---|---|
| **00_README_上手指南.md** | 本文件，30 秒看懂系统 | 一次性看完 |
| **01_批量生成breakdown_prompt.md** | 提示词：让 AI 生成 5 个 NBME 文件 | 每套 NBME 用 1 次（**发给朋友**） |
| **02_截图识别填表_prompt.md** | 提示词：截图喂 AI 自动填做题结果 | 每套 NBME 用 4 次（分 Section） |
| **03_做题结果模板.md** | 模板：每套 NBME 用一份 | 由文件 01 自动生成，备用 |
| **04_单套学习Dashboard模板.md** | 模板：每套 NBME 复制一份 | 每套 NBME 复制 1 份 |
| **05_全局学习Dashboard.md** | 全局唯一，跨 8 套汇总 | 永久放 1 份 |
| **06_给朋友的任务说明书.md** | 给朋友看的工作指南 | **发给朋友** |
| **07_补充专题链接_prompt模板.md** | 4 个场景的链接维护 prompt | 建专题时按需用 |

---

## 🚀 一次性准备（5 分钟）

### Step 1：安装 Dataview 插件

Obsidian → 设置 → 第三方插件 → 浏览 → 搜 `Dataview` → 安装 → 启用 → 开 **Enable JavaScript Queries**

### Step 2：放置全局 Dashboard

把 `05_全局学习Dashboard.md` 放到 vault 的 `NBME/nbme-records/` 目录下，重命名为 `NBME_全局学习Dashboard.md`。**永久不动**。

---

## 📅 做一套 NBME 的完整流程（6 步）

### Step 1：生成 5 个详解文件（10 分钟）

把 `01_批量生成breakdown_prompt.md` 的内容 + NBME PDF 喂给 Claude Code。

它会输出 5 个文件：
```
NBME12_breakdown.md             ← 200 题详解
NBME12_套题索引.md
NBME12_学科索引.md
NBME12_考点索引.md
_做题结果_NBME12.md             ← 已预填 Q#/学科/主题/HY
```

入库：`NBME/nbme-records/NBME12/`

### Step 2：复制单套 Dashboard（30 秒）

`04_单套学习Dashboard模板.md` 复制到 `NBME12/` 文件夹，改名 `NBME12_学习Dashboard.md`。
打开改 frontmatter `nbme: 12`。

### Step 3：做题（模拟考试环境）

用 NBME Fighter 软件做完整 200 题。**做完后用 Fighter 的标记功能标出不确定的题**。

### Step 4：截图填表（阶段 1，10-15 分钟）

打开 NBME Fighter 题目分析页 → 滚动到 Q1-50 → 截图。

把 `02_截图识别填表_prompt.md` 里的**极简版 prompt** 复制：

```
这是 NBME 12 Section 1 截图（题号 1-50）。

请：
1. 读取 [[_做题结果_NBME12]] 的 Section 1 表格
2. 用截图更新 r/w 和 mk 列（小写 r/w/m，看到红旗就 m）
3. 保留学科、主题、HY、选、备注列原值
4. 输出完整 Section 1 表格（50 行 + 表头）
5. 最后报告：对X错X标记X未识别X

[贴截图]
```

发给 Claude Code → 输出 Section 1 完整表格 → 替换到 `_做题结果_NBME12.md` 对应位置。

**重复 4 次**（Section 1/2/3/4）。

### Step 5：复盘补关键题（阶段 2，20-30 分钟）

打开 `NBME12_学习Dashboard.md` → 看 3 类列表：
- ⚠️ **伪掌握**（最优先）
- 🔴 **干净错**
- 🟡 **标记错**

点击题号 → 跳到 `NBME12_breakdown.md` 对应 callout → 看解析。

回到 `_做题结果_NBME12.md` 补关键题的 `选` 和 `备注` 列：
```
| 12 | 心内 | PPCM | 4 | w | m | C | 时间窗搞反 |
```

在 breakdown callout 末尾追加你的复盘（**每行加 `>` 保持在 callout 内**）：
```markdown
> 
> ---
> 
> ### 🤯 我的复盘（2026-05-15）
> 
> **我选了**：C
> **我的思路**：[一句话还原]
> **根本错因**：把时间窗搞反
> 
> ### ✏️ 复盘行动
> - [ ] 1 周后重做
> - [ ] 去「心内」主笔记加「薄弱点」标签（或对应章节加标记）
```

### Step 6：跑复盘 prompt 生成报告（10 分钟）

复制 `NBME12_学习Dashboard.md` 底部的复盘 prompt → 给 Claude Code → 生成 `NBME12_复盘报告.md`。

---

## 🔄 二刷（错题 + 标记题）

```bash
copy _做题结果_NBME12.md _做题结果_NBME12_R2.md
```

打开新文件：
1. frontmatter 改 `round: 2`
2. 清空 `r/w` `mk` `选` `备注` 4 列
3. 学科/主题/HY 保留
4. 只填你计划二刷的题（一般是一刷的 wrong + marked）

全局 Dashboard 自动识别两次刷的数据。

---

## 🎯 4 种题目状态（系统核心）

| 你做的 | r/w | mk | 状态 | 复盘优先级 |
|---|---|---|---|---|
| 答对 + 没标记 | r | （空） | 🟢 干净对 | 低 |
| 答对 + 有标记 | r | m | ⚠️ **伪掌握** | 🔴 **最高** |
| 答错 + 有标记 | w | m | 🟡 标记错 | 🟡 中 |
| 答错 + 没标记 | w | （空） | 🔴 干净错 | 🔴 高 |

⚠️ **伪掌握是真考试翻车高危区**——你蒙对了但不踏实，比错题还危险。

---

## 📁 vault 最终目录结构

```
NBME/nbme-records/
├── NBME_全局学习Dashboard.md          ← 全局唯一
├── NBME09/
│   ├── NBME09_breakdown.md             ← Step 1 生成
│   ├── NBME09_套题索引.md              ← Step 1 生成
│   ├── NBME09_学科索引.md              ← Step 1 生成
│   ├── NBME09_考点索引.md              ← Step 1 生成
│   ├── _做题结果_NBME09.md             ← Step 1 生成 + Step 4 填
│   └── NBME09_学习Dashboard.md         ← Step 2 复制
├── NBME10/...
└── ...
```

每套 NBME 6 个文件，全部自动联动（Dataview）。

---

## ⚠️ 常见问题速查

**Q：Dataview 没显示数据？**
A：检查 (1) JS Queries 开了 (2) Section 标题格式 `## Section 1（Item 1-50）` (3) r/w/m 是小写英文 (4) Ctrl+P → "Dataview: Force refresh all"

**Q：breakdown 里的内容能改吗？**
A：完全能改。直接编辑 callout 内文本（保持每行 `>` 前缀）。追加复盘用 `### 🤯 我的复盘` 区块分隔。

**Q：学科填错了怎么办？**
A：在做题结果文件直接改"学科"列单元格。学科名要与 22 个 vault 白名单一致（见文件 01）。

**Q：跨学科题怎么填？**
A：在学科列填 `主学科/副学科`，如 `GI/外科`。

---

## 🎓 我建议的实战起步顺序

1. **今天**：完成"一次性准备"（5 分钟）
2. **今天**：用文件 01 给 NBME 12（或其他套）跑一次 5 文件生成（10 分钟）
3. **今天**：在 Obsidian 里打开生成的文件，验证 Dataview 渲染正常
4. **明天**：模拟做 NBME 12，做完用文件 02 填表
5. **后天**：复盘、补 my_choice/my_note、跑复盘 prompt
6. **如果一切顺利**：批量做 NBME 9-16
7. **3 个月后**：二刷错题+标记题

---

## 🆘 卡壳了？

把以下信息告诉我，我精准帮你：
1. 你卡在第几步
2. 截图错误信息或异常渲染
3. 错误的文件名

**所有迭代版本里只有这 5 个文件是最终版**。其他历史版本可以全部删除。
