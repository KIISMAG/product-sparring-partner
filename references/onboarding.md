# Onboarding

Use this reference when a user starts the skill for the first time, has no stored level/domain context, asks for screening, or wants to change the practice domain.

## Purpose

Quickly calibrate the user's current product-management level and choose a case domain that makes practice feel realistic. Do not turn onboarding into an exam. The goal is to place the user in the right difficulty band and start practice quickly.

## PM Levels

Use the canonical five-level system from `references/level_system.md`.

Levels are calibration bands, not titles. Avoid saying the user "is L2" as a fixed identity. Say "we'll start around L2/L3 and recalibrate."

## Screening Flow

Offer a lightweight screening on first entry:

```text
Могу начать с короткого скрининга на 10 вопросов, чтобы подобрать уровень: часть вопросов про метрики и воронки, часть про гипотезы, эксперименты и приоритизацию. Это не экзамен, а калибровка сложности.
```

If the user accepts, ask 10 questions one at a time. Prefer case-style questions over definitions. Score reasoning, not memorized terminology.

Use `references/screening_bank.md` for the default 10-question screening and scoring signals. Do not dump all questions at once.

If the user declines the full screening, offer a fast start:

```text
Окей, тогда сделаем быструю калибровку на 2-3 вопроса и сразу перейдем к кейсу. Уровень потом уточним по ходу.
```

Recommended structure:

- 2 questions for metrics and funnel reading.
- 2 questions for hypothesis generation.
- 2 questions for experiment design and guardrails.
- 2 questions for prioritization and trade-offs.
- 1 question for stakeholder/business context.
- 1 decision-under-uncertainty question.

After the screening, provide:

- estimated starting level, for example `L2+ / L3-`.
- two strongest observed skills.
- two risks to train.
- recommended first case mode.

Keep the review concise and start the first case in the same session when possible.

Limit the post-screening debrief to: estimated level, two strengths, two training risks, recommended first domain/case. Avoid a long lecture before practice.

## First-Run Orchestration

For a true first run or an unconfirmed saved state, use this sequence:

1. If existing state is present and unconfirmed, ask whether to use it or start fresh.
2. If starting fresh, offer two paths:
   - full screening: 10 questions, one at a time.
   - fast start: 2-3 calibration questions, then a first case.
3. After calibration, ask for domain selection or accept custom context.
4. Show a compact learning path summary only after calibration.
5. Start the first case immediately after the user chooses the domain.

Suggested first-run message when state exists:

```text
Я нашел сохраненную память тренажера. Используем ее как твой профиль или начинаем с чистого скрининга? Если начинаем с нуля, могу сделать полный скрининг на 10 вопросов или быстрый старт на 2-3 вопроса и сразу перейти к кейсу.
```

Suggested first-run message when no state exists:

```text
Давай откалибруем уровень и быстро перейдем к практике. Могу сделать полный скрининг на 10 вопросов или быстрый старт на 2-3 вопроса, а потом выберем домен кейсов.
```

## Domain Selection

After level calibration, ask the user to choose a practice domain. Offer four broad, high-coverage PM domains plus random. Do not present these as a statistically proven market ranking unless the agent has current market data; present them as practical default domains that cover many common PM case patterns:

1. B2B SaaS / productivity / workflow tools.
2. Consumer mobile / subscription / retention.
3. E-commerce / marketplace / supply-demand matching.
4. FinTech / payments / banking / rewards.
5. Random domain.

Also allow the user to provide custom context:

- a vacancy or job description.
- a company/product they are applying to.
- a real product they worked on.
- a market they want to practice.

Examples of custom domains include TravelTech, HealthTech, EdTech, HRTech, gaming, creator tools, AI products, logistics, real estate, and embedded partner products.

When a vacancy is provided, adapt the case domain, metrics, and stakeholder pressure to that role without turning the session into interview coaching unless requested.

## Changing Domain

The user can change the domain at any time. When they do:

1. Keep the existing skill level and thinking profile.
2. Ask for either a new domain choice or a provided product/company/vacancy.
3. Start with a smaller case in the new domain to recalibrate domain-specific intuition.
4. Mark the previous active simulation inactive or replaced in `simulation_backlog.md`.
5. Continue updating the same skill matrix unless the user asks for a separate profile.

## Existing State Consent

If `state/` contains an existing user profile, session log, or active simulation and the current user has not confirmed that it belongs to them, ask before using it:

```text
Я нашел сохраненную память тренажера. Используем ее как твой профиль или начинаем с чистого скрининга?
```

If the user starts fresh, ignore previous state for calibration and create/update a new profile only after onboarding.

## State Updates

After onboarding, update state files when available:

- `user_thinking_profile.md`: current focus, preferred domain, observed strengths and risks.
- `skill_matrix.md`: starting level estimates by dimension.
- `session_log.md`: screening summary and recommended next practice.
- `simulation_backlog.md`: active simulation domain and first scenario, if a live simulation begins.

Do not store private vacancy text, personal profile details, or sensitive career data in public template files. For a publishable GitHub version, keep state files empty or use anonymized examples.
