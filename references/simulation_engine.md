# Simulation Engine

Use this mode when the user wants realistic product-management practice rather than isolated exercises.

## Purpose

Create a live product simulator that gives the user safe "battle experience" through decisions, consequences, stakeholder pressure, incomplete data, and changing metrics.

Adapt the simulation to the user's chosen domain, screening result, and stated goals. Do not hard-code one user's background into public cases. If the user provides a resume, vacancy, company, or past product, use it only as session context and store only cautious, useful thinking patterns.

## Simulation Loop

Run scenarios in turns:

1. Present the current product/business situation.
2. Give only the data a PM would plausibly have at that moment.
3. Ask for one decision or next action.
4. Evaluate the reasoning.
5. Reveal consequences: metric movement, user feedback, stakeholder reaction, technical constraint, or unexpected second-order effect.
6. Update the scenario state.
7. Ask for the next decision.

Do not reveal all future consequences upfront. Let the user's decisions shape the next state.

When starting or materially changing a simulation, use the state template from `references/simulation_state.md` so outcomes remain causal rather than arbitrary.

## Scenario Ingredients

Prefer realistic situations involving:

- funnel leakage
- activation and retention problems
- CRM and lifecycle messaging
- onboarding and first value
- partner distribution and B2B2C launches
- monetization, cashback, commission, pricing, or revenue share
- stakeholder conflict between sales, support, product, engineering, finance, and partners
- analytics gaps and misleading metrics
- experiments with imperfect sample sizes
- trade-offs between quick wins and strategic bets

## Difficulty

Start around L2+/L3-:

- require the user to read a funnel and identify the likely problem
- require at least three plausible hypotheses before choosing one
- require a decision even when data is incomplete
- avoid heavy L4/L5 strategy until the user can repeatedly move from metrics to diagnosis to action

Increase difficulty only after the user shows repeated competence in:

- naming the business goal
- separating symptoms from causes
- comparing hypotheses
- choosing a next action
- naming risks and early signals

## Consequence Design

Consequences should be plausible, mixed, and educational:

- A decision can improve one metric but hurt another.
- A local funnel improvement may fail to move revenue.
- A stakeholder-favored feature may have poor expected value.
- A small experiment may show directional evidence but not statistical certainty.
- A partner or sales request may hide a real strategic opportunity.

Do not make every user decision fail. Reward good reasoning with improved state, but still include real-world messiness.

## Interview Bridge

The training goal is real product thinking, but the user also wants to get a product-management job. After a simulation turn, optionally translate the learning into interview language:

```text
How this sounds in an interview:
...
```

Keep this secondary. Do not turn the simulation into memorized interview prep.
