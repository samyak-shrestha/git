# Re-define and save markdown content for Day 1, Day 2, and Day 3 after code state reset

# Day 1 content
day1 = """
# 📅 Day 1 – Git Basics & Local Setup
**Theme:** Getting Started with Git and SSH

## 🔧 Topics Covered
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
"""

# Day 2 content
day2 = """
# 📅 Day 2 – Collaboration & GitHub Essentials
**Theme:** Working in Teams and Resolving Conflicts

## 🤝 Topics Covered
- Cloning a repository (`git clone`)
- Pulling updates (`git pull`)
- Branching in Git
  - `git branch`, `git checkout`, `git switch`
- Making changes on a new branch
- Merging branches with `git merge`
- Resolving merge conflicts
- Introduction to GitHub Desktop
  - Installing and basic usage
  - Visualizing branches, commits, pushes
- Best Practices
  - Commit messages
  - Using `.gitignore`
  - Adding a `README.md`
"""

# Day 3 content
day3 = """
# 📅 Day 3 – GitHub Pages & Portfolio Building
**Theme:** Showcasing Yourself as a Developer

## 🌐 Topics Covered
- Introduction to GitHub Pages
- Creating a portfolio or CV repository (e.g., `username.github.io`)
- Writing in Markdown (`README.md`, `index.md`)
- Publishing static websites using GitHub Pages
- Using templates (starter HTML/CSS or Markdown files)
- Optional: Setting up a custom domain
- Updating and managing GitHub Pages
- Overview of GitHub Student Developer Pack
- Q&A and task submission instructions for certificate
"""

# Save each day as markdown file
paths = {
    "Day1_Git_Basics.md": day1,
    "Day2_Collaboration.md": day2,
    "Day3_GitHub_Pages.md": day3
}

saved_files = []

for filename, content in paths.items():
    path = f"/mnt/data/{filename}"
    with open(path, "w") as f:
        f.write(content)
    saved_files.append(path)

saved_files
