# Documentation Repository Branch Structure

For managing graphic asset repositories effectively, use the following branch structure:

- **`main`**: This branch holds the **finalized and published documentation**. It is always stable and reflects the live version of the documents.
- **`draft`**: This branch is used for **ongoing updates and drafts**. It contains the latest changes but may not be finalized or ready for publication.

Additionally, use the following branch prefixes for specific purposes:

| Prefix        | Purpose                                                                         |
| ------------- | ------------------------------------------------------------------------------- |
| `update/`     | For **updating existing graphic asset**. Branches off `draft`.                  |
| `add/`        | For creating **new graphic asset**. Branches off `draft`.                       |
| `remove/`     | For **removing outdated graphic asset**. Branches off `draft`.                  |
| `hotfix/`     | For **urgent corrections** to published graphic asset directly on `main`.       |
| `archive/`    | For **archiving outdated graphic asset** that is no longer relevant.            |
| `experiment/` | For **testing new formats, layouts, or tools** for graphic asset.               |
| `chore/`      | For **repository maintenance tasks** like updating templates or configurations. |

## Example Adding a Graphic Asset (e.g., Logo)

1. Create a branch `add/logo` off `draft`.
1. Add the logo files to the branch.
1. Commit the changes with a descriptive message, such as `Add new logo for branding`.
1. Push the branch `add/logo` to the remote repository.
1. Review and finalize the changes in `draft`. If everything looks good, merge `draft` into `main` to publish the updates via pull request.
