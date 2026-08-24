# Product Sparring Partner

Product Sparring Partner is a Codex skill for deliberate product-management practice. It runs realistic PM cases, challenges reasoning, simulates consequences, and tracks progress across analytics, prioritization, experimentation, business judgment, and product sense.

The skill is designed to act like a Product Lead in a practice session, not like an interviewer or a lecturer.

The core promise:

```text
Practice product decisions before you have to make them at work.
```

## What It Does

- Calibrates the user's PM level with a short 3-question first-run calibration, with a full 10-question screening available on request.
- Supports English or Russian training, with language selection during onboarding when needed.
- Lets the user choose a practice domain or provide a vacancy/product/company context.
- Runs live simulations where decisions change the next situation.
- Gives concise feedback on reasoning, assumptions, risks, trade-offs, and metrics.
- Shows progress without over-grading: local signals after answers, compact progress every few substantial turns, and official level updates at case or level boundaries.
- Ends practice turns with the trainer's chosen next question; numbered quick actions are reserved for real learner-choice boundaries.
- Uses adaptive practice: if the learner repeats the same gap, it steps back to a focused exercise and a small transfer check before returning to the case.
- Adds stakeholder pressure from roles such as CEO, Sales, Support, Finance, Engineering, Legal, Customer Success, partners, or customers.
- Maintains optional local memory through private `state/` files.
- Provides a finite, criterion-based learning path from L1 to L5.

## How It Differs From A Normal ChatGPT Case

This is not just a prompt that generates random PM cases. The skill has a defined training loop:

1. Calibrate the learner's level.
2. Show an approximate, adaptive learning path.
3. Give one product decision at a time.
4. Challenge the reasoning before revealing a stronger answer.
5. Simulate consequences and stakeholder conflict.
6. Track recurring thinking patterns.
7. Use level criteria and a final check before marking progress.

The point is to improve product judgment, not to memorize ideal case answers.

## Install

Copy this folder into your Codex skills directory:

```bash
~/.codex/skills/product-sparring-partner
```

On Windows, the typical path is:

```text
C:\Users\<you>\.codex\skills\product-sparring-partner
```

Then restart Codex if needed and invoke it:

```text
Use $product-sparring-partner
```

## Quick Start

Start from scratch:

```text
Use $product-sparring-partner. I want to train product thinking from scratch.
```

Start in Russian:

```text
Use $product-sparring-partner. Хочу тренировать продуктовое мышление на русском языке.
```

Start with a specific domain:

```text
Use $product-sparring-partner. Give me a FinTech case around activation and monetization.
```

Use your own context:

```text
Use $product-sparring-partner. I am preparing for a PM role in B2B SaaS. Start with calibration and then run a realistic case.
```

## First Run

Recommended first prompt:

```text
Use $product-sparring-partner. I want to train product thinking from scratch.
```

The skill should run a short 3-question calibration, estimate a starting level, ask for a domain, and begin the first case.

The training path is finite: users progress when they meet level criteria consistently, not after a fixed number of cases.

If the user's language is unclear, the skill should ask whether to train in English or Russian before calibration.

Expected first-run flow:

```text
1. Language selection, if unclear.
2. Short 3-question calibration.
3. Starting level estimate, for example L2+ / L3-.
4. Domain selection.
5. Approximate adaptive learning map.
6. First realistic case.
```

## Practice Domains

Default domains:

1. B2B SaaS / productivity / workflow tools
2. Consumer mobile / subscription / retention
3. E-commerce / marketplace / supply-demand matching
4. FinTech / payments / banking / rewards
5. Random domain

You can also provide a custom domain, company, vacancy, or product.

## Levels

The skill uses five calibration bands:

| level | focus |
|---|---|
| L1 | basic product vocabulary and simple metrics |
| L2 | funnel reading, obvious problems, simple tests |
| L3 | hypotheses, segmentation, guardrails, imperfect data |
| L4 | prioritization, rollout, stakeholder pressure, opportunity cost |
| L5 | strategy, portfolio trade-offs, monetization quality, systems thinking |

Levels are not job titles. They are practice bands used to choose the right difficulty.

## Runtime State And Privacy

The `state/` folder is private runtime memory. It may contain user profiles, session logs, skill levels, and simulation history. Do not publish personal `state/*.md` files.

Use the templates in `templates/` to create a clean local state if needed.

For public release, publish from Git-tracked files only. Do not zip and upload a local working folder that contains real `state/*.md` files.

Before publishing, check:

```bash
git status --short --ignored
```

Ignored `state/*.md` files are expected locally. They should not be committed.

## Example Prompts

```text
Use $product-sparring-partner. Start with the full 10-question screening.
```

```text
Use $product-sparring-partner. Start with a quick 3-question calibration and then a case.
```

```text
Use $product-sparring-partner. I want a B2B SaaS retention case around L3.
```

```text
Use $product-sparring-partner. Change the domain to FinTech and continue at my current level.
```

```text
Use $product-sparring-partner. Give me tough feedback on my product reasoning, but don't reveal the ideal answer too early.
```

Russian examples:

```text
Use $product-sparring-partner. Давай начнем с полного скрининга на 10 вопросов.
```

```text
Use $product-sparring-partner. Давай начнем с быстрой калибровки на 3 вопроса и потом сразу кейс.
```

```text
Use $product-sparring-partner. Хочу кейс по FinTech на уровне L3: активация, монетизация и защитные метрики.
```

```text
Use $product-sparring-partner. Смени домен на marketplace, но оставь мой текущий уровень.
```

## Package Structure

```text
product-sparring-partner/
  SKILL.md
  README.md
  LICENSE
  .gitignore
  PUBLICATION_CHECKLIST.md
  agents/
    openai.yaml
  references/
    philosophy.md
    session_protocol.md
    review_engine.md
    memory.md
    level_system.md
    learning_path.md
    onboarding.md
    screening_bank.md
    hint_ladder.md
    curriculum.md
    case_engine.md
    simulation_engine.md
    simulation_state.md
  templates/
    user_thinking_profile.template.md
    skill_matrix.template.md
    session_log.template.md
    simulation_backlog.template.md
  state/
    .gitkeep
```

## Notes For Contributors

- Keep public files free of private user data.
- Keep the agent practical: one question at a time, short feedback, live decisions.
- Prefer adding focused references over making `SKILL.md` too large.
- Run the skill validator after changes.
