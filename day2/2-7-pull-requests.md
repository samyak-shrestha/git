🏠 [Homepage](../README.md)
🏠 [Syllabus of Day 2](./2-1-intro.md)
⬅️ **Previous:** 🍴 [Forking a Repository](./2-6-forking.md)

# 6. Opening a Pull Request (PR)

## What is a Pull Request?

A Pull Request (PR) is a way to propose your changes from your branch or fork to be merged into another repository’s branch (usually the main branch). It allows others to review, discuss, and approve your changes before they become part of the main codebase.

## When to Open a Pull Request

- After pushing your branch with your changes to GitHub.
- When you want your changes to be reviewed and merged into the original repository.

## How to Open a Pull Request on GitHub

1. **Push your branch to GitHub:**
   ```sh
   git push origin my-feature-branch
   ```

2. **Go to your repository on GitHub.**

3. **Click the "Compare & pull request" button** that appears near the top of your repo.

4. **Fill in the PR title and description:**
   - **Title:** A short summary of your changes.
   - **Description:** Details about what you changed and why.

5. **Select the base repository and branch** you want to merge into (usually `main`), and the compare branch (your feature branch).

6. **Submit the pull request.**

## Example PR Title and Description

- **Title:**  
  `Add login feature`

- **Description:**  
  ```
  This PR adds a login page with authentication logic.  
  - Implements form validation  
  - Connects to backend API  
  - Adds basic styling  
  ```

## What Happens Next?

- Reviewers can comment, request changes, or approve your PR.
- Once approved, your PR can be merged into the main branch.

## Summary Table

| Step                | Action/Description                                 |
|---------------------|----------------------------------------------------|
| Push branch         | `git push origin my-feature-branch`                |
| Open PR             | Click "Compare & pull request" on GitHub           |
| Fill PR details     | Add title and description                          |
| Submit PR           | Click "Create pull request"                        |

---

**Tip:**  
Write clear titles and descriptions to help reviewers understand your changes.

➡️**Up Next:** 👥 [Adding Collaborators](./2-8-collaborators.md)