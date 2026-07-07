# ═══════════════════════════════════════════════════════
# SECTION 11: GIT & GITHUB (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 11.1 Git Fundamentals & Commands

### ✅ Important Topics
- [ ] Version Control System (VCS) concepts
- [ ] Git States (Working Directory, Staging Area, Local Repo)
- [ ] Basic commands (`add`, `commit`, `status`, `log`, `diff`)
- [ ] `fetch` vs `pull`

### 📋 Interview Questions
1. What is a Version Control System? Why is Git considered a "Distributed" VCS?
2. Explain the three main states/areas in Git (Working Directory, Staging/Index, Repository).
3. What is a `.gitignore` file? How does it work?
4. What is the exact difference between `git pull` and `git fetch`?
5. How do you view the commit history?
6. How do you see the differences between your working directory and the staging area? (`git diff`)

---

## 11.2 Branching, Merging & Conflict Resolution

### ✅ Important Topics
- [ ] Branching concept (`git branch`, `git checkout`, `git switch`)
- [ ] `git merge` (Fast-forward vs 3-way merge)
- [ ] Merge Conflicts
- [ ] Conflict Resolution strategies

### 📋 Interview Questions
1. What is a branch in Git? How does branching work under the hood?
2. What is the `HEAD` pointer? What does a "detached HEAD" state mean?
3. What is a Merge Conflict? When does Git fail to merge automatically?
4. Walk me through the exact steps you take to resolve a merge conflict.
5. What is the difference between a Fast-Forward merge and a 3-way (recursive) merge?

---

## 11.3 Advanced Git Operations

### ✅ Important Topics
- [ ] `git rebase`
- [ ] Merge vs Rebase (Golden Rule of Rebasing)
- [ ] `git cherry-pick`
- [ ] `git stash`
- [ ] Undo operations (`git reset`, `git revert`)
- [ ] Types of reset (`--soft`, `--mixed`, `--hard`)

### 📋 Interview Questions
1. What is `git rebase`? How does it rewrite history?
2. What is the difference between `git merge` and `git rebase`? When should you use which?
3. What is the "Golden Rule of Rebasing"? (Never rebase public/shared branches).
4. What is `git cherry-pick`? Give a scenario where you would use it.
5. What is `git stash`? How do you retrieve stashed changes?
6. What is the difference between `git reset` and `git revert`?
7. Explain the difference between `git reset --soft`, `git reset --mixed`, and `git reset --hard`.
8. You committed and pushed a file containing sensitive API keys to GitHub. How do you properly remove it from the repository's history? (Hint: Revert is not enough).

---

## 11.4 GitHub & CI/CD Basics

### ✅ Important Topics
- [ ] Git vs GitHub
- [ ] Forking vs Cloning
- [ ] Pull Requests (PR) / Merge Requests
- [ ] Git Flow (Branching Strategy)
- [ ] CI/CD Basics (Continuous Integration / Continuous Deployment)
- [ ] GitHub Actions

### 📋 Interview Questions
1. What is the difference between Git and GitHub?
2. What does it mean to "Fork" a repository? How is it different from "Cloning"?
3. What is a Pull Request (PR)? What makes a good PR description?
4. What is Git Flow? Explain the typical branches used in this workflow (master, develop, feature, release, hotfix).
5. What is CI/CD?
6. How do Continuous Integration and Continuous Deployment differ?
7. What is GitHub Actions? How can you use it to automate testing on every Pull Request?

### 🎯 Scenario Based Questions
8. **Scenario:** You are working on a `feature` branch. Your teammate just merged a critical security fix into `main`. How do you get that fix into your `feature` branch without messing up history?
9. **Scenario:** You realize your last commit message had a typo, and you forgot to include a file. You haven't pushed yet. How do you fix this? (`git commit --amend`).
10. **Scenario:** You ran `git reset --hard` by accident and lost two days of unpushed commits. Is it possible to recover them? (`git reflog`).

---

### 🎯 What Interviewer Expects (Git & GitHub)
- [ ] Understanding that Git operates on snapshots, not just file differences.
- [ ] Clear ability to articulate the difference between Merge and Rebase.
- [ ] Knowledge of how to safely undo mistakes (Revert vs Reset).
- [ ] Understanding the purpose of PRs and Code Reviews in a collaborative environment.

### ❌ Common Mistakes (Git & GitHub)
- [ ] Using `git reset --hard` as a go-to solution for everything.
- [ ] Rebasing public branches and causing issues for the rest of the team.
- [ ] Not understanding that `git pull` automatically performs a merge (or rebase).

---

> **📌 SECTION 11 COMPLETE — Git & GitHub**
>
> Say **"Continue"** to generate **Section 12: Docker**

---
