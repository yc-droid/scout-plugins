---
name: dependency-audit
description: Audit a project's dependencies for known vulnerabilities, malware and deprecated packages. Use when the user asks to audit, security-check or upgrade dependencies, mentions npm audit, pip-audit or a CVE in their project, or shares a package.json, requirements.txt, go.mod, Cargo.toml or pom.xml.
---

To audit a project's dependencies:

1. Find the manifest files: package.json and lockfiles, requirements*.txt, pyproject.toml, go.mod, Cargo.toml, pom.xml or *.csproj. In chat, ask the user to paste them.
2. Extract exact versions. Prefer lockfile versions; if a range like ^4.17.0 is all you have, use the version written and say so.
3. Call `check_dependencies` with `packages` (up to 50 per call, each with name, version and, for mixed projects, ecosystem) and a default `ecosystem`. Batch larger projects.
4. Report in this order: malicious or compromised packages (remove now), then critical and high vulnerabilities, then medium and low, then deprecated or unmaintained packages.
5. For each problem, give the package, current version, the minimum safe version from the result, and the change to make. Group upgrades that cross a major version separately as possibly breaking.
6. In Claude Code, offer to apply the safe non-breaking upgrades and re-run the audit afterwards.

A clean result means no known advisory for that version, not a guarantee. Transitive dependencies are only checked if they appear in the lockfile you passed.
