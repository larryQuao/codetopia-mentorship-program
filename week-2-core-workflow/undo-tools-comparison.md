# Undo Tools - Which to Use and When

## Overview

Git gives you multiple ways to undo mistakes. This file explains which tool works best for each scenario encountered during Week 2.

-----

## The Four Undo Tools

### 1. `git restore <file>`

**Use when:** You edited a file and want to throw away the changes before staging.

```bash
git restore notes.md
```

- Discards uncommitted changes in the working directory
- Cannot be undone — the change is gone
- Best for: “I changed my mind before staging”

-----

### 2. `git restore --staged <file>`

**Use when:** You accidentally staged a file and want to unstage it without losing your edits.

```bash
git restore --staged notes.md
```

- Moves the file back from staging to the working directory
- Your edits are kept, just unstaged
- Best for: “I staged the wrong file”

-----

### 3. `git revert HEAD`

**Use when:** You already committed something bad and want to undo it safely while keeping the history clean.

```bash
git revert HEAD
```

- Creates a **new commit** that reverses the last commit
- History is preserved — safe for shared/public repos
- Best for: “I committed something wrong and others might see it”

-----

### 4. `git reset --soft HEAD~1`

**Use when:** You committed too early and want to re-stage and recommit with a better message or more changes included.

```bash
git reset --soft HEAD~1
```

- Removes the last commit but keeps changes **staged**
- History is rewritten — only use on local/private work
- Best for: “I committed too soon or with a bad message”

-----

## Quick Decision Guide

|Situation                                     |Best Tool                    |
|----------------------------------------------|-----------------------------|
|Edited a file, not staged yet, want to discard|`git restore <file>`         |
|Staged by accident, want to unstage           |`git restore --staged <file>`|
|Committed something bad, want safe undo       |`git revert HEAD`            |
|Committed too early, want to redo             |`git reset --soft HEAD~1`    |