# Taller Academy — Module 8: Name What You Already Own

**Lab:** Name What You Already Own  
**Project area:** Backend Engineering — GraphQL Integrations  
**Self-assessed ownership:** Level 2, with demonstrated Level 3 behaviors  
**Evidence:** Self-reported activities; confidential client records are not reproduced.

## Exercise 1 — Ambiguity Recall

### Three ambiguities managed in the last two weeks

| # | Unspecified issue | Action | Communication |
|---|---|---|---|
| 1 | An external backend dependency failed during GraphQL integration work, and the assigned task did not cover how to proceed. | Investigated failing calls, recorded the technical evidence, and identified the responsible team rather than claiming to fix its service. | Findings documented and shared via the established channels. |
| 2 | QA requirements did not fully define which additional integration scenarios to validate. | Selected additional tests to assess the relevant behavior. | Validation approach and findings communicated through team tracking. |
| 3 | Scope or task priority required clarification. | Raised the ambiguity and sought a decision from the appropriate owner rather than changing business priorities unilaterally. | The need for clarification was communicated. |

**Two counts:**

- Ambiguities resolved or brought to an actionable decision: **3**
- Those communicated to others: **3**
- Uncommunicated decisions: **0**
- Communication rate: **3 / 3 = 100%**

The third case was resolved through appropriate clarification/escalation rather than an independently made priority decision. These three cases are the selected resolved or clarified instances; a GraphQL edge-case area was also considered during initial recall but is not counted as an additional verified resolution.

**Ownership reflection:** My baseline is Level 2 because I own assigned work through completion. Investigating unspecified dependencies, deciding appropriate QA checks, and ensuring scope questions reach a decision-maker demonstrate Level 3 behaviors. These examples do not establish that I own an entire workstream.

**Two-week habit:** Whenever I resolve a reversible technical ambiguity within my authority, I will write one line in the ticket covering the decision and reasoning and notify the relevant people. When a decision affects other teams, compliance, money, or sensitive data, I will ask for approval rather than decide silently.

## Exercise 2 — Extend One Boundary

**Assigned task:** Investigate an external backend service error affecting a GraphQL integration.

**One step beyond:** After identifying the affected dependency, I checked whether the same failure pattern affected other integrations. I kept the extra check narrowly scoped instead of starting an unrelated investigation.

**Observed result:** **No additional related integration issues were identified.** This does not mean the original external-service defect was fixed.

**Record:** The additional check and its outcome were documented in Jira, according to my work record.

**Why it demonstrates ownership:** I looked one step beyond the originally failing interaction, assessed a related risk, and made the negative finding available to the team rather than simply closing the assigned task.

**Sanitized closing-comment example (illustration, not a verbatim private Jira comment):**

> **What I did:** Investigated an external dependency failure and checked whether the same observed pattern affected other integrations.  
> **Why:** A shared dependency might cause similar failures outside the initial operation.  
> **Result:** No additional affected integration was identified during the bounded check. The dependency owner remains responsible for any underlying fix.  
> **For whoever is next:** Confirm external-service resolution and validate the affected flow in the approved QA environment. Do not infer that unrelated integrations were exhaustively tested.

## Exercise 3 — Glue Work Audit

### Last month's collaboration

| Glue work | Contribution | Record visibility |
|---|---|---|
| Pull request reviews | Supported change quality and shared technical reasoning. | Recorded in the established Jira/PR process. |
| Troubleshooting | Helped investigate backend and integration problems. | Recorded. |
| Technical meetings | Contributed context and coordinated technical work. | Recorded. |
| Documentation | Preserved useful explanations for other engineers. | Recorded. |
| Mentoring | Provided technical guidance to teammates. | Recorded. |

These are **five categories**, not a claimed count of individual interventions. The learner confirmed that all have existing records; private URLs and ticket details are intentionally not public.

### Two most valuable glue-work contributions

**1. PR reviews.** Reviews made implementation concerns and feedback visible to other developers. Their durable record is in the existing code-review/tracking workflow.

**2. Troubleshooting.** Investigations helped clarify external-service blockers and support the engineers responsible for follow-up. These findings were written down rather than left only in informal conversations.

### Turn a repeated explanation into an artifact

**Existing internal artifact:** External service troubleshooting guidance in Jira or internal team documentation, as reported by the learner. It has not been copied into this public repository.

**Public, sanitized companion:** [External Service Troubleshooting Guide](docs/EXTERNAL_SERVICE_TROUBLESHOOTING.md). This repository version is a newly authored educational reference, not a claim to reproduce the restricted internal document. It lays out a repeatable, bounded investigation and communication approach.

**Avoiding the glue trap:** I will keep documenting reviews, troubleshooting, meetings, and mentoring while continuing to ship concrete GraphQL-related tasks.

## Final reflection

My self-assessed level remains **Level 2**, but I have evidence of **Level 3 behaviors**: managing three ambiguities, communicating all three, identifying a related integration risk beyond the ticket boundary, and making collaboration discoverable. My next goal is to participate earlier in defining technical scope, dependencies, and success criteria, while escalating decisions outside my authority.

## Self-check

- [x] Selected three managed ambiguities and documented the response to each.
- [x] Counted three managed ambiguities and three communicated outcomes.
- [x] Set a two-week decision-reporting habit.
- [x] Extended one task boundary and recorded its negative finding in Jira.
- [x] Audited five glue-work categories and their visibility.
- [x] Highlighted two significant glue-work contributions.
- [x] Identified existing internal documentation and provided a separate public reference.
- [ ] Independently inspect private Jira records against this sanitized summary, if an authorized reviewer requires more detail.

**Data handling:** No client identities, private Jira references, internal service names, proprietary code, or customer data are published.
