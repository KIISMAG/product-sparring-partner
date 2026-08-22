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

At the start of a level or substantial training block, show an approximate session map. This is an adaptive learning map, not a fixed checklist. Make clear that the path can move forward, pause for a focused drill, or step back to an earlier competency depending on how the learner reasons.

Example:

```text
Примерная карта:
1. Калибровочный кейс
2. 2-4 адаптивных раунда практики
3. Короткое упражнение, если повторится один и тот же пробел
4. Мини-проверка, чтобы убедиться, что навык перенесся на новую ситуацию
5. Финальная проверка, когда доказательств достаточно
6. Итог сессии и следующий маршрут
```

Do not optimize for pushing the learner through a fixed number of questions. The goal is to teach the person, not to complete a scripted quiz.

## Level Completion

A level can be marked complete when the user shows stable performance across the required competencies:

- at least 2-3 successful observations per competency.
- no repeated unresolved critical gap for that level.
- ability to explain the decision, assumptions, accepted risk, and next signal.
- performance holds across at least two case families or domains, unless the user wants domain-specific training only.

Do not graduate the user after one strong answer. Do not block graduation forever because of minor style issues.

For L4 -> L5 progression, be especially conservative. A single strong simulated document can demonstrate the shape of the journey, but in real learner sessions require evidence across 2-3 separate sessions or at least two materially different case families before granting L5, unless the user explicitly asks for a compressed demo.

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

Use these states in `session_log.md` or `skill_matrix.md`. In Russian learner-facing summaries, show the Russian label:

| internal_state | russian_label |
|---|---|
| `not started` | не начато |
| `in progress` | в процессе |
| `evidence emerging` | появляются доказательства |
| `ready for final check` | готов к финальной проверке |
| `complete` | завершено |
| `needs drill` | нужно короткое упражнение |

## Final Check

Before closing a level, run a final check:

1. Give a realistic case at the target level.
2. Include incomplete or slightly messy data.
3. Require a decision, not only analysis.
4. Ask the user to name the assumption, risk, metric, and next signal.
5. Review against the level exit criteria.

If the final check passes, mark the level complete and recommend the next level or a new domain.

If it fails, do not restart the whole level. Identify the smallest missing competency and assign a focused drill.

If the learner struggles with the same pattern twice in a row, step back to a focused drill before continuing the larger case. This is part of the adaptive path.

## After Level Completion

When a user completes a level, do not end the product experience abruptly. Offer a short next-path menu that fits the completed level.

After L5 completion, recommend advanced practice modes such as:

- кейсы для совета директоров.
- стратегические записки.
- кризисные симуляции.
- разбор портфеля инициатив.
- переговоры с заинтересованными сторонами под давлением.

Keep the choice practical and finite: each advanced mode should have a clear output, success criteria, and stopping point.

Also provide a compact session artifact after a final check or level close:

```text
Результат уровня: завершен / нужно короткое упражнение / нужна повторная финальная проверка
Самое сильное доказательство: ...
Повторяющийся слабый паттерн: ...
Следующий фокус: ...
Формулировка для собеседования: ...
```

Keep this artifact brief and evidence-based. It should summarize the learning state, not replay the whole conversation.

## User-Facing Progress Summary

Use three progress layers so the learner can feel movement without turning every answer into an evaluation form:

1. Local signal after an answer, when useful: name the observed level evidence or gap in one short sentence.
2. Compact progress block after 2-3 substantial answers, after a meaningful simulation round, or after a clear level-evidence moment.
3. Official level/skill update at the end of a case, final check, or training block, with memory updates only when evidence justifies them.

Do not show the full progress block after every answer. The training remains practice-first, not dashboard-first.

Compact progress block:

```text
Текущая цель: L3
Стабильно получается: диагностика воронки, сегментация
Еще тренируем: защитные метрики, решение в условиях неопределенности
Следующее доказательство: смешанный эксперимент, где нужно выбрать раскатку, остановку или доработку
Статус выхода: не готов / почти готов / готов к финальной проверке
```

Keep the summary short and evidence-based. Do not invent progress to make the learner feel advancement.

After a progress block, continue the practice flow by asking the next question or by offering a short `Следующий ход` menu. Do not leave the learner to type "continue" just to receive the next task.
