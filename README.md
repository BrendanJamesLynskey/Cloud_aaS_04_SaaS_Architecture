# 🧑‍💼 SaaS Architecture — Multi-Tenancy, B2B Identity, Metering

Deck **04 of 6** in the [Cloud `*aaS` series](https://github.com/BrendanJamesLynskey/Cloud_aaS_Hub). The architectural side of SaaS — multi-tenancy patterns, tenant isolation, B2B identity (SAML/OIDC/SCIM), Auth-as-a-Service providers, metering data models, per-tenant observability, residency and compliance.

Companion to [Monetising &amp; Distributing Software](https://github.com/BrendanJamesLynskey/Monetising_and_Distributing_Software) (the business side of SaaS — Stripe, MRR, churn, pricing) and [Introduction to OAuth](https://github.com/BrendanJamesLynskey/Introduction_to_OAuth) (identity foundations).

## ▶ [Open the Presentation](https://brendanjameslynskey.github.io/Cloud_aaS_04_SaaS_Architecture/)

## 🧭 [Series hub](https://github.com/BrendanJamesLynskey/Cloud_aaS_Hub)

---

## Contents

| # | Topic | Description |
|---|-------|-------------|
| 01 | Title | Tenant → IdP → App → Meter → Bill |
| 02 | Topics | Multi-tenancy / B2B identity / metering / operations |
| 03 | What "SaaS architecture" means | The unique problems SaaS poses; B2C vs B2B; PLG vs sales-led |
| 04 | Multi-tenancy — four patterns | Pool / Bridge / Silo / Hybrid — annotated comparison diagram |
| 05 | Pool deep dive | Schema pattern, Postgres RLS, sharded pool, hard parts |
| 06 | Bridge | Schema-per-tenant, where bridge wins / breaks, real-world examples |
| 07 | Silo | Why customers ask for it, BYO-cloud, single-tenant SaaS as a category, hidden tax |
| 08 | Tenant isolation | Defence-in-depth across app / DB / network / operations |
| 09 | B2B identity | Why B2B is different; SAML / OIDC / SCIM matrix; SSO &amp; SCIM flows |
| 10 | Auth-as-a-Service | Auth0 / WorkOS / Stytch / Clerk / FrontEgg / Cognito / Entra / Keycloak / ZITADEL |
| 11 | Metering data model | Usage events, pricing rules, build-vs-buy (Stripe / Lago / Orb / Metronome / m3ter), reconciliation |
| 12 | Per-tenant observability | Golden signals per-tenant, OTel attributes, tier-aware SLOs, rate limits |
| 13 | Data residency &amp; multi-region | Tenant pinning, cell-per-region, GDPR/DPF/UK adequacy/FedRAMP, the metadata leak |
| 14 | Audit logs as a feature | What to log, expose, build vs buy, tamper-evidence |
| 15 | Compliance shapes | SOC 2 / ISO 27001 / HIPAA / GDPR / PCI / FedRAMP / EU AI Act with year-1 cost |
| 16 | Tenant lifecycle | State machine: prospect → trial → active → past-due → cancelled → deleted; GDPR right-to-erasure |
| 17 | Cell-based architecture | Slack / Stripe / Salesforce PODs, when to start, cross-cell features |
| 18 | Anti-patterns | Optional tenant_id, DIY SAML, late metering, shared audit DB, shared rate limits |
| 19 | Summary | Three takeaways &amp; next-deck pointer |

---

## Slide Controls

| Action | Key |
|--------|-----|
| Next / Previous | `→` `←` or swipe |
| Overview | `Esc` |
| Fullscreen | `F` |
| Speaker notes | `S` |
| Export to PDF | append `?print-pdf` to URL, then print |

## Technology

[Reveal.js 4.6](https://revealjs.com) · [highlight.js](https://highlightjs.org) · Playfair Display + DM Sans + JetBrains Mono · inline SVG diagrams. Single self-contained `index.html`.

## See also

- Companion: [Monetising &amp; Distributing Software](https://github.com/BrendanJamesLynskey/Monetising_and_Distributing_Software) — Stripe, subscription pricing, MRR/churn
- Companion: [Introduction to OAuth](https://github.com/BrendanJamesLynskey/Introduction_to_OAuth) — the auth foundation B2B identity rests on
- Companion: [Introduction to OpenID Connect](https://github.com/BrendanJamesLynskey/Introduction_to_OpenID_Connect) — the OIDC primitives (ID tokens, discovery, JWKS, federation) used by every B2B SSO integration in this deck
- Companion: [OAuth for MCP](https://github.com/BrendanJamesLynskey/OAuth_for_MCP) — full provider tour
- Companion: [Web Authentication](https://github.com/BrendanJamesLynskey/Introduction_to_Web_Authentication) — sessions, JWTs, MFA
- Next in series: [Cloud_aaS_05_Cloud_Security](https://github.com/BrendanJamesLynskey/Cloud_aaS_05_Cloud_Security) — the cloud-security cross-cuts
- Cross-link: [Introduction to Databases](https://github.com/BrendanJamesLynskey/Introduction_to_Databases) — the storage layer behind every SaaS

## License

Educational use. Code examples provided as-is.
