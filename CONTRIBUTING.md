# Contributing to Projgen

Thank you for your interest in contributing! Projgen is an open-source TypeScript CLI and community contributions are what make it great.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Development Setup](#development-setup)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Reporting Bugs](#reporting-bugs)
- [Requesting Features](#requesting-features)

---

## Code of Conduct

Please be respectful and constructive. We follow the [Contributor Covenant](https://www.contributor-covenant.org/). Harassment of any kind will not be tolerated.

---

## How to Contribute

There are many ways to help:

- Report bugs via [Issues](https://github.com/Projgen/core_v2/issues)
- Suggest features or new stack templates
- Fix open issues (check `good first issue` label)
- Improve documentation

---

## Development Setup

**Prerequisites:** Node.js v18+, npm v11+

```bash
# 1. Fork and clone the core repo
git clone https://github.com/YOUR_USERNAME/core_v2.git
cd core_v2

# 2. Install dependencies
npm install

# 3. Build
npm run build

# 4. Link globally so you can run `projgen` locally
npm link --global
```

Now run `projgen` in any directory to test your changes.

---

## Submitting a Pull Request

1. **Create a branch** from `master`:
   ```bash
   git checkout -b feat/my-feature
   ```
2. **Make your changes** with clear, focused commits
3. **Follow the code style** — run `npm run lint` ans `npm run format` before committing
4. **Build and test** — run `npm run build` and verify the CLI works by running `npm run start`
5. **Open a PR** against `main` with a clear title and description
6. Fill in the PR template completely

### Commit Message Convention

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add Vue.js template
fix: resolve path issue on Windows
docs: update README install instructions
chore: bump dependencies
```

---

## Reporting Bugs

Use the [Bug Report template](https://github.com/Projgen/core_v2/issues/new?template=bug_report.yml). Include:

- Node.js version (`node -v`)
- npm version
- Operating system
- Full error output
- Any additional context

---

## Requesting Features

Use the [Feature Request template](https://github.com/Projgen/core_v2/issues/new?template=feature_request.yml). Explain the use case before the implementation — a well-described problem is worth more than a half-formed solution.

---

## Requesting Templates

Use the [Template Request template](https://github.com/Projgen/core_v2/issues/new?template=template_request.yml). Explain what the template is for and what it should include.
