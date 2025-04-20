# Tag Versioning Guidelines

We follow [Semantic Versioning](https://semver.org/) to ensure consistency and clarity in version tracking. Follow these guidelines for tagging versions in the repository.

## Format

```
<Major>.<Minor>.<Patch>
```

Where:

| Part      | Description                                                            |
| --------- | ---------------------------------------------------------------------- |
| **Major** | Incremented for major updates, such as new graphic asset categories or breaking changes. |
| **Minor** | Incremented for backward-compatible additions or enhancements to graphic assets. |
| **Patch** | Incremented for backward-compatible fixes, such as minor updates or corrections to graphic assets. |

Examples:

- `2.0.0` – Added a new category of graphic assets, such as "branding".
- `1.1.0` – Minor release adding new icons to the "UI" category.
- `1.0.1` – Patch release with updated color profiles for existing assets.

## Guidelines to Follow

- Before tagging a version, ensure the following:
  - The document is merged into the `main` branch.
  - Documentation is updated to reflect the changes in the new version.
- Ensure the tag adheres to the semantic versioning format.
- Avoid overwriting existing tags.

# Tagging `draft` versions
- Use prefix `draft-` for draft or development versions if needed on `dev` branch.
- Example: `draft-1.0.0` for a draft or development version of the 1.0.0 release.
