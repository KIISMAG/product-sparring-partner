# Publication Checklist

Use this before publishing the skill to GitHub.

## Must Check

- `state/*.md` files are not committed.
- `.gitignore` excludes private runtime state.
- `templates/` contains clean starter files.
- `references/simulation_engine.md` is not personalized to one user.
- `README.md` explains install, first run, domains, privacy, and examples.
- `LICENSE` is present.
- The skill validator passes.
- Release is created from Git-tracked files only, not from a zip of the local folder.

## Suggested Git Flow

```bash
git init
git add SKILL.md README.md LICENSE .gitignore PUBLICATION_CHECKLIST.md agents references templates state/.gitkeep
git status
git commit -m "Add product sparring partner skill"
```

Before committing, confirm `git status` does not show personal files under `state/`.

## First Public Test

Test these prompts in a clean install:

```text
Use $product-sparring-partner. I want to train product thinking from scratch.
```

```text
Use $product-sparring-partner. Start with the 10-question screening.
```

```text
Use $product-sparring-partner. Change the domain to FinTech.
```

Expected behavior:

- The agent offers screening or fast start.
- It asks one question at a time.
- It does not rely on another user's state.
- It lets the user choose or change domain.
- It gives feedback after the user's attempt, not before.
