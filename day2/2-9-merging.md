🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** 👥 [Adding Collaborators](./2-8-collaborators.md)

# 8. Merging the PR into Main

## What is Merging?

Merging is the process of integrating changes from one branch (often a feature branch) into another branch (usually `main`). This is typically done after a pull request (PR) is reviewed and approved.
## Ways to Merge Changes

There are multiple ways to bring changes from a remote repository into your local branch:

### 1. Merging via GitHub Pull Request

- Open a Pull Request (PR) on GitHub to propose your changes.
- After review and approval, click **Merge pull request** on GitHub.
- This is the recommended way for team collaboration and open source projects.

---

### 2. Merging Locally with `git pull`

```sh
git pull origin main
```

- This command **fetches** changes from the remote and **merges** them into your current branch in one step.
- **Which branch am I on?**
  - If you are on `main`, this updates your local `main` with the remote `main`.
  - If you are on another branch (e.g., `feature-branch`), this merges `origin/main` into your current branch (`feature-branch`).
- **You can pull from any remote branch into any current branch:**
  ```sh
  git pull origin other-branch
  ```
  This will merge `origin/other-branch` into your current branch.

**Example:**
```sh
git checkout feature-branch
git pull origin main
# This brings changes from remote main into your feature-branch
```

---

### 3. Merging Locally with `git fetch` + `git merge`

```sh
git fetch origin main
git merge origin/main
```

- `git fetch` downloads changes from the remote but does **not** merge them.
- `git merge origin/main` merges the fetched changes into your current branch.
- **Which branch am I on?**
  - If you are on `main`, this updates your local `main` with the remote `main`.
  - If you are on another branch, this merges `origin/main` into your current branch.
- **You can fetch and merge from any branch:**
  ```sh
  git fetch origin other-branch
  git merge origin/other-branch
  ```

**Example:**
```sh
git checkout feature-branch
git fetch origin main
git merge origin/main
# This brings changes from remote main into your feature-branch, but lets you inspect first
```
---

## `git pull` vs `git fetch` + `git merge`

| Use Case                        | Recommended Command(s)                |
|----------------------------------|---------------------------------------|
| Personal quick updates           | `git pull`                            |
| Team collaboration & safety      | `git fetch` + `git merge`             |
| Need to inspect before merging   | `git fetch` + `git diff`              |

- **`git pull`**: Fast, automatic, but can cause unexpected conflicts.
- **`git fetch` + `git merge`**: Safer, lets you review changes before merging.

**Pro Tip:**  
If you're unsure or working on shared branches, always prefer:
```sh
git fetch
git diff origin/main   # optional: inspect changes
git merge origin/main
```

---

## Summary Table

| Current Branch    | Command                  | Result                                              |
|-------------------|-------------------------|-----------------------------------------------------|
| main              | `git pull origin main`   | Updates local main with remote main                 |
| feature-branch    | `git pull origin main`   | Merges remote main into feature-branch              |
| any-branch        | `git pull origin branch` | Merges specified remote branch into current branch  |
| main              | `git fetch origin main` + `git merge origin/main` | Updates local main with remote main (with review)   |
| feature-branch    | `git fetch origin main` + `git merge origin/main` | Merges remote main into feature-branch (with review)|

---

**Tip 1:** Always check which branch you are on with `git status` before pulling or merging, especially in team settings.

**Tip 2:** Always pull or fetch the latest changes after a merge to keep your local repository up to date.

➡️**Up Next:** ⚡[Resolving Merge Conflicts](./2-10-resolving-merge-conflicts.md)