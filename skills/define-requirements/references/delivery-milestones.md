# Delivery milestones

Milestones should unlock a demonstrable feature or reduce an important risk, not merely describe tasks. Link to feature labels such as `F1` and `F2`, note evidence needed to validate completion, and update progress from reliable engineering signals. A merged PR is evidence, not proof of customer validation. Dates are optional, but explicit when commitments exist.

Each milestone lists included feature labels in its **Features** field. Feature definitions describe agreed behavior independently of release scheduling and never mention milestones, milestone labels, release membership, or milestone assignments. Moving a feature between milestones updates membership in the milestone entries while leaving the feature definition unchanged.

The last milestone represents completion of the initiative, including general availability (GA) where applicable. Use its existing **Outcome** field to define what must be available or achieved. Use **Completion evidence** to show whether that outcome holds, with **Features**, **Status**, **Target**, and **Dependencies / blockers** as relevant. Keep these expectations in the plan rather than adding a separate completion workflow.

Distinguish shipped behavior from demonstrated user outcomes. Compare the evidence with requirements, agreed supporting definitions, and narrative success. Keep unknown results explicit without treating them as proof of success. Missing evidence required by the milestone prevents marking it complete. If an outcome will be measured later, make that limit clear in the milestone's expectations.
