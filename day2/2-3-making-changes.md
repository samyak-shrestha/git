🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** 🌿 [ Branching in Git](./2-2-branching.md)

# 2. Making Changes & Committing

## Editing Files

After cloning a repository and switching to your branch, you can edit files using your preferred code editor (e.g., VS Code).

## Staging Changes

Before you can commit changes, you need to stage them. Staging lets you choose which changes to include in your next commit.

- Stage a specific file:
  ```sh
  git add filename.txt
  ```
- Stage all changed files:
  ```sh
  git add .
  ```

## Committing Changes

A commit saves your staged changes to the local repository. Always write a clear, descriptive commit message.

```sh
git commit -m "Describe your changes here"
```

## Example Workflow

1. **Edit a file:**  
   Make your changes in the code editor.

2. **Stage the changes:**  
   ```sh
   git add .
   ```

3. **Commit the changes:**  
   ```sh
   git commit -m "Add feature X or fix bug Y"
   ```

## Checking Status

You can check which files have changed and which are staged using:

```sh
git status
```

## Summary Table

| Action           | Command Example                        |
|------------------|----------------------------------------|
| Stage file       | `git add filename.txt`                 |
| Stage all files  | `git add .`                            |
| Commit changes   | `git commit -m "Your message"`         |
| Check status     | `git status`                           |

---

**Tip:**  
Commit often with meaningful messages to keep your project history clear and easy to


➡️**Up Next:** ✅ [Pushing Changes](./2-4-pushing-changes.md)
