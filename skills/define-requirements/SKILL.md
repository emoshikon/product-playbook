---
name: define-requirements
description: Draft or refine structured living requirements for an initiative, including features, acceptance criteria, delivery milestones, and open items. Use for requirements definition rather than narrative writing or evidence reconciliation.
---

# Define Requirements

## Goal

Help a product owner express the current agreement about what the product must do. Requirements evolve as the team learns, while the separate narrative expresses lasting purpose and intended outcome.

The narrative and requirements are the canonical documents, supported by linked artifacts such as mockups, API examples, schemas, or other suitable definitions. Requirements and agreed supporting definitions specify the product together. Requirements prose need not repeat every detail.

## Process

1. Read the narrative, existing requirements, and relevant linked artifacts when available. Use the intended outcome to guide requirements work. For narrative drafting or revision, use `write-initiative-narrative` when available. If no narrative is available, clarify enough intent to discuss requirements and keep missing intent explicit. Flag inaccessible supporting definitions rather than assuming their contents.
2. Use [the requirements template](assets/initiative-template.md) for a new document. Save requirements as `prd-<initiative-name>.md`. Link the narrative at `initiative-<initiative-name>.md`. Refine the canonical requirements when they already exist. Ask for metadata only when useful. Consult the [API example](references/examples/api-initiative.md) or [UI example](references/examples/ui-initiative.md) when a worked example would help.
3. Work from the available material to define **features**: expected behavior, important constraints, and acceptance criteria. Ask focused questions where missing information changes a requirement. Challenge ambiguous behavior, premature technical prescriptions, and requirements that are really implementation tasks.
4. For an API, consult [API guidance](references/api-design.md). For a UI change, consult [UI guidance](references/ui-changes.md). Consult [acceptance criteria](references/acceptance-criteria.md) and [delivery milestones](references/delivery-milestones.md) when helpful. Use relevant guidance without turning it into a compulsory checklist.
5. Propose outcome-oriented delivery milestones linked to feature labels such as `F1` and `F2`. The last milestone defines initiative completion, including general availability (GA) where applicable, through its outcome and completion evidence. Keep Open Items as a simple numbered list of consequential issues, questions, and dependencies. Remove resolved items after updating the agreement.
6. Check proposed requirements and supporting definitions against each other and the narrative's intended outcome, beneficiaries, and meaning of success. Surface conflicts for a product-owner decision rather than silently changing agreed intent. Present proposed requirements and affected artifact changes for review. Keep one canonical requirements document with clear links from relevant features to supporting artifacts. Briefly identify what each artifact defines and whether it is agreed, proposed, or illustrative. Preserve useful links without copying all artifact content into prose.

## Rules

- The product owner owns substantive product decisions. Do not claim approval from silence.
- Keep the narrative separate and flexible. Keep requirements structured and open to revision as agreements change.
- Use simple feature labels such as `F1` and `F2`. Preserve existing labels and update references consistently when a label changes.
- Feature definitions describe agreed product behavior independent of release scheduling. Never include milestones, milestone labels, release membership, or milestone assignments in feature definitions. Only milestone entries identify included features through their existing **Features** field.
- Distinguish agreed requirements and supporting definitions from proposals, illustrations, assumptions, and implementation evidence. A link alone does not establish agreement. Substantive product changes require an explicit product-owner decision regardless of which artifact contains the detail.
- Keep unknowns visible and avoid forced completeness.
- Update requirements directly to state the current agreement without narrating edits. Keep useful source links and version history for traceability.
- Use the PRD appendix selectively for rejected ideas and decisions made, with useful rationale or context. Keep unresolved proposals in Open Items rather than presenting them as decisions. Do not add an appendix entry for every edit or turn it into a chronological change log.
- For comparing new discussions or delivery evidence with the documents and supporting artifacts, use `reconcile-initiative` when available. Preserve evidence and uncertainty if that skill is unavailable.
- Assess completion through the final milestone's agreed outcome and evidence. Distinguish shipped behavior from demonstrated outcomes and unknown results. Later initiatives link back to the preceding initiative.
