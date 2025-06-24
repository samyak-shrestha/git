
# 📅 Day 2 – Collaboration, Branching & GitHub Essentials
**Theme:** Teamwork, Branching, Merge Conflicts & Pull Requests

---

## 🔧 Topics Covered
- Cloning repositories from GitHub
- Creating and switching branches
- Editing files as a team
- Staging, committing, and pushing changes
- Creating and reviewing Pull Requests
- Handling merge conflicts
- Intro to GitHub Desktop (Optional)

---

## 🔄 Clone the Shared Repository
[Github repo](https://github.com/samyak-shrestha/git-repo-example)
```bash
git clone git@github.com:samyak-shrestha/git-repo-example.git
cd git-repo-example
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

## ⚠️ Simulate a Merge Conflict (Instructor or 2 users)
1. Edit the same line in `contributors.md` in two branches
2. Merge one PR
3. Pull latest and fix conflict

```bash
git pull origin main
# Manually fix conflict in file
git add .
git commit -m "Fix merge conflict"
git push
```

---

## ✅ Merge the PR into `main`
```bash
git checkout main
git pull
git merge feature-yourname
```

---

## 🖥️ Optional: Use GitHub Desktop
1. Create branch
2. Edit file
3. Commit changes
4. Push and open PR using GUI

---

## 🎯 Final Team Task (Optional)
- Add 1 personal bio in `contributors.md`
- Create your own page in `/people/yourname.md` or `.html`
