# Product Sparring Partner

Product Sparring Partner is a Codex skill for deliberate product-management practice. It runs realistic PM cases, challenges reasoning, simulates consequences, and tracks progress across analytics, prioritization, experimentation, business judgment, and product sense.

The skill is designed to act like a Product Lead in a practice session, not like an interviewer or a lecturer.

## What It Does

- Calibrates the user's PM level with a lightweight 10-question screening.
- Lets the user choose a practice domain or provide a vacancy/product/company context.
- Runs live simulations where decisions change the next situation.
- Gives concise feedback on reasoning, trade-offs, assumptions, risks, and metrics.
- Maintains optional local memory through private `state/` files.
- Provides a finite, criterion-based learning path from L1 to L5.

## Install

Copy this folder into your Codex skills directory:

```bash
~/.codex/skills/product-sparring-partner
```

Then invoke it in Codex:

```text
Use $product-sparring-partner
```

## First Run

Recommended first prompt:

```text
Use $product-sparring-partner. I want to train product thinking from scratch.
```

The skill should offer a short screening, estimate a starting level, ask for a domain, and begin the first case.

The training path is finite: users progress when they meet level criteria consistently, not after a fixed number of cases.

## Practice Domains

Default domains:

1. B2B SaaS / productivity / workflow tools
2. Consumer mobile / subscription / retention
3. E-commerce / marketplace / supply-demand matching
4. FinTech / payments / banking / rewards
5. Random domain

You can also provide a custom domain, company, vacancy, or product.

## Runtime State And Privacy

The `state/` folder is private runtime memory. It may contain user profiles, session logs, skill levels, and simulation history. Do not publish personal `state/*.md` files.

Use the templates in `templates/` to create a clean local state if needed.

For public release, publish from Git-tracked files only. Do not zip and upload a local working folder that contains real `state/*.md` files.

## Example Prompts

```text
Use $product-sparring-partner. Start with the 10-question screening.
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
