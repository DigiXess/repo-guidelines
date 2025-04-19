# Commit Message Conventions

Below are the conventions for writing commit messages in this documentation repository. Following these conventions helps maintain a clear and consistent history of changes, making it easier for everyone to understand the evolution of the documentation.

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
| `add:`      | Adding new documents                   |
| `remove:`   | Removing outdated or redundant documents            |
| `archive:`   | Archiving unused or outdated documents            |
| `update:`   | Updating existing documents                 |
| `fix:`      | Fixing errors or inconsistencies in documentation       |
| `style:`    | Formatting or structure changes in documentation        |
| `chore:`    | Maintenance tasks related to documentation              |
| `refactor:` | Reorganizing or restructuring documentation             |

Example:

```
fix: correct typos in installation guide
add: create new section for API documentation
remove: delete deprecated usage examples
```

## Guidelines to Follow

- Use present tense: "fix typo" not "fixed typo".
- Keep the summary under 80 characters.
- Use the body to explain "why", if needed.
- Link issues in the footer, if applicable.

## Full Example Commit Message

```
add: add FAQ section to documentation

Introduced a new FAQ section to address common questions and provide quick answers for users. This improves the usability of the documentation.

Issue #52
```
