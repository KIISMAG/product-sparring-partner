# Screening Bank

Use these questions for the default 10-question onboarding screening. Ask one question at a time. Adapt numbers and domains lightly if the user has provided context.

Score reasoning, not exact wording.

When a screening question includes numeric data, present the data as a copy-friendly table. Use raw values without thousands separators.

## Questions

1. Funnel reading.
   A product has this monthly funnel:

   | metric | value |
   |---|---:|
   | visitors | 100000 |
   | signups | 20000 |
   | activated_users | 10000 |
   | paid_users | 2000 |

   Which step would you inspect first and why?

2. Metric choice.
   A team improves onboarding completion from 40% to 55%, but paid conversion is flat. What would you check next?

3. Hypotheses.
   Search usage dropped 20% week over week. Name three plausible explanations before choosing one.

4. Segmentation.
   Activation fell only for new users from paid ads. What segments or cuts would you request?

5. Experiment design.
   You want to test a new paywall. What is the main success metric and two guardrails?

6. Guardrails.
   A push campaign increases app opens but complaints also rise. How do you decide whether to continue?

7. Prioritization.
   You have two initiatives: one has high upside and high risk, the other has modest upside and low risk. What information do you need to choose?

8. Trade-off.
   Sales wants an enterprise integration for one large lead. Engineering says it will delay activation work by a month. How do you frame the decision?

9. Stakeholder/business context.
   Marketing wants more traffic, support wants fewer tickets, finance wants margin. How do you choose the product goal for the next quarter?

10. Decision under uncertainty.
   Data is incomplete and the team must decide this week. What decision do you make, what assumption are you making, and what signal would change your mind?

## Scoring Signals

L1 signals:

- defines terms but struggles to choose a next action.
- names metrics without connecting them to a decision.

L2 signals:

- identifies the visible funnel problem.
- proposes a reasonable metric or simple test.
- may stop at one hypothesis.

L3 signals:

- generates competing hypotheses.
- asks about base rates, segments, sample size, and event definitions.
- distinguishes leading and lagging metrics.

L4 signals:

- makes a bounded decision under constraints.
- includes guardrails, rollout, stakeholder incentives, and opportunity cost.

L5 signals:

- reasons across strategy, portfolio effects, monetization quality, and second-order consequences.
- explains what not to optimize and why.

## Debrief Template

Keep it short:

```text
Стартовая калибровка: примерно Lx / Ly.
Сильные стороны: ...
Риски для тренировки: ...
Первый рекомендованный режим: ...
```
