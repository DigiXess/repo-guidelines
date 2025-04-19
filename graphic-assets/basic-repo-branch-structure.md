# Documentation Repository Branch Structure

For managing documentation repositories effectively, use the following branch structure:

- **`main`**: This branch holds the **finalized and published documentation**. It is always stable and reflects the live version of the documents.
- **`draft`**: This branch is used for **ongoing updates and drafts**. It contains the latest changes but may not be finalized or ready for publication.

Additionally, use the following branch prefixes for specific purposes:

| Prefix        | Purpose                                                                         |
| ------------- | ------------------------------------------------------------------------------- |
| `update/`     | For **updating existing documentation**. Branches off `draft`.                  |
| `new-doc/`    | For creating **new documentation**. Branches off `draft`.                       |
| `hotfix/`     | For **urgent corrections** to published documentation directly on `main`.       |
| `archive/`    | For **archiving outdated documentation** that is no longer relevant.            |
| `experiment/` | For **testing new formats, layouts, or tools** for documentation.               |
| `chore/`      | For **repository maintenance tasks** like updating templates or configurations. |

### Example Workflow

1. A new feature requires documentation. Create a branch `new-doc/feature-guide` off `draft`.
2. Write the documentation and push changes to the `new-doc/feature-guide` branch.
3. Once complete, merge `new-doc/feature-guide` into `draft` via a pull request.
4. Review and finalize the changes in `draft`. If everything looks good, merge `draft` into `main` to publish the updates via pull request.

### Managing Digital Graphic Assets

For repositories containing digital graphic assets, follow these additional guidelines:

- **File Formats**: Use standard formats like `.png`, `.jpg`, `.svg`, or `.pdf` for compatibility.
- **Compression**: Optimize images to reduce file size without compromising quality. Use tools like [TinyPNG](https://tinypng.com/) or [ImageOptim](https://imageoptim.com/).
- **Naming Convention**: Use descriptive, lowercase filenames with hyphens (`-`) as separators. Avoid spaces or special characters. Example: `project-logo-v1.png`.
- **Storage**: Store graphic assets in a dedicated folder structure. For example:
  ```
  /graphic-assets/
    /logos/
    /diagrams/
    /screenshots/
  ```
- **Versioning**: Use branch prefixes like `update/graphics` or `new-doc/graphics` for changes related to graphic assets.
- **Attribution**: If using third-party assets, include attribution details in a `README.md` file within the `graphic-assets` folder.

### Example Workflow for Graphic Assets

1. A new diagram is required for documentation. Create a branch `new-doc/diagram-update` off `draft`.
2. Add the diagram to the appropriate folder under `graphic-assets/`.
3. Optimize the file and ensure it follows the naming convention.
4. Push changes to the `new-doc/diagram-update` branch.
5. Create a pull request to merge the branch into `draft`.
6. Once reviewed and approved, merge the changes into `draft` and eventually into `main` following the standard workflow.
