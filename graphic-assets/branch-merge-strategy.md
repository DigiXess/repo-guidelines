# Branch and Merge Strategy

Keep your branch strategy simple for managing graphic asset repositories.

- Always push to the `main` branch from the `draft` branch only.
- **Pull before pushing:** Always pull the latest changes before pushing your work to avoid conflicts.
- Follow the branch name restrictions mentioned at [Branch name conventions](/common/branch-naming-rules.md).
- After a successful merge, delete the remote branch. **Never delete `draft` branches.**
- **Always branch from the correct base:**
    - `update/`, `add/`,`remove/` `experiment/`, `chore/` should branch from `draft`.
    - `hotfix/` should branch directly from `main`.
- Avoid `hotfix/` branches unless absolutely necessary. They should be used for urgent corrections directly on `main`.
- **Use Pull Requests for all merges:**
    - All changes must be merged via a Pull Request (PR) — no direct commits to `main` or `draft`.
    - Review and get approval before merging.
- **Rebase or Merge?**
    - Use Rebase (`git pull --rebase`) when syncing your local branch with `draft` — keeps history linear.
    - Use Merge commits when merging PRs — provides traceability.
- **Resolve Conflicts Proactively:**
    - Regularly pull from `draft` and resolve conflicts before opening a PR.
    - Avoid large, long-lived branches to minimize conflict risk.
- **Always Test:** Always review and test your graphic assets thoroughly before merging it into the `main` or `draft` branches to ensure it doesn't introduce any errors or inconsistencies.
- **Use `git stash` for uncommitted work:** If you're working on something and need to switch to a different branch, use `git stash` to temporarily save your changes without committing them. This prevents messy commits when you're in the middle of work.
- **Always verify the following before merging to `main`:**
    - ✅ Changes are reviewed and approved.
    - ✅ No merge conflicts.
    - ✅ Commit messages follow convention.
    - ✅ A pull request must be created for all changes.
    - ✅ Branch is up-to-date with `draft`.