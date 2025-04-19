## Protecting `main` Branch

The `main` branch should be protected to avoid accidental changes and to ensure that all updates are made through **Pull Requests (PRs)** with proper review.

This enforces quality control and maintains a clean, production-ready codebase.

Below are the steps to enable protection rules and enforce PR-based merges in 
- [GitHub](/common/protecting-repo-github.md "GIthub Repo Protection")
- [Bitbucket](/common/protecting-repo-bitbucket.md "Bitbucket Repo Protection")

### Recommendations

To ensure the `main` branch remains stable and secure, consider the following best practices:

- Require at least one reviewer for every Pull Request.
- Enable status checks to ensure all tests pass before merging.
- Restrict who can push directly to the `main` branch.
- Regularly audit branch protection rules to ensure compliance with organizational policies.
- Require signed commits to verify the authenticity of code changes.
- Enable linear history to avoid merge commits and keep the commit history clean.
- Automatically dismiss stale pull request approvals when new changes are pushed.
- Use code owners to enforce review by relevant experts for specific parts of the codebase.
- Enforce conversation resolution before allowing merges, ensuring all feedback is addressed.
- Require up-to-date branches to prevent merging outdated code into `main`.