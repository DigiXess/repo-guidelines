# Changelog Guidelines

Keep the CHANGELOG.md updated with production-ready changes, and maintain separate dev and release changelogs for each version. 

**Table of Contents**
- [General Guidelines](#general-guidelines)
- [For larger projects with major releases:](#for-larger-projects-with-major-releases)
- [When Merging from `dev` → `main` (Release)](#when-merging-from-dev--main-release)
- [Automation Tips](#automation-tips)

## General Guidelines

- **Use a consistent format** across all changelog files.
- **Always keep** the [`CHANGELOG.md`](/CHANGELOG.md) file **up to date** with the latest changes — including bug fixes, new features, and improvements — for the production (`main`) branch.
- Use a **versioning system** (e.g., [Semantic Versioning](https://semver.org/)) to track changes and releases.
  
## For larger projects with major releases:

  - Store detailed changelogs in a separate folder:  
    ```
    /changelog/release/<tag-number>/
    ```
  - Reference the latest version number and release date in the main [`CHANGELOG.md`](/CHANGELOG.md).
  - **Maintain a draft or development changelog** for ongoing work in:
    ```
    /changelog/dev/<tag-number>/
    ```
    - This should include WIP features, internal improvements, and partial implementations.

## When Merging from `dev` → `main` (Release)

Before completing the merge:
- ✅ Ensure `CHANGELOG.md`  is updated with:
  - The final **release version number**
  - The correct **release date**
- 🧹 Clean up the dev changelog:
  - Remove **WIP**, **internal-only**, or **incomplete features** not meant for release.
- 📦 Move finalized entries from if necessary:
  - `/changelog/dev/<tag-number>/` → `/changelog/release/<tag-number>/`


## Automation Tips

To streamline changelog management, consider using automation tools like:
- `auto-changelog`
- `standard-version`

These tools help enforce consistency and reduce manual effort.

**Note**: Ensure that any automated tools you use are compatible with your project's workflow and versioning strategy.