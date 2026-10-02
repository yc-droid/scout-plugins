# FundScout India

FundScout India connects Claude to official daily NAV data for Indian mutual funds (published by AMFI, via mfapi.in) and does every return calculation on the server, so the numbers are exact rather than recalled from memory.

## What's included

- **FundScout India connector**: the remote MCP server at `https://fundscout.salesup.workers.dev/mcp`. No account, sign-in or API key needed.
- **fund-review**: Review an Indian mutual fund's performance factually.
- **sip-check**: Check how a mutual fund SIP or lumpsum investment has actually performed.

## Use it

Ask for a fund's NAV and returns, compare funds, or work out what a past SIP or lumpsum is worth now. The fund-review skill produces a structured review of one fund; the sip-check skill checks how a user's SIP has actually performed.

## Data

FundScout India sends the fund names, scheme codes, amounts and dates you ask about to the FundScout server (fundscout.salesup.workers.dev), which uses public AMFI NAV data via mfapi.in to look up NAVs and calculate returns. It never accesses your holdings or accounts and stores nothing about you. See the privacy policy at https://fundscout.salesup.workers.dev/privacy and the terms at https://fundscout.salesup.workers.dev/terms.

## Support

Email yc@salesup.club or visit https://fundscout.salesup.workers.dev/support. FundScout India is an independent tool by Yash Chowdhury and isn't affiliated with the data providers it uses.
