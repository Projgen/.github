# Contributing to Projgen

Thank you for your interest in contributing! Projgen is an open-source TypeScript CLI and community contributions are what make it great.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Development Setup](#development-setup)
- [Project Structure](#project-structure)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Adding a Recipe](#adding-a-recipe)
- [Reporting Bugs](#reporting-bugs)
- [Requesting Features](#requesting-features)

---

## Code of Conduct

Please be respectful and constructive. We follow the [Contributor Covenant](https://www.contributor-covenant.org/). Harassment of any kind will not be tolerated.

---

## How to Contribute

There are many ways to help:

- 🐛 Report bugs via [Issues](https://github.com/Projgen/core/issues)
- 💡 Suggest features or new stack recipes
- 🔧 Fix open issues (check `good first issue` label)
- 📚 Improve documentation
- 🧩 Submit new recipes

---

## Development Setup

**Prerequisites:** Node.js v18+, pnpm v10+

```bash
# 1. Fork and clone the core repo
git clone https://github.com/YOUR_USERNAME/core.git
cd core

# 2. Install dependencies
pnpm install

# 3. Watch mode (rebuilds on save)
pnpm run dev

# 4. Link globally so you can run `projgen` locally
pnpm link --global
```

Now run `projgen` in any directory to test your changes.

---

## Project Structure

```
src/
├── builders/     # Project scaffolding logic (copies templates, installs deps)
├── prompts/      # Interactive CLI prompt definitions (@inquirer/prompts)
├── templates/    # File templates copied into new projects
├── types/        # Shared TypeScript types
└── utils/        # Helper utilities
index.ts          # CLI entry point
```

---

## Submitting a Pull Request

1. **Create a branch** from `main`:
   ```bash
   git checkout -b feat/my-feature
   ```
2. **Make your changes** with clear, focused commits
3. **Follow the code style** — run `pnpm run lint` before committing
4. **Build and test** — run `pnpm run build` and verify the CLI works
5. **Open a PR** against `main` with a clear title and description
6. Fill in the PR template completely

### Commit Message Convention

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add Vue.js recipe
fix: resolve path issue on Windows
docs: update README install instructions
chore: bump dependencies
```

---

## Adding a Recipe

A recipe is a preset stack definition. To propose a new recipe:

1. Open a `recipe_request` issue first to discuss
2. Once approved, either implement it in `core` or wait for the `recipes` repo
3. Recipes should be composable — build on existing options rather than duplicating logic

---

## Reporting Bugs

Use the [Bug Report template](https://github.com/Projgen/core/issues/new?template=bug_report.yml). Include:
- Node.js version (`node -v`)
- pnpm/npm/yarn version
- Operating system
- Full error output

---

## Requesting Features

Use the [Feature Request template](https://github.com/Projgen/core/issues/new?template=feature_request.yml). Explain the use case before the implementation — a well-described problem is worth more than a half-formed solution.
