# Git Commands Reference: Basic to Advanced

This document is a comprehensive reference for Git commands, starting from the fundamentals and progressing to advanced workflows. It is designed for daily use, interviews, and real-world development scenarios.

---

## 1. Git Basics

### 1.1 git init

Initializes a new Git repository in the current directory.

Use case: Start version control for a new project.

```
git init
```

---

### 1.2 git clone

Creates a local copy of a remote repository.

Use case: Work on an existing project hosted on GitHub, GitLab, or Bitbucket.

```
git clone https://github.com/user/repo.git
```

---

### 1.3 git status

Shows the current state of the working directory and staging area.

Use case: Check which files are modified, staged, or untracked before committing.

```
git status
```

---

### 1.4 git add

Adds changes to the staging area.

Use case: Prepare files to be included in the next commit.

```
git add file.txt
git add .
```

---

### 1.5 git commit

Records staged changes into the repository history.

Use case: Save a logical unit of work.

```
git commit -m "Initial commit"
```

---

### 1.6 git log

Displays commit history.

Use case: Review past changes and authorship.

```
git log
git log --oneline
```

---

## 2. Working with Branches

### 2.1 git branch

Lists, creates, or deletes branches.

Use case: Isolate features or fixes from the main codebase.

```
git branch
git branch feature-login
```

---

### 2.2 git checkout

Switches branches or restores files.

Use case: Move between branches during development.

```
git checkout feature-login
```

---

### 2.3 git switch

Modern alternative to checkout for switching branches.

Use case: Cleaner branch navigation.

```
git switch main
git switch -c new-feature
```

---

### 2.4 git merge

Combines changes from one branch into another.

Use case: Merge a completed feature into the main branch.

```
git merge feature-login
```

---

### 2.5 git rebase

Reapplies commits on top of another base commit.

Use case: Maintain a clean, linear project history.

```
git rebase main
```

---

## 3. Remote Repositories

### 3.1 git remote

Manages connections to remote repositories.

Use case: Verify or add remote repository URLs.

```
git remote -v
git remote add origin https://github.com/user/repo.git
```

---

### 3.2 git fetch

Downloads objects and refs from a remote repository.

Use case: Update local references without modifying working files.

```
git fetch origin
```

---

### 3.3 git pull

Fetches and merges changes from a remote branch.

Use case: Sync local branch with remote updates.

```
git pull origin main
```

---

### 3.4 git push

Uploads local commits to a remote repository.

Use case: Share work with team members.

```
git push origin main
```

---

## 4. Undoing and Fixing Mistakes

### 4.1 git restore

Restores files to a previous state.

Use case: Discard unwanted local changes.

```
git restore file.txt
```

---

### 4.2 git reset

Moves HEAD and optionally modifies staging and working directory.

Use case: Unstage files or rewrite commit history.

```
git reset file.txt
git reset --soft HEAD~1
git reset --hard HEAD~1
```

---

### 4.3 git revert

Creates a new commit that undoes a previous commit.

Use case: Safely undo changes in shared branches.

```
git revert <commit-hash>
```

---

### 4.4 git reflog

Shows a log of all HEAD movements.

Use case: Recover lost commits after reset or rebase.

```
git reflog
```

---

## 5. Stashing Work

### 5.1 git stash

Temporarily saves uncommitted changes.

Use case: Switch branches without committing incomplete work.

```
git stash
git stash push -m "wip"
```

---

### 5.2 git stash list

Lists all stashed entries.

```
git stash list
```

---

### 5.3 git stash apply and pop

Restores stashed changes.

Use case: Resume previously paused work.

```
git stash apply
git stash pop
```

---

## 6. Inspecting Changes

### 6.1 git diff

Shows differences between commits, branches, or working tree.

Use case: Review changes before committing.

```
git diff
git diff --staged
```

---

### 6.2 git show

Displays details of a specific commit.

Use case: Inspect what changed in a particular commit.

```
git show <commit-hash>
```

---

## 7. Tags and Releases

### 7.1 git tag

Creates and manages tags.

Use case: Mark release points like v1.0.

```
git tag v1.0
git tag -a v1.1 -m "release"
```

---

### 7.2 git push tags

Pushes tags to remote repository.

```
git push origin v1.0
git push origin --tags
```


