# Git Standards

This document defines the guidelines for code versioning and management. The goal is to maintain a clean, readable, and easily traceable history for all team members.

---

## 1. Commit Message Standards

We adopt the **Conventional Commits** specification. This format makes the history readable for both humans and automation tools.

### Message Structure

Every commit must follow this structure:

```
<type>: <subject>

[optional body]

[optional footer(s)]
```

### Grammar Rules

- **Language:** English (International Standard).
- **Imperative Mood:** Use the imperative present tense ("Add" not "Added", "Fix" not "Fixed"). *Example: "Add new filter component"* (It is as if you are telling the codebase: "do this").
- **Capitalization:** The first letter of the `subject` should be lowercase (optional, but recommended for consistency).
- **Punctuation:** Do not end the `subject` line with a period.

### Commit Types

- `feat`: A new feature for the user.
- `fix`: A bug fix.
- `docs`: Documentation only changes.
- `style`: Formatting, missing semi-colons, etc. (no code change).
- `refactor`: A code change that neither fixes a bug nor adds a feature (structural improvement).
- `test`: Adding missing tests or correcting existing tests.

### Examples

> ✅ **Correct:** `feat: add google oauth` or `fix: resolve overlapping items on mobile`
>

> ❌ **Incorrect:** `Added login (Missing type and uses past tense)` or `Fixed bug (Too vague)`
>

---

## 2. Branch Naming Standards

Branch names must be descriptive and follow a specific hierarchy to facilitate filtering and sorting.

### Branch Format

`category/ticket-id-short-description`

### Grammar Rules

- **Separator:** Always use hyphens  (kebab-case), never underscores `_` or spaces.
- **Lowercase:** The entire branch name must be lowercase.

### Branch Categories

1. `feature/`: Development of new features.
    - *Ex:* `feature/PROJ-101-user-profile-page`
2. `bugfix/` (or `fix/`): Bug corrections during a sprint.
    - *Ex:* `bugfix/PROJ-102-calendar-date-picker`
3. `hotfix/`: Urgent fixes to be applied directly to production (master/main).
    - *Ex:* `hotfix/security-patch-v1`
4. `release/`: Preparation for a new version release.
    - *Ex:* `release/v1.2.0`
5. `chore/`: Technical maintenance (library updates, config).
    - *Ex:* `chore/update-react-version`