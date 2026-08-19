# Learning Path

Use this when creating, reviewing, or closing a finite training plan for a user.

The program is finite, but not based on a fixed number of cases. A level is complete when the user repeatedly demonstrates the required competencies in realistic cases.

## Core Principle

Do not keep saying "let's do one more case" without explaining what the user is trying to prove. Every session should connect to:

- current target level.
- target competencies.
- evidence already observed.
- remaining gaps.
- next best practice block.
- exit criteria for the level.

## Level Completion

A level can be marked complete when the user shows stable performance across the required competencies:

- at least 2-3 successful observations per competency.
- no repeated unresolved critical gap for that level.
- ability to explain the decision, assumptions, accepted risk, and next signal.
- performance holds across at least two case families or domains, unless the user wants domain-specific training only.

Do not graduate the user after one strong answer. Do not block graduation forever because of minor style issues.

## Level Exit Criteria

L1 is complete when the user can:

- explain basic product metrics in plain language.
- read a simple funnel.
- distinguish product problem, solution, feature, and metric.

L2 is complete when the user can:

- identify the most suspicious funnel or metric step.
- choose a relevant success metric.
- propose a simple bounded action or check.
- avoid obvious metric traps such as optimizing clicks while ignoring downstream value.

L3 is complete when the user can:

- generate multiple plausible hypotheses.
- request useful segments or cuts without asking for unlimited data.
- notice data-quality issues.
- define success and guardrail metrics.
- make a directional decision under imperfect evidence.

L4 is complete when the user can:

- prioritize initiatives across impact, risk, effort, and business context.
- design rollout plans with constraints and guardrails.
- handle stakeholder conflict without losing the product goal.
- name opportunity cost and accepted trade-offs.
- decide what to do now and what to learn next.

L5 is complete when the user can:

- reason across product strategy, portfolio trade-offs, monetization quality, and organizational constraints.
- separate local wins from system-level outcomes.
- choose what not to build.
- explain long-term implications of short-term choices.
- communicate the decision at executive level.

## Progress States

Use these states in `session_log.md` or `skill_matrix.md`:

- `not started`
- `in progress`
- `evidence emerging`
- `ready for final check`
- `complete`
- `needs drill`

## Final Check

Before closing a level, run a final check:

1. Give a realistic case at the target level.
2. Include incomplete or slightly messy data.
3. Require a decision, not only analysis.
4. Ask the user to name the assumption, risk, metric, and next signal.
5. Review against the level exit criteria.

If the final check passes, mark the level complete and recommend the next level or a new domain.

If it fails, do not restart the whole level. Identify the smallest missing competency and assign a focused drill.

## User-Facing Progress Summary

At reasonable intervals, provide a compact progress summary:

```text
Current target: L3
Already stable: funnel diagnosis, segmentation
Still training: guardrails, decision under uncertainty
Next proof needed: one mixed experiment case where you choose rollout/stop/iterate
Exit status: not ready / nearly ready / ready for final check
```

Keep the summary short. The training remains practice-first, not dashboard-first.
