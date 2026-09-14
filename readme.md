# Git Course

A practical guide to learning Git for version control, collaboration, and project management.

## 1. What is Git?

Git is a distributed version control system that tracks changes in files and helps teams work together efficiently. It lets you:

- save versions of your project
- compare changes over time
- collaborate with others
- create branches for features or fixes
- recover older versions when needed

## 2. Installation

Download Git from:

- https://git-scm.com/downloads

After installing, verify:

```bash
git --version
```

Set your identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## 3. Initialize a Repository

Create a new project folder and initialize Git:

```bash
mkdir my-project
cd my-project
git init
```

## 4. Basic Workflow

Check repository status:

```bash
git status
```

Add files to staging area:

```bash
git add file.txt
git add .
```

Create a commit:

```bash
git commit -m "Initial commit"
```

## 5. View History

See commit log:

```bash
git log
```

Compact log view:

```bash
git log --oneline --decorate --graph --all
```

## 6. Branching

Create a new branch:

```bash
git branch feature-login
```

Switch to a branch:

```bash
git checkout feature-login
```

Or create and switch in one step:

```bash
git checkout -b feature-login
```

Modern Git command:

```bash
git switch -c feature-login
```

Merge a branch into the current branch:

```bash
git checkout main
git merge feature-login
```

## 7. Remotes and GitHub

Connect a local repository to GitHub:

```bash
git remote add origin https://github.com/USERNAME/REPO.git
```

Push code:

```bash
git push -u origin main
```

Pull updates:

```bash
git pull origin main
```

## 8. Cloning a Repository

```bash
git clone https://github.com/USERNAME/REPO.git
```

## 9. Undoing Changes

Discard unstaged changes in a file:

```bash
git restore file.txt
```

Revert a file to the last committed version:

```bash
git checkout -- file.txt
```

Unstage a file:

```bash
git restore --staged file.txt
```

Delete a branch:

```bash
git branch -d feature-login
```

## 10. .gitignore

Create a file named `.gitignore` to ignore files like logs, build folders, or environment files:

```gitignore
node_modules/
.env
*.log
```

## 11. Common Commands Summary

```bash
git init
git status
git add .
git commit -m "message"
git branch
git checkout -b feature
git merge feature
git push origin main
git pull origin main
git log
git clone URL
```

## 12. Best Practices

- commit often with clear messages
- keep each commit focused
- pull before pushing
- use branches for features and bug fixes
- review diffs before merging

## 13. Example Workflow

```bash
git init
git add .
git commit -m "Initial project setup"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```

## 14. Useful Resources

- https://git-scm.com/docs
- https://github.com/git-guides
- https://www.atlassian.com/git/tutorials

## Conclusion

Git is essential for tracking code changes, working in teams, and managing software projects. Practice the basic commands regularly and build confidence by working on small projects.


# this is feature branch
# This is feature 2.0