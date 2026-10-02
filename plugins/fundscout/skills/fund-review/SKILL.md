---
name: fund-review
description: Review an Indian mutual fund's performance factually. Use when the user asks how a mutual fund has performed, its NAV, returns or CAGR, or wants to compare it with similar funds.
---

To review a mutual fund:

1. Call `search_mutual_funds` to find the exact scheme. Confirm the plan (Direct or Regular) and option (Growth or IDCW) the user means, because they have different NAVs. Default to Direct Growth only if the user doesn't say, and state that you did.
2. Call `get_fund_nav` for the latest NAV and the 1M to 10Y returns.
3. If the user names other funds, or asks how it compares, call `compare_funds` with up to 5 scheme codes in the same category.
4. Present a table of periods and returns, the NAV date, and the fund's category and history start date.
5. Close with the disclaimer: past performance doesn't guarantee future returns, figures exclude exit loads, stamp duty and tax, and this is factual data, not investment advice.

Never recommend buying, selling or switching funds, and never rank funds as "best".
