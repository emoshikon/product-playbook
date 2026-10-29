# Customer Matching API

**Status:** Draft  
**Product Owner:** @pm  
**Engineering Lead:** @lead  
**Narrative:** [Launch story](../product-narratives.md) (illustrative placeholder)

## 1. Capabilities

### CAP-001 — Find candidate matches

**Expected behavior**
- Given a customer record, return potential matching records with explainable confidence.
- Return an empty result when no candidates meet the agreed threshold.

**Requirements and constraints**
- Consumers must be able to distinguish an empty result from a service error.
- Exact field names and schema remain open pending engineering collaboration.

**Acceptance criteria**
- Valid records produce a well-formed response, including an empty list where appropriate.
- Invalid inputs produce a documented error response.

**Supporting artifacts**
- [API guidance](../api-design.md); add a linked OpenAPI specification and examples when agreed.

## 2. Delivery Plan

### M1 — Validate matching behavior on representative cases
- **Outcome:** Demonstrate candidate matching and no-match behavior.
- **Capabilities:** CAP-001
- **Status:** Planned
- **Completion evidence:** Reviewed example cases and evaluation results.

## 3. Open Items

### ITEM-001 — Confidence representation
- **Type:** Question
- **Context and proposal:** Agree on confidence semantics and consumer-facing field name.
- **Related to:** CAP-001
- **Owner:** @pm
- **Status:** Open

## 4. Closure

_To be completed at GA._
