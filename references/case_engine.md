# Case Engine

## Case Families

Use and rotate across:

- analytics
- prioritization
- growth
- retention
- discovery
- strategy
- board meeting
- incident
- experimentation
- debugging
- marketplace
- subscription
- B2B
- SaaS

Avoid giving the same family repeatedly unless the user explicitly wants a focused block.

## Selection Logic

Choose the case by training goal:

- weak decision-making under uncertainty -> ambiguous data, limited time, no perfect answer
- weak prioritization -> competing initiatives with different impact, cost, and risk
- weak discovery -> unclear user problem, conflicting qualitative signals
- weak analytics -> metrics movement with multiple plausible causes
- weak business thinking -> product choice with revenue, cost, segment, or GTM implications
- weak strategy -> long-term positioning, sequencing, or system design

## Case Format

Keep setup compact:

```text
Context:
Known data:
Constraints:
Decision required:
```

Include enough information to reason, but leave meaningful uncertainty.

When a case contains quantitative data, present it as a copy-friendly table, not as a bullet list. Prefer Markdown tables with one metric per row and raw numeric values without thousands separators so the user can copy the data into Excel or Google Sheets. If the table needs calculated columns, include clear column names such as `metric`, `value`, `conversion`, `segment`, `control`, `test`, or `period`.

Example:

```text
| metric | value |
|---|---:|
| visitors | 100000 |
| signups | 20000 |
| activated_users | 10000 |
| paid_users | 2000 |
```

## Difficulty Ladder

Use the canonical L1-L5 scale from `references/level_system.md`.

L1: reads simple metrics and explains basic product concepts.

L2: finds visible problems in a funnel or metric movement.

L3: builds competing hypotheses and chooses what to investigate first.

L4: prioritizes initiatives and makes constrained product decisions.

L5: reasons across strategy, systems, organization, monetization, and long-term trade-offs.

Use the user's current matrix to pick cases slightly above their comfort level.
