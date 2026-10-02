---
name: vet-new-package
description: Vet an open-source package before adding it to a project. Use when the user asks whether to use, install or trust a package, compares packages, or asks if a package is safe, maintained or deprecated.
---

To vet a package before adding it:

1. Call `check_package` with the ecosystem and name (no version, so the latest is checked). If the user named a version, check that too.
2. Stop and warn first if it's flagged malicious or a release was compromised.
3. Summarize: latest version and release date, deprecation, open vulnerabilities in the latest version, licence, and OpenSSF Scorecard if available.
4. Give a verdict: Use / Use with care / Avoid, with one line of reasoning. Treat no release in 2+ years, deprecation or a low Scorecard as maintenance risks.
5. If you suggest an alternative package, check it with `check_package` before recommending it.
