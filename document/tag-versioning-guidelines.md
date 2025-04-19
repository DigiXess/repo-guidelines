# Tag Versioning Guidelines

We follow [Semantic Versioning](https://semver.org/) to ensure consistency and clarity in version tracking. Follow these guidelines for tagging versions in the repository.
## Format

```
<Major>.<Minor>.<Patch>
```

Where:

| Part      | Description                                                            |
| --------- | ---------------------------------------------------------------------- |
| **Major** | Incremented for major updates, such as new documentation structure or breaking changes. |
| **Minor** | Incremented for backward-compatible additions or enhancements to documentation. |
| **Patch** | Incremented for backward-compatible fixes, such as typo corrections or minor updates. |

Examples:

- `2.0.0` – Added new document `docC` with a new structure.
- `1.1.0` – Minor release adding new sections Tto `docA` and `docB`.
- `1.0.1` – Patch release with typo corrections to file `docA`.

## Guidelines to Follow

- Before tagging a version, ensure the following:
  - The document is merged into the `main` branch.
  - Documentation is updated to reflect the changes in the new version.
- Do not tag `draft`, `update/`, or other WIP branches.
- Ensure the tag adheres to the semantic versioning format.
- Avoid overwriting existing tags.
