# 財務データ

- `YYYY-MM.csv`: その月の支出・収入。1行1件、金額は税込の整数（円）。
  - `type`: expense / income
  - `category`: subscription / api / misc（諸経費・検証費） / ad / revenue
  - `payment`: 支払方法（カード名などは書かず「カード」「無料」など）
- `hours.csv`: オーナーの作業時間（5万円枠には入れない、記事の題材）。
- 月の上限は5万円（目安: subscription 1万、api 1万、misc 1万）。計上範囲は `decisions/2026-11-15-initial.md`。
