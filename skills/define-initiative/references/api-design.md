# API initiative reference

Use only when an initiative exposes an API or interface contract.

Consider: endpoint purpose; consumer and workflow; request/response field semantics, requiredness and types; error behavior; pagination and idempotency if relevant; authentication and authorization; compatibility and versioning; latency and reliability promises; representative success, no-result, invalid-input and ambiguous cases.

Product-significant schema fields can live in a capability's optional **Interface Specification** table. For large schemas, link an engineering-owned OpenAPI file instead of duplicating it. Include a few canonical examples inline; put extensive input/output cases in a linked examples file. Examples should distinguish normative expectations from illustration and can later inform tests.
