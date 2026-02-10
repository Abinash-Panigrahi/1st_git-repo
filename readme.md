# 📘 Git & GitHub Knowledge Base

This repository is a comprehensive guide to Version Control. It documents the commands, workflows, and best practices learned during my development journey.

---

## 📍 Quick Navigation
* [Core Workflow](#-core-workflow)
* [Remote Management](#-remote-management)
* [Branching & Merging](#-branching--merging)
* [Tracking History (Logs)](#-tracking-history-the-logs)
* [Visualizing Git (VS Code)](#-visualizing-git-history-vs-code)
* [Standard Deletion](#-standard-deletion)
* [Nuclear Options (History Scrubbing)](#-nuclear-options-deep-cleaning)
* [Download Sources](#-essential-download-sources)

---

## 🚀 Core Workflow
* **`git init`**: Initializes a new Git repository (creates the `.git` folder).
* **`git status`**: Shows the current state of your folder (tracked vs. untracked files).
* **`git add .`**: Stages all files in the current directory for the next commit.
* **`git commit -m "message"`**: Saves your staged changes with a descriptive note.

## 🌐 Remote Management
* **`git remote add origin <url>`**: Links your local folder to a GitHub repository.
* **`git remote -v`**: Lists all remote connections to verify where your code is going.
* **`git push -u origin main`**: Uploads commits to GitHub and sets the default branch.
* **`git remote remove origin`**: Deletes the link to the online repository.

## 🌿 Branching & Merging
* **`git branch`**: Lists all local branches. (The one with `*` is your current branch).
* **`git checkout -b <name>`**: Creates a new branch and switches to it immediately.
* **`git checkout <name>`**: Switches back to an existing branch.
* **`git merge <name>`**: Combines work from a different branch into your current branch.

## 📜 Tracking History (The Logs)
* **`git log --oneline`**: Shows a condensed, one-line version of your history.
* **`git log --graph --oneline --all`**: Draws a visual branch tree directly in the terminal.
* **`git log -n 5`**: Shows only the last 5 commits.
* *Note: Press **'q'** to exit the log view in terminal.*

## 👁️ Visualizing Git History (VS Code)
I use the **Git Graph** extension (by **mhutchie**) in VS Code for a professional visual map of my project.
* **Usage**: Install from the Extensions marketplace and click the "Git Graph" button in the status bar.

---

## 🧹 Standard Deletion
* **`git rm <file>`**: Deletes a file from the current version. The file remains in past history.
* **`git branch -d <name>`**: Deletes a branch locally.
* **`git push origin --delete <branch>`**: Removes a branch from the GitHub server.

## ☢️ Nuclear Options (Deep Cleaning)
When you need to **rewrite history** (e.g., you accidentally committed a password), use this to erase a file from **every commit ever made**:

```bash
git filter-branch --force --index-filter \
  "git rm --cached --ignore-unmatch README.md" \
  --prune-empty --tag-name-filter cat -- --all

---

## 📥 Essential Download Sources

To keep your development environment up to date, use these official sources:

* **[Download Git for Windows](https://git-scm.com/download/win)**: The official CLI and Git Bash tool.
* **[Visual Studio Code](https://code.visualstudio.com/)**: The best code editor for Git integration.
* **[GitHub Desktop](https://desktop.github.com/)**: A GUI for managing repositories without the terminal.

---

## 💡 The Profile README Secret
To display a professional bio on your GitHub profile:
1. Create a public repository named exactly like your username: `Abinash-Panigrahi`.
2. Add a `README.md` to that repository.
3. This content will now appear at the top of your GitHub homepage.

---
*Created by Abinash Panigrahi | Last Updated: February 2026*