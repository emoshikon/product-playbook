# Customer Matching API

> Starter sketch illustrating the document structure. This has not been tested in real delivery and does not establish the level of detail an initiative needs.

Save as `prd-customer-matching-api.md`.

**Status:** Draft  
**Product Owner:** @pm  
**Engineering Lead:** @lead  
**Narrative:** [Link to `initiative-customer-matching-api.md`]

## 1. Features

### F1: Find candidate matches

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

### M1: Validate matching behavior on representative cases
- **Outcome:** Demonstrate candidate matching and no-match behavior.
- **Features:** F1
- **Status:** Planned
- **Completion evidence:** Reviewed example cases and evaluation results.

### M2: Make the matching API generally available
- **Outcome:** Intended consumers can use F1 with the agreed matching, no-match, and error behavior.
- **Features:** F1
- **Status:** Planned
- **Completion evidence:** Contract checks against agreed schemas and examples, consumer validation, and evidence against narrative success measures with unmeasured outcomes explicit.
- **Dependencies / blockers:** Agree on confidence semantics and field representation for F1 before finalizing the contract.

## 3. Open Items

1. What confidence semantics and consumer-facing field name should F1 use? The contract and M2 depend on this agreement.

## 4. Appendix: Rejected ideas and decisions

_None yet._
