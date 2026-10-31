# Product Playbook

An opinionated, initiative-scoped way to define and deliver software products in an agentic engineering environment.

**One initiative, one living product document, one bounded delivery lifecycle.** The product manager owns the document; engineers challenge and contribute; AI proposes changes but does not silently redefine the product.

Read the thinking behind it: [Keeping decisions, requirements, and delivery in sync](docs/philosophy/README.md).

## Start here

1. Write a **narrative** in whatever form best conveys the outcome: announcement, blog post, customer story, or vision. Include desired outcome and success metrics. See [narrative guidance](skills/define-initiative/references/product-narratives.md).
2. Copy [the initiative template](skills/define-initiative/assets/initiative-template.md) into your initiative as `product.md`. Link the narrative, epic, and Slack channel.
3. Work through capabilities, delivery milestones, and open items with the team. Use [Define Initiative](skills/define-initiative/SKILL.md) for a guided interview.
4. Reconcile new evidence from meetings, Slack, PRs, and Jira using [Reconcile Initiative](skills/reconcile-initiative/SKILL.md). The PM approves substantive product changes.
5. At GA, summarize what shipped and what was deferred, then archive. Subsequent iterations get a new initiative linked to the old one.

## Repository map

- [docs/philosophy/](docs/philosophy/README.md): the thinking behind the method.
- `skills/`: portable, focused agent skills for defining and reconciling initiatives.
- `skills/define-initiative/references/`: narrative, API, UI, acceptance, and milestone guidance, plus starter sketches.
- `skills/define-initiative/assets/`: the canonical initiative document template.
- `CONTRIBUTING.md`: ownership and contribution rules.

This is not a universal PRD standard. Keep it lightweight, useful to humans, and easy to revise.

## Improve through use

This playbook is a starting skeleton. Use it on real initiatives, notice recurring friction, and bring proven improvements back into the template and skills. The current example files are starter sketches; add or replace them with examples tested through actual delivery and reconciliation.
