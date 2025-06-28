🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** 🔀 [Merging the PR into Main](./2-9-merging.md)

# 9. Resolving Merge Conflicts

## What are Merge Conflicts?

A merge conflict occurs when Git cannot automatically combine changes from different branches because the same lines in a file have been changed in both branches. This usually happens during merging or rebasing.

## When Do Merge Conflicts Happen?

- When two people edit the same line in a file on different branches.
- When a file is deleted in one branch but modified in another.
- When changes overlap in a way Git cannot resolve automatically.

## How to Resolve Merge Conflicts

1. **Try to merge branches:**
   ```sh
   git merge branch-name
   ```
   If there are conflicts, Git will pause the merge and mark the conflicted files.

2. **Identify conflicted files:**
   ```sh
   git status
   ```
   Conflicted files will be listed as "both modified".

3. **Open the conflicted files in your editor.**
   - Git marks conflicts like this:
     ```
     <<<<<<< HEAD
     Your changes
     =======
     Incoming changes
     >>>>>>> branch-name
     ```
   - Edit the file to keep the correct changes and remove the conflict markers.

4. **Stage the resolved files:**
   ```sh
   git add filename.txt
   ```

5. **Complete the merge:**
   ```sh
   git commit
   ```
   (If you were in the middle of a merge, this will finish it.)

## Example Workflow

```sh
git checkout main
git pull origin main
git merge feature-branch
# Resolve conflicts in your editor
git add conflicted-file.txt
git commit
```

## Tips for Avoiding Conflicts

- Pull the latest changes from the main branch before starting new work.
- Communicate with your team about which files you are editing.
- Make small, frequent commits and merges.

## Summary Table

| Step                    | Command/Action                        |
|-------------------------|---------------------------------------|
| Start merge             | `git merge branch-name`               |
| Check conflicts         | `git status`                          |
| Edit files              | Resolve conflict markers in editor    |
| Stage resolved files    | `git add filename.txt`                |
| Complete merge          | `git commit`                          |

---

**Tip:**  
Take your time resolving conflicts and test your code after merging to ensure everything works


➡️ **Up Next:** [ 🏠  Homepage](../README.md)