# Git and GitHub Learning Guide

## 📅 Day 1 – Git Basics & Local Setup
**Theme:** Getting Started with Git and SSH

### 🔧 Topics Covered
- Introduction to Version Control
- Installing Git and VS Code
- Basic Git Workflow
  - `git init`, `git status`, `git add`, `git commit`
- Understanding Repositories (Local vs Remote)
- Setting up GitHub Account
- Setting up SSH Keys
  - Why SSH is important
  - Generating SSH keys
  - Adding SSH key to GitHub
  - Verifying SSH connection
- Connecting local repo to GitHub using SSH
- Pushing first commit using `git remote` and `git push`

### ✅ Setup & Configuration
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

### 🗂️ Initialize Repository
```bash
git init
```


### 📂 Stage & Commit Changes
```bash
git status
git add .          # Stage all changes
git add filename   # Stage specific file
git commit -m "Your commit message"
```


### 🌐 Connect to Remote (GitHub)
```bash
git remote add origin git@github.com:username/repo.git
git push -u origin main   # First time push
```

### 🔐 Generate and Add SSH Key

```bash

ssh-keygen
```
or

```bash

ssh-keygen -t ed25519 -C "you@example.com"

cat ~/.ssh/id_ed25519.pub
```

##### Copy the output and add to GitHub → Settings → SSH and GPG Keys


### 🔍 Test SSH Connection
```bash
ssh -T git@github.com
```
