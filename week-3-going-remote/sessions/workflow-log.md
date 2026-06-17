# Workflow Log - Week 3

## Every Step Performed

### 1. Created GitHub Repository

- Went to github.com and logged in as Rosieeee344
- Clicked “New repository”
- Named it `codetopia-mentorship-program`
- Set visibility to Public
- Did NOT initialise with README (to avoid merge conflicts)
- Copied the SSH remote URL

### 2. Connected Local Repository

```bash
cd ~/Documents/codetopia-mentorship-program
git remote add origin git@github.com:Rosieeee344/codetopia-mentorship-program.git
git remote -v  # verified origin was set correctly
```

### 3. Pushed Local Commits

```bash
git push -u origin main
# All week 1, 2, and 3 files pushed to GitHub
```

### 4. Edited README on GitHub

- Opened the repo on GitHub
- Clicked the pencil (edit) icon on README.md
- Added a line describing the Week 3 capstone
- Committed directly on GitHub with message: `docs: update README with week 3 description`

### 5. Pulled Remote Changes

```bash
git pull origin main
# Downloaded the README edit made on GitHub
```

### 6. Verified Synchronisation

```bash
git log --oneline
# Confirmed the GitHub commit appeared in local history

git status
# Output: nothing to commit, working tree clean
```