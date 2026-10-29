---
name: define-initiative
description: Interview a product owner to draft a flexible product narrative and a structured initiative-scoped living product document.
---

# Define Initiative

## Goal

Help a product owner establish shared human intent, not instructions for a coding agent.

## Process

1. Ask whether a narrative exists. If not, consult [narrative guidance](references/product-narratives.md) and ask concise, conversational questions about the customer, problem, desired end state, why now, and success measures. Offer formats (announcement, blog post, customer story, vision memo); do not mandate one.
2. Confirm the narrative's essential intent before detailing requirements. Mark unknowns explicitly; don't fabricate decisions.
3. Copy the structure in [the initiative template](assets/initiative-template.md). Ask for initiative metadata only when useful. Consult the [API example](references/examples/api-initiative.md) or [UI example](references/examples/ui-initiative.md) when a worked example would help.
4. Elicit **capabilities** one at a time: expected behavior, important constraints, and acceptance criteria. Challenge ambiguous outcomes, premature technical prescriptions, and requirements that are really implementation tasks.
5. Detect the initiative type. For an API, consult [API guidance](references/api-design.md); for a UI change, consult [UI guidance](references/ui-changes.md). Consult [acceptance criteria](references/acceptance-criteria.md) and [delivery milestones](references/delivery-milestones.md) when helpful. Don't dump checklists on the user.
6. Propose outcome-oriented delivery milestones tied to capability IDs. Collect only consequential open questions.
7. Present drafts for product-owner review. Preserve a single canonical initiative document and link large supporting examples/specs instead of duplicating them.

## Rules

- PM owns substantive product decisions. Do not claim approval from silence.
- Keep narrative separate and flexible; keep the initiative document structured.
- Keep unknowns visible and avoid forced completeness.
- No compulsory meeting journal or standalone decision log.
- Initiative ends at GA/agreed closure; later iterations start fresh and link back.
