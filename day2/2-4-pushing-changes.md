🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** 📝 [Making Changes & Committing](./2-3-making-changes.md)


# 3. Pushing Changes

## What is Pushing?

Pushing is the process of uploading your local branch commits to a remote repository on GitHub. This makes your changes available to others and allows you to open pull requests.

## When to Push

- After committing your changes locally.
- When you want to share your work or back it up remotely.
- Before opening a pull request.

## How to Push Changes

### Push Your Current Branch

```sh
git push origin my-feature-branch
```
Replace `my-feature-branch` with the name of your branch.

### Push All Branches (not common)

```sh
git push --all origin
```

## Example Workflow

1. **Make and commit your changes:**
   ```sh
   git add .
   git commit -m "Describe your changes"
   ```

2. **Push your branch to GitHub:**
   ```sh
   git push origin my-feature-branch
   ```

## Checking Remote Branches

To see which branches exist on the remote:

```sh
git branch -r
```

## Summary Table

| Action            | Command Example                        |
|-------------------|----------------------------------------|
| Push branch       | `git push origin my-feature-branch`    |
| Push all branches | `git push --all origin`                |
| List remote branches | `git branch -r`                     |

---

**Tip:**  
Always push your branch before opening a pull request so your changes are available on

➡️**Up Next:** 🔄 [Cloning a Repository](./2-5-cloning.md)