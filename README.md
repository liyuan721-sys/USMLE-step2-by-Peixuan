# USMLE Step 2 学习笔记

> Peixuan 的 USMLE Step 2 CK 备考知识库
> 按 UWorld 系统分类组织，配合 NBME 模考与错题回顾

---

## 1. 这个项目是什么

这是一份基于 **Obsidian + Git** 的个人备考知识库，用于：

- 📚 **系统笔记**：按 UWorld Step 2 CK 的 20 个学科系统组织复习要点
- 📝 **错题整理**：UWorld 做题后用模板化流程消化吸收，带病机可视化
- 📊 **模考记录**：NBME / UWSA 成绩与错题分析
- 🔗 **资源汇总**：教材、视频、题库的索引

所有内容用 **Markdown** 写作，纯文本、终生可读、版本可追溯。

---

## 2. 文件夹结构

```
USMLE-step2-by-Peixuan/
├── README.md                       # 本文件
├── resources.md                    # 学习资源汇总
├── .gitignore                      # 忽略 .obsidian/ .claude/ 图片 PDF
│
├── notes/                          # 系统笔记 (按 UWorld 分类)
│   ├── allergy-immunology.md       # 过敏与免疫
│   ├── biostatistics.md            # 生物统计与流行病学
│   ├── cardiovascular.md           # 心血管
│   ├── dermatology.md              # 皮肤
│   ├── endocrine.md                # 内分泌、糖尿病与代谢
│   ├── ent.md                      # 耳鼻喉
│   ├── female-reproductive.md      # 女性生殖与乳腺
│   ├── gastrointestinal.md         # 消化与营养
│   ├── hematology-oncology.md      # 血液与肿瘤
│   ├── infectious-diseases.md      # 感染病
│   ├── male-reproductive.md        # 男性生殖
│   ├── nervous-system.md           # 神经
│   ├── ophthalmology.md            # 眼科
│   ├── poisoning-environmental.md  # 中毒与环境
│   ├── pregnancy.md                # 妊娠、分娩与产褥
│   ├── psychiatric.md              # 精神与物质使用
│   ├── pulmonary.md                # 呼吸与重症
│   ├── renal-urinary.md            # 肾脏、泌尿与电解质
│   ├── rheumatology-orthopedics.md # 风湿、骨科与运动
│   └── social-sciences.md          # 伦理、沟通与患者安全
│
├── mistakes/                       # UWorld 错题整理
│   ├── README.md                   # 错题工作流说明 + 提示词模板
│   ├── _template.md                # 单题错题模板（病机+鉴别+决策图）
│   ├── _weekly_review_template.md  # 周总结模板
│   ├── YYYY-MM-DD.md               # 每日错题记录（按需创建）
│   ├── weekly-YYYY-Www.md          # 周总结（按 ISO 周）
│   └── uworld-mistakes_2026-05.md          # 旧版索引（历史归档）
│
└── NBME/                           # NBME 模考记录
    └── nbme-records.md
```

**单文件结构约定**（每个 `notes/*.md`）：

```markdown
# 系统名称 (英文) 笔记

> UWorld Step 2 CK · 高频考点大纲

## 1. 疾病分类一
- 高频考点
- 鉴别诊断要点
- 经典治疗

## 2. 疾病分类二
...

---
**关联资源**：UWorld、AMBOSS、Pathoma 等
```

---

## 3. 用 Claude Code 添加新笔记

本仓库已配置好供 Claude Code 协作编辑。常用对话模板如下：

### 3.1 展开某个章节

> "把 `notes/cardiovascular.md` 第 1 节 *缺血性心脏病* 展开成详细笔记，包含临床表现、ECG、酶谱、药物。"

### 3.2 录入错题

> "我做错了 UW#12345，[一句话题型]，帮我用 mistakes/_template.md 套个错题笔记。"

