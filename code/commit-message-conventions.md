# Commit Message Gui

Below are the conventions for writing commit messages in this repository. Following these conventions helps maintain a clear and consistent history of changes, making it easier for everyone to understand the evolution of the codebase.

**Table of Contents**
- [Format](#format)
  - [Common Types (Prefixes):](#common-types-prefixes)
- [Guidelines to Follow](#guidelines-to-follow)
- [Full Example Commit Message](#full-example-commit-message)

## Format

```
<type>: <short, imperative summary> --------------------> Header

[optional body: more details or reasoning
...                                                 ----> Body
end of body ]
[optional footer: issue link, breaking changes]   ------> Footer

```

- **Header**: A concise summary of the change.
- **Body**: Additional details or reasoning behind the change (optional).
- **Footer**: References to issues or breaking changes (optional).
- **type**: A list of standard prefixes that can be used in commit messages are mentioned below.
  
### Common Types (Prefixes):

| Type        | Purpose                                                 |
| ----------- | ------------------------------------------------------- |
| `feat:`     | Adding a new feature                                    |
| `fix:`      | Bug fix                                                 |
| `docs:`     | Documentation-only changes                              |
| `style:`    | Formatting, missing semi colons, etc. (no code change)  |
| `refactor:` | Code change that neither fixes a bug nor adds a feature |
| `perf:`     | Performance improvement                                 |
| `test:`     | Adding or fixing tests                                  |
| `chore:`    | Maintenance, build tools, dependencies                  |
| `revert:`   | Reverting a previous commit                             |
| `ci:`       | Continuous integration-related changes                  |
| `user:`     | User-specific branches or sandbox experiments           |

Example:

```
feat: add user profile page
fix: resolve crash when logging out
docs: update README with setup steps
```

## Guidelines to Follow

- Use present tense: "fix bug" not "fixed bug".
- Keep the summary under 80 characters.
- Use the body to explain "why", if needed.
- Link issues in the footer.

## Full Example Commit Message

```
feat: add JWT-based authentication system

Implemented JWT token handling for login and user sessions.
Refactored the auth controller and added token expiration checks.
This helps prepare for scalable, secure user management.

BREAKING CHANGE: Legacy session-based auth has been removed.

Closes #102
Related to #88
```
