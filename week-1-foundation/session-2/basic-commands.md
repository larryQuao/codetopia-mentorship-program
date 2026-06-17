# Basic Git Commands

## Commands Used to Initialise a Repo

```bash
# Create and enter a new folder
mkdir my-project
cd my-project

# Initialise Git tracking
git init
```

This creates a hidden `.git` folder that tracks all changes going forward.

-----

## Right Commit Messages When Committing

Good commit messages follow the **imperative tense** and describe *what* the commit does, not *what you did*.

|Good ✅                        |Bad ❌        |
|------------------------------|-------------|
|`docs: add setup notes`       |`added notes`|
|`fix: correct typo in README` |`fixed stuff`|
|`feat: create git-states file`|`asdf`       |

**Format:** `type: short description (under 72 characters)`

Common types: `docs`, `feat`, `fix`, `chore`, `refactor`

-----

## Command to Check All Commits

```bash
# Full commit history
git log

# Clean one-line summary
git log --oneline

# Visual graph of all branches
git log --oneline --graph --all
```

-----

## Most Personally Used Commands in Git and CLI

```bash
git status          # Always run this first
git add .           # Stage everything
git commit -m ""    # Commit with a message
git log --oneline   # Check commit history
cd <folder>         # Navigate into a folder
mkdir <name>        # Create a new folder
ls                  # List files in current directory
clear               # Clear the terminal
```