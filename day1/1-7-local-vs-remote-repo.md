[ 🏠 Homepage](../README.md)

⬅️ **Previous:** [🔄 Basic Git Workflow](./1-6-basic-git-workflow.md)

## 7. 📂 Understanding Repositories: Local vs Remote

When working with Git and GitHub, it’s important to understand the difference between **local** and **remote** repositories.

---

### 🖥️ Local Repository

A **local repository** exists on your own computer. It is where you:
- Write your code
- Track changes with Git
- Make commits

#### ✅ Example:
```bash
git init my-project
cd my-project
touch index.html
git add .
git commit -m "Initial commit"
```

_Now you have a Git repository only on your computer._

---

### 🌐 Remote Repository

A remote repository is hosted on a server like GitHub. It's used to:

- Backup your work online

- Share code with others

- Collaborate in teams

You can **connect** your local repo to GitHub:
✅ Example:
```bash
git remote add origin git@github.com:username/my-project.git
git push -u origin main
```

This pushes your local changes to the **remote GitHub repository**.


### 🔁 Common Git Commands

| Action        | Command                              |
|---------------|---------------------------------------|
| Clone repo    | `git clone <repo-url>`                |
| Add remote    | `git remote add origin <repo-url>`    |
| Push changes  | `git push origin main`                |
| Pull updates  | `git pull origin main`                |

---

### 🎯 Summary

| Feature              | Local Repository       | Remote Repository          |
|----------------------|------------------------|----------------------------|
| Location             | On your device         | On a server (e.g., GitHub) |
| Access               | Only you               | Anyone with permission     |
| Purpose              | Write & test code      | Share & collaborate        |

---

> 💡 **Tip:** Always commit locally first, then push to remote to save and share your work.

➡️**Up Next:** [🔐 Setting up SSH Keys](./1-8-ssh-keys.md)