🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** [📂 Introduction of Day 2](./2-1-intro.md)

# 1. Branching in Git

## What is a Branch?

A branch in Git is a lightweight movable pointer to a commit. It allows you to work on new features, bug fixes, or experiments in isolation from the main codebase.

## Why Use Branches?

- To develop features or fixes without affecting the main branch.
- To collaborate with others without interfering with each other's work.
- To organize work and manage releases.

## Creating a Branch

You can create a new branch using:

```sh
git branch my-feature-branch
```

Or create and switch to a new branch in one step:

```sh
git checkout -b my-feature-branch
```

With newer versions of Git, you can also use:

```sh
git switch -c my-feature-branch
```

## Switching Branches

To switch to an existing branch:

```sh
git checkout my-feature-branch
```

Or with the new command:

```sh
git switch my-feature-branch
```

## Best Practices for Naming Branches

- Use descriptive names, e.g., `feature/login-page`, `bugfix/fix-header`, `docs/update-readme`.
- Use lowercase and hyphens to separate words.

## Example Workflow

1. **Create and switch to a new branch:**
   ```sh
   git checkout -b feature/add-login
   ```

2. **Work on your changes and commit:**
   ```sh
   git add .
   git commit -m "Add login feature"
   ```

3. **Push your branch to GitHub:**
   ```sh
   git push origin feature/add-login
   ```

## Summary Table

| Action                  | Command Example                        |
|-------------------------|----------------------------------------|
| Create branch           | `git branch my-feature-branch`         |
| Create & switch branch  | `git checkout -b my-feature-branch`    |
| Switch branch           | `git checkout my-feature-branch`       |
| Push branch             | `git push origin my-feature-branch`    |

---

**Tip:**  
Always create a new branch for each feature or fix to keep your work organized and make collaboration


➡️**Up Next:**  [Making Changes & Committing](./2-3-making-changes.md)