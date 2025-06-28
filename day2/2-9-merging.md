🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** 👥 [Adding Collaborators](./2-8-collaborators.md)

# 8. Merging the PR into Main

## What is Merging?

Merging is the process of integrating changes from one branch (often a feature branch) into another branch (usually `main`). This is typically done after a pull request (PR) is reviewed and approved.

## When to Merge

- After your pull request has been reviewed and approved.
- When you want to bring feature or bugfix changes into the main codebase.

## How to Merge a Pull Request on GitHub

1. **Go to the original repository on GitHub.**
2. Click on the **Pull Requests** tab.
3. Select the pull request you want to merge.
4. Review the changes and discussion.
5. Click the **Merge pull request** button.
6. Confirm the merge by clicking **Confirm merge**.

## Pulling Merged Changes Locally

After merging a PR on GitHub, update your local repository:

1. **Switch to the main branch:**
   ```sh
   git checkout main
   ```

2. **Pull the latest changes:**
   ```sh
   git pull origin main
   ```

## Example Workflow

1. **Merge the PR on GitHub (as above).**
2. **Update your local main branch:**
   ```sh
   git checkout main
   git pull origin main
   ```

## Summary Table

| Action                | Command/Step                        |
|-----------------------|-------------------------------------|
| Merge PR on GitHub    | Click "Merge pull request"          |
| Switch to main branch | `git checkout main`                 |
| Pull latest changes   | `git pull origin main`              |

---

**Tip:**  
Always pull the latest changes after a merge to keep your local repository up to

➡️**Up Next:** ⚡[Resolving Merge Conflicts](./2-10-merge-conflicts.md)