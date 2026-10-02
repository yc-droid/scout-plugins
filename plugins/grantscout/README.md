# GrantScout

GrantScout connects Claude to live US federal grant listings on Grants.gov, so you can find funding your organization can actually apply for, with real deadlines and eligibility.

## What's included

- **GrantScout connector**: the remote MCP server at `https://grantscout.salesup.workers.dev/mcp`. No account, sign-in or API key needed.
- **grant-match**: Find federal grants that fit an organization or project.
- **grant-brief**: Turn one federal grant opportunity into an eligibility checklist and application plan.

## Use it

Describe your organization and project and ask Claude to find matching grants. The grant-match skill builds a ranked shortlist with deadlines; the grant-brief skill turns one opportunity into an eligibility checklist and application plan.

## Data

GrantScout sends the search terms and filters you ask about (topics, applicant type, category, agency, opportunity numbers) to the GrantScout server (grantscout.salesup.workers.dev), which looks them up on the public Grants.gov API. It stores nothing about you. See the privacy policy at https://grantscout.salesup.workers.dev/privacy and the terms at https://grantscout.salesup.workers.dev/terms.

## Support

Email yc@salesup.club or visit https://grantscout.salesup.workers.dev/support. GrantScout is an independent tool by Yash Chowdhury and isn't affiliated with the data providers it uses.
