# ═══════════════════════════════════════════════════════
# SECTION 10: GIT & VERSION CONTROL (COMPLETE)
# ═══════════════════════════════════════════════════════

---

## 10.1 Git Fundamentals

### ✅ Important Topics
- [ ] Version Control Systems (VCS)
- [ ] Centralized vs Distributed VCS
- [ ] What is Git
- [ ] Git vs GitHub
- [ ] Three stages of Git (Working Directory, Staging Area, Local Repository)
- [ ] .git folder
- [ ] .gitignore file

### 📋 Interview Questions
1. What is a Version Control System? Why is it important?
2. What is the difference between a Centralized VCS (like SVN) and a Distributed VCS (like Git)?
3. What is Git?
4. What is the difference between Git and GitHub?
5. Explain the three main states/areas in Git (Working Directory, Staging/Index, Repository).
6. What is the purpose of the `.git` folder?
7. What is a `.gitignore` file? What kind of files should be put in it?

---

## 10.2 Basic Git Commands

### ✅ Important Topics
- [ ] git init, git clone
- [ ] git add, git commit
- [ ] git status, git log
- [ ] git push, git pull, git fetch
- [ ] git diff

### 📋 Interview Questions
1. How do you initialize a new Git repository?
2. What is the difference between `git pull` and `git fetch`?
3. How do you stage files? How do you unstage a file?
4. What does `git commit -m` do? What is a good commit message?
5. How do you view the commit history?
6. What does `git diff` do?
7. How do you clone an existing repository?

---

## 10.3 Branching & Merging

### ✅ Important Topics
- [ ] Branches in Git
- [ ] git branch, git checkout, git switch
- [ ] git merge
- [ ] Merge Conflicts
- [ ] Fast-forward merge vs 3-way merge
- [ ] git rebase
- [ ] Merge vs Rebase

### 📋 Interview Questions
1. What is a branch in Git? Why do we use branches?
2. How do you create a new branch and switch to it?
3. What is the main branch usually called? (master/main)
4. How do you merge a branch into another?
5. What is a Merge Conflict? How do you resolve it?
6. What is `git rebase`?
7. What is the difference between `git merge` and `git rebase`? When should you use which?
8. Why is it dangerous to rebase commits that have already been pushed to a public repository?

---

## 10.4 Advanced Git Concepts

### ✅ Important Topics
- [ ] HEAD
- [ ] git stash
- [ ] git reset (soft, mixed, hard)
- [ ] git revert
- [ ] git cherry-pick
- [ ] Pull Requests (PR)
- [ ] Forking

### 📋 Interview Questions
1. What is `HEAD` in Git? What is a "detached HEAD" state?
2. What is `git stash`? When would you use it?
3. How do you apply stashed changes?
4. What is the difference between `git reset` and `git revert`?
5. Explain the difference between `git reset --soft`, `--mixed`, and `--hard`.
6. You accidentally committed a password and pushed it. How do you remove it?
7. What is `git cherry-pick`?
8. What is a Pull Request (PR)? How is it different from a Merge Request?
9. What does it mean to "Fork" a repository on GitHub? How is it different from cloning?

### 🎯 Scenario Based Questions
10. You are working on a feature branch, but you need to quickly fix a bug on the main branch. How do you handle your uncommitted changes?
11. You made a commit with a typo in the commit message. How do you fix it? (`git commit --amend`)
12. You want to bring only one specific commit from branch B into branch A. How do you do it?
13. You accidentally ran `git reset --hard` and lost your work. Is there a way to recover it? (Reference `git reflog`)

---

### 🎯 What Interviewer Expects (Git)
- [ ] Understanding of the Distributed nature of Git.
- [ ] Clear understanding of Working Directory → Staging → Repository flow.
- [ ] Knowing how to resolve merge conflicts.
- [ ] Understanding the critical difference between `merge` and `rebase`.
- [ ] Knowing how to undo mistakes (revert vs reset).

### ❌ Common Mistakes (Git)
- [ ] Not knowing the difference between `git fetch` and `git pull`.
- [ ] Confusing `git reset` and `git revert` (using reset on public branches).
- [ ] Not understanding what `git stash` is used for.

---

> **📌 SECTION 10 COMPLETE — Git & Version Control**
>
> Say **"Continue"** to generate **Section 11: Prompt Engineering & AI** + **Section 12: Gemini API & LLMs**

---
