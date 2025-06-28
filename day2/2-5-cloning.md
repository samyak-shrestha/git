🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** ✅ [Pushing Changes](./2-4-pushing-changes.md)

# 4. Cloning a Repository

## What is Cloning?

Cloning is the process of creating a local copy of a remote repository on your computer. This allows you to work on the project files, make changes, and use Git commands locally.

## When to Use Cloning

- When you want to start working on a project locally.
- When you have forked a repository and want to work on your fork.
- When you are a collaborator and want to contribute directly.

## Cloning Your Own Repo vs. a Forked Repo

- **Cloning your own repo:** You have full access and can push changes directly.
- **Cloning a forked repo:** You work on your own copy and usually create pull requests to contribute back to the original.

## How to Clone a Repository

### Example: Cloning Your Fork

Suppose you have forked [https://github.com/samyak-shrestha/git-repo-example](https://github.com/samyak-shrestha/git-repo-example) to your own account.

1. **Copy the SSH or HTTPS URL from your fork:**
   - SSH: `git@github.com:<your-username>/git-repo-example.git`
   - HTTPS: `https://github.com/<your-username>/git-repo-example.git`

2. **Run the clone command in your terminal:**
   ```sh
   git clone git@github.com:<your-username>/git-repo-example.git
   ```

3. **Navigate into the cloned directory:**
   ```sh
   cd git-repo-example
   ```

4. **(Optional) Add the Original Repo as Upstream for Syncing:**
   This step helps you keep your fork up to date with the original repository.
   ```sh
   git remote add upstream git@github.com:samyak-shrestha/git-repo-example.git
   ```

### Example: Cloning the Original Repo

If you have permission to contribute directly, you can clone the original repository:

```sh
git clone git@github.com:samyak-shrestha/git-repo-example.git
cd git-repo-example
```
### Next Steps After Cloning

After cloning, you typically:

1. **Create and switch to a new branch:**
   ```sh
   git checkout -b my-feature-branch
   ```

2. **Make changes to files in your editor.**

3. **Stage your changes:**
   ```sh
   git add .
   ```

4. **Commit your changes:**
   ```sh
   git commit -m "Describe your changes"
   ```

5. **Push your branch to GitHub:**
   ```sh
   git push origin my-feature-branch
   ```

Now you’re ready to open a pull request or continue working!

---

## Summary Table

| Scenario                | Command Example                                               |
|-------------------------|--------------------------------------------------------------|
| Clone your fork (SSH)   | `git clone git@github.com:<your-username>/git-repo-example.git` |
| Clone your fork (HTTPS) | `git clone https://github.com/<your-username>/git-repo-example.git` |
| Clone original repo     | `git clone git@github.com:samyak-shrestha/git-repo-example.git`    |

---

**Tip:**  
- Use SSH for convenience if you have set up SSH keys.
- Always clone your fork if you plan to contribute

➡️**Up Next:** 🍴 [Forking a Repository](./2-6-forking.md)