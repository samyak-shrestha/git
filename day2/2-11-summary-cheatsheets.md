🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** ⚡[Resolving Merge Conflicts](./2-10-resolving-merge-conflicts.md)

## 📋 Day 2 Summary

### 🚦 Key Concepts Covered

- **Branching:** Create and switch between branches to work on features or fixes independently.
- **Making Changes & Committing:** Edit files, stage changes, and commit with meaningful messages.
- **Pushing Changes:** Upload your branch and commits to GitHub.
- **Cloning:** Get a local copy of a remote repository (your own, a fork, or as a collaborator).
- **Forking:** Make your own copy of someone else’s repository to contribute without direct access.
- **Pull Requests:** Propose your changes for review and merging into the main project.
- **Collaborators:** Add trusted team members for direct access and contribution.
- **Merging:** Integrate changes from one branch into another (locally or via GitHub PR).
- **Resolving Merge Conflicts:** Handle situations where changes overlap and Git cannot merge automatically.

---

### 🔁 Common Git Workflow (Collaboration)

```bash
1. Create and switch to a new branch
    git checkout -b feature/my-feature

2. Make changes and stage them
    git add .

3. Commit your changes
    git commit -m "Add my feature"

4. Push your branch to GitHub
    git push origin feature/my-feature

5. Open a Pull Request on GitHub
6. Review, resolve conflicts if any, and merge the PR
```

## 📘 Useful Git & Bash Commands

---

### 🧰 Git Commands

| Command | Description |
|--------|-------------|
| `git branch` | List all local branches |
| `git branch branch-name` | Create a new branch |
| `git checkout branch-name` | Switch to a branch |
| `git checkout -b branch-name` | Create and switch to a new branch |
| `git switch branch-name` | Switch to a branch (newer syntax) |
| `git switch -c branch-name` | Create and switch to a new branch (newer syntax) |
| `git add filename` | Stage a specific file |
| `git add .` | Stage all changes in current directory |
| `git commit -m "message"` | Commit staged files with a message |
| `git push origin branch-name` | Push current branch to GitHub |
| `git pull origin branch-name` | Pull changes from remote branch and merge |
| `git fetch origin branch-name` | Fetch changes from remote branch (no merge) |
| `git merge branch-name` | Merge another branch into current branch |
| `git log --oneline --graph` | Visualize commit history as a graph |
| `git status` | Show current status (what's staged, unstaged, untracked) |
| `git diff` | Show unstaged changes |
| `git diff branch1..branch2` | Show differences between two branches |
| `git remote -v` | Show remote repositories |
| `git clone repo-url` | Clone a remote repository |
| `git stash` | Temporarily save uncommitted changes |

---

### 💻 Bash Commands

| Command | Description |
|--------|-------------|
| `cd foldername` | Change directory |
| `cd ..` | Go up one level |
| `ls` | List files/folders |
| `ls -a` | List all files including hidden |
| `touch filename` | Create a new empty file |
| `mkdir foldername` | Create a new directory |
| `cat filename` | View file content |
| `rm filename` | Delete a file |
| `clear` | Clear terminal screen |
| `pwd` | Show current directory path |
---

---

> 💡 **Tip:** Use `git status` often to keep track of your changes

➡️**Up Next:** 📝[Hands-On Exercise](./2-12-task.md)