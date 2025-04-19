# Contributing Guidelines to Repository

This document outlines the guidelines for contributing to the document repository for consistent and collaborative development across all DigiXess projects.

***Table of Contents**
- [How to Push Changes to the `dev` Branch](#how-to-push-changes-to-the-dev-branch)
- [How to Make Changes to the `main` Branch](#how-to-make-changes-to-the-main-branch)
  - [Steps to Merge `dev` into `main`](#steps-to-merge-dev-into-main)
    - [Without a "staging" Branch](#without-a-staging-branch)
    - [With a "staging" Branch](#with-a-staging-branch)

## How to Push Changes to the `dev` Branch

Contributors and Developers have the permission to push changes directly to the `dev` branch. The `dev` branch is the main development branch where all changes are made before being merged into the `main` branch. Follow these steps to contribute to the `dev` branch:

1. Create a branch from `dev` by using:
   - Branch name conventions mentioned in [Branch name conventions](/common/branch-naming-rules.md). 
   - Proper prefixes for the branch name. See [Basic Repository Branch Structure](/code/basic-repo-branch-structure.md) for more details.
   - Use Rebase (`git pull --rebase`) when syncing your local branch with `dev` 
1. Make changes to files in your branch.
1. Commit your changes with a clear and concise commit message that describes the changes made. See [Commit message guidelines](/code/commit-message-conventions.md) for more details.
1. Push your changes to the remote repository by following guidelines at [Guidelines to create a pull request (PR)][pr-guidelines].
1. Once the PR is approved, merge it into the `dev` branch if you can.
1. Verify that the changes are successfully reflected in the `dev` branch.
1. Delete your branch after the PR is merged to keep the repository clean.

## How to Make Changes to the `main` Branch

Only Integrators and Administrators have the permission to push changes directly to the `main` branch.

### Steps to Merge `dev` into `main`

Once the changes in the `dev` branch are finalized and tested, follow these steps to push them to the `main` branch.

#### Without a "staging" Branch
1. Ensure the `dev` branch is up to date with the latest changes.
1. Create a pull request (PR) to merge the `dev` branch into the `main` branch by following the guidelines in [Guidelines to create a pull request (PR)][pr-guidelines].
1. Once the PR is approved, merge it into the `main` branch.
1. Verify that the changes are successfully reflected in the `main` branch.

#### With a "staging" Branch
1. Ensure the `dev` branch is up to date with the latest changes.
1. Create a pull request (PR) to merge the `dev` branch into the `staging` branch by following the guidelines in [Guidelines to create a pull request (PR)][pr-guidelines].
1. Once the PR is approved, merge it into the `staging` branch.
1. Verify that the changes are successfully reflected in the `staging` branch.
1. Prepare the `staging` branch for production. This may involve additional testing or other changes to ensure the code is ready for production.
1. Create a pull request (PR) to merge the `staging` branch into the `main` branch by following the guidelines in [Guidelines to create a pull request (PR)][pr-guidelines].
1. Once the PR is approved, merge it into the `main` branch.
1. Verify that the changes are successfully reflected in the `main` branch.
1. Delete the `staging` branch after the PR is merged to keep the repository clean.

---

[pr-guidelines]: /common/guidelines-to-create-pull-request.md "Guidelines to create a pull request (PR)"







