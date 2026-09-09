# {Project Name}

> {One-line description of what this system does — e.g., "Customer portal for ACME Logistics with role-based access and audit logging."}

Built by [CODE:EXO](https://codeexo.com) — custom software development, privacy by design.

## Overview

| | |
| --- | --- |
| **Client** | {Client name} |
| **Repository scope** | {e.g., "Web application + REST API"} |
| **Status** | 🟢 Active / 🟡 Maintenance / 🔴 Archived |
| **Live environment** | {URL or "private deployment"} |
| **CodeExo contact** | {delivery-lead email} |

## Tech Stack

| Layer | Technology |
| :--- | :--- |
| Frontend | {e.g., React, TypeScript} |
| Backend | {e.g., Node.js, Express} |
| Database | {e.g., PostgreSQL} |
| Infra/Hosting | {e.g., AWS, Docker} |
| Auth | {e.g., OIDC via Okta} |

## Getting Started (authorized users only)

This repository is restricted to {Client} and CodeExo personnel.

```bash
git clone git@github.com:codeexolabs/{repo-name}.git
cd {repo-name}
cp .env.example .env   # never commit real credentials
npm install && npm run dev
```

## Repository Structure
```tree
├── src/           # application source
├── tests/         # automated tests
├── docs/          # architecture decisions (ADRs), runbooks
└── .github/       # workflows, security config
```

## Security & Confidentiality
- 🔒 This repository is private and confidential to {Client} and CodeExo.
- 🕵️ Report suspected vulnerabilities privately — see our Security Policy or email security@codeexo.com.
- 🔑 All secrets are injected via GitHub Actions secrets / vault — never committed.
- 📜 Access is least-privilege; access requests go through {process/contact}.

## Documentation

- Architecture decisions: docs/adr/
- Runbooks & deployment: docs/runbook.md
- Change log: see Releases

## Support

| Issue Type | Channel |
| :--- | :--- |
| Bugs / feature requests | GitHub Issues in this repo |
| Security vulnerabilities | security@codeexo.com (private) |
| Contract / billing | info@codeexo.com |

## Repository Naming & Visibility Conventions

Applies to all repositories under the [codeexolabs](https://github.com/codeexolabs) organization.
New repositories must follow these tiers and rules...

**Structure the org around four tiers, sorted alphabetically by tier:**

| Prefix | Purpose | Visibility | Examples |
| --- | --- | --- | --- |
| `client-{name}-{system}` | Paid client work, one repo per deliverable | **Private** | `client-acme-portal`, `client-acme-mobile`, `client-orion-api` |
| `product-*` | CodeExo-owned IP / repeatable offerings | Private (public only if open-sourced deliberately) | `product-auth-scaffold`, `product-notify-service` |
| `internal-*` | Company ops: policies, proposals, infra-as-code, docs | Private | `internal-infra`, `internal-handbook` |
| `.github` | Org profile + community health files | Public | *(already done)* |

**Convention rules worth fixing now, while you're the only committer:**

1. **One deliverable = one repo.** Avoid mono-monsters like `client-acme-everything`; split `portal` / `api` / `infra` so access can be scoped per team later.
2. **Lowercase, hyphen-separated** (`client-acme-web-portal`, never `ClientAcmeWebPortal`) — GitHub convention and grep-friendly.
3. **Short branch prefixes** contract: `feat/`, `fix/`, `chore/`, `release/` — matches your CONTRIBUTING.md.
4. **Archive, don't delete**, ended engagements: *Settings → Archive repository*. This preserves the audit trail clients may request years later, and keeps your dashboard clean.
5. **Never** encode client secrets, IPs, or sensitive identifiers in names or descriptions — for a "privacy by design" brand, the org page should show nothing that reveals who your clients are without permission.
6. Consider a lightweight wiki/README section listing active vs. archived engagements in `internal-handbook` rather than relying on memory.

This tier system pays off the moment you hire: you grant a contractor access to exactly one `client-*` repo, and nothing else is visible.

