# Contributing Guidelines to Repository

This document outlines the guidelines for contributing to the document repository for consistent and collaborative development across all DigiXess projects.

***Table of Contents**
- [How to Push Changes to the `draft` Branch](#how-to-push-changes-to-the-draft-branch)
- [How to Make Changes to the `main` Branch](#how-to-make-changes-to-the-main-branch)

## How to Push Changes to the `draft` Branch

Contributors and Developer user group members have permission to push changes directly to the `draft` branch. The `draft` branch is the main development branch where all changes are made before being merged into the `main` branch. Follow these steps to contribute to the `draft` branch:

1. Create a branch from `draft` by using:
   - Branch name conventions mentioned in [Branch name conventions](/common/branch-naming-rules.md). 
   - Proper prefixes for the branch name. See [Basic Repository Branch Structure](/document/basic-repo-branch-structure.md) for more details.
   - Use Rebase (`git pull --rebase`) when syncing your local branch with `draft`.
1. Make changes to files in your branch.
1. Commit your changes with a clear and concise commit message that describes the changes made. See [Commit message guidelines](/document/commit-message-guidelines.md) for more details.
1. Push your changes to the remote repository by following guidelines at [Guidelines to create a pull request (PR)][pr-guidelines].
1. Once the PR is approved, merge it into the `draft` branch if you can.
1. Verify that the changes are successfully reflected in the `draft` branch.
1. Delete your branch after the PR is merged to keep the repository clean.

## How to Make Changes to the `main` Branch

Only members of the Integrators and Administrators user groups have permission to push changes directly to the `main` branch. 

Follow these steps to push changes to the `main` branch.

1. Ensure the `draft` branch is up to date with the latest changes.
1. Create a pull request (PR) to merge the `draft` branch into the `main` branch by following the guidelines in [Guidelines to create a pull request (PR)][pr-guidelines].
1. Once the PR is approved, merge it into the `main` branch.
1. Verify that the changes are successfully reflected in the `main` branch.

---

[pr-guidelines]: /common/guidelines-to-create-pull-request.md "Guidelines to create a pull request (PR)"









