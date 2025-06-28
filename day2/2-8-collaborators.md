🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** 🔁 [Opening a Pull Request (PR)](./2-7-pull-requests.md)

# 7. Adding Collaborators (Alternative to Forking)

## What is a Collaborator?

A collaborator is someone who has been granted direct write access to a repository. Collaborators can push changes, create branches, and merge pull requests without needing to fork the repository.

## When to Add Collaborators

- For private or team projects where you want to work closely with others.
- When you trust contributors to make direct changes to the repository.
- To simplify the workflow (no need to fork and create pull requests from forks).

## How to Add Collaborators on GitHub

1. **Go to your repository on GitHub.**
2. Click on the **Settings** tab.
3. In the left sidebar, click **Collaborators & teams** (or **Manage access**).
4. Click **Add people**.
5. Enter the GitHub username of the person you want to add and click **Add**.

## Permissions Required

- Only repository owners or users with admin rights can add collaborators.
- Collaborators can push, pull, and create branches.

## Cloning as a Collaborator

Once added as a collaborator, you can clone the repository and push changes directly:

```sh
git clone git@github.com:owner/repo-name.git
cd repo-name
```

## Example Workflow for Collaborators

1. **Clone the repository:**
   ```sh
   git clone git@github.com:owner/repo-name.git
   cd repo-name
   ```

2. **Create a new branch for your changes:**
   ```sh
   git checkout -b feature/your-feature
   ```

3. **Make changes, commit, and push:**
   ```sh
   git add .
   git commit -m "Describe your changes"
   git push origin feature/your-feature
   ```

4. **Open a pull request** (recommended for code review).

## Summary Table

| Action                | Description/Command                                  |
|-----------------------|-----------------------------------------------------|
| Add collaborator      | Settings → Collaborators & teams → Add people       |
| Clone repo            | `git clone git@github.com:owner/repo-name.git`      |
| Create branch         | `git checkout -b feature/your-feature`              |
| Push branch           | `git push origin feature/your-feature`              |

---

**Tip:**  
Adding collaborators is best for trusted team members working on private or shared projects.

➡️**Up Next:** 🔀 [Merging the PR into Main](./2-9-merging.md)