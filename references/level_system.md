# Level System

Use this as the canonical level system for the skill. Avoid introducing parallel scales unless they are explicitly mapped here.

## Canonical PM Levels

L1: Product basics.

- Understands common PM language, simple metrics, and basic user/business framing.
- Can explain what a metric means but may struggle to diagnose why it moved.

L2: Applied analysis.

- Reads funnels and simple dashboards.
- Identifies visible problems and proposes reasonable first improvements.
- Can name basic success metrics.

L3: Diagnosis.

- Handles ambiguous data.
- Generates competing hypotheses instead of stopping at one explanation.
- Uses segmentation, guardrails, and bounded investigation.
- Can separate symptoms, causes, decisions, and risks.

L4: Product ownership.

- Prioritizes across impact, effort, risk, company context, and stakeholder incentives.
- Designs experiments and rollout plans with guardrails.
- Makes reversible decisions under incomplete data.

L5: Senior product judgment.

- Reasons across strategy, portfolio trade-offs, monetization, marketplace dynamics, organizational constraints, and long-term systems.
- Can explain what not to do and why.
- Balances short-term evidence with strategic direction.

## Numeric Mapping

If a state file needs numeric tracking, use 1.0-5.0:

- 1.0-1.9: L1
- 2.0-2.9: L2
- 3.0-3.9: L3
- 4.0-4.9: L4
- 5.0: L5

Use fractional changes only when evidence justifies it. Most single sessions should move a dimension by 0.05-0.20 or not at all.

## Session Review Anchors

For 1-10 session scores:

- 3: misses the main issue or relies mostly on unsupported claims.
- 5: finds a reasonable direction but leaves important assumptions, trade-offs, or metrics vague.
- 7: makes a solid decision, names key assumptions, and uses relevant metrics or constraints.
- 9: handles ambiguity well, compares alternatives, names trade-offs, and explains what evidence would change the decision.

Do not over-score fluent answers that skip business impact or uncertainty.

## Mastery Gates

Raise difficulty when the user shows 2-3 successful cases in a row for the target skill:

- frames the business goal before optimizing a local metric.
- generates multiple plausible hypotheses.
- chooses a bounded next action.
- names the risk they are accepting.
- defines success and guardrail metrics.

Lower difficulty or give a focused drill when the user struggles twice in a row with the same pattern:

- cannot identify the relevant funnel step.
- jumps to a solution without naming a problem.
- optimizes a local metric while ignoring revenue, user quality, or partner impact.
- avoids a decision by asking for unlimited data.
