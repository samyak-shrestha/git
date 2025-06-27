🏠 [Homepage](../README.md)

⬅️ **Previous:** [Connecting local repo to GitHub using SSH & Push to origin](./1-9-connecting-local-repo-to-remote-push.md)


## 10. 📋 Summary

### 🚀 Initialize & Push First Repo (Summary)

```bash
echo "# my-first-repo" >> README.md     # Create a README
git init                                # Initialize Git repo
git add README.md                       # Stage the README
git commit -m "first commit"            # Commit it
git branch -M main                      # Rename branch to main
git remote add origin git@github.com:samyak-shrestha/my-first-repo.git  # Link to GitHub
git push -u origin main                 # Push to GitHub
```

---

### 🔁 Repeated Git Workflow (Save & Push Changes)

```bash
git add .                             # Stage all changes
git commit -m "commit message"        # Commit with a message
git push origin branch-name           # Push to the correct branch
```

---

### 📘 Basic Git & Bash Commands (Cheat Sheet)

---

#### 🧰 Git Commands

| Command | Description |
|--------|-------------|
| `git status` | Show current status (what's staged, unstaged, untracked) |
| `git add filename` | Stage a specific file |
| `git add .` | Stage all changes in current directory |
| `git commit -m "message"` | Commit staged files with a message |
| `git push origin branch-name` | Push current branch to GitHub |
| `git log` | Show commit history |
|`git stash` | temporarily saves your uncommitted changes so you can work on something else and reapply them later.|
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

> 💡 **Tip:** Combine `git status` and `git add`/`git restore` regularly to keep your workflow clean.


---
### 🔐 SSH Setup Summary

```bash
# Generate SSH key
ssh-keygen -t ed25519 -C "your_email@example.com"

# Start SSH agent and add key
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519

# Copy public key
cat ~/.ssh/id_ed25519.pub

# Test connection
ssh -T git@github.com
```



➡️ **Up Next:** [ 📝 Hands-On Exercise](../day1/1-11-task.md)