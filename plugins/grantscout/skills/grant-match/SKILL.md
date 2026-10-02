---
name: grant-match
description: Find federal grants that fit an organization or project. Use when the user describes their nonprofit, school, tribe, government, research group or small business and asks for funding, grants or opportunities.
---

To match an organization to federal grants:

1. Get the essentials, asking only for what's missing: organization type (for example 501(c)(3), tribal government, county, university, small business), the project topic, and the US state if relevant.
2. If you're unsure which filter values exist, call `list_grant_filters`.
3. Call `search_grants` with a short topic keyword, the matching `eligibility` values and a `category`. Run 2 or 3 searches with different keywords or categories when the topic is broad.
4. Drop results the organization isn't eligible for, then show a shortlist table: Grant | Agency | Closes | Award range | Why it fits. Sort by soonest deadline and flag anything closing within 30 days.
5. Offer to brief any grant in detail (the grant-brief skill).

For for-profit small businesses, say plainly that federal grants are uncommon and point to SBIR/STTR and SBA programs. Always tell the user to confirm details in the official announcement.