详见 [§4 错题处理工作流](#4--错题处理工作流) 与 [`mistakes/README.md`](./mistakes/README.md)。

### 3.3 录入 NBME 模考

> "NBME Form 10 我得了 235，错了 X 题，请把成绩和错题分类记录到 `NBME/nbme-records.md`。"

### 3.4 新建一个学科外的专题笔记

> "在 `notes/` 下新建 `pharmacology-cheatsheet.md`，做一份高频药物速查表。"

### 3.5 复习提问

> "请基于 `notes/endocrine.md` 出 5 道 NBME 风格的选择题考我。"

**写作风格约定**（已存入 Claude Code 记忆，自动遵循）：

- 中文为主，医学术语保留英文（如 STEMI、HFrEF、SIADH）
- 偏好「疾病分类 → bullet 高频考点」的大纲结构
- 不写冗长段落

---

## 4. 📝 错题处理工作流

错题是 USMLE 备考的核心引擎。本仓库提供一套 **模板化、自动化、版权合规** 的错题处理流程。

### 4.1 三个核心文件

| 文件 | 用途 |
|------|------|
| [`mistakes/_template.md`](./mistakes/_template.md) | 单道错题的标准格式（含病机、鉴别表、决策图、复习提醒） |
| [`mistakes/_weekly_review_template.md`](./mistakes/_weekly_review_template.md) | 每周错题统计与反思总结 |
| [`mistakes/README.md`](./mistakes/README.md) | 完整使用指南 + 3 个提示词模板 + ⚠️ 版权说明 |

### 4.2 日常错题流程

**📅 每日做题后** — 把错题用一句话提炼后告诉 Claude Code，配合 [`mistakes/README.md`](./mistakes/README.md) 里的提示词：

| 题型 | 用哪个模板 |
|------|-----------|
| 纯文字题 | **模板 A** |
| 含 ECG / 影像 / 病理图的题 | **模板 B** |

Claude 会基于 First Aid / Master the Boards / UpToDate / AMBOSS 等通用医学知识 **重新整合** 病机、鉴别表、决策图，写入 `mistakes/YYYY-MM-DD.md`。

**📊 每周末** — 用 **模板 C** 让 Claude 扫描本周错题文件，套用周总结模板生成统计 + 反思 + 下周复习清单。

### 4.3 ⚠️ 版权合规底线（必读）

- ❌ **不要**直接复制 UWorld 题干、解析、原图、原表格到笔记里
- ✅ Claude Code 基于 **First Aid / Master the Boards / UpToDate / AMBOSS** 等公开教科书 **重新整合** 病理生理与流程图
- ✅ 你的笔记应该是 **"消化后的知识"**，不是 "UW 内容存档"
- ✅ 这种 **"通用医学知识可视化"** 既能帮你深入理解，又完全合法
- 🔒 `.gitignore` 已自动忽略 `*.png/jpg/pdf`，防止误推 UW 截图

完整说明见 [`mistakes/README.md`](./mistakes/README.md)。

---

## 5. 用 Obsidian 打开这个 Vault

[Obsidian](https://obsidian.md/) 是免费的 Markdown 双链笔记工具，对这种学科笔记非常友好。

### 5.1 首次打开

1. 下载安装 [Obsidian](https://obsidian.md/download)
2. 启动后选择 **"Open folder as vault"**
3. 选中本仓库根目录 `C:\Users\liyua\Desktop\USMLE-step2-by-Peixuan`
4. 完成 — Obsidian 会在 `.obsidian/` 写入它的工作区配置（已被 `.gitignore` 忽略）

### 5.2 推荐插件

- **Outline** (内置)：右侧大纲跳章节
- **Tag pane** (内置)：用 `#cardio #high-yield` 等标签筛选
- **Templates** (内置)：把 `mistakes/_template.md` 设为模板，新建笔记一键套用
- **Dataview** (社区插件)：把所有错题按系统、错因、复习日期排序成表格
- **Excalidraw** (社区插件)：画机制图、鉴别流程图
- **Mermaid 内置渲染**：错题模板里的 `mermaid` 流程图与饼图自动可视化

### 5.3 常用快捷键

| 操作 | 快捷键 |
|---|---|
| 快速打开文件 | `Ctrl + O` |
| 全局搜索 | `Ctrl + Shift + F` |
| 命令面板 | `Ctrl + P` |
| 切换编辑/预览 | `Ctrl + E` |
| 双链跳转 | `[[文件名]]` |

### 5.4 双链用法（推荐）

错题文件双向链到知识点：

```markdown
错题：心包填塞 → [[cardiovascular#6. 心包疾病]]
```

知识点反向链回错题：

```markdown
**易错点**：ACS vs dissection → [[mistakes/2026-05-09]]
```

点击即可跳转。

---

## 6. Commit 与推送到 GitHub

### 6.1 仓库地址

`git@github.com:liyuan721-sys/USMLE-step2-by-Peixuan.git`

主分支：`main`

### 6.2 日常工作流（PowerShell）

```powershell
# 查看改动
git status

# 查看具体修改
git diff

# 添加单个文件
git add notes/cardiovascular.md

# 或添加所有改动 (注意：.gitignore 已排除 .obsidian/ .claude/ 图片 PDF)
git add .

# 提交（Windows PowerShell 单行写法）
git commit -m "更新心血管笔记：补充 ACS 处理时间窗"

# 推送
git push origin main
```

### 6.3 提交信息建议

| 场景 | 示例 |
|---|---|
| 新建笔记 | `新增 notes/pharmacology-cheatsheet.md` |
| 扩充内容 | `扩充心血管笔记：缺血性心脏病` |
| 错题整理 | `录入 UWorld block 12 错题` |
| 周总结 | `添加 weekly-2026-W19 周总结` |
| 模考记录 | `添加 NBME Form 10 模考记录` |
| 修正 | `修正肾内电解质章节钠紊乱处理` |

### 6.4 让 Claude Code 帮你 commit

直接说：

> "帮我把 notes/ 下的改动 commit 并推送到 GitHub，commit message 用 '扩充心血管笔记'"

Claude 会自动执行 `git status → git add → git commit → git push`，并在每一步报告结果。

### 6.5 多机同步

如果在另一台机器克隆：

```powershell
git clone git@github.com:liyuan721-sys/USMLE-step2-by-Peixuan.git
```

每次开始工作前先拉取：

```powershell
git pull origin main
```

避免冲突。

### 6.6 常见问题

- **冲突 (merge conflict)**：让 Claude Code 帮你解决，告诉它 "解决 git merge conflict"
- **误删文件**：`git checkout HEAD -- 文件路径` 还原
- **想撤销最后一次 commit (未推送)**：`git reset --soft HEAD~1`
- **`.obsidian/` 出现在 `git status`**：检查 `.gitignore` 是否在仓库根目录
- **不小心把 UW 原文 commit 了**：推送前用 `git reset --soft HEAD~1` 撤销；已推送的话让 Claude 协助处理

---

## 备考资源参考

详见 [`resources.md`](./resources.md)。

核心组合：**UWorld + First Aid + Master the Boards + AMBOSS + NBME**

---

🤖 本仓库由 Claude Code 协助维护
