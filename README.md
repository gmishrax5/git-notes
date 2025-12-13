# ✨ Git Notes — A Friendly Git & GitHub Cheatsheet
A compact, practical guide to the most used Git and GitHub commands — ideal for beginners and a quick reference for experienced users.

## 📌 Table of Contents
- [Quick Start](#-quick-start)
- [Common Workflow](#-common-workflow)
- [Cheat Sheet (by category)](#-cheat-sheet-by-category)
- [Advanced Tips](#-advanced-tips)
- [VSCode Tips](#-vscode-tips)
- [Contributing](#-contributing)
- [Resources](#-resources)
- [Contact](#-contact)

---

## 🚀 Quick Start
Install Git and configure your identity:

```bash
# install: go to https://git-scm.com for platform-specific installers
git --version

...

## ✅ Common Workflow
The typical flow for feature development:

1. Create a branch
```bash
git checkout -b feature/your-feature
```
2. Make changes, stage, and commit
```bash
git add .
git commit -m "Short, descriptive message"
```
3. Sync with remote and push
```bash
git fetch origin
git pull --rebase origin main
git push -u origin feature/your-feature
```
4. Open a PR, then delete the branch after merge
```bash
git branch -d feature/your-feature
git push origin --delete feature/your-feature
```

---

## 🎯 Cheat Sheet (by category)

### Setup & Quick Actions
- `git init` — initialize a repo
- `git clone <url>` — clone a remote repo
- `git status` — see working state
- `git add <file> | .` — stage changes
- `git commit -m "msg"` — commit
- `git push` — push to remote
- `git pull` — fetch & merge

### Branching & Merging
- `git branch` — list branches
- `git checkout <branch>` — switch
- `git checkout -b <branch>` — create+switch
- `git merge <branch>` — merge into current
- `git rebase <base>` — replay commits

### Inspecting History
- `git log --oneline --graph --decorate` — condensed log
- `git show <commit>` — inspect a commit

### Undoing & Cleanup
- `git restore <file>` — discard local changes
- `git reset --soft HEAD~1` — undo last commit (keep changes staged)
- `git reset --hard HEAD~1` — undo last commit and discard changes
- `git clean -f` — remove untracked files

### Tags & Stashes
- `git tag <tag>` — lightweight tag
- `git tag -a <tag> -m "message"` — annotated tag
- `git stash` / `git stash pop` — stash and restore

### Remote Controls
- `git remote -v` — list remotes
- `git remote add origin <url>` — add a remote
- `git remote set-url origin <new-url>` — change remote

---

## 💡 Advanced Tips & Best Practices
- Use clear, concise commit messages.
- Keep PRs small and focused.
- Rebase onto the main branch before opening a PR to keep history linear.
- Resolve conflicts locally with `git status` and `git diff` to inspect changes.

Short commands for speed:
```bash
git status -s               # short status
git log --oneline --graph   # compact log w/graph
```

---

## 🛠️ VSCode Tips
- Try extensions: GitLens, Git Graph, and GitHub Pull Requests for better visibility.
- Use the Source Control view to stage commits and manage branches.
- Open the integrated terminal for quick git commands without leaving the editor.

---

## 🤝 Contributing
To contribute:

1. Fork the repository on GitHub.
2. Clone your fork and create a branch for your work.
3. Make changes, add tests if applicable, and commit.
4. Stay in sync with upstream and rebase often:
```bash
git remote add upstream https://github.com/ORIGINAL/REPO.git
git fetch upstream
git rebase upstream/main
```
5. Push your branch to your fork and open a PR with a helpful description.

---

## 📚 Resources
- Official Git docs: https://git-scm.com/docs
- GitHub docs: https://docs.github.com/en
- GitHub Git Cheat Sheet: https://education.github.com/git-cheat-sheet-education.pdf

---

## ✉️ Contact
Found something missing? Open an issue or a PR — contributions and suggestions are welcome!

---

Made with ❤️

## 📌 Table of Contents
- [Quick Start](#-quick-start)
- [Common Workflow](#-common-workflow)
- [Cheat Sheet (by category)](#-cheat-sheet-by-category)
- [Advanced Tips](#-advanced-tips)
- [VSCode Tips](#-vscode-tips)
- [Contributing](#-contributing)
- [Resources](#-resources)
- [Contact](#-contact)

---

## 🚀 Quick Start
Install Git and configure your identity:

```bash
# install: go to https://git-scm.com for platform-specific installers
git --version

# configure (one-time):
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Clone a repo and open it:

```bash
git clone https://github.com/<username>/<repo>.git
cd <repo>
```

---

## ✅ Common Workflow
The typical flow for feature development:

1. Create a branch
```bash
git checkout -b feature/your-feature
```
2. Make changes, stage, and commit
```bash
git add .
git commit -m "Short, descriptive message"
```
3. Sync with remote and push
```bash
git fetch origin
git pull --rebase origin main
git push -u origin feature/your-feature
```
4. Open a PR, then delete the branch after merge
```bash
git branch -d feature/your-feature
git push origin --delete feature/your-feature
```

---

## 🎯 Cheat Sheet (by category)

### Setup & Quick Actions
- `git init` — initialize a repo
- `git clone <url>` — clone a remote repo
- `git status` — see working state
- `git add <file> | .` — stage changes
- `git commit -m "msg"` — commit
- `git push` — push to remote
- `git pull` — fetch & merge

### Branching & Merging
- `git branch` — list branches
- `git checkout <branch>` — switch
- `git checkout -b <branch>` — create+switch
- `git merge <branch>` — merge into current
- `git rebase <base>` — replay commits

### Inspecting History
- `git log --oneline --graph --decorate` — condensed log
- `git show <commit>` — inspect a commit

### Undoing & Cleanup
- `git restore <file>` — discard local changes
- `git reset --soft HEAD~1` — undo last commit (keep changes staged)
- `git reset --hard HEAD~1` — undo last commit and discard changes
- `git clean -f` — remove untracked files

### Tags & Stashes
- `git tag <tag>` — lightweight tag
- `git tag -a <tag> -m "message"` — annotated tag
- `git stash` / `git stash pop` — stash and restore

### Remote Controls
- `git remote -v` — list remotes
- `git remote add origin <url>` — add a remote
- `git remote set-url origin <new-url>` — change remote

---

## 💡 Advanced Tips & Best Practices
- Use clear, concise commit messages.
- Keep PRs small and focused.
- Rebase onto the main branch before opening a PR to keep history linear.
- Resolve conflicts locally with `git status` and `git diff` to inspect changes.

Short commands for speed:
```bash
git status -s               # short status
git log --oneline --graph   # compact log w/graph
```

---

## 🛠️ VSCode Tips
- Try extensions: GitLens, Git Graph, and GitHub Pull Requests for better visibility.
- Use the Source Control view to stage commits and manage branches.
- Open the integrated terminal for quick git commands without leaving the editor.

---

## 🤝 Contributing
To contribute:

1. Fork the repository on GitHub.
2. Clone your fork and create a branch for your work.
3. Make changes, add tests if applicable, and commit.
4. Stay in sync with upstream and rebase often:
```bash
git remote add upstream https://github.com/ORIGINAL/REPO.git
git fetch upstream
git rebase upstream/main
```
5. Push your branch to your fork and open a PR with a helpful description.

---

## 📚 Resources
- Official Git docs: https://git-scm.com/docs
- GitHub docs: https://docs.github.com/en
- GitHub Git Cheat Sheet: https://education.github.com/git-cheat-sheet-education.pdf

---

## ✉️ Contact
Found something missing? Open an issue or a PR — contributions and suggestions are welcome!

---

Made with ❤️

## 📌 Table of Contents
- [Quick Start](#-quick-start)
- [Common Workflow](#-common-workflow)
- [Cheat Sheet (by category)](#-cheat-sheet-by-category)
- [Advanced Tips](#-advanced-tips)
- [Contributing](#-contributing)
- [Resources](#-resources)
- [Contact](#-contact)

---

Made with ❤️
```

---

## 🎯 Cheat Sheet (by category)

### Setup & Quick Actions
- `git init` — initialize a repository
- `git clone <url>` — copy a remote repo locally
- `git status` — see current changes
- `git add <file> | .` — stage changes
- `git commit -m "message"` — commit staged changes
- `git push` — send commits to remote
- `git pull` — fetch + merge latest remote changes

### Branching & Merging
- `git branch` — list branches
- `git checkout <branch>` — switch branch
- `git checkout -b <branch>` — create+switch
- `git merge <branch>` — merge a branch into current one
- `git rebase <base>` — replay changes onto base

### History & Log
- `git log --oneline --graph --decorate` — compact visual commit log
- `git show <commit>` — show commit details

### Undoing & Cleanup
- `git restore <file>` — restore file to last commit state
- `git reset --soft HEAD~1` — undo commit (keep changes staged)
- `git reset --hard HEAD~1` — undo commit and discard changes
- `git clean -f` — remove untracked files

### Tags & Releases
- `git tag <tag>` — add a lightweight tag
- `git tag -a <tag> -m "message"` — annotated tag
- `git push origin <tag>` — push tag to remote

### Stashes
- `git stash` — stash uncommitted changes
- `git stash apply` — restore latest stash
- `git stash pop` — restore and remove stash

### Remote
- `git remote -v` — list remotes
- `git remote add origin <url>` — add remote
- `git remote set-url origin <new-url>` — change remote URL

---

## 💡 Advanced Tips & Best Practices
- Use meaningful commit messages and keep them short.
- Keep branches small and focused.
- Prefer PRs for code review and CI checks before merging.
- Use `git pull --rebase` to keep history linear when you pull.
- Resolve conflicts on a clean branch; use `git status` and `git diff` frequently.

Short commands:
```bash
git status -s               # short status
git log --oneline --graph   # brief log with graph
```

---

## 🛠️ VSCode Tips
- Install useful extensions: GitLens, Git Graph.
- Use built-in Source Control to stage and commit quickly.
- Use the integrated terminal for small Git workflows.

---

## 🤝 Contributing
If you want to contribute to this project or another GitHub repo:

1. Fork the repository on GitHub.
2. Clone your fork, create a branch for your change.
3. Make changes, add tests where appropriate, and commit.
4. Rebase/sync with upstream before opening a PR.
5. Push your branch and open a pull request with a clear description.

Quick commands:
```bash
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
git remote add upstream https://github.com/ORIGINAL-USER/REPO-NAME.git
git fetch upstream && git rebase upstream/main
```

---

## 📚 Resources
- Official Git docs: https://git-scm.com/docs
- Git cheatsheet: https://education.github.com/git-cheat-sheet-education.pdf
- GitHub docs: https://docs.github.com/en

---

## ✉️ Contact
If you want to suggest improvements, open an issue or a PR. I appreciate your feedback — thanks for checking out Git Notes!

---

Made with ❤️





This documentation serves as a comprehensive reference for all major Git and GitHub commands, along with their descriptions and usage.

---

## 1. Initializing and Adding Local Files to GitHub

### Initialize Git Repository
```bash
git init
```
**Description**: Initializes a new local Git repository in the current directory.

### Stage Files
```bash
git add <file-name>
git add .
```
**Description**: Adds specific files or all files in the current directory to the staging area.

### Commit Changes
```bash
git commit -m "Initial commit"
```
**Description**: Saves the changes in the staging area to the local repository with a descriptive message.

### Connect to a GitHub Remote Repository
```bash
git remote add origin <repository-url>
```
**Description**: Links your local repository to a GitHub remote repository.

### Push Files to GitHub
```bash
git push -u origin <branch-name>
```
**Description**: Pushes the local files to the specified branch of the GitHub repository.

---

## 2. Making Changes to an Existing Repository

### Clone a Repository
```bash
git clone <repository-url>
```
**Description**: Downloads an existing GitHub repository to your local machine.

### Navigate to the Repository
```bash
cd <repository-folder>
```
**Description**: Moves into the cloned repository directory.

### Edit Files
**Description**: Modify or create new files using any text editor (e.g., VSCode).

### Check Changes
```bash
git status
```
**Description**: Displays the status of changes in the working directory.

### Stage Changes
```bash
git add <file-name>
git add .
```
**Description**: Stages the modified or added files for commit.

### Commit Changes
```bash
git commit -m "Descriptive commit message"
```
**Description**: Saves the staged changes to the local repository with a commit message.

### Pull Latest Changes from GitHub
```bash
git pull origin <branch-name>
```
**Description**: Syncs your local branch with the latest changes from the remote branch.

### Push Changes to GitHub
```bash
git push origin <branch-name>
```
**Description**: Pushes the committed changes to the same branch on GitHub.

### Resolve Conflicts (If Any Arise)
**Steps**:
1. Edit the conflicting files to resolve merge conflicts.
2. Stage and commit the resolved files:
```bash
git add <file-name>
git commit -m "Resolved merge conflict"
```

---

## 3. Branch Management

### Create a New Branch
```bash
git branch <branch-name>
```
**Description**: Creates a new branch for feature development or bug fixes.

### Switch to a Branch
```bash
git checkout <branch-name>
```
**Description**: Moves to an existing branch.

### Create and Switch to a Branch
```bash
git checkout -b <branch-name>
```
**Description**: Creates and switches to a new branch in one command.

### List All Branches
```bash
git branch
```
# ✨ Git Notes — A Friendly Git & GitHub Cheatsheet

A compact, practical guide to the most used Git and GitHub commands — ideal for beginners and a quick reference for experienced users.

---

## 📌 Table of Contents
- [Quick Start](#-quick-start)
- [Common Workflow](#-common-workflow)
- [Cheat Sheet (by category)](#-cheat-sheet-by-category)
- [Advanced Tips](#-advanced-tips)
- [VSCode Tips](#-vscode-tips)
- [Contributing](#-contributing)
- [Resources](#-resources)
- [Contact](#-contact)

---

## 🚀 Quick Start
Install Git and configure your identity:

```bash
# install: go to https://git-scm.com for platform-specific installers
git --version

# configure (one-time):
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Clone a repo and open it:

```bash
git clone https://github.com/<username>/<repo>.git
cd <repo>
```

---

## ✅ Common Workflow
The typical flow for feature development:

1. Create a branch
```bash
git checkout -b feature/your-feature
```
2. Make changes, stage, and commit
```bash
git add .
git commit -m "Short, descriptive message"
```
3. Sync with remote and push
```bash
git fetch origin
git pull --rebase origin main
git push -u origin feature/your-feature
```
4. Open a PR, then delete the branch after merge
```bash
git branch -d feature/your-feature
git push origin --delete feature/your-feature
```

---

## 🎯 Cheat Sheet (by category)

### Setup & Quick Actions
- `git init` — initialize a repo
- `git clone <url>` — clone a remote repo
- `git status` — see working state
- `git add <file> | .` — stage changes
- `git commit -m "msg"` — commit
- `git push` — push to remote
- `git pull` — fetch & merge

### Branching & Merging
- `git branch` — list branches
- `git checkout <branch>` — switch
- `git checkout -b <branch>` — create+switch
- `git merge <branch>` — merge into current
- `git rebase <base>` — replay commits

### Inspecting History
- `git log --oneline --graph --decorate` — condensed log
- `git show <commit>` — inspect a commit

### Undoing & Cleanup
- `git restore <file>` — discard local changes
- `git reset --soft HEAD~1` — undo last commit (keep changes staged)
- `git reset --hard HEAD~1` — undo last commit and discard changes
- `git clean -f` — remove untracked files

### Tags & Stashes
- `git tag <tag>` — lightweight tag
- `git tag -a <tag> -m "message"` — annotated tag
- `git stash` / `git stash pop` — stash and restore

### Remote Controls
- `git remote -v` — list remotes
- `git remote add origin <url>` — add a remote
- `git remote set-url origin <new-url>` — change remote

---

## 💡 Advanced Tips & Best Practices
- Use clear, concise commit messages.
- Keep PRs small and focused.
- Rebase onto the main branch before opening a PR to keep history linear.
- Resolve conflicts locally with `git status` and `git diff` to inspect changes.

Short commands for speed:
```bash
git status -s               # short status
git log --oneline --graph   # compact log w/graph
```

---

## 🛠️ VSCode Tips
- Try extensions: GitLens, Git Graph, and GitHub Pull Requests for better visibility.
- Use the Source Control view to stage commits and manage branches.
- Open the integrated terminal for quick git commands without leaving the editor.

---

## 🤝 Contributing
To contribute:

1. Fork the repository on GitHub.
2. Clone your fork and create a branch for your work.
3. Make changes, add tests if applicable, and commit.
4. Stay in sync with upstream and rebase often:
```bash
git remote add upstream https://github.com/ORIGINAL/REPO.git
git fetch upstream
git rebase upstream/main
```
5. Push your branch to your fork and open a PR with a helpful description.

---

## 📚 Resources
- Official Git docs: https://git-scm.com/docs
- GitHub docs: https://docs.github.com/en
- GitHub Git Cheat Sheet: https://education.github.com/git-cheat-sheet-education.pdf

---

## ✉️ Contact
Found something missing? Open an issue or a PR — contributions and suggestions are welcome!

---

Made with ❤️
### View Stashes
```bash
git stash list
```
**Description**: Shows all stashed changes.

### Drop a Specific Stash
```bash
git stash drop <stash-name>
```
**Description**: Deletes a specific stash.

---

## 9. Other Essential Commands

### Check Current Branch
```bash
git branch --show-current
```
**Description**: Shows the branch you are currently working on.

### Create `.gitignore`
**Description**: Add unwanted files or folders in a `.gitignore` file to exclude them from being tracked.

### Pull with Rebase
```bash
git pull --rebase origin <branch>
```
**Description**: Rebases your branch with the latest changes from the remote branch.

### Squash Commits
```bash
git rebase -i HEAD~<n>
```
**Description**: Combines multiple commits into one.

### Cleanup Unnecessary Files
```bash
git clean -f
```
**Description**: Removes untracked files from the working directory.

---

This document serves as a quick reference to efficiently use Git and GitHub. Let me know if you need examples or further clarification on any command!


# Contributing to GitHub Projects: A Comprehensive Guide

This guide explains how to contribute to GitHub projects, covering essential Git commands, workflows, and useful VS Code extensions to enhance your Git experience. It is particularly useful for contributing to open-source projects or preparing for **Google Summer of Code (GSoC)**.

## 1. Forking the Repository

Forking creates a copy of the original repository in your GitHub account, allowing you to work independently.

### Steps:
1. Go to the GitHub repository you want to contribute to.
2. Click the **Fork** button (top right corner).
3. Your forked repository will now appear under your GitHub account.

## 2. Cloning the Forked Repository

Cloning downloads the repository to your local system.

### Command:
```bash
# Replace YOUR-USERNAME and REPO-NAME with your details
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
```

### Navigate into the project directory:
```bash
cd REPO-NAME
```

## 3. Setting Upstream Remote

Linking the original repository (upstream) ensures you can fetch updates from the main project.

### Command:
```bash
# Replace ORIGINAL-USERNAME and REPO-NAME with the repository details
git remote add upstream https://github.com/ORIGINAL-USERNAME/REPO-NAME.git
```

### Verify remotes:
```bash
git remote -v
```

You should see:
- **origin**: Your forked repository
- **upstream**: The original repository

## 4. Creating a New Branch

Always create a new branch for each feature or bug fix.

### Command:
```bash
git checkout -b feature-branch
```
Replace `feature-branch` with a descriptive name, e.g., `add-login-functionality`.

## 5. Making Changes

1. Edit the necessary files in your preferred code editor.
2. Stage changes:
```bash
git add .
```
Or, to stage specific files:
```bash
git add filename.ext
```
3. Commit changes:
```bash
git commit -m "Brief description of changes"
```

### Tips:
- Use clear and concise commit messages.
- Follow the [Conventional Commit](https://www.conventionalcommits.org/) format for readability.

## 6. Pushing Changes

Push your branch to your forked repository.

### Command:
```bash
git push origin feature-branch
```

## 7. Creating a Pull Request (PR)

1. Go to the original repository on GitHub.
2. Click the **Compare & pull request** button.
3. Write a clear title and description for your PR:
- Mention the issue number (if applicable).
- Explain your changes.
4. Submit the pull request.

## 8. Syncing Your Fork with the Original Repository

To keep your fork updated with the main project, sync it regularly.

### Commands:
```bash
# Fetch changes from the upstream repository
git fetch upstream

# Switch to the main branch
git checkout main

# Merge upstream changes into your local branch
git merge upstream/main

# Push the updated branch to your fork
git push origin main
```

## 9. Deleting Branches

### Delete locally:
```bash
git branch -d feature-branch
```

### Delete remotely:
```bash
git push origin --delete feature-branch
```

## 10. Useful Git Commands

| Command | Description |
|------------------------------|-----------------------------------------------|
| `git status` | Check the current status of the repository. |
| `git log` | View commit history. |
| `git diff` | Show changes not yet staged. |
| `git stash` | Temporarily save changes without committing. |
| `git pull upstream main` | Sync your local branch with the main project.|
| `git rebase -i` | Interactively rebase commits. |

## Tips for GSoC Contributions

### Start Early:
- Explore projects and understand their codebase.
- Look for **"Good First Issue"** or **"Help Wanted"** tags.

### Understand the Project:
- Read the `README.md` and `CONTRIBUTING.md` files.
- Set up the project locally and run tests.

### Communicate Effectively:
- Join the project’s Slack, Discord, or mailing lists.
- Discuss your ideas before starting work.

### Write Clean Code:
- Follow coding standards.
- Add comments and documentation.

### Test Your Changes:
- Ensure your changes don’t break existing functionality.
- Write unit tests if required.

## Common Mistakes to Avoid

- **Not Syncing Regularly**: Always pull updates from the upstream repository.
- **Large PRs**: Break your changes into small, manageable PRs.
- **Ignoring Guidelines**: Follow the project’s contribution guidelines.
- **Poor Commit Messages**: Use descriptive and meaningful commit messages.

## VS Code Extensions for Git and GitHub

### 1. **GitLens – Git supercharged**
- View Git history, line changes, and blame directly in VS Code.
- Features:
- File and line blame annotations.
- Commit browsing and searching.

### 2. **Git Graph**
- Visualize the Git history and branches in graph format.
- Features:
- Interactive branch management.
- Detailed commit visualization.

### 3. **GitHub Pull Requests and Issues**
- Manage PRs and issues directly within VS Code.
- Features:
- Create and review PRs.
- Browse and edit issues.

### 4. **ErrorLens**
- Highlights errors and warnings in your code as you type.

### 5. **Markdown All in One**
- Easily write and preview markdown files.
- Features:
- Live preview.
- Table of contents generation.

### 6. **Prettier**
- Auto-format code to maintain consistency.
- Features:
- Supports multiple languages.
- Customizable formatting rules.

## Resources

- [GitHub Documentation](https://docs.github.com/)
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [GSoC Program Details](https://summerofcode.withgoogle.com/)

By following this guide, you can effectively contribute to GitHub projects and prepare for GSoC or any open-source initiative. **Happy coding!**

# Merging in Team Projects: A Guide for Maintainers

## Introduction
In a team project, as the maintainer of the repository, you will manage the contributions of other developers. Contributors will fork your repository, create branches, and submit pull requests (PRs) to merge their changes. The process of merging PRs requires careful review, testing, and ensuring that the code adheres to project standards. This guide provides detailed instructions on how to handle contributions, review PRs, and merge changes effectively.

---

## Workflow Overview

### 1. Contributor's Workflow
- **Fork the repository**: If contributors don’t have direct write access, they fork the repository.
- **Create a new branch**: Contributors create a new branch for their changes.
- **Make changes**: Changes are made in the new branch.
- **Commit and push**: Changes are committed and pushed to the contributor’s fork.
- **Create a pull request (PR)**: Contributors submit a PR to the original repository for merging.

### 2. Maintainer's Workflow
- **Review pull requests (PRs)**: Review the submitted PRs from contributors.
- **Test the changes**: Ensure the changes are functional and do not break existing code.
- **Handle merge conflicts**: Resolve any conflicts between branches before merging.
- **Merge the PR**: Once reviewed and approved, the PR is merged into the main branch.

---

## Step-by-Step Guide for Contributors

### 1. Forking the Repository (Contributor’s Side)
If you don't have write access to the repository, you need to fork it first. This allows you to make changes without directly affecting the original codebase.

#### Instructions:
1. Go to the repository page on GitHub.
2. Click on the **"Fork"** button at the top-right corner.
3. Once the repository is forked, clone it to your local machine:

```bash
git clone https://github.com/your-username/repository-name.git
cd repository-name
```

---

### 2. Creating a New Branch (Contributor’s Side)
It’s important to create a separate branch to work on your changes, rather than working directly on the main branch.

#### Instructions:
Create and switch to a new branch:

```bash
git checkout -b feature/branch-name
```

---

### 3. Making Changes (Contributor’s Side)
Once on your new branch, make the necessary changes to the codebase.

#### Instructions:
Make the required changes (bug fixes, features, or updates).
Stage the changes:

```bash
git add .
```

Commit the changes with a clear message:

```bash
git commit -m "Describe the changes made"
```

---

### 4. Pushing Changes to the Forked Repository (Contributor’s Side)
After committing your changes, push the changes to your forked repository.

#### Instructions:
Push your branch to your forked repository:

```bash
git push origin feature/branch-name
```

---

### 5. Creating a Pull Request (PR) (Contributor’s Side)
After pushing your changes, submit a pull request (PR) to propose merging your branch into the original repository.

#### Instructions:
1. Go to the **Pull Requests** tab in the original repository.
2. Click **"New Pull Request"**.
3. Select the branch you want to merge and compare it with the main branch.
4. Provide a descriptive title and explanation for your changes.
5. Click **"Create Pull Request"**.

---

## Step-by-Step Guide for Maintainers

### 1. Reviewing Pull Requests
Before merging a PR, review the changes thoroughly to ensure they meet the following criteria:

- **Code Quality**: Ensure that the code is clean, well-structured, and follows the project's coding guidelines.
- **Documentation**: Verify that the code is well-commented and documented if necessary.
- **Testing**: Ensure that the changes are adequately covered by unit or integration tests.
- **Functionality**: Ensure the code changes work as expected and address the original issue or feature request.

#### Instructions to Review a PR:
1. Go to the **Pull Requests** tab in the repository.
2. Click on the PR to view the changes.
3. Review the files changed, check for any issues, and verify the functionality.

---

### 2. Running Tests
Before merging, make sure the changes pass all tests. This can be done by:

- Running the tests locally on your machine.
- Verifying that the PR passes the CI (Continuous Integration) tests.

#### Instructions to Run Tests Locally:

```bash
# Example for Python projects with pytest
pytest
```

If the tests fail, communicate with the contributor about the issues and request changes.

---

### 3. Handling Merge Conflicts
Sometimes, changes in the pull request might conflict with the changes in the main branch. In such cases, you need to resolve merge conflicts manually.

#### Steps to Handle Merge Conflicts:
1. Fetch the latest changes from the main branch:

```bash
git fetch origin
git checkout main
git pull origin main
```

2. Switch to the contributor's branch:

```bash
git checkout feature/branch-name
```

3. Merge the main branch into the feature branch to resolve conflicts:

```bash
git merge main
```

4. If there are any conflicts, manually resolve them by editing the conflicted files.
5. Stage the resolved files:

```bash
git add .
```

6. Commit the merge:

```bash
git commit -m "Resolved merge conflicts"
```

---

### 4. Merging the Pull Request
Once the PR is approved and all tests pass, it’s time to merge it into the main branch.

#### Instructions:
1. Go to the **Pull Requests** tab.
2. Ensure the PR is ready to be merged (no conflicts, all tests passing).
3. Click on **"Merge Pull Request"**.
4. Confirm the merge.

You can choose to merge via:
- **Merge Commit**: Keeps the full history of the branch.
- **Squash and Merge**: Combines all commits into one.
- **Rebase and Merge**: Reapplies commits from the PR on top of the base branch.

---

## Post-Merge Actions

After merging a pull request, there are a few post-merge actions to consider:

1. **Delete the Feature Branch**: You can delete the contributor's branch after merging it.
2. **Update the Repository**: If there are any new dependencies or configurations, update the repository’s documentation or settings.
3. **Communicate with the Contributor**: Inform the contributor that their PR has been merged and thank them for their contribution.

---

## Conclusion
Merging is a crucial part of team collaboration in software development. As the maintainer, you must ensure that the code is well-reviewed, tested, and correctly merged to keep the project’s codebase stable. By following the steps outlined in this guide, you can effectively manage contributions and maintain a high-quality codebase.

---

### Best Practices:
- Always create a new branch for each change.
- Write clear commit messages.
- Make sure to run tests before submitting a PR.
- Stay up-to-date with the main branch to avoid conflicts.
