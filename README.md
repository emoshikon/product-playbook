# Product Playbook

An opinionated, initiative-scoped way to define and deliver software products in an agentic engineering environment.

**One initiative, two canonical documents, one bounded delivery lifecycle.** A flexible narrative expresses lasting purpose and intended outcome. Structured living requirements capture the current product agreement. The product owner owns both documents. Engineers challenge and contribute. AI proposes changes but does not silently redefine the product.

The canonical documents can reference supporting artifacts such as mockups, API examples, schemas, or other suitable definitions. Requirements and agreed supporting definitions specify finer details together without copying every detail into requirements prose.

Read the thinking behind it: [Keeping decisions, requirements, and delivery in sync](docs/philosophy/README.md).

## Start here

1. Explore or write a **narrative** with [Write Initiative Narrative](skills/write-initiative-narrative/SKILL.md). Use whatever form conveys who benefits, the lasting change for them, why it matters, and what success means.
2. Copy [the requirements template](skills/define-requirements/assets/initiative-template.md) into your initiative as `product.md`. Link the narrative. Add epic or discussion links when useful.
3. Work through capabilities, delivery milestones, and open items with the team. Link supporting artifacts and identify what they define. Use [Define Requirements](skills/define-requirements/SKILL.md) to draft or refine the agreement.
4. Check both documents and affected supporting artifacts against new evidence using [Reconcile Initiative](skills/reconcile-initiative/SKILL.md). The product owner decides substantive changes wherever the product definition lives.
5. At general availability (GA) or agreed closure, compare delivery with requirements and narrative success. Record deferred work and unknown outcomes. Archive requirements after confirmation. Subsequent iterations get a new initiative linked to the old one.

## Repository map

- [docs/philosophy/](docs/philosophy/README.md): the thinking behind the method.
- `skills/`: portable, focused agent skills for writing narratives, defining requirements, and reconciling initiatives.
- `skills/define-requirements/references/`: API, UI, acceptance, and milestone guidance, plus starter sketches.
- `skills/define-requirements/assets/`: the canonical requirements template.
- `CONTRIBUTING.md`: ownership and contribution rules.

This is not a universal PRD standard. Keep it lightweight, useful to humans, and easy to revise.

## Improve through use

This playbook is a starting skeleton. Use it on real initiatives, notice recurring friction, and bring proven improvements back into the template and skills. The current example files are starter sketches; add or replace them with examples tested through actual delivery and reconciliation.
