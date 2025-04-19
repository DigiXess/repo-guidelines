# Commit Message Conventions

Below are the conventions for writing commit messages in this graphic assets repository. Following these conventions helps maintain a clear and consistent history of changes, making it easier for everyone to understand the evolution of the assets.

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
| `add:`      | Adding new graphic assets                               |
| `remove:`   | Removing outdated or redundant graphic assets           |
| `archive:`  | Archiving unused or outdated graphic assets             |
| `update:`   | Updating existing graphic assets                        |
| `fix:`      | Fixing errors or inconsistencies in graphic assets      |
| `style:`    | Formatting or structure changes in graphic assets       |
| `chore:`    | Maintenance tasks related to graphic assets             |
| `refactor:` | Reorganizing,Optimizing, or restructuring graphic assets            |

Example:

```
fix: correct color profile in logo asset
add: add new banner graphic for homepage
remove: delete outdated icons from branding folder
```

## Guidelines to Follow

- Use present tense: "fix typo" not "fixed typo".
- Keep the summary under 80 characters.
- Use the body to explain "why", if needed.
- Link issues in the footer, if applicable.

## Full Example Commit Message

```
add: add new logo asset for branding

Added a new logo asset to the branding folder. This logo will be used across all marketing materials and replaces the old version.

Closes Issue #46