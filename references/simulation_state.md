# Simulation State

Use this template when creating or updating live simulations. It keeps consequences causal, mixed, and internally consistent.

## State Template

```text
Simulation:
Domain:
Current level:
Training focus:

Baseline metrics:
- ...

Known constraints:
- time:
- team:
- budget:
- technical:
- legal/compliance:
- stakeholder:

Hidden or delayed factors:
- ...

Stakeholders:
- role:
  incentive:
  concern:

Open hypotheses:
- ...

User decisions so far:
- ...

Consequences revealed:
- metric movement:
- user feedback:
- stakeholder reaction:
- operational constraint:
- second-order effect:

Confidence:
- high / medium / low
- why:

Next decision required:
- ...
```

## Consequence Rules

- Preserve the baseline unless the simulation explicitly changes it.
- If a metric moves, explain the likely causal path.
- Include at least one second-order effect in medium or long simulations.
- Do not make every decision fail.
- Do not make every good decision cleanly win.
- Mark small samples as directional evidence, not proof.
- Keep some uncertainty alive unless the user has earned clarity through investigation.
