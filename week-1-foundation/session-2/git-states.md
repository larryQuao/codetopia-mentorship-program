# Git States

## The 3 Git States (In My Own Words)

### 1. Working Directory (Modified)

This is where I make changes to my files. Git can see that something has changed but it hasn’t been told to track it yet. Think of it as a draft on your desk — you’ve written something but haven’t saved it officially.

### 2. Staging Area (Staged)

This is where I place files I want to include in my next commit. Using `git add`, I move files from the working directory into the staging area. It’s like putting your finished pages into an envelope before sealing it.

### 3. Repository (Committed)

Once I run `git commit`, the staged changes are saved permanently into the Git history. This is the sealed envelope — a snapshot in time that I can always go back to.

-----

## Visual Summary

```
Working Directory  →  Staging Area  →  Repository
   (edit files)       (git add)        (git commit)
```

-----

## Key Commands Per State

```bash
# Check what state your files are in
git status

# Move from Working Directory → Staging
git add filename.md

# Move from Staging → Repository
git commit -m "docs: describe what you did"

# See what's staged but not yet committed
git diff --staged
```