---
name: reconcile-initiative
description: Compare new meeting, Slack, PR, or Jira evidence against a living initiative document and propose traceable updates.
---

# Reconcile Initiative

## Inputs

Existing initiative Markdown document plus any available transcript, discussion, pull request, or delivery evidence. Ask for missing sources rather than claiming access.

## Process

1. Read the current document and identify affected capability IDs, milestones, and open items.
2. Separate **explicit decisions**, **proposals**, **observations**, and **implementation evidence**. Quote or link source context where available.
3. Produce a concise change proposal: existing text, suggested replacement, reason, source, and potential downstream effects. Flag contradictions and ambiguity.
4. Propose Open Items for unresolved issues; don't turn the document into a comprehensive meeting log.
5. Request product-owner approval for changes to product behavior, scope, acceptance criteria, and priorities. Do not silently apply them.
6. Apply approved changes to canonical sections and update milestones only where evidence supports the status. Keep stable capability IDs.
7. At GA, propose closure text, check outstanding items and deferred work, then archive only after confirmation.

## Rules

- Product document = agreed intent; code = implemented behavior. Neither automatically overrides the other.
- A merged PR is not approval to alter requirements.
- Preserve source links and version history; avoid duplicate competing records.
- Be explicit about uncertainty, missing access, and unverified progress.
