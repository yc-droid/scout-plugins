# DepScout

DepScout connects Claude to live vulnerability and malware data from OSV.dev and deps.dev, so answers about whether a package is safe, and which version to use, come from current advisories instead of model memory.

## What's included

- **DepScout connector**: the remote MCP server at `https://depscout.salesup.workers.dev/mcp`. No account, sign-in or API key needed.
- **dependency-audit**: Audit a project's dependencies for known vulnerabilities, malware and deprecated packages.
- **vet-new-package**: Vet an open-source package before adding it to a project.

## Use it

Ask Claude whether a package is safe, which version fixes a CVE, or to audit your project. In Claude Code, the dependency-audit skill reads your manifest files (package.json, requirements.txt, go.mod and others) and produces a prioritized upgrade plan.

## Data

DepScout sends the package names, versions and advisory IDs you ask about to the DepScout server (depscout.salesup.workers.dev), which looks them up in OSV.dev and deps.dev. When you audit a project, only package names and versions are sent; your source code is never sent or stored. See the privacy policy at https://depscout.salesup.workers.dev/privacy and the terms at https://depscout.salesup.workers.dev/terms.

## Support

Email yc@salesup.club or visit https://depscout.salesup.workers.dev/support. DepScout is an independent tool by Yash Chowdhury and isn't affiliated with the data providers it uses.
