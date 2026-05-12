---
nbme: 12
date: 2026-05-12
status: in_progress
total_score: 
target: 250
duration_minutes: 
review_pass: 0
tags:
  - USMLE-Step2
  - NBME模拟题
  - 做题结果
---

# NBME 12 做题结果

> [!info] 套题信息
> - **主文件**：[[NBME12_breakdown]]
> - **套题索引**：[[NBME12_套题索引]]
> - **学科索引**：[[NBME12_学科索引]]
> - **考点索引**：[[NBME12_考点索引]]

> [!warning] 当前进度
> - ✅ Section 1（Q001-Q050）已录入
> - ✅ Section 2（Q051-Q100）已录入
> - ⬜ Section 3（Q101-Q150）待做
> - ⬜ Section 4（Q151-Q200）待做
>
> ⚠️ **待核对**：Q074（Section 2 第 24 题），截图 3 vs 截图 4 显示不一致，目前按 `wrong` 入库。

---

## 📊 实时统计（Dataview 自动生成）

```dataview
TABLE WITHOUT ID
  "已答题数" as "字段",
  length(filter(this.qs, (q) => q.result != null)) as "数值"
WHERE file.name = this.file.name
```

> [!tip]- 📈 详细统计（点击展开）
> 
> ```dataviewjs
> const page = dv.current();
> const qs = page.qs || [];
> 
> const answered = qs.filter(q => q.result && q.result !== "blank");
> const correct = qs.filter(q => q.result === "right");
> const wrong = qs.filter(q => q.result === "wrong");
> const marked = qs.filter(q => q.result === "marked");
> const unanswered = qs.filter(q => !q.result || q.result === "blank");
> 
> const lowConf = qs.filter(q => q.conf === "low");
> const highConfRight = qs.filter(q => q.result === "right" && q.conf === "high");
> const lowConfRight = qs.filter(q => q.result === "right" && q.conf === "low");
> 
> dv.table(["指标", "数值", "占比"],
>   [
>     ["✅ 答对", correct.length, ((correct.length / 200) * 100).toFixed(1) + "%"],
>     ["❌ 答错", wrong.length, ((wrong.length / 200) * 100).toFixed(1) + "%"],
>     ["🏷️ 标记/犹豫", marked.length, ((marked.length / 200) * 100).toFixed(1) + "%"],
>     ["⬜ 未答", unanswered.length, ((unanswered.length / 200) * 100).toFixed(1) + "%"],
>     ["---", "---", "---"],
>     ["🟢 高置信度答对（真会）", highConfRight.length, "确认掌握"],
>     ["🔴 低置信度答对（蒙对/伪掌握）", lowConfRight.length, "⚠️ 高危区"],
>     ["📊 正确率（已答）", correct.length + "/" + answered.length, 
>      answered.length > 0 ? ((correct.length / answered.length) * 100).toFixed(1) + "%" : "—"],
>   ]
> );
> ```

---

## 📝 题目状态表

### 题目列表

```dataview
TABLE WITHOUT ID
  qid as "Q#",
  result as "结果",
  conf as "置信度",
  my_choice as "我选",
  my_note as "备注"
FROM ""
WHERE file.name = this.file.name
FLATTEN qs as q
WHERE q.qid
SORT q.qid ASC
```

<!-- ↓↓↓ 数据存储区（不要删除这部分）↓↓↓ -->

> [!example]- 📋 完整 200 题数据（点击展开/折叠编辑）

