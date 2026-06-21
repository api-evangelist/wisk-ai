# WISK (wisk-ai)

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
