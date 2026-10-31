# Proactis

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Proactis is a source-to-pay software provider whose platform covers eSourcing, contract management, supplier management, purchase-to-pay, marketplace and accounts payable automation for mid-market and public-sector organisations. Its developer surface is a set of ten separate REST APIs — accounting, contract, eInvoice, invoice, order, receipt, requisition, supplier, timecard and user — documented at docs.proactis.com and deployed across four regional environments (EU, NL, UK and US), each with a paired UAT and production estate. The APIs are standards-based rather than proprietary: transactional documents move as cXML, electronic invoices as UBL 2.1, identity and department master roles as SCIM 2.0, and timecards as HR-XML, all behind OAuth 2.0 client-credentials tokens paired with a fixed API key. Proactis also pushes transactional documents outbound to customer-configured endpoints. Access is gated: credentials are issued only by Proactis support, and no machine-readable contract is published.

**Areas:** Procurement · Purchase-To-Pay · Source-to-Pay · Spend Management · Contract Management · E-Invoicing · Accounts Payable · Supplier Management · eSourcing · cXML · UBL · SCIM

## Proactis on APIs.io

Everything profiled for Proactis is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/proactis/](https://apis.io/providers/proactis/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [Proactis Accounting API](https://apis.io/apis/proactis/proactis-accounting/) — Configure the accounting structures that spend is coded against — departments, cost centers, cost accounts and cost dimensions, plus department addresses.…
- [Proactis Contract API](https://apis.io/apis/proactis/proactis-contract/) — Create contracts in Proactis from an external system. The narrowest of the ten services — creation is the only capability the public documentation describes.
- [Proactis eInvoice API](https://apis.io/apis/proactis/proactis-einvoice/) — Import electronic invoices created in another application into Proactis as OASIS UBL 2.1 documents. Each invoice requires at least one line item; the API…
- [Proactis Invoice API](https://apis.io/apis/proactis/proactis-invoice/) — Retrieve invoices from Proactis, receive them pushed to your own endpoint as they reach a configured status, and write back payment information. Entry…
- [Proactis Order API](https://apis.io/apis/proactis/proactis-order/) — Create ERP orders in Proactis and retrieve them, or have them pushed outbound as cXML. The order service is the only one that supports multiple push…
- [Proactis Receipt API](https://apis.io/apis/proactis/proactis-receipt/) — Import goods receipts against existing orders and retrieve them. Receipts are posted as cXML ReceiptRequest documents referencing an order and line number,…
- [Proactis Requisition API](https://apis.io/apis/proactis/proactis-requisition/) — Retrieve requisitions, receive them pushed outbound, and run budget checks. Both an import and an export cXML definition are published, and requisition…
- [Proactis Supplier API](https://apis.io/apis/proactis/proactis-supplier/) — Create, modify, delete and retrieve suppliers. Retrieval is paged and filterable — online status, name prefix and last-modified date are all supported query…
- [Proactis Timecard API](https://apis.io/apis/proactis/proactis-timecard/) — Create and retrieve timecards, with a dedicated HR-XML validation endpoint and timecard import operations. Timecards are one of the five document types…
- [Proactis User API (SCIM 2.0)](https://apis.io/apis/proactis/proactis-user/) — Provision users and department master roles into Proactis using SCIM 2.0. Users support POST, GET with filtering and pagination, PATCH or PUT, and DELETE —…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Proactis Webhooks](https://apis.io/asyncapis/proactis/proactis-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Proactis MCP server](https://apis.io/servers/proactis/proactis-mcp-server/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Proactis Authentication](https://apis.io/security/proactis/proactis-authentication/)
- [Proactis Domain Security](https://apis.io/security/proactis/proactis-domain-security/)
- [Proactis Trust Center](https://apis.io/security/proactis/proactis-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Proactis Scopes](https://apis.io/scopes/proactis/proactis-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Proactis Plans Pricing](https://apis.io/plans/proactis/proactis-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Proactis Rate Limits](https://apis.io/rate-limits/proactis/proactis-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Proactis Finops](https://apis.io/finops/proactis/proactis-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.proactis.com/)
- [Documentation](https://docs.proactis.com/)
- [Getting started](https://docs.proactis.com/introduction/)
- [API reference](https://docs.proactis.com/apis/overview)
- [Support](https://www.proactis.com/support/)
- [Blog](https://www.proactis.com/uk/resources/?group=resource-type&categoryIds=1568)
- [Compliance](https://www.proactis.com/uk/about-us/accreditations-certifications/)
- [Terms of service](https://www.proactis.com/us/customers/contractual-terms-and-conditions/)
- [Privacy policy](https://www.proactis.com/privacy-policy/)
- [GitHub](https://github.com/proactis-documentation)

## API Evangelist rating

**Kin Score 52.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 50.5 |
| Contract governance | 18.2 |
| Operational transparency | 57.9 |
| Developer ergonomics | 64.3 |
| Access clarity | 28.9 |

**Agent readiness 26.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 39.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/proactis/](https://apis.io/providers/proactis/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Proactis: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/proactis/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
