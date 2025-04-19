# Branch and Merge Strategy

Keep your branch strategy simple.

- Always push to the `main` branch from the `dev` or `staging` branch only.
- **Pull before pushing:** Always pull the latest changes before pushing your work to avoid conflicts.
- Follow the branch name restrictions mentioned at [Branch name conventions](/code/branch-naming-rules.md).
- After a successful merge, delete the remote branch. **Never delete `dev` and `staging` branches.**
- **Always branch from the correct base:**
    - `feature/`, `bugfix/`, `experiment/`, `chore/`, `docs/`, `test/`, `user/username/` should branch from `dev`.
    - `staging/` should branch from `dev` (when the code is stable).
    - `hotfix/` should branch directly from `main`.
- **Use Pull Requests for all merges:**
    - All changes must be merged via a Pull Request (PR) — no direct commits to `main` or `dev`.
    - Review and get approval before merging.
- **Rebase or Merge?**
    - Use Rebase (`git pull --rebase`) when syncing your local branch with `dev` — keeps history linear.
    - Use Merge commits when merging PRs — provides traceability.
- **Resolve Conflicts Proactively:**
    - Regularly pull from `dev` and resolve conflicts before opening a PR.
    - Avoid large, long-lived branches to minimize conflict risk.
- **Always Test:** Always test your code thoroughly before merging it into the `main`, `dev`, or `staging` branches to ensure it doesn't introduce any bugs or break existing functionality.
- **Use `git stash` for uncommitted work:** If you're working on something and need to switch to a different branch, use `git stash` to temporarily save your changes without committing them. This prevents messy commits when you're in the middle of work.
- **Always verify the following before merging to `main`:**
    - ✅ Code is reviewed and approved.
    - ✅ Tests have passed (CI pipeline is green).
    - ✅ No merge conflicts.
    - ✅ Commit messages follow convention.
    - ✅ A pull request must be created for all changes.
    - ✅ Branch is up-to-date with `dev` or `staging`.