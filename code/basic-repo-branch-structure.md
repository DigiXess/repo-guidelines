# Basic Repository Branch Structure

Any code project should have the following branches:

- **`main`**: This branch holds the **production-ready** code. It's always stable and is deployed. If there is a `master`, rename it to the `main` branch.
- **`dev`**: This branch is used for **active development**. It contains the latest features and updates, but might not always be stable.
- **`staging`**: This branch is used for **staging or pre-production**. It contains the latest features and updates, but is used for testing before merging into `main`.

Additionally, create different branches using the below prefixes for specific purposes:

| Prefix           | Purpose                                                                                                 |
| ----------------- | ----------------------------------------------------------------------------------------------------- |
| `feature/`       | For developing **new features**. Branches off `dev`.                                                  |
| `bugfix/`        | For fixing **non-critical bugs** found during development.                                            |
| `release/`       | For preparing a **versioned release** (QA, final polish).                                             |
| `hotfix/`        | For **urgent fixes** directly on `main`. Usually patching production. Try avoiding as much as possible.|
| `experiment/`    | For trying out **prototypes, research, etc.** that might not be merged.                               |
| `chore/`         | For **non-functional updates** like config changes, CI setup, etc.                                    |
| `docs/`          | For updates to **documentation**.                                                                     |
| `test/`          | For adding **tests or test cases**.                                                                   |
| `user/username/` | Developer-specific branches for long-term or private work.                                            |

### Example

```
main ← release ← dev ← feature/login-page ← bugfix/navbar-issue
```
