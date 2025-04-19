# Documentation Repository Branch Structure

For managing documentation repositories effectively, use the following branch structure:

- **`main`**: This branch holds the **finalized and published documentation**. It is always stable and reflects the live version of the documents.
- **`draft`**: This branch is used for **ongoing updates and drafts**. It contains the latest changes but may not be finalized or ready for publication.

Additionally, use the following branch prefixes for specific purposes:

| Prefix        | Purpose                                                                         |
| ------------- | ------------------------------------------------------------------------------- |
| `update/`     | For **updating existing documentation**. Branches off `draft`.                  |
| `add/`        | For creating **new documentation**. Branches off `draft`.                       |
| `remove/`     | For **removing outdated documentation**. Branches off `draft`.                  |
| `hotfix/`     | For **urgent corrections** to published documentation directly on `main`.       |
| `archive/`    | For **archiving outdated documentation** that is no longer relevant.            |
| `experiment/` | For **testing new formats, layouts, or tools** for documentation.               |
| `chore/`      | For **repository maintenance tasks** like updating templates or configurations. |

### Example Workflow

1. A new feature requires documentation. Create a branch `add/feature-guide` off `draft`.
2. Write the documentation and push changes to the `add/feature-guide` branch.
3. Once complete, merge `add/feature-guide` into `draft` via a pull request.
4. Review and finalize the changes in `draft`. If everything looks good, merge `draft` into `main` to publish the updates via pull request.
