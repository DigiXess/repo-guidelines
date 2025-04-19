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
  - The graphic assets are merged into the `main` branch.
  - Any relevant documentation or metadata for the assets is updated to reflect the changes in the new version.
- Do not tag `draft`, `update/`, or other WIP branches.
- Ensure the tag adheres to the semantic versioning format.
- Avoid overwriting existing tags.
