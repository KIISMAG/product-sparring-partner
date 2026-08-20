# Curriculum

Use this when choosing the next training block or deciding whether to raise/lower difficulty.

For finite progression and level completion criteria, use `references/learning_path.md` together with this curriculum.

## L1 Focus

- Product vocabulary through practical examples.
- Simple metrics: conversion, retention, activation, revenue, churn.
- Difference between user problem, solution, feature, and metric.

Move on when the user can explain a basic funnel and name what each step measures.

## L2 Focus

- Funnel diagnosis.
- Choosing success metrics.
- Basic activation, retention, and monetization cases.
- Simple experiments and before/after reasoning.

Move on when the user can find the most suspicious funnel step and propose a bounded next check.

## L3 Focus

- Multiple hypotheses.
- Segmentation.
- Event-definition and data-quality issues.
- Guardrail metrics.
- Reading mixed experiment results.

Move on when the user can compare hypotheses and choose the first investigation without requiring perfect data.

## L4 Focus

- Prioritization under constraints.
- Rollout design.
- Stakeholder pressure.
- Opportunity cost.
- Reversible versus hard-to-reverse decisions.
- Business impact and unit economics.

Move on when the user repeatedly makes decisions with clear assumptions, trade-offs, and success/guardrail metrics.

## L5 Focus

- Product strategy.
- Portfolio trade-offs.
- Marketplace/system effects.
- Monetization quality.
- Organization and execution constraints.
- Long-term product direction.

Use L5 sparingly. The user should already be comfortable with L3/L4 mechanics.

## Recalibration

Run a short recalibration:

- after 5-7 sessions.
- after switching domains.
- before raising the user by a full level.
- when the user repeatedly succeeds or struggles in ways that contradict the current profile.

## Adaptive Movement

The learner can move forward or step back within a level based on observed reasoning. Do not force a fixed path.

Move forward when the learner repeatedly:

- makes a decision instead of only asking for data.
- names assumptions, risks, and next signals.
- protects the business goal under stakeholder pressure.
- defines success metrics and guardrails.

Step back to a focused drill when the learner twice repeats the same gap. In Russian sessions, call this a `короткое упражнение`, not a `drill`.

| повторяющийся пробел | короткое упражнение |
|---|---|
| путает метрику и цель | короткое упражнение на различение цели и метрики |
| забывает защитные метрики | метрика успеха плюс две защитные метрики |
| избегает решения | шаблон принятия решения |
| просит слишком много данных | упражнение на ограниченный запрос данных |
| оптимизирует только локальную конверсию | упражнение на downstream-эффект |

After a focused drill, do not return directly to the full live case. First run one micro-check that tests transfer of the same skill in a new tiny situation. If the micro-check passes, return to the live case with a smaller decision. If it fails, give one more narrower micro-check or lower the difficulty.

In Russian sessions, call this `мини-проверка`.

| короткое упражнение | мини-проверка |
|---|---|
| ограниченный запрос данных | выбрать 2 среза для новой гипотезы |
| защитные метрики | назвать метрику успеха и 2 защитные метрики |
| шаблон принятия решения | сформулировать решение, допущение, риск и следующий сигнал |
| цель против метрики | отделить бизнес-цель от продуктовой метрики в 3 примерах |
| downstream-эффект | объяснить, какая нижняя метрика может испортиться |

The purpose is learning, not punishment.
