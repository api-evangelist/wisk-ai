# WISK (wisk-ai)

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

WISK is a bar, restaurant, and hospitality inventory and cost-management platform that tracks items, counts inventory across venues, scans and reconciles supplier invoices, and integrates with 60+ POS systems to compare theoretical vs. actual usage. WISK's programmatic surface is partner-gated - a documented Public Sales upload API lets POS providers and partners push sales data into WISK, and customer API access is offered on the top (Premium) plan. There is no public, self-serve developer portal or published OpenAPI as of this catalog date.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/wisk-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/wisk-ai/refs/heads/main/apis.yml)

## API Availability

WISK is a SaaS product first. Its documented developer/API surface is thin and partner-gated:

- **Public Sales upload (POS providers):** WISK publishes a Public Sales upload flow so POS providers can push sales data into customer accounts; POS providers contact WISK partnerships to begin. WISK can alternatively pull from a POS provider's Sales and Product/Menu APIs, or ingest an automated daily sales report email.
- **Customer API access:** Offered on the top **Premium** plan ("custom reporting & API access"); not part of lower tiers.
- **No public self-serve portal:** WISK does not publish an open developer portal, public base URL, or an OpenAPI specification. Inventory/items, venues, and invoices exist as product capabilities but are not published as self-serve developer APIs.
- **No public webhooks API:** No documented self-serve webhook/event-subscription surface is published; event exchange with POS partners is arranged through the partner integration process.

## Tags

- Inventory
- Restaurant
- Bar
- Hospitality
- Cost Management
- POS Integration

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### WISK Inventory & Items API

Tracks bottles, ingredients, and SKUs with counts, par levels, and variance across the venue's item catalog. Exposed in the WISK product and apps; not published as a public, self-serve developer API. Customer API access is available on the Premium plan.

- **Human URL:** [https://www.wisk.ai/features/restaurant-bar-inventory-management-software](https://www.wisk.ai/features/restaurant-bar-inventory-management-software)

#### Tags

- Inventory
- Items
- Stock

#### Properties

- [Documentation](https://help.wisk.ai/en/collections/2572511-new-user-guide)
- [OpenAPI](openapi/wisk-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wisk-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wisk-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WISK Venues API

Organizes inventory, users, and reporting per venue (location) for single sites and multi-location groups. Surfaced in the WISK platform; not published as a public, self-serve developer API.

- **Human URL:** [https://www.wisk.ai/](https://www.wisk.ai/)

#### Tags

- Venues
- Locations
- Multi-Location

#### Properties

- [Documentation](https://help.wisk.ai/en/collections/2572511-new-user-guide)
- [OpenAPI](openapi/wisk-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wisk-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wisk-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WISK Invoices API

Captures, AI-processes, and reconciles supplier invoices against purchases and pricing to track cost of goods. Available in the WISK product; not published as a public, self-serve developer API.

- **Human URL:** [https://www.wisk.ai/](https://www.wisk.ai/)

#### Tags

- Invoices
- Cost Management
- Reconciliation

#### Properties

- [Documentation](https://help.wisk.ai/en/collections/2572511-new-user-guide)
- [OpenAPI](openapi/wisk-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wisk-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wisk-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WISK POS Integration (Public Sales Upload) API

Partner-gated integration for POS providers to push sales data (POS code or item name, quantity sold, net sales) into WISK customer accounts via a documented Public Sales upload flow. WISK can alternatively pull from a POS provider's Sales and Product/Menu APIs, or ingest a daily sales report email. POS providers contact WISK partnerships to begin.

- **Human URL:** [https://www.wisk.ai/pos](https://www.wisk.ai/pos)

#### Tags

- POS Integration
- Sales
- Partner

#### Properties

- [Documentation](https://help.wisk.ai/en/articles/5071983-integrating-with-wisk-for-pos-providers)
- [OpenAPI](openapi/wisk-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wisk-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wisk-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WISK Webhooks

No public, documented webhook or event-subscription surface is published by WISK as of this catalog date. Event-driven exchange with POS partners is arranged through WISK's partner integration process rather than a self-serve webhooks API. Documented here for completeness and reconciled false.

- **Human URL:** [https://www.wisk.ai/pos](https://www.wisk.ai/pos)

#### Tags

- Webhooks
- Events

#### Properties

- [Documentation](https://help.wisk.ai/en/articles/5071983-integrating-with-wisk-for-pos-providers)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/wisk)
- [Website](https://www.wisk.ai/)
- [Documentation](https://help.wisk.ai/)
- [Plans](plans/wisk-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/wisk-ai-rate-limits.yml)
- [Fin Ops](finops/wisk-ai-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
