# Tag Versioning Guidelines

We follow [Semantic Versioning](https://semver.org/) to ensure consistency and clarity in version tracking. Follow these guidelines for tagging versions in the repository.

**Table of Contents**
- [Format](#format)
- [Guidelines to Follow](#guidelines-to-follow)
- [Pre-release Tags](#pre-release-tags)
- [Automation](#automation)

## Format

```
<Major>.<Minor>.<Patch>
```

Where:

| Part      | Description                                                            |
| --------- | ---------------------------------------------------------------------- |
| **Major** | Incremented for major releases, new architecture, or breaking changes. |
| **Minor** | Incremented for backward-compatible feature additions or enhancements. |
| **Patch** | Incremented for backward-compatible bug fixes or small updates.        |

Examples:

- `2.0.0` – Major release with breaking changes or architecture revamp
- `1.1.0` – Minor release adding features, still backward compatible
- `1.0.1` – Patch release with bug fixes or minor improvements

## Guidelines to Follow

- Before tagging a version, ensure the following:
  - CI/CD pipelines are green.
  - The code is merged into the `main` branch.
  - Documentation is updated to reflect the changes in the new version.
- Do not tag `dev`, `feature/`, or other WIP branches.
- Ensure the tag adheres to the semantic versioning format.
- Avoid overwriting existing tags.

## Pre-release Tags

For pre-release versions, use the following format:

```
<Major>.<Minor>.<Patch>-<PreRelease>
```

Examples:
- `1.0.0-alpha` – Alpha release for testing purposes.
- `1.0.0-beta` – Beta release for broader testing.

## Automation

If your team uses CI/CD pipelines to automate tagging, ensure the pipeline adheres to these guidelines and includes proper validation steps.
