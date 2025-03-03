﻿# github_demo
# Getting Started with GitHub

Welcome to this beginner-friendly guide on using Git and GitHub! This repository will walk you through the basics of Git version control while using a simple Python project as an example.

## Table of Contents

1. [Setting Up Git](#setting-up-git)
2. [Initializing a Repository](#initializing-a-repository)
3. [Basic Git Workflow](#basic-git-workflow)
4. [Branching and Merging](#branching-and-merging)
5. [Handling Merge Conflicts](#handling-merge-conflicts)
6. [Working with Pull Requests](#working-with-pull-requests)
7. [Advanced Git Features](#advanced-git-features)
8. [Common Git Commands](#common-git-commands)

---

## Setting Up Git

If you haven't installed Git yet, download and install it from [git-scm.com](https://git-scm.com/). Once installed, configure it:

```sh
# Set your name and email
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

## Initializing a Repository

To start using Git, navigate to your project folder and initialize a Git repository:

```sh
git init
```

This creates a hidden `.git` folder that tracks changes in your project.

## Basic Git Workflow

1. **Check the repository status:**
   ```sh
   git status
   ```
2. **Stage files for commit:**
   ```sh
   git add filename.py  # Add a specific file
   git add .            # Add all changes
   ```
3. **Commit changes:**
   ```sh
   git commit -m "Initial commit"
   ```
4. **Push to GitHub:**
   ```sh
   git push origin main
   ```

## Branching and Merging

1. **Create a new branch:**
   ```sh
   git checkout -b feature-branch
   ```
2. **Switch to an existing branch:**
   ```sh
   git checkout main
   ```
3. **Merge changes:**
   ```sh
   git merge feature-branch
   ```

## Handling Merge Conflicts

If you face a merge conflict:

1. Open the conflicting file(s) and resolve conflicts manually.
2. Stage the resolved files:
   ```sh
   git add filename.py
   ```
3. Commit the resolution:
   ```sh
   git commit -m "Resolved merge conflict"
   ```

## Working with Pull Requests

1. **Fork and clone the repository.**
2. **Create a feature branch and make changes.**
3. **Push changes to your GitHub fork.**
4. **Open a Pull Request (PR) on GitHub.**

## Advanced Git Features

1. **Find a bad commit using `git bisect`:**
   ```sh
   git bisect start
   git bisect bad  # Mark current commit as bad
   git bisect good commit-hash  # Mark an earlier commit as good
   ```
2. **Undo commits using `git reset`:**
   ```sh
   git reset --hard HEAD~1  # Undo last commit completely
   ```
3. **View commit history:**
   ```sh
   git log --oneline --graph
   ```
4. **Save work temporarily using `git stash`:**
   ```sh
   git stash  # Stash current changes
   git stash list  # View stashed changes
   git stash apply  # Reapply the most recent stash
   ```
5. **View commit logs with details:**
   ```sh
   git log --pretty=format:"%h - %an, %ar : %s"
   ```

## Common Git Commands

| Command                    | Description                                 |
| -------------------------- | ------------------------------------------- |
| `git init`                 | Initialize a new Git repository             |
| `git clone <repo-url>`     | Clone a repository from GitHub              |
| `git status`               | Check the status of your working directory  |
| `git add <file>`           | Stage changes for commit                    |
| `git add .`                | Stage all changes for commit                |
| `git commit -m "message"`  | Commit staged changes                       |
| `git push origin <branch>` | Push commits to remote repository           |
| `git pull origin <branch>` | Pull the latest changes from the repository |
| `git checkout -b <branch>` | Create and switch to a new branch           |
| `git merge <branch>`       | Merge a branch into the current branch      |
| `git bisect start`         | Start a binary search for a bad commit      |
| `git reset --hard HEAD~1`  | Undo the last commit                        |
| `git stash`                | Save uncommitted changes temporarily        |
| `git stash apply`          | Reapply the most recent stash               |
| `git log --oneline --graph`| View a compact commit history               |

---

This guide provides an overview of Git basics to help you get started. Happy coding!

