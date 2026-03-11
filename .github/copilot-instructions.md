# Git Standards

This document defines the guidelines for code versioning and management.
The goal is to maintain a clean, readable, and easily traceable history for all team members.


## Commit Message Structure

We adopt the [**Conventional Commits**](https://www.conventionalcommits.org/) specification to ensure a clean, readable, and machine-parsable commit history.

Every commit message must follow this format:

```
<type>: <subject>
```

- **Subject line:** maximum 72 characters, lowercase start, no trailing period.

## Grammar Rules

| Rule            | Standard                                                                                                           |
| --------------- | ------------------------------------------------------------------------------------------------------------------ |
| Language        | English (International Standard).                                                                                  |
| Tense and Mood  | **Imperative present tense** — write as if you are commanding the codebase (e.g., "add", "fix", "remove").         |
| Capitalization  | The first letter of the subject must be **lowercase**.                                                             |
| Punctuation     | Do **not** end the subject line with a period.                                                                     |

## Commit Types

| Type       | Description                                                                                     |
| ---------- | ----------------------------------------------------------------------------------------------- |
| `feat`     | A new feature visible to the end user.                                                          |
| `fix`      | A bug fix that corrects incorrect behavior.                                                     |
| `docs`     | Changes to documentation only (README, comments, etc.).                                         |
| `style`    | Code formatting, whitespace, or cosmetic changes that do **not** affect functionality.          |
| `refactor` | A code change that neither fixes a bug nor adds a feature (e.g., restructuring, renaming).      |
| `test`     | Adding, updating, or correcting tests.                                                          |

## Examples

**Correct:**

```
feat: add publications section to homepage
fix: resolve navbar overlap on mobile viewports
docs: update README with deployment instructions
style: align indentation in index.html
refactor: extract hero section into reusable block
chore: add .editorconfig for consistent formatting
```

**Incorrect:**

```
Added login                → Missing type prefix; uses past tense.
Fixed bug                  → Too vague; uses past tense.
feat: Add new section.     → Subject starts with uppercase; ends with a period.
update stuff               → No type prefix; non-descriptive subject.
```