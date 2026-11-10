# GPA What-If Calculator 預測 GPA 計算機

**Work out your GPA now, and what grades you need to reach your target GPA. Free, no login, no server, your data never leaves your device.**

**計而家 GPA,計要攞幾多分先達到目標。免費、免登入、無伺服器,資料唔會離開你部機。**

## Try it

Open `index.html` in any browser (double-click works, no server needed).

## Use it in 2 minutes

1. Add each finished course: semester, credits, grade (4.0 scale).
2. Read your current GPA at the top, plus a GPA per semester.
3. Type your target GPA and how many credits you still plan to take — it tells you the average grade you need and whether it is reachable.
4. Try a trial grade on a planned course to see the GPA it would give.
5. Your courses auto-save in this browser; press **匯出 CSV Export CSV** to download the list.

## 兩分鐘用法

1. 逐科輸入學期、學分、成績 (4.0 制)。
2. 睇而家 GPA,每個學期嘅 GPA 會分組顯示。
3. 輸入目標 GPA 同餘下學分,佢會話你知平均要攞幾多分、做唔做得到。
4. 試一科假設成績,睇下 GPA 會變成幾多。
5. 資料自動儲存喺呢部瀏覽器,撳 **匯出 CSV** 可以下載成 CSV。

## What it does

- Course list with semester grouping and per-semester GPA.
- Live current GPA (4.0 scale, always shown with its scale).
- Target-GPA solver with a reachable / not-reachable verdict; impossible targets show the best GPA reachable with the planned credits.
- Per-course trial grade: "If I get A in this 3-credit course, my GPA becomes…"
- Auto-save to localStorage; CSV export (Blob download, no server).

## Honest limits — what it does NOT do

- **No grade prediction or AI.** It never guesses what grade you will get.
- **No official record.** Planning aid only, not your university transcript. Grade scales differ between universities — this calculator uses the HK 4.0 scale; if yours differs, check your own scale.
- **No retake / grade-replacement rules.** Retaken courses count twice unless you delete the old row yourself.
- **No server storage, no sharing, no login.** Your data lives only in this browser's localStorage. Clearing browser data erases it.

## Tests

`node tests/test_gpa.js` — 13 checks: GPA maths (3cr A + 3cr B = 3.50), solver reachable/impossible, semester grouping, CSV format, ES5-only scan, zero external resources.
