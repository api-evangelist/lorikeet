# Lorikeet (lorikeet)

Lorikeet (Lorikeet CX) is an AI customer support agent built for complex and regulated businesses across chat, email, and voice. Rather than a single chatbot, it uses a workflow / "skills"-based orchestration layer that follows a company's standard operating procedures, calls into helpdesks (Zendesk, Intercom, Front) and internal systems through typed, no-code tools, and produces a per-step audit trail. Its programmatic surface centers on conversations, inbound and outbound webhooks / events, actions/tools, and knowledge ingestion, secured with scoped Bearer/API-key credentials.

> **Honesty note:** Lorikeet's authoritative API reference at `docs.lorikeetcx.ai` is gated behind a customer access code. The base URL, endpoints, and schemas in this catalog entry are **modeled** from Lorikeet's public integration and security materials and common conventions for this class of AI support agent. Treat them as a best-effort model to reconcile against the official reference, not a field-verified contract.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/apis.yml)

## Tags

- AI
- Customer Support
- AI Agent
- Support Automation
- Workflows
- Helpdesk

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Lorikeet Conversations API

Programmatically create and continue conversations (support tickets) with the Lorikeet AI agent, post end-user and agent messages, and retrieve conversation state and resolution.

- **Human URL:** [https://docs.lorikeetcx.ai/guides/quickstart](https://docs.lorikeetcx.ai/guides/quickstart)
- **Base URL:** `https://api.lorikeetcx.ai/v1`

#### Tags

- Conversations
- Support Tickets
- AI Agent

#### Properties

- [Documentation](https://docs.lorikeetcx.ai/guides/quickstart)
- [OpenAPI](openapi/lorikeet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lorikeet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lorikeet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lorikeet Messages API

Append and list messages within a conversation, carrying end-user input and the agent's replies. Messages drive the workflow orchestration layer forward toward resolution or human handoff.

- **Human URL:** [https://docs.lorikeetcx.ai/guides/quickstart](https://docs.lorikeetcx.ai/guides/quickstart)
- **Base URL:** `https://api.lorikeetcx.ai/v1`

#### Tags

- Messages
- Conversations
- Chat

#### Properties

- [Documentation](https://docs.lorikeetcx.ai/guides/quickstart)
- [OpenAPI](openapi/lorikeet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lorikeet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lorikeet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lorikeet Webhooks & Events API

Register and manage webhook subscriptions and receive Lorikeet events (conversation created, updated, resolved, escalated / handoff). Lorikeet supports inbound HMAC-signed webhooks that are cryptographically verified before the agent acts, and outbound async request/response callbacks so internal APIs are never exposed to the open internet.

- **Human URL:** [https://www.lorikeetcx.ai/articles/ai-support-secure-api-webhook-integrations-2026](https://www.lorikeetcx.ai/articles/ai-support-secure-api-webhook-integrations-2026)
- **Base URL:** `https://api.lorikeetcx.ai/v1`

#### Tags

- Webhooks
- Events
- HMAC

#### Properties

- [Documentation](https://www.lorikeetcx.ai/articles/ai-support-secure-api-webhook-integrations-2026)
- [OpenAPI](openapi/lorikeet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lorikeet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lorikeet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lorikeet Actions & Tools API

Lorikeet's "tools" primitive — typed actions with defined inputs and outputs and optional JavaScript output transforms, built no-code in the UI — lets the agent call into your systems (via synchronous scoped-credential API, inbound webhook, or outbound async callback) and chain multiple typed actions across systems. This surface is configured primarily in the Lorikeet UI; any programmatic management is not publicly documented.

- **Human URL:** [https://www.lorikeetcx.ai/articles/ai-support-secure-api-webhook-integrations-2026](https://www.lorikeetcx.ai/articles/ai-support-secure-api-webhook-integrations-2026)
- **Base URL:** `https://api.lorikeetcx.ai/v1`

#### Tags

- Actions
- Tools
- Integrations

#### Properties

- [Documentation](https://www.lorikeetcx.ai/articles/ai-support-secure-api-webhook-integrations-2026)
- [OpenAPI](openapi/lorikeet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lorikeet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lorikeet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lorikeet Knowledge Ingestion API

Ingest and manage the knowledge sources (help-center articles, documents, URLs) the agent draws on when following workflows. Public materials confirm knowledge is a first-class concept; the exact ingestion endpoints are access-gated and modeled here honestly rather than asserted as verified.

- **Human URL:** [https://docs.lorikeetcx.ai/guides/quickstart](https://docs.lorikeetcx.ai/guides/quickstart)
- **Base URL:** `https://api.lorikeetcx.ai/v1`

#### Tags

- Knowledge
- Ingestion
- Documents

#### Properties

- [Documentation](https://docs.lorikeetcx.ai/guides/quickstart)
- [OpenAPI](openapi/lorikeet-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lorikeet.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lorikeet.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/lorikeetcx)
- [Website](https://lorikeet.ai)
- [Documentation](https://docs.lorikeetcx.ai/guides/quickstart)
- [Plans](plans/lorikeet-plans-pricing.yml)
- [Rate Limits](rate-limits/lorikeet-rate-limits.yml)
- [Fin Ops](finops/lorikeet-finops.yml)

> **GitHub:** No official Lorikeet CX GitHub organization was found. A `github.com/Lorikeet` org exists but is an unrelated 2014-era namesake, so `GitHubOrganization` is intentionally omitted from `apis.yml`.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
