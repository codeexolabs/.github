# Security Policy — CODE:EXO

At CODE:EXO, security isn't a layer added at the end — it's designed in from the
first line of code. We build custom software with **privacy by design**, and this
policy explains how to reach us if you discover a vulnerability in anything we ship.

## Reporting a Vulnerability

**Please do NOT open a public GitHub issue for security vulnerabilities.**

Email us at: **security@codeexo.com**

Please include:

- A description of the vulnerability and its potential impact
- Steps to reproduce (proof-of-concept code is welcome)
- The affected repository, URL, or version
- Any logs, screenshots, or request traces that help us triage

If the issue is reproducible only in a specific deployment, include environment
details but **never include live customer credentials or production data**.

## Our Commitment

- **Acknowledgement** within 48 hours of receipt
- **Triage** and severity assessment within 7 days
- Regular status updates until resolution
- Credit for responsible disclosure, if you wish (in our hall of thanks, never without consent)
- No legal action against researchers acting in good faith within this policy

## Scope

**In scope:**
- All public repositories under the [codeexolabs](https://github.com/codeexolabs) organization
- The CodeExo website and any publicly exposed services

**Out of scope:**
- Social engineering, phishing, or physical attacks
- Denial-of-service or volumetric attacks
- Spam or automated scanning against production systems
- Findings from compromised client accounts or endpoints

## Privacy by Design Commitments

Across all CodeExo engagements:

1. **Data minimization** — we collect and retain only what the product genuinely needs.
2. **Encryption everywhere** — data encrypted in transit (TLS 1.2+) and at rest by default.
3. **Least privilege** — access to client systems is scoped, time-boxed, and audited.
4. **Secure defaults** — no secrets in source control; secrets live in managed vaults only.
5. **Shippable assurance** — dependency scanning and secret scanning enabled on all repos.

## Supported Versions

| Component | Version | Supported |
| :--- | :--- | :--- |
| CODE:EXO client deliverables | latest | ✅ |
| Public repositories | main | ✅ |
| Older releases | — | ❌ |

## Safe Harbor

We consider security research conducted in accordance with this policy to be
authorized and will not pursue legal action against good-faith researchers,
provided you avoid privacy violations, data destruction, and service degradation.

---

Thank you for helping us keep CODE:EXO — and the software we build for you — secure.
