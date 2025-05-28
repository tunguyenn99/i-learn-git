
# 🧰 Git for Developers – Practical Cheatsheet & Guide

A comprehensive and beginner-friendly guide to using **Git** for version control. This repo includes practical commands, visual workflows, and real-world examples to help you work efficiently with local and remote repositories.

---

## 📚 Table of Contents

1. [Git Overview](#git-overview)
2. [Git Structure](#git-structure)
3. [Common Git Commands](#common-git-commands)
   - [Initialize & Track Files](#1-initialize--track-files)
   - [Staging & Committing](#2-staging--committing)
   - [Undo & Restore](#3-undo--restore)
   - [Working with History](#4-working-with-history)
   - [Branching & Merging](#5-branching--merging)
   - [Working with Remote Repositories](#6-working-with-remote-repositories)
   - [Repository Management](#7-repository-management)
   - [Stash Workflow](#8-stash-workflow)
   - [Command Line Setup Examples](#demo-git-cli-setup)
4. [Visuals](#visuals)

---

## ⚙️ Git Overview

Git is a distributed version control system that helps you manage changes in your codebase. It supports both local development and collaboration via remote repositories (e.g., GitHub, GitLab).

---

## 🧱 Git Structure

### Git includes **two main components**:

#### 1. Local Repository

- **Working Area**: Where you modify and create files.
- **Staging Area (Index)**: Where you prepare changes before committing.
- **Local Repository**: Stores all committed snapshots of your project.

#### 2. Remote Repository

- Hosted on a remote server (e.g., GitHub).
- Enables team collaboration and code sharing.

---

## 🛠️ Common Git Commands

### 1. Initialize & Track Files

```bash
git --version                # Check Git version
git init                     # Initialize a new Git repository
git clone <repo-url>         # Clone a remote repo to local
git status                   # View current file states
```

### 2. Staging & Committing

```bash
git add <file>              # Add a file to the staging area
git add .                   # Add all changes
git commit -m "message"     # Commit changes with a message
git commit --amend -a       # Amend the latest commit
```

### 3. Undo & Restore

```bash
git restore <file>                   # Restore file to last commit
git restore --staged <file>         # Unstage file
git reset                           # Unstage everything
git reset --hard HEAD               # Discard all uncommitted changes
```

### 4. Working with History

```bash
git log                            # View commit history
git log --oneline                  # Compact commit log
git show <commit-hash>            # Show details of a commit
git revert <commit-hash>          # Undo a specific commit safely
git reset <commit-hash>           # Reset to a previous commit
```

### 5. Branching & Merging

> Visualize: [learngitbranching.js.org](https://learngitbranching.js.org/)

```bash
git branch                         # List branches
git branch <branch>                # Create a new branch
git checkout <branch>              # Switch to a branch
git checkout -b <branch>           # Create and switch to a branch
git merge <branch>                 # Merge a branch into current
git branch -d <branch>             # Delete a branch
```

---

## 📸 Visuals

![Git Basic Workflow](https://xuanthulab.net/photo/basic-remote-workflow.png)
![Branch Workflow](https://www.atatus.com/blog/content/images/2021/06/git-branch-workflow-2.png)

---

## 📄 License

This repository is licensed under the [MIT License](./LICENSE).
