# Initiative suite review

Reviewed October 31, 2026. The suite now separates lasting narrative intent, evolving requirements, and reconciliation against evidence. This review found and repaired handoff and ownership gaps without changing the requirements template structure.

## Scope and method

Reviewed all three skills, the four requirements references, both starter examples, the template, README, philosophy, and contribution instructions. The review used sequential manual passes: contract inspection, complete user journeys, adversarial scenarios, and a final consistency pass. These are tabletop walkthroughs of the written instructions, not independent agent executions or evidence from real delivery.

## Findings and repairs

| Finding | Repair |
| --- | --- |
| Reconciliation checked a single product document and could miss narrative drift. | Added separate narrative and requirements checks, explicit missing-input limits, and owner decisions for intent changes. |
| Requirements drafting did not explicitly surface conflicts with narrative intent. | Added a consistency check before review and a handoff to reconciliation for new evidence. |
| Narrative revision did not explicitly cover changed beneficiaries or success, or trigger requirements review. | Aligned intent-change decisions across skills and added the downstream requirements check. |
| Contribution instructions assumed every change affected a feature or milestone. | Made document and section the primary reference, with feature and milestone labels where relevant. |
| README required epic and Slack links while the skill treated metadata as optional. | Made those links optional without changing template fields. |
| Closure guidance outside reconciliation could equate shipping with success or omit confirmation. | Aligned closure on requirements, narrative outcomes, unknown results, and confirmed archival of requirements. The existing Closure section holds the comparison. |

## Pass 1: Contracts and resources

Checked discovery descriptions, resource paths, and the responsibilities assigned to each skill. Requirements resources remain inside their skill directory. Other skills are referenced by name with availability qualifications, so an installed skill does not depend on repository-relative sibling paths.

The template retains Features, Delivery Plan, Open Items, and Closure. API and UI guidance remains conditional. The examples remain explicitly untested starter sketches. Feature labels use `F1`, `F2`, and so on without renumbering existing features.

## Pass 2: Complete user journeys

The following inputs are hypothetical review fixtures, not new canonical initiative examples.

| Journey and input | Walkthrough result after repairs |
| --- | --- |
| Notes to narrative to requirements: reviewers should spend less time resolving duplicate customer records. Notes also propose a particular screen and delivery date. | Narrative writing keeps the benefit and proposed success measures. Screen and date details pass to requirements without becoming approved commitments. Requirements link the narrative and seek missing behavior details. |
| Existing narrative to a different solution: replace a review screen with an integration that achieves the same reviewer outcome. | Requirements can change with approval. Reconciliation checks the same beneficiaries and outcome, so the solution change alone does not trigger a narrative rewrite. |
| Requirement conflicts with intent: a proposed shortcut removes explanations, while the narrative requires reviewers to understand match recommendations. | Define Requirements surfaces the conflict for an owner decision before treating the shortcut as agreed. It does not silently weaken the narrative. |
| Explicit purpose change: the owner chooses to prioritize integration operators rather than reviewers and authorizes document edits. | Reconciliation identifies the intent change and its source. Narrative revisions remain explicit, and affected requirements return for review. Existing approval covers only the changes actually decided. |
| Closure and later work: matching features shipped, but reviewer time has not been measured. | Closure records delivered behavior and the unknown outcome in the existing section. The narrative is not rewritten to imply success. Requirements archive after confirmation, and later work links back. |

These journeys exposed the requirements consistency check and the missing downstream review after narrative changes. Both are repaired.

## Pass 3: Adversarial and partial inputs

| Scenario | Walkthrough result after repairs |
| --- | --- |
| Narrative missing, requirements and a PR available. | Check the PR against requirements. Report that narrative alignment could not be checked. Do not invent a narrative or claim full alignment. |
| Requirements missing, narrative and discussion available. | Check the discussion against intent. Keep the missing requirements comparison explicit. Requirements drafting is a separate handoff. |
| A source link is inaccessible. | Retain uncertainty and ask for relevant source material. A linked but unread source does not prove a decision. |
| A merged PR changes an agreed empty result into an error. | Treat it as implementation evidence of a mismatch, not approval. Propose a resolution with the source and affected feature. |
| A later engineer message conflicts with an earlier owner decision. | Expose the conflicting evidence. Recency alone does not establish a replacement agreement. Seek the unresolved owner decision. |
| A source already contains explicit owner approval and the user requests the covered edit. | Apply the authorized change without requiring duplicate approval. Do not extend that approval to unrelated narrative or requirement changes. |
| `F1` is deferred while `F2` still supports milestone `M1`. | Preserve labels and update affected references. Do not renumber `F2` for appearance. Record deferred work at closure. |
| Only one skill is installed. | Local resources remain usable. Named handoffs are optional. Define Requirements still exposes unmeasured outcomes and requires confirmation before archival when reconciliation is unavailable. |

The standalone closure case exposed a remaining gap in Define Requirements after the first repairs. The final wording now includes the outcome comparison directly.

## Pass 4: Final verification and stopping point

Replayed the journeys and partial-input cases against the repaired instructions. Checked both directions of narrative and requirements changes, evidence classification, approval scope, labels, source preservation, and closure. This pass found no new material conflict in the covered scenarios.

All three skills pass the skill validator. Local Markdown links resolve, skill resource links remain local to their skill, and template and example label references resolve. No old skill name, old feature label, or em dash remains in the maintained Markdown. Diff formatting checks pass.

## Remaining limits and choices

The suite has not been tested through actual team delivery. The walkthroughs do not prove that an agent will follow every instruction or that the template needs no further work. Keep the template stable until use supplies evidence for changes.

The suite records unknown outcomes at closure but does not assign a mandatory follow-up owner, schedule, or measurement document. Decide those arrangements for an initiative when needed. No additional skill or required process is justified by this review.

## Follow-up: Supporting definitions

A subsequent user clarification established that the two canonical documents can reference supporting artifacts that define finer product details. The earlier review did not test that model explicitly. Updated all three skills, README, philosophy, contribution guidance, and API and UI references. The template received wording changes in its existing feature introduction and Supporting artifacts placeholder, with no structural change.

The following hypothetical walkthroughs check the revised instructions. These are manual checks, not executions against external design or API tools.

| Input | Walkthrough result |
| --- | --- |
| `F1` requires reviewers to inspect a rationale before deciding. A linked agreed mockup defines interaction details but hides the rationale until after the decision. | Define Requirements links the mockup and states its role. Reconciliation identifies the conflict and proposes coordinated changes for an owner decision. Neither form automatically wins. The chosen design can retain finer interaction details without copying them all into requirements. Narrative intent remains unchanged if the reviewer outcome still holds. |
| `F1` links an agreed schema with `candidates: []` for no matches, but a linked agreed API example uses `candidates: null`. The owner confirms the array contract and authorizes the correction. | Reconciliation identifies the conflicting definitions, preserves the decision source, and proposes correcting the example. The broad requirement and narrative need no change. The schema and corrected example continue to carry the fine detail. A merged implementation returning `null` remains mismatch evidence, not a replacement agreement. |
| The affected mockup or API example cannot be opened, or its agreement status is unknown. | Report the unverified definition and missing comparison. Request access or relevant content, and keep any proposed edit conditional. A link alone does not establish approval or prove consistency. |

Rechecked skill validation, local links, portability, labels, and formatting after these changes. The template's section structure remains intact. No new mandatory artifact type, approval hierarchy, or document format was added. Real delivery use remains untested.
