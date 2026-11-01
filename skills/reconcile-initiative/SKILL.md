---
name: reconcile-initiative
description: Compare an initiative's narrative, living requirements, and affected supporting artifacts with new decisions, discussions, or delivery evidence. Detect drift and propose coordinated, traceable updates for product-owner review.
---

# Reconcile Initiative

## Inputs

The canonical filenames are `initiative-<initiative-name>.md` for the narrative and `prd-<initiative-name>.md` for requirements.

Use the initiative's narrative, canonical requirements, affected linked artifacts, and available transcripts, discussions, pull requests, or delivery evidence. The narrative and requirements are the canonical documents. Supporting artifacts can define finer product details without duplicating them in requirements prose. Ask for missing sources rather than claiming access. If either document, an affected artifact, or relevant evidence is unavailable, state what cannot be checked and continue the checks that the available material supports.

## Process

1. Read both documents and affected linked artifacts when available. Identify the narrative's purpose, intended outcome, beneficiaries, and meaning of success. Identify affected requirements, feature labels such as `F1`, milestones, and open items. Determine which artifacts provide agreed definitions, proposals, illustrations, or implementation evidence from the available context. Do not infer agreement from a link alone.
2. Separate **explicit decisions**, **proposals**, **observations**, and **implementation evidence**. Identify who made a decision and what it covers. Quote or link source context where available. Flag contradictory evidence without treating the latest message or implemented behavior as the agreed direction.
3. Check whether requirements, supporting definitions, and new evidence remain consistent with the narrative's lasting intent. A different solution or evolving requirement does not by itself justify rewriting the narrative. Flag apparent drift and distinguish a change in how the outcome is achieved from a proposed change in purpose, outcome, beneficiaries, or success.
4. Compare requirements and agreed supporting definitions with each other and the evidence. Identify changes to behavior, scope, acceptance criteria, priorities, milestones, and open items. Flag conflicting mockups, API examples, or other definitions rather than automatically giving one form precedence. Distinguish implementation mismatches from approved changes to the agreement.
5. Propose coordinated changes with the affected document or artifact, section or identifiable element, existing content, suggested change, reason, source, and downstream effects. Changes may belong in an artifact without duplicating its detail in requirements prose. Include affected links and state when a checked document or artifact needs no change. Keep missing checks and unresolved conflicts visible, including in requirements Open Items when appropriate. Do not turn the documents into a comprehensive meeting log.
6. Require an explicit product-owner decision before changing narrative intent or substantive product definitions, including details in supporting artifacts. A genuine purpose or outcome change must be decided explicitly, not inferred from a requirements or artifact edit. Existing explicit approval can support the edit it covers when the user has authorized applying it. Otherwise request the missing decision before applying the change. Silence and a merged PR do not establish approval.
7. Apply authorized, approved changes to canonical sections, affected supporting artifacts, and references. Preserve stable feature labels and source links. Update milestone status only where evidence supports it. If narrative intent changes, flag affected requirements and supporting definitions for review rather than assuming they still fit.
8. At general availability (GA) or agreed closure, compare delivery with requirements, agreed supporting definitions, and narrative success. Distinguish shipped behavior from demonstrated outcomes and unknown results. Record that comparison in the existing requirements Closure section. Check outstanding items and deferred work, then archive requirements only after confirmation. Do not rewrite the narrative to make delivery appear successful.

## Rules

- The narrative expresses lasting intent. Requirements and agreed supporting definitions express the current product agreement. Code provides implementation evidence. None automatically overrides the others.
- The product owner owns substantive product decisions, including changes to narrative intent.
- Preserve source links and version history without creating competing records.
- Be explicit about uncertainty, missing access, and unverified progress. A partial check is not confirmation that the documents and delivery agree.
