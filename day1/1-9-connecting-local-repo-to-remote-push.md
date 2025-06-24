[ 🏠 Homepage](../README.md)

⬅️ **Previous:** [🔐 Setting up SSH Keys](./1-8-ssh-keys.md)

## 9. 🌐 Connect Local Repo to Remote (GitHub)

```bash
git remote add origin git@github.com:username/repo.git
```

➡️ This command connects your local repository to a remote GitHub repository named `origin`.

> 🔗 Replace the URL with your actual repository URL.

---

### 10. Pushing First Commit

Once you've made your first commit locally, you need to connect your local repository to a remote repository (like GitHub) and push the code.


Use the -u flag with git push to set the upstream branch:

```bash
git push -u origin main
```

- `git push` → the command to upload your commits.

- `-u` tells Git to remember the remote branch (`origin/main`), so you can just use `git push` or `git pull` in the future.

- `origin` → the name of the remote (you can rename or have multiple remotes).



- `main`  → the branch you're pushing.

✅ Now your local project is connected and pushed to GitHub!


➡️**Up Next:**[📋 Summary](./1-10-summary.md)
