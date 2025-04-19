# Code Repository Guidelines

This document outlines the guidelines for contributing to the code repository for consistent and collaborative development across all DigiXess projects.

**Table of Contents**

Follow the below guidelines:

- Commit frequently: Make small, logical commits to track changes effectively.
- Write clear commit messages: Use descriptive messages to explain what changes were made and why.
- Follow:
    - [Basic Repository Branch Structure][basic-repo-branch-structure]
    - [Branch and Merge Strategy][branch-merge-strategy]
    - [Commit Message Conventions][commit-message-conventions]
    - [Tag Versioning Guidelines][tag-versioning-guidelines]
- Always branch instead of fork.
- Don't commit sensitive information: Avoid committing passwords, API keys, or other sensitive data.
- Avoid force pushing or rewriting history on shared branches.
- Don't commit large binary files: Use Git LFS or other solutions for large files instead.
- Set up branch protection rules to prevent direct pushes and require pull requests for changes. See [Protecting `main` Branch](/common/protecting-main-branch.md "Protecting `main`") for more details.

---

[basic-repo-branch-structure]: /code/basic-repo-branch-structure.md "Basic Repository Branch Structure"
[branch-merge-strategy]:/code/branch-merge-strategy.md "Branch and Merge Strategy"
[commit-message-conventions]: /code/commit-message-conventions.md "Commit Message Conventions"
[tag-versioning-guidelines]: /code/tag-versioning-guidelines.md "Tag Versioning Guidelines"


