```python
content = """# QuickCart Release v2.0 - Git & GitHub Collaborative Lab Challenge

[![Git & GitHub](https://img.shields.io/badge/Git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)
[![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)
[![Status](https://img.shields.io/badge/Status-Active-success.svg?style=for-the-badge)]()

Welcome to the **QuickCart Collaborative Lab Challenge**! This repository serves as a hands-on, realistic team exercise designed to master advanced Git and GitHub workflows. 

Your team has joined **QuickCart**, an e-commerce startup preparing for **Release v2.0**. Throughout this challenge, you will experience real-world software engineering hurdles, including feature branching, handling intentional merge conflicts, code reviews, pull requests, hotfixes, and release tagging.

---

## 📑 Table of Contents
1. [Scenario & Context](#-scenario--context)
2. [Repository Structure](#-repository-structure)
3. [Team Roles & Responsibilities](#-team-roles--responsibilities)
4. [Lab Challenges Workflow](#-lab-challenges-workflow)
5. [Strict Collaboration Rules](#-strict-collaboration-rules)
6. [Essential Git Commands Reference](#-essential-git-commands-reference)
7. [Deliverables Checklist](#-deliverables-checklist)

---

## 🛒 Scenario & Context

QuickCart's e-commerce application is currently incomplete. Four team members must collaborate using GitHub to complete Release v2.0. The goal of this lab is **not coding complexity, but correct and disciplined Git workflow**.

---

## 📁 Repository Structure

```text
quickcart/
├── index.html       # Landing page (subject to intentional merge conflict challenge)
├── login.html       # Authentication portal
├── payment.html     # Checkout and payment gateway
├── config.txt       # Configuration settings (subject to hotfix challenge)
└── README.md        # Project documentation

```

---

## 👥 Team Roles (4 Members)

| Role | Responsibilities & Focus Areas |
| --- | --- |
| **Developer A** | **Homepage & Login feature.** Works on `feature/login` branch, commits frequently, raises Pull Requests. Collaborates on index.html conflict. |
| **Developer B** | **Payment feature.** Creates independent payment branch, handles checkout UI, resolves merge conflicts, raises Pull Requests. |
| **Developer C** | **Bug fixes & Documentation.** Pulls latest code, performs hotfixes, manages debugging text (`git restore`, `git reset`, `git revert`), and cherry-picks if instructed. |
| **Engineering Manager** | **Repository Governance.** Protects `main` branch, reviews PRs, requests code changes, approves, and merges *only* after proper verification. |

---

## 🚀 Lab Challenges Workflow

Complete the following 10 sequential challenges to ensure a smooth release process:

* **Challenge 1: Clone & Branch**
Clone the repository locally and create personal feature branches.
* *Hints:* `git clone`, `git switch -c`, `git status`


* **Challenge 2: Meaningful Commits**
Each developer modifies their assigned files and writes meaningful commit messages explaining *why* the change was made.
* *Hints:* `git add`, `git commit -m`, `git log --oneline`


* **Challenge 3: Push to Remote**
Push your local feature branches up to GitHub.
* *Hints:* `git push -u origin <branch-name>`


* **Challenge 4: Merge Conflict Resolution**
Developer A and Developer B intentionally edit the **same line** in `index.html`. Merge feature branches into `main` one after another, inspect conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`), resolve manually, stage, and commit.
* *Hints:* Inspect markers, manual code edit, `git add`, `git commit`


* **Challenge 5: Pull Request Review**
The Engineering Manager reviews Pull Requests, inspects changed files and commit messages, requests changes if necessary, and approves after fixes.
* **Challenge 6: Debugging & Accidental Commits**
Developer C accidentally commits debug text. Decide whether to use `git restore`, `git reset`, or `git revert` depending on whether the commit was already pushed.
* **Challenge 7: Synchronization**
The Manager updates `README.md` directly on `main`. All developers must synchronize their local environments before continuing work.
* *Hints:* `git pull origin main`


* **Challenge 8: Emergency Hotfix**
Create a `hotfix/login-crash` branch directly from `main`, fix `config.txt`, and merge via a fast-tracked PR review.
* **Challenge 9: Commit Squashing (Bonus)**
Clean up commit history by squashing multiple WIP commits before merging into `main`.
* *Hints:* Interactive rebase (`git rebase -i`) or GitHub Squash Merge.


* **Challenge 10: Release Tagging**
Tag the final stable state for production release v2.0.
* *Hints:* `git tag -a v2.0 -m 'Release v2.0'`; `git push origin v2.0`



---

## ⚙️ Strict Collaboration Rules

1. **No Direct Commits:** Nobody commits directly to `main` except the Engineering Manager.
2. **Feature Branching:** Every feature, bug fix, or hotfix must be developed in its own dedicated branch.
3. **Pull Request Mandate:** Every merge into `main` requires a formal Pull Request and code review.
4. **Conflict Practice:** Developers must successfully resolve at least one merge conflict.
5. **Explanatory Commits:** Every commit message must clearly explain **why** the change was made, not just what changed.
6. **Manager Authority:** The Manager may reject a PR and demand code corrections before approval.

---

## 🛠️ Essential Git Commands Reference

| Command | Description |
| --- | --- |
| `git clone <url>` | Clone a remote repository onto your local machine |
| `git switch -c <branch>` | Create and switch to a new feature branch |
| `git add <file>` | Stage changes for the next commit |
| `git commit -m "<msg>"` | Record staged changes to the local repository with a message |
| `git push -u origin <branch>` | Push local branch to remote repository and set upstream |
| `git pull origin main` | Fetch and merge changes from remote `main` into your current branch |
| `git status` | Check the state of your working directory and staging area |
| `git log --oneline` | View condensed commit history |
| `git tag -a v2.0 -m "msg"` | Create an annotated tag for release milestones |

---

## 📦 Deliverables Checklist

Ensure your team submits the following upon completion of the lab:

1. **Final Repository:** A clean commit history on GitHub with all features merged into `main`.
2. **Conflict Proof:** Screenshot showcasing manual merge conflict resolution in `index.html`.
3. **PR Screenshot:** Screenshot of an approved Pull Request with code review comments.
4. **Command Log:** A comprehensive list of Git commands used along with explanations of their purpose.
5. **Reflection:** A brief team reflection answering: *"Which Git command was most useful and why?"*

---
