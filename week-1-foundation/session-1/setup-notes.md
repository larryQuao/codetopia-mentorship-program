# Setup Notes - Session 1

## Git Installation Verification

```bash
git --version
# Output: git version 2.x.x
```

## Git Configuration Commands

```bash
# Set global username
git config --global user.name "Rosemary Boahemaa"

# Set global email
git config --global user.email "your-email@example.com"

# Verify configuration
git config --list
```

## Git Commands Learned During Week 1

|Command                  |Purpose                                  |
|-------------------------|-----------------------------------------|
|`git init`               |Initialise a new local repository        |
|`git status`             |Check the state of your working directory|
|`git add <file>`         |Stage a file for commit                  |
|`git add .`              |Stage all changes                        |
|`git commit -m "message"`|Save staged changes with a message       |
|`git log`                |View full commit history                 |
|`git log --oneline`      |View compact commit history              |
|`git diff --staged`      |See staged changes before committing     |
|`git commit --amend`     |Fix the last commit message              |

## CLI vs GUI

**CLI (Command Line Interface)** is more useful when you need precise control, are working with Git commands, scripting, or SSH into a remote server. It is faster for experienced developers.

**GUI (Graphical User Interface)** is more useful for beginners who are visualising file structures or staging changes. Tools like GitHub Desktop make it easier to see what’s happening at a glance.