---
tags:
  - USMLE-Step2
  - 心血管
  - 专题笔记
created: 2026-05-18
type: 专题笔记
source: 2026-05-18 Claude.ai 草稿 v1 整合（Q15973 触发）
---

# Beta Blockers 分类大全（β-Blockers Complete Classification）

> [!info] 笔记定位
> 这是 BB 章节的**根基笔记**。所有 BB 相关错题、临床决策、副作用陷阱都从这里展开。
> **跨学科引用**：心内 / 内分泌（甲亢、嗜铬、DM）/ 产科（孕期 HTN）/ 神经（migraine 预防、表演焦虑）/ 消化（门脉高压）/ 眼科（青光眼）。
>
> **触发错题**：[[mistakes/uworld-mistakes#^Q15973]]（Conventional BB → weight gain + glucose intolerance）
>
> **姐妹专题**：[[完整笔记/专题笔记/心内_降压药副作用速查]]（HTN 药物广覆盖 — 5+2 类降压药矩阵）；本笔记是 **BB-specific 深度**。

---

## 目录

- [[#零、认知升级：从"一维"到"二维"分类 ⭐ 必读|零、认知升级 一维→二维]]
- [[#一、三大分类维度（完整版）|一、三大分类维度]]
- [[#二、维度 1：选择性（β1 vs Non-selective）|二、维度 1 选择性]]
- [[#三、维度 2：血管效应（Conventional vs Vasodilatory）⭐|三、维度 2 血管效应]]
- [[#四、机制深度 — 为什么 Vasodilatory BB 代谢友好？|四、机制深度]]
- [[#五、四象限药物完整图谱 ⭐|五、四象限药物图谱]]
- [[#六、临床应用矩阵 ⭐|六、临床应用矩阵]]
- [[#七、HFrEF "三剑客" BMC 必背 ⭐|七、HFrEF 三剑客 BMC]]
- [[#八、反直觉高频陷阱 ⭐|八、反直觉陷阱 6 个]]
- [[#九、副作用全谱|九、副作用全谱]]
- [[#十、Memory Hook ⭐|十、Memory Hook]]
- [[#十一、自测题（盲做）|十一、自测题]]
- [[#关联|关联]]

---

## 零、认知升级：从"一维"到"二维"分类 ⭐ 必读

## 0.1 你可能熟悉的旧分类（一维）

```
Beta Blockers
        ↓
   ┌────┴────┐
   ↓         ↓
β1 选择性   Non-selective
(metoprolol) (propranolol)
```

旧分类**没错**，但**不完整**。它解释不了：
- 为什么 Carvedilol（non-selective）反而比 Metoprolol（β1 选择性）代谢更友好？
- 为什么 HF + DM 不选 β1 选择性的 metoprolol，而选 non-selective 的 carvedilol？

## 0.2 升级到完整分类（二维矩阵）

```
                    维度 1：选择性
                    ─────────────────
                    β1 选择性       Non-selective
                    (只封 β1)       (封 β1+β2)
维度 2：           ─────────────────────────────────
血管效应
─────────
Conventional        Metoprolol      Propranolol
(不舒张血管)         Atenolol        Nadolol
                    Bisoprolol      Timolol
                    Esmolol

Vasodilatory        Nebivolol       Carvedilol
(舒张血管)          (NO 释放)        Labetalol
                                    (+ α1 阻断)
```

> [!success] 核心顿悟
> **"选择性"和"血管效应"是两个独立维度，不是一条线上的对立！**
>
> 一个 BB 可以同时是：
> - β1 选择性 **+** Conventional（如 Metoprolol）
> - β1 选择性 **+** Vasodilatory（如 Nebivolol）
> - Non-selective **+** Conventional（如 Propranolol）
> - Non-selective **+** Vasodilatory（如 Carvedilol / Labetalol）

## 0.3 三句话整合 ⭐

> [!tip] 二维分类的核心
>
> 1. **选择性 = "封不封 β2"**（横轴）
> 2. **血管效应 = "封不封 α1（或释不释放 NO）"**（纵轴）
> 3. **代谢副作用的真凶 = "β2 被封 + α1 没人封"**（孤军作战的 α1）
>
> 解药 = **把 α1 也封了**（carvedilol/labetalol）**或** **干脆别封 β2**（β1 选择性）
>
> 最差组合 = **封 β2 + 不封 α1**（propranolol = 元凶）
> 最优组合 = **封 β2 + 封 α1**（carvedilol = 神药）

## 0.4 为什么旧分类停留在一维？

> [!info] 教科书的历史包袱
> 大部分中文药理教材停留在"选择性 vs non-selective"是因为：
> - 这是**最早**的 BB 分类（1960s-70s）
> - Carvedilol（1995）和 Nebivolol（2007）是**后期药物**，没及时更新进基础教材
> - USMLE 考的是**临床应用 + 现代证据**，所以必须用 2 维分类
>
> 旧分类不是错，是**不完整**。补上"血管效应"这第二个维度就够用了。

---

# 一、三大分类维度（完整版）

```
Beta Blockers 分类
─────────────────────────────────────
        ↓               ↓              ↓
   维度 1：选择性    维度 2：血管效应   维度 3：ISA
   (Selectivity)   (Vasodilatory?)   (内在拟交感活性)
        ↓               ↓              ↓
   β1 选择性 vs       有 / 无          有 / 无
   non-selective    α1 阻断或 NO 释放  (基本不考)
```

考试 90% 考前两个维度。ISA（pindolol, acebutolol 有 ISA）几乎不考。

---

## 二、维度 1：选择性（β1 vs Non-selective）

### 2.1 受体定位回顾

```
β1 受体（主要在心脏）
─────────────────────
   位置：心肌、肾脏 JG 细胞
   阻断后：心率↓、收缩力↓、肾素↓


β2 受体（主要在心脏外）
─────────────────────
   位置：支气管平滑肌、骨骼肌血管、
        肝脏（糖原分解）、胰腺
   阻断后：支气管收缩、肌肉血流↓、
          糖原分解↓、胰岛素分泌变化
```

### 2.2 分类对照

| 类型 | 阻断什么 | 代表药 | 安全谱 |
|---|---|---|---|
| **β1 选择性**（cardioselective）| 主要 β1 | Metoprolol, Atenolol, Bisoprolol, Esmolol | 哮喘、COPD、DM 相对安全 |
| **Non-selective**（β1 + β2）| β1 + β2 | Propranolol, Nadolol, Timolol | 哮喘禁忌、DM 慎用、PVD 慎用 |

> [!tip] β1 选择性口诀 — "A BEAM"
> **字母 A–M 开头 ≈ β1 选择性**：
> - **A**tenolol / **A**cebutolol
> - **B**isoprolol / **B**etaxolol
> - **E**smolol
> - **M**etoprolol
>
> **字母 N–Z 开头 ≈ Non-selective**：
> - **N**adolol / **P**ropranolol / **P**indolol / **S**otalol / **T**imolol
>
> 例外：**C**arvedilol 和 **L**abetalol = non-selective + α1（见维度 2）

---

## 三、维度 2：血管效应（Conventional vs Vasodilatory）⭐

### 3.1 核心区别

```
Conventional BB（传统 BB）
─────────────────────────────
   只阻断 β1（或 β1+β2）
   不直接作用于血管
        ↓
   血管效应：无 / 收缩（α1 失对抗）
   TPR：↑ 或不变
   代谢副作用：恶化


Vasodilatory BB（血管舒张型 BB）
─────────────────────────────
   阻断 β + 额外的血管舒张机制
        ↓
   ┌─────────────┬──────────────┐
   ↓             ↓              ↓
 α1 阻断       NO 释放        β3 激动
 (carvedilol,  (nebivolol)    (nebivolol)
  labetalol)
        ↓
   血管效应：舒张（后负荷↓）
   TPR：↓
   代谢副作用：中性 / 改善
```

### 3.2 主要药物完整受体图谱

| 药物 | β1 | β2 | α1 | 其他 | 类别 | 特点 |
|---|---|---|---|---|---|---|
| Metoprolol | ✅ | ❌ | ❌ | — | Conventional | β1 选择性 |
| Atenolol | ✅ | ❌ | ❌ | — | Conventional | β1 选择性，**亲水**（不入脑）|
| Bisoprolol | ✅ | ❌ | ❌ | — | Conventional | β1 选择性最强，HFrEF 三剑客 |
| Esmolol | ✅ | ❌ | ❌ | — | Conventional | **超短效**（t½ 9 min），ICU 静脉 |
| Propranolol | ✅ | ✅ | ❌ | — | Conventional | Non-selective，**亲脂**（入脑）|
| Nadolol | ✅ | ✅ | ❌ | — | Conventional | Non-selective，长效 |
| Timolol | ✅ | ✅ | ❌ | — | Conventional | 青光眼局部 |
| **Carvedilol** | ✅ | ✅ | **✅** | 抗氧化 | **Vasodilatory** | HFrEF + DM 首选 |
| **Labetalol** | ✅ | ✅ | **✅** | — | **Vasodilatory** | **孕期 / HTN 急症首选** |
| **Nebivolol** | ✅ | ❌ | ❌ | **NO 释放** | **Vasodilatory** | β1 选择性 + NO，老年 HTN |

---

## 四、机制深度 — 为什么 Vasodilatory BB 代谢友好？

```
Conventional BB（metoprolol / propranolol）
──────────────────────────────────────────
   阻断 β1 ± β2
        ↓
   骨骼肌：β2 封（如果 non-selective）
          α1 失去对抗
        ↓
   骨骼肌血管收缩 → 血流↓ → 葡萄糖摄取↓
        ↓
   ⚠️ 胰岛素抵抗 + 体重↑ + 糖耐量↓
   ⚠️ TPR ↑


Vasodilatory BB（carvedilol / labetalol / nebivolol）
──────────────────────────────────────────
   阻断 β1 + β2 + 额外舒张机制
        ↓
   ┌─────────────────────┐
   ↓                     ↓
 β2 封导致的            α1 也被封
 血管收缩倾向    ←抵消→  或 NO 释放
        ↓
   净效果：血管舒张
        ↓
   骨骼肌血流↑ → 葡萄糖摄取↑ → 胰岛素敏感↑
        ↓
   ✅ 代谢中性 / 改善
   ✅ TPR ↓（后负荷↓，HF 患者获益）
```

> [!success] 一句话总结
> Vasodilatory BB = "封了 α1 让肌肉吃饭" 或 "释放 NO 让血管放松"
> → 这就是它们代谢友好 + HF 友好的根本原因。

---

## 五、四象限药物完整图谱 ⭐

| 药物 | 选择性 | 血管效应 | 代谢副作用 | 代表用法 |
|---|---|---|---|---|
| **Metoprolol** | β1 | Conventional | 轻度恶化 | 心绞痛、HFrEF（succinate）|
| **Atenolol** | β1 | Conventional | 轻度恶化 | 心绞痛（老年慎用）|
| **Bisoprolol** | β1（最强）| Conventional | 轻度恶化 | HFrEF |
| **Esmolol** | β1 | Conventional | — | ICU 急性房颤 / 主动脉夹层 |
| **Propranolol** | Non-selective | Conventional | **最严重** ⚠️ | 甲亢、migraine、门脉高压 |
| **Nadolol** | Non-selective | Conventional | 严重 | 门脉高压 |
| **Timolol** | Non-selective | Conventional | 严重（局部不影响）| 青光眼 |
| **Carvedilol** | Non-selective | **Vasodilatory** ⭐ | **中性 / 改善** | HFrEF + DM、HFrEF + HTN |
| **Labetalol** | Non-selective | **Vasodilatory** ⭐ | 中性 | 孕期、HTN 急症 |
| **Nebivolol** | β1 | **Vasodilatory** ⭐ | **改善**（NO）| 老年 HTN |

---

# 六、临床应用矩阵 ⭐
#难记

| 临床情境 | 首选 BB | 为什么 | 避免 |
|---|---|---|---|
| **HFrEF** | Carvedilol / Metoprolol succinate / Bisoprolol | 唯一证明降死亡率的三个 | 其他 BB（atenolol, propranolol 等）|
| **HFrEF + DM** | **Carvedilol** ⭐ | α1 阻断改善代谢 | Metoprolol（次选）|
| **HFrEF + 哮喘 / COPD** | Bisoprolol / Metoprolol succinate | β1 选择性 | Carvedilol（β2 阻断）|
| **HTN + DM**（无强适应症）| **不用 BB** | BB 恶化代谢 | Conventional BB |
| **HTN + 孕期** | **Labetalol** ⭐ | 安全 + vasodilatory | ACEI/ARB（致畸）|
| **高血压急症 / preeclampsia** | **Labetalol IV** | 起效快、可控 | — |
| **心梗后二级预防** | Metoprolol succinate / Carvedilol | 降死亡率 | Atenolol（证据弱）|
| **稳定型心绞痛** | Metoprolol / Atenolol | 降心肌耗氧 | — |
| **房颤控制心率** | Metoprolol / Esmolol（急）| 降 AV 传导 | — |
| **甲亢症状控制** | **Propranolol** ⭐ | non-selective + 抑制 T4→T3 | β1 选择性 |
| **表演焦虑 / 震颤** | **Propranolol** | 亲脂入脑 | β1 选择性 |
| **Migraine 预防** | Propranolol / Metoprolol / Timolol | 经典适应症 | — |
| **门脉高压预防出血** | **Propranolol / Nadolol** ⭐ | **必须 non-selective**（缩内脏血管）| β1 选择性（无效）|
| **青光眼**（眼局部）| **Timolol** | 减少房水生成 | — |
| **嗜铬细胞瘤** | **先 α 后 β** | 单独用 BB 会致 HTN 危象 | 先用 BB |

---

## 七、HFrEF "三剑客" BMC 必背 ⭐

> [!danger] HFrEF 降死亡率的 BB 只有 3 个
> - **B**isoprolol（比索洛尔）
> - **M**etoprolol succinate（琥珀酸美托洛尔，**长效**，Toprol-XL）
> - **C**arvedilol（卡维地洛）
>
> ⚠️ **Metoprolol tartrate**（酒石酸，短效）**不算**！HF 必须 succinate。
> ⚠️ Atenolol、propranolol **不用于 HFrEF**。
>
> UW 陷阱：HF 患者用 metoprolol tartrate → 应换 succinate。

### Carvedilol vs Metoprolol succinate（HF + DM 选哪个？）

| 指标 | Metoprolol succinate | Carvedilol |
|---|---|---|
| HbA1c | ↑（恶化）| ↓ 或不变 |
| 胰岛素敏感性 | ↓ | ↑（改善）|
| 新发 T2DM | ↑ | ↓ |
| 微量白蛋白尿 | 不变 | ↓（肾保护）|
| LDL / TG | 轻度恶化 | 中性 / 改善 |
| 体重 | ↑ | 中性 |
| HF 死亡率 | 同等降低 | 同等降低 |

**结论**：HF + DM → **Carvedilol**；HF + 哮喘/COPD → **Bisoprolol** 或 **Metoprolol succ**。

---

## 八、反直觉高频陷阱 ⭐

### 7.1 门脉高压必须 Non-selective

> [!warning] 门脉高压 = Propranolol / Nadolol
> 食道静脉曲张预防出血需要 **β2 阻断**来缩内脏血管 → 降门脉压。
> **β1 选择性药（metoprolol）无效**。
> UW 陷阱：肝硬化用 metoprolol → 错，换 propranolol。

### 7.2 甲亢必须 Propranolol

> [!warning] 甲亢风暴 = Propranolol
> 不只是 non-selective，还**抑制外周 T4 → T3 转化**（独家优势）。

### 7.3 孕期 = Labetalol（不是 Carvedilol）

> [!warning] 孕期记 Labetalol
> 虽然两者都 non-selective + α1，但**孕期数据 Labetalol 最全**。
> 孕期一线 HTN：**Labetalol > Methyldopa > Nifedipine**
> 记法：**"妈妈生宝宝靠 LMN"**

### 7.4 嗜铬细胞瘤先 α 后 β

> [!warning] Pheochromocytoma 用药顺序
> 必须**先 phenoxybenzamine（α 阻断）→ 再 BB**。
> 单独用 BB → β2 失对抗 → α 介导血管收缩 → **HTN 危象**。

### 7.5 Atenolol 老年 HTN 不推荐

> [!info] 冷门考点
> Atenolol 在老年单纯 HTN 降中风获益弱于其他药。
> 老年 HTN 一线：ACEI/ARB / CCB / Thiazide。

### 7.6 BB 不能突然停药

> [!danger] BB 撤药综合征
> 长期用 BB 后骤停 → 受体上调反弹 → **HTN 危象 / 心梗 / 心绞痛恶化**。
> 必须**逐渐减量**（2-4 周）。

---

## 九、副作用全谱

### 8.1 Conventional BB

| 系统 | 副作用 | 机制 |
|---|---|---|
| 心血管 | Bradycardia、AV block、HF 加重（急性期）、低血压 | β1 阻断 |
| 呼吸 | 支气管痉挛（哮喘 / COPD 加重）| β2 阻断（仅 non-selective）|
| 代谢 | 体重↑、血糖↑、糖耐量↓、TG↑、HDL↓ | β2 阻断 + α1 失对抗 |
| 神经 | 疲劳、抑郁、噩梦、性功能障碍 | 亲脂药入脑（propranolol > metoprolol > atenolol）|
| 循环 | 雷诺现象加重、PVD 恶化 | β2 阻断 → 外周血管收缩 |
| 内分泌 | **掩盖低血糖症状**（除出汗外）| β1 阻断心悸、震颤 |

### 8.2 Vasodilatory BB 的差异

- ✅ 代谢副作用大幅减轻
- ✅ TPR↓（后负荷友好）
- ⚠️ Carvedilol / Labetalol 仍有 β2 阻断 → 哮喘仍禁忌
- ⚠️ α1 阻断 → 体位性低血压风险（尤其首剂）

---

## 十、Memory Hook ⭐

> [!tip] 七大记忆锚点
>
> **锚点 1**：横纵两轴
> - 横轴：选择性 = "封不封 β2"
> - 纵轴：血管效应 = "封不封 α1 / 释不释放 NO"
>
> **锚点 2**："A–M 选 β1，N–Z 通杀"
>
> **锚点 3**：词尾规律
> - Metoprolol / Atenolol / Propranolol = **conventional**
> - Carve**dilol** / Labe**talol** = **vasodilatory**（多两个字母 = 多一个 α1）
> - Nebi**volol** = **vasodilatory**（NO 介导）
>
> **锚点 4**：三大 vasodilatory 用法
> - **C**arvedilol = HF**C** (HF + DM)
> - **L**abetalol = **L**ady（孕期）+ **L**ife-threatening HTN（急症）
> - **N**ebivolol = **N**inety（老年 HTN）
>
> **锚点 5**：HFrEF 三剑客 = **"BMC"**（Bisoprolol, Metoprolol succinate, Carvedilol）
>
> **锚点 6**：传统 BB 三宗罪 = **"心慢、喘、糖胖"**（bradycardia / bronchospasm / metabolic syndrome）
>
> **锚点 7**：代谢副作用元凶 vs 神药
> - 最差 = **Propranolol**（封 β2 + α1 单飞 + 无 NO）
> - 最优 = **Carvedilol**（封 β2 + 封 α1 救场）
>
> **锚点 8**：**"β-blocker 是代谢小偷"**（Q15973 触发）
> - 偷走**肌肉血流**：β2 阻断 → α1 无对抗 → 骨骼肌血管收缩 → 葡萄糖进不去
> - 偷走**脂肪分解**：β1 阻断 → 脂肪锁住 → 体重↑
> - **Carvedilol / Labetalol 不偷**：自带 α1 钥匙 → 血管开门 → 肌肉照常吃饭
>
> **锚点 9**：**血糖代谢三态**（HTN 选药速记）
> - ✅ **改善**：ACEi / ARB / α1-blocker
> - ⚪ **中性**：CCB（DHP + Non-DHP）/ Vasodilatory BB（carv / labet / nebiv）
> - ❌ **恶化**：**Conventional BB** / Thiazide（剂量相关）

---

## 十一、自测题（盲做）

> [!question]- Q1：HFrEF + 新诊断 T2DM 患者用 metoprolol tartrate，下一步？
> 换成 **Carvedilol**（HFrEF 适应症 + DM 代谢友好）。也可考虑 metoprolol succinate，但 DM 患者优选 carvedilol。

> [!question]- Q2：肝硬化患者预防食道静脉曲张出血，开始 metoprolol 50mg bid，对吗？
> ❌ 错误。门脉高压必须用 **non-selective BB**（propranolol 或 nadolol），β1 选择性无效。

> [!question]- Q3：孕 32 周 + BP 160/105，选哪个降压药？
> **Labetalol**（一线）。也可 methyldopa 或 nifedipine。避免 ACEI/ARB（致畸）。

> [!question]- Q4：嗜铬细胞瘤患者，按"心率快"开始用 propranolol，对吗？
> ❌ 错误。必须先 α 阻断（phenoxybenzamine），后 BB。单独 BB → HTN 危象。

> [!question]- Q5：甲亢风暴症状控制选哪个 BB，为什么？
> **Propranolol**。non-selective + 抑制 T4→T3 转化。

> [!question]- Q6：哮喘 + HFrEF 患者，可以用 BB 吗？选哪个？
> 可以。选 **β1 选择性**：bisoprolol 或 metoprolol succinate。避免 carvedilol（β2 阻断）。

> [!question]- Q7：Nebivolol 既是 β1 选择性又是 vasodilatory，它和 Metoprolol 的核心区别是什么？
> 两者都 β1 选择性 = 不直接封 β2。
> 但 Nebivolol 额外**释放 NO** → 血管舒张 → 代谢更友好 + 老年 HTN 适用。
> Metoprolol 没有 NO 释放 → 中性血管效应。

> [!question]- Q8：为什么 Propranolol 是"代谢副作用最严重"的 BB？
> 满足"最差组合"：
> - **封 β2**（non-selective）→ 骨骼肌血管收缩倾向
> - **不封 α1**（无 vasodilatory 机制）→ α1 单飞、肌肉血流↓
> - **无 NO 释放**
> 三重缺陷叠加 → 代谢恶化最严重。

> [!question]- Q9：HFrEF + DM + 哮喘患者，选哪个 BB？为什么 Carvedilol 不行？
> 选 **Bisoprolol** 或 **Metoprolol succinate**。
> Carvedilol 虽然代谢友好，但是 **non-selective**（封 β2）→ 哮喘加重风险。
> 哮喘患者必须 **β1 选择性**，宁可代谢稍差也不能诱发支气管痉挛。

---

## 关联

- 🔁 同主题错题：
  - [[mistakes/uworld-mistakes#^Q15973]] 降压药 + DM 代谢副作用（首题，触发本笔记，2026-05-18）
  - 等积累后续：HFrEF GDMT 用药 / 甲亢风暴 / 孕期 HTN / 门脉高压预防 等
- 📚 主笔记 / 姐妹专题：
  - [[完整笔记/Peixuan分科笔记/心内]]（HF / HTN / 心律失常 / CAD 章节都用 BB）
  - [[完整笔记/专题笔记/心内_降压药副作用速查]]（HTN 药物广覆盖 5+2 类矩阵 — 与本笔记 BB-specific 深度互补）
  - [[完整笔记/专题笔记/心内_Vaughan_Williams抗心律失常药]]（BB = Class II 抗心律失常）
- 🏥 跨学科：
  - [[完整笔记/Peixuan分科笔记/endocrine]]（甲亢 Propranolol 抑制 T4→T3 / 嗜铬先 α 后 β / DM 选 carvedilol）
  - [[完整笔记/Peixuan分科笔记/OB]]（孕期 HTN — Labetalol / Methyldopa / Nifedipine 三剑客）
  - [[完整笔记/Peixuan分科笔记/消化补充内容]]（门脉高压预防出血 — propranolol / nadolol 必须 non-selective）
  - [[完整笔记/Peixuan分科笔记/神经]]（migraine 预防 / 表演焦虑 propranolol 亲脂入脑）
  - [[完整笔记/Peixuan分科笔记/眼科]]（青光眼局部 timolol）
  - [[完整笔记/专题笔记/USMLE_实验室指纹诊断大全]] §5.8（BB 中毒指纹 — 慢心率 + 低血糖 + glucagon 解毒）
- 🌱 TODO（待生成衍生 / 待扩充本笔记）：
  - 收集 HFrEF 完整 GDMT 题（ACEI/ARNI + BB + MRA + SGLT2i）→ 生成 [[完整笔记/专题笔记/心内_HFrEF四联药物方案]]（启动顺序与禁忌）
  - 收集嗜铬 / 甲亢风暴 / 孕期 HTN 题积累 → 强化本笔记 §七反直觉陷阱
  - 待补 (v2 候选)：ISA 药物（pindolol, acebutolol）详解；β 受体激动剂对照（dobutamine, isoproterenol）；**BB 过量解救 glucagon 机制**（已部分见指纹大全 §5.8）

---

## 更新日志

- **v2 (2026-05-18)**：新增"认知升级"章节（§零）+ 四象限图谱（§五）。
  - §零 一维 → 二维分类教学路径 + 核心顿悟 + 三句话整合 + 教科书历史包袱解释
  - §五 四象限药物完整图谱（选择性 × 血管效应 × 代谢副作用 × 代表用法 10 行）
  - Memory Hook 锚点 5 → 7 个（新增 横纵两轴 + 元凶/神药对照）
  - 自测题 6 → 9 道（新增 Q7 Nebivolol vs Metoprolol / Q8 Propranolol 为何最差 / Q9 HFrEF+DM+哮喘 carvedilol 为何不行）
  - 后续章节 §五-§十 → §六-§十一 改号

- **v1 (2026-05-18)**：初版建立。Q15973（降压药 + DM 代谢副作用）触发整合。
  - 三大分类维度（选择性 / 血管效应 / ISA）+ 完整受体图谱 10 行
  - 14 行临床应用矩阵
  - 6 个反直觉陷阱 + 5 个 Memory Hooks 锚点
  - 6 道自测题
