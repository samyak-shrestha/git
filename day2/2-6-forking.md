🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** 🔄 [Cloning a Repository](./2-5-cloning.md)

# 5. Forking a Repository

## What is Forking?

Forking is the process of creating a personal copy of someone else’s repository on your own GitHub account. This allows you to freely experiment with changes without affecting the original project.

## When to Use Forking

- **Open Source Contributions:** When you want to contribute to a project you don’t own or don’t have write access to.
- **Experimentation:** When you want to try new features or fixes without impacting the main repository.
- **Learning:** When you want to study or modify a project for your own understanding.

**You should fork when you do NOT have collaborator access to the repository.**

## Why Fork Instead of Clone?

- **Fork:** Creates a copy on your GitHub account, allowing you to propose changes via Pull Requests.
- **Clone:** Only creates a local copy; you cannot push changes to the original repo unless you have write access.

## How to Fork a Repo on GitHub

1. **Go to the Repository:**  
   Visit [https://github.com/samyak-shrestha/git-repo-example](https://github.com/samyak-shrestha/git-repo-example).

2. **Click the "Fork" Button:**  
   At the top right of the page, click the **Fork** button.

3. **Choose Your Account:**  
   Select your GitHub account as the destination for the fork.

4. **Your Fork is Created:**  
   You now have a copy at `https://github.com/<your-username>/git-repo-example`.

## Example Workflow: Fork, Clone, and Contribute

1. **Fork the Repository**  
   As described above.

2. **Clone Your Fork Locally**
   ```sh
   git clone git@github.com:<your-username>/git-repo-example.git
   cd git-repo-example
   ```

3. **Add the Original Repo as Upstream (Optional, for syncing)**
   ```sh
    git remote add upstream git@github.com:samyak-shrestha/git-repo-example.git
   ```


4. **Create a Branch for Your Changes**
   ```sh
    git checkout -b my-feature-branch
   ```

5. **Make Changes, Commit, and Push**
   ```sh
    git add .
    git commit -m "Add my feature"
    git push origin my-feature-branch
   ```

6. **Open a Pull Request**
    - Go to your fork on GitHub.
    - Click "Compare & pull request".
    - Fill in the details and submit.


### Summary Table    
| Topic                | Description/Goal                                              |
|----------------------|--------------------------------------------------------------|
| Fork              | Click "Fork" on GitHub                       |
| Clone fork              | `git clone git@github.com:<your-username>/git-repo-example.git`              |
| Add upstream            | `git remote add upstream git@github.com:samyak-shrestha/git-repo-example.git`        |
| Create branch       | `git checkout -b my-feature-branch`                                 |
| Pushing Changes      | `git push origin my-feature-branch`                                 |
| Pull Requests        | Open PR from your fork to the original repo                   |

---


**Tip**: Forking is the standard workflow for contributing to open source projects when you don’t have write access.


➡️**Up Next:** 🔁 [Opening a Pull Request (PR)](./2-7-pull-requests.md)