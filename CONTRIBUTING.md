# Contributing Guide — Pauliceia 2.0

This is the **centralized contribution guide** for all repositories under the **[Pauliceia 2.0](https://github.com/pauliceia)** organization.

It defines the official naming conventions, code language guidelines, and the end-to-end development workflow for **Issues**, **Branches**, **Pull Requests**, and **Commits**, helping maintain consistency and traceability across every repository (`pauliceia`, `vgiws`, `GeocodingAPI`, `database`, etc.).

---

## Table of Contents

- [General Rules & Language](#general-rules--language)
- [1. Issue Naming Convention](#1-issue-naming-convention)
- [2. Branch Naming Convention](#2-branch-naming-convention)
- [3. Pull Request Convention](#3-pull-request-convention)
- [4. Commit Message Convention](#4-commit-message-convention)
- [5. Complete Workflow: Issue to Done](#5-complete-workflow-issue-to-done)
- [6. Repository Setup & Contribution Steps](#6-repository-setup--contribution-steps)

---

## General Rules & Language

- **English as default:** Documentation, code comments, variables, methods, Issue titles, and Pull Request titles should be written in **English**.
- **Base branch:** Always create feature/fix/docs branches from the repository's active default branch (`master`) unless explicitly instructed otherwise by the maintainers. Do not commit directly to `master`.

---

## 1. Issue Naming Convention

Issue titles must start with a **category in brackets**, followed by a short, objective description. When available in the repository, always select the appropriate Issue Template under `.github/ISSUE_TEMPLATE/`.

### Categories

| Prefix       | When to use                                               |
| :----------- | :-------------------------------------------------------- |
| `[FEATURE]`  | Propose a new feature or enhancement                      |
| `[FIX]`      | Plan or track the fix of a known defect                   |
| `[BUG]`      | Report an unexpected behavior or bug identified           |
| `[DOCS]`     | Create, update, or standardize documentation              |
| `[REFACTOR]` | Refactor code without changing external behavior          |
| `[CHORE]`    | Technical maintenance tasks (dependencies, CI/CD, config) |

### Format

```text
[CATEGORY] Short and objective description
```

### Examples

```text
[FEATURE] Add layer filtering by time period
[FIX] Fix error popup on valid geocoding coordinates
[BUG] Map fails to load layers after user login
[DOCS] Standardize repository README
[REFACTOR] Simplify authentication store module
[CHORE] Configure CI pipeline on GitHub Actions
```

> **Tip:** On GitHub, remember to set **Assignees**, **Labels**, and link the Issue to the corresponding **Project** board so the team can track its progress.

---

## 2. Branch Naming Convention

Branches must be created from `master` following the pattern:

```text
type/issue-number-short-description
```

- Use **kebab-case** (lowercase letters separated by hyphens).
- Always include the related **Issue number**.
- Keep the description short and objective (2–4 words).

### Branch Types

| Type       | When to use                     |
| :--------- | :------------------------------ |
| `feature`  | New functionality               |
| `fix`      | Defect or bug fix               |
| `docs`     | Documentation changes           |
| `refactor` | Code refactoring                |
| `chore`    | Maintenance and technical tasks |
| `hotfix`   | Urgent fix in production        |

### Examples

```text
feature/201-layer-period-filter
fix/202-geocoding-error-popup
docs/205-standardize-readme
refactor/208-simplify-auth-service
chore/212-update-webpack-dependencies
hotfix/215-urgent-login-fix
```

---

## 3. Pull Request Convention

Pull Request titles must follow the **[Conventional Commits](https://www.conventionalcommits.org/)** specification.

### Format

```text
type: short description in imperative mood
```

Optionally, include a **scope** in parentheses:

```text
type(scope): short description in imperative mood
```

### PR Types

| Type       | When to use                           |
| :--------- | :------------------------------------ |
| `feat`     | New feature                           |
| `fix`      | Bug fix                               |
| `docs`     | Documentation                         |
| `refactor` | Code refactoring (no behavior change) |
| `chore`    | Maintenance and technical tasks       |
| `style`    | Code formatting (no logic change)     |
| `test`     | Adding or updating tests              |
| `ci`       | CI/CD configuration                   |

### Examples

```text
feat: add layer filtering by time period
fix: fix false error popup on geocoding search
fix(geocoding): validate point coordinates before rendering
docs: standardize repository README
refactor: simplify authentication logic
chore: update Webpack dependencies
```

### PR Body & Issue Linking

In the Pull Request description:

1. Summarize what was changed and why (following the repository's Pull Request template).
2. Link the related Issue using the `Closes` keyword so GitHub automatically closes the Issue upon merge:

```text
Closes #205
```

> If a PR only completes part of a larger Issue (or references an Issue in another repository), use `Part of #205` or `Related to pauliceia/issues#20`.

---

## 4. Commit Message Convention

All commits must follow **[Conventional Commits](https://www.conventionalcommits.org/)**:

```text
type(optional scope): description in imperative mood
```

### Examples

```text
feat: add export layer button
fix(geocoding): fix address search query
docs: standardize repository README
refactor: remove unused state properties in Vuex
chore: configure ESLint v9 rules
test: add user registration step definitions
```

---

## 5. Complete Workflow: Issue to Done

Below is an end-to-end example connecting an Issue, Branch, Pull Request, Code Review, and Project Board status:

### Practical Example

- **Issue:** `#205 [DOCS] Standardize README`
- **Branch:** `docs/205-standardize-readme`
- **Pull Request (#210):**
  - **Title:** `docs: standardize repository README`
  - **Body:** `Closes #205`

### Lifecycle Flow

```text
Issue #205
    ↓
docs/205-standardize-readme
    ↓
PR #210 (docs: standardize repository README | Closes #205)
    ↓
review
    ↓
merge into master
    ↓
Issue #205 automatically closed
    ↓
Project → Done
```

### Quick Reference Summary

| Stage                 | Example                                                              |
| :-------------------- | :------------------------------------------------------------------- |
| **1. Issue**          | `#205` — `[DOCS] Standardize README`                                 |
| **2. Branch**         | `docs/205-standardize-readme`                                        |
| **3. Commit**         | `docs: standardize repository README`                                |
| **4. Pull Request**   | `PR #210` — `docs: standardize repository README` (`Closes #205`)    |
| **5. Review & Merge** | Peer review → Merged into `master`                                   |
| **6. Result**         | Issue `#205` closed automatically → Card moved to **Project → Done** |

---

## 6. Repository Setup & Contribution Steps

1. **Ensure an Issue exists** in the target repository (or create one using the Issue template).
2. **Fork or clone** the target repository:
   ```bash
   git clone https://github.com/pauliceia/<repository-name>.git
   cd <repository-name>
   ```
3. **Sync `master` and create your branch** following the naming convention:
   ```bash
   git checkout master
   git pull origin master
   git checkout -b <type>/<issue-number>-<short-description>
   ```
4. **Follow repository-specific setup & quality checks** (check the target repository's `README.md` for environment setup, dependency installation, and linting commands such as `npm run lint` or `npm run build`).
5. **Commit and push** your changes using Conventional Commits:
   ```bash
   git add .
   git commit -m "<type>: <short description>"
   git push origin <type>/<issue-number>-<short-description>
   ```
6. **Open a Pull Request** targeting **`master`**, fill out the PR template checklist, include `Closes #<issue-number>`, and wait for peer review.
