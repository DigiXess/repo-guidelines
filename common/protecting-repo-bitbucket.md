# Protecting Your Repository in Bitbucket

Follow the below procedure to protect a repository:
1. Go to your **repository**.
2. Click on **Repository settings** (⚙️ in the left sidebar).
3. Under **Workflow**, click **Branch restrictions**.
4. Click **Add a branch permission**.
5. Make the following if necessary changes:
    - **Branch name pattern**: `main`
    - **Write access**: Add the users or groups who should have write access to the `main` branch.
    - **Merge via pull request**: Add the users or groups who should be able to merge pull requests into the `main` branch.
    - **Allow deleting this branch**  (only if you want to allow branch deletion).
    - **Merge checks**: Make sure to select the appropriate checks that need to be passed before merging.
6. Click **Save**.

For more information, refer to the [Bitbucket documentation](https://support.atlassian.com/bitbucket-cloud/docs/set-up-branch-permissions/ "Grant repository access to users and groups
 ").