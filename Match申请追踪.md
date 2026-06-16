---
tags:
  - USMLE-Step2
  - Match申请
  - ECFMG
created: 2026-06-05
type: 申请追踪
---

# Match 申请追踪 — ECFMG → FSMB → Prometric

> [!info] 这张卡管什么
> Step 2 CK **报考链路**的分步追踪：做完一步勾一步。
> 核心顺序见 [[复习入口_Dashboard]] §「考前 10 周计划 / OET+ECFMG 平行线」。
> **关键认知**：报考 Step 2 只需「**认证资格 eligibility**」（ECFMG 申请状态到 Accepted/Pending），**不是 full certification**。

---

## 关键状态速览（随时回填）

| 项目 | 状态 | 日期 / 编号 |
|---|---|---|
| ECFMG / USMLE ID | 已有 ✓ | |
| MyIntealth ID | 已有 ✓ | **601079276** |
| ECFMG 认证申请状态 | 填写中 | |
| EPIC 学历核验 | ⚠️ 成绩单认证**被驳回**（待 ECFMG 答复）| Case C-25971872 / 2026-06-15 |
| FSMB Step 2 报考 | 未开始 | |
| Eligibility 窗（须含 8/20） | — | |
| Scheduling permit | — | |
| Prometric 考位 | — | |
| 目标考期 | 暂定 2026-08-18~20 | |

> [!danger] 三条贯穿全程的红线
> 1. **姓名**：ECFMG / FSMB / Prometric / 护照 / ERAS **五处完全一致**，一字不差（名字不符 = 最常见延误 + 考场被拒）
> 2. **顺序不能反**：认证资格(eligibility) → FSMB 报考 → Prometric。认证(certification) 是终点，CK 过了才拼齐
> 3. **eligibility 窗必须把 8/20 包进去且留 buffer**，窗卡太窄后面改期会被锁死

---

## Phase 0 — 前置确认

- [x] 已有 **ECFMG/USMLE ID**（考过 Step 1 → 已有）
- [x] **Step 1 已通过** ✓（认证资格科目前提，只差 Step 2）

---

## Phase 1 — ECFMG 认证申请（MyIntealth）→ 拿到 eligibility ⏳进行中

> [!tip] 这一步的目的
> 不是"拿认证"，是把申请状态推到 **Accepted / Pending Credential Verification** —— 到了这个状态就能去 FSMB 报考。

- [ ] 登录 **MyIntealth**，开启「Application for ECFMG Certification」
- [ ] **姓名**与护照/政府 ID **完全一致**（对照红线 1 核三遍）
- [ ] **选对医学院**：World Directory 里带 **ECFMG sponsor note** 的那条，别选错同名校
- [ ] 完成 **Form 186（Certification of Identification Form）**：贴照片 + 按要求公证/认证
- [ ] **交认证申请费**（没交不进处理）
- [ ] 提交申请
- [ ] **回填状态**：等状态变 **Accepted / Pending Credential Verification**（有人工核验，留几天~1~2 周）
- [ ] ✅ 里程碑：状态到位 = **可以去 FSMB 报考**

并行（不卡本 Phase）：

- [ ] **EPIC 学历核验**继续跑（认证用，不影响报考 Step 2）

> [!danger] EPIC 进展 — 2026-06-15-16（待处理 ⏳）
> **① 成绩单认证被驳回（Credential Verification – CV Rejected）**
> - Case **C-25971872**（Final Medical School Transcript, West China School of Medicine / Sichuan University, Graduation Year 2005）；Parent Case **C-25901694**
> - 时间线：2024-02-13 建案 → 2025-09-23 送学校核验 → 学校压 ~9 个月 → **2026-06-15 晚 CV Rejected**
> - **问题**：portal 未给驳回原因（External Instructions 空 / Action Needed = No / 无 pending action）→ 自相矛盾，界面查不到 why
> - **下一步**：已发 inquiry（Help → Contact us），等真人回复；客服自动回执提示"CS 看不到 portal 外更多细节"→ 若只回套话需升级追问 specific reason + 补救步骤
> - **盯**：这几天每天看 **My Cases** —— 关注 C-25971872 / C-25901694 状态变化、Action Needed 翻 Yes、External Instructions 出现文字、或冒出新子 case
>
> **② Final Medical Diploma 上传一直报错（与①是两件事）**
> - 报错：Azure `AuthenticationFailed – Signature did not match`
> - 根因：**ECFMG 签发上传令牌（SAS）的服务器时钟快约 60 秒**（每次精确差 60s）；本机时钟实测仅差 0.65s（准）→ 非用户问题，是 ECFMG 服务端
> - **下一步**：别连续猛试；错峰（美西白天）重登重传；持续失败拿 RequestId 一并报 ECFMG

---

## Phase 2 — FSMB 报考 Step 2 CK（usmle.fsmb.org）

> [!warning] 入口变了
> IMG 的 USMLE 报考 **2024 起从 ECFMG 转到 FSMB**（`usmle.fsmb.org`）。FSMB 后台自动核你的 ECFMG eligibility。

- [ ] 在 **FSMB 门户**注册账号 / 登录
- [ ] 申请 **Step 2 CK**
- [ ] **选 3 个月 eligibility 窗**：必须覆盖 **8/20**，且前后留 buffer（对照红线 3）
- [ ] **交考试费**
- [ ] FSMB 核验 ECFMG eligibility → 通过
- [ ] **收到 scheduling permit**（回填日期）
- [ ] ✅ 里程碑：拿到 permit = **可以约 Prometric**

---

## Phase 3 — Prometric 约考

- [ ] 用 **permit** 上的信息登录 Prometric 约位
- [ ] **约到 8/20 前后**的考位（确认考点城市 / 地址 / 是否要早起远途）
- [ ] 确认考位日期**落在 eligibility 窗内**
- [ ] **越早约越好**：8 月热门点位会满，先锁位再说
- [ ] 保存 / 打印**预约确认**
- [ ] 记下 **reschedule 政策**（提前多久可免费改期 / 改期费）
- [ ] ✅ 里程碑：考位确认 = **报考完成** 🎉

---

## 后续平行线（另见 Dashboard，本卡不展开）

- [ ] **OET**：7 月考（先裸做 1 套模拟定要不要练）→ 占晚上练 Writing 信 + Speaking role-play
- [ ] **EPIC**：完成后推进 ECFMG 认证最终核验
- [ ] **ERAS**：9/2-3 提交（提交时认证 in progress 是常态）

---

## 关联

- 总时间线 / Go-No-Go → [[复习入口_Dashboard]]
- OET 复习怎么不影响 CK → Dashboard §平行线
