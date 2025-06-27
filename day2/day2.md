
# 📅 Day 2 – Collaboration, Branching & GitHub Essentials
**Theme:** Teamwork, Branching, Merge Conflicts & Pull Requests

---

## 🔧 Topics Covered
- 🔄 Forking a repository or Add user from Collaboration
- 🔄 Cloning a repository (`git clone`)
- 🌿 Branching in Git
  - `git branch`, `git checkout`
- 📝 Making changes on a new branc
- ✅ Staging, committing, and pushing changes
- 🚀 Push Your Branch to GitHub
- 🔁 Open a Pull Request (PR)
- Merge the PR into main
- Resolving merge conflicts (optional)

---

## 🔄 Fork the Shared Repository
[Github repo Link](https://github.com/samyak-shrestha/git-repo-example)

---
#### OR
---

## 🔄 Add User in Collboration
> add Users in Colloration and acts as a team

---

## 🔄 Clone the Repository

```bash
git clone git@github.com:your-username/your-repo-name.git
cd your-git-repo-name
```

---

## 🌿 Create Your Own Branch
```bash
git checkout -b feature-yourname
```

---

## 📝 Edit the `contributors.md` File

Example entry to add:
```markdown
### Samiksha Lama
- 🧠 Learner in Git & GitHub
- 💼 Interested in Web Dev
- 🔗 GitHub: [@samiksha-lama](https://github.com/samiksha-lama)
```

Or create a new personal file:
```bash
touch samiksha-lama.md
```

Add something like:
```markdown
# Samiksha Lama
Aspiring developer from Kathmandu learning Git & GitHub through hands-on practice.
```

---

## ✅ Stage & Commit Your Changes
```bash
git add .
git commit -m "Add my contribution"
```

---

## 🚀 Push Your Branch to GitHub
```bash
git push origin feature-yourname
```

---

## 🔁 Open a Pull Request (PR)
1. Go to your repo on GitHub
2. Click **“Compare & pull request”**
3. Add a meaningful title and description
4. Submit the PR

---

## ✅ Merge the PR into `main`
```bash
git checkout main
git fetch origin
git merge origin/feature-yourname
```

---


## 🎯 Final Task
- Add 1 personal bio in `contributors.md`
- Create your own page in `/people/yourname.md`