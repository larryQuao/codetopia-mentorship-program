# Push-Pull Workflow - Week 3

## Command 1: `git remote add origin`

**Purpose:**
Links your local repository to a remote repository on GitHub. Without this, Git doesn’t know where to send or receive changes.

**Syntax:**

```bash
git remote add origin <repo-url>
```

**Example:**

```bash
git remote add origin git@github.com:Rosieeee344/codetopia-mentorship-program.git
```

**Expected Outcome:**
No output means it worked. Verify with:

```bash
git remote -v
```

You should see `origin` listed with fetch and push URLs.

-----

## Command 2: `git push -u origin main`

**Purpose:**
Uploads your local commits to the remote repository on GitHub. The `-u` flag sets `origin main` as the default upstream, so future pushes only need `git push`.

**Syntax:**

```bash
git push -u origin main
```

**Example:**

```bash
git push -u origin main
# Output: Branch 'main' set up to track remote branch 'main' from 'origin'.
```

**Expected Outcome:**
Your files appear on GitHub. The `-u` flag means next time you can just run `git push`.

-----

## Command 3: `git pull origin main`

**Purpose:**
Downloads and merges the latest changes from the remote repository into your local branch. Used when someone else (or you via GitHub’s editor) has made changes remotely.

**Syntax:**

```bash
git pull origin main
```

**Example:**

```bash
git pull origin main
# Output: Updating abc123..def456
# Fast-forward
#  README.md | 2 ++
```

**Expected Outcome:**
Your local files are updated to match what is on GitHub. Any new commits from the remote are added to your local history.
