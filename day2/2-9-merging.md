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

### 2. Merging Locally with `git pull`

```sh
git pull origin main
```
- This command **fetches** changes from the remote and **merges** them into your current branch in one step.
- Good for quick updates and personal projects.

### 3. Merging Locally with `git fetch` + `git merge`

```sh
git fetch origin main
git merge origin/main
```
- `git fetch` downloads changes but does **not** merge them.
- You can inspect changes (e.g., with `git diff origin/main`) before merging.
- `git merge origin/main` applies the changes when you're ready.
- Recommended for team settings or when you want more control.

---

## Pulling Merged Changes Locally

After merging a PR on GitHub, update your local repository:

1. **Switch to the main branch:**
   ```sh
   git checkout main
   ```

2. **Option 1: Quick update (automatic merge):**
   ```sh
   git pull origin main
   ```

3. **Option 2: Safer, manual update:**
   ```sh
   git fetch origin main
   git diff origin/main   # (optional) inspect incoming changes
   git merge origin/main
   ```

## Example Workflow

1. **Merge the PR on GitHub (as above).**
2. **Update your local main branch:**
   ```sh
   git checkout main
   git pull origin main
   # OR for more control:
   git fetch origin main
   git diff origin/main
   git merge origin/main
   ```

## Summary Table

| Action                | Command/Step                        |
|-----------------------|-------------------------------------|
| Merge PR on GitHub    | Click "Merge pull request"          |
| Switch to main branch | `git checkout main`                 |
| Pull & merge (quick)  | `git pull origin main`              |
| Fetch & merge (safe)  | `git fetch origin main` + `git merge origin/main` |
| Inspect changes       | `git diff origin/main`              |

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

**Tip:**  
Always pull or fetch the latest changes after a merge to keep your local repository up to date.

➡️**Up Next:** ⚡[Resolving Merge Conflicts](./2-10-merge-conflicts.md)