```yaml
qs:
  - qid: "001"
    result: right
    conf: low
    my_choice: 
    my_note: 
  - qid: "002"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "003"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "004"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "005"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "006"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "007"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "008"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "009"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "010"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "011"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "012"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "013"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "014"
    result: right
    conf: low
    my_choice: 
    my_note: 
  - qid: "015"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "016"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "017"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "018"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "019"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "020"
    result: right
    conf: low
    my_choice: 
    my_note: 
  - qid: "021"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "022"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "023"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "024"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "025"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "026"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "027"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "028"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "029"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "030"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "031"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "032"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "033"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "034"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "035"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "036"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "037"
    result: right
    conf: low
    my_choice: 
    my_note: 
  - qid: "038"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "039"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "040"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "041"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "042"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "043"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "044"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "045"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "046"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "047"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "048"
    result: right
    conf: low
    my_choice: 
    my_note: 
  - qid: "049"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "050"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "051"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "052"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "053"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "054"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "055"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "056"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "057"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "058"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "059"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "060"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "061"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "062"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "063"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "064"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "065"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "066"
    result: right
    conf: low
    my_choice: 
    my_note: 
  - qid: "067"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "068"
    result: right
    conf: low
    my_choice: 
    my_note: 
  - qid: "069"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "070"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "071"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "072"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "073"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "074"
    result: wrong
    conf: 
    my_choice: 
    my_note: "⚠️ 截图识别不一致（截图3=✗，截图4=✓），请核对"
  - qid: "075"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "076"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "077"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "078"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "079"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "080"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "081"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "082"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "083"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "084"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "085"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "086"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "087"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "088"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "089"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "090"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "091"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "092"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "093"
    result: wrong
    conf: 
    my_choice: 
    my_note: 
  - qid: "094"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "095"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "096"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "097"
    result: wrong
    conf: low
    my_choice: 
    my_note: 
  - qid: "098"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "099"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "100"
    result: right
    conf: 
    my_choice: 
    my_note: 
  - qid: "101"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "102"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "103"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "104"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "105"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "106"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "107"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "108"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "109"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "110"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "111"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "112"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "113"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "114"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "115"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "116"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "117"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "118"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "119"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "120"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "121"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "122"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "123"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "124"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "125"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "126"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "127"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "128"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "129"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "130"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "131"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "132"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "133"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "134"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "135"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "136"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "137"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "138"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "139"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "140"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "141"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "142"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "143"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "144"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "145"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "146"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "147"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "148"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "149"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "150"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "151"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "152"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "153"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "154"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "155"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "156"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "157"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "158"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "159"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "160"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "161"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "162"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "163"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "164"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "165"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "166"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "167"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "168"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "169"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "170"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "171"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "172"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "173"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "174"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "175"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "176"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "177"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "178"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "179"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "180"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "181"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "182"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "183"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "184"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "185"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "186"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "187"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "188"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "189"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "190"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "191"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "192"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "193"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "194"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "195"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "196"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "197"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "198"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "199"
    result: blank
    conf: 
    my_choice: 
    my_note: 
  - qid: "200"
    result: blank
    conf: 
    my_choice: 
    my_note: 
```

---

## 🎯 错题快速跳转（Dataview 自动筛选）

```dataviewjs
const page = dv.current();
const qs = page.qs || [];
const wrong = qs.filter(q => q.result === "wrong");
const marked = qs.filter(q => q.result === "marked");
const lowConfRight = qs.filter(q => q.result === "right" && q.conf === "low");
const nbme = page.nbme;

if (wrong.length > 0) {
  dv.header(3, "❌ 错题（" + wrong.length + " 道）");
  dv.list(wrong.map(q => 
    `[[NBME${nbme}_breakdown#Q${q.qid}|Q${q.qid}]] — 我选 ${q.my_choice || "?"} | ${q.my_note || ""}`
  ));
}

if (marked.length > 0) {
  dv.header(3, "🏷️ 标记题（" + marked.length + " 道）");
  dv.list(marked.map(q => 
    `[[NBME${nbme}_breakdown#Q${q.qid}|Q${q.qid}]] — ${q.my_note || "待复查"}`
  ));
}

if (lowConfRight.length > 0) {
  dv.header(3, "⚠️ 伪掌握警报：低置信度答对（" + lowConfRight.length + " 道）");
  dv.paragraph("> 这些题虽然答对，但你不确定。真考试可能翻车，**和错题同等优先级**！");
  dv.list(lowConfRight.map(q => 
    `[[NBME${nbme}_breakdown#Q${q.qid}|Q${q.qid}]] — 选了 ${q.my_choice} | ${q.my_note || ""}`
  ));
}
```

---

## ✏️ 复盘行动清单

- [x] 完成 Section 1+2，截图入库
- [ ] 完成 Section 3+4 做题
- [ ] 抽查 5-10 题验证 AI 识别准确率
- [ ] 检查"伪掌握警报"区，标记真正需要复盘的题
- [ ] 把错题 + 标记题 + 伪掌握题对应的 breakdown callout 打开看一遍
- [ ] 在错题对应的 callout 末尾补充【🤯 我为什么错】区块
- [ ] 让 Claude Code 跑复盘 prompt → 生成本套薄弱点报告
- [ ] 1 周后选 10-20 道关键题重做（错题 + 伪掌握）
