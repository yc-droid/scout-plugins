---
name: sip-check
description: Check how a mutual fund SIP or lumpsum investment has actually performed. Use when the user asks what their SIP or one-time investment would be worth now, their XIRR, or whether a step-up SIP made a difference.
---

To check a SIP or lumpsum:

1. Find the exact scheme with `search_mutual_funds` (confirm Direct/Regular and Growth/IDCW).
2. For a SIP, call `calculate_sip_returns` with the monthly amount and start date (and `annual_step_up_pct` if they step up). For a one-time investment, call `calculate_lumpsum_returns`.
3. Report total invested, current value, gain and XIRR or CAGR, with the NAV date used. Show the year-by-year table if the tool returns one.
4. If the start date is before the fund's history begins, say so and use the date the tool suggests.
5. Close with the disclaimer: calculations use NAVs only and exclude exit loads, stamp duty and tax; past performance doesn't guarantee future returns; not investment advice.
