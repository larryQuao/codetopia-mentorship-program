# Reflection - Week 3 Capstone

## Why Do Remote Repositories Matter?

Remote repositories matter because they take your work off a single machine and make it accessible from anywhere. If your laptop crashes or gets lost, your code is safe on GitHub. They also make collaboration possible — multiple developers can push and pull from the same repo without emailing files back and forth. For a developer, having your work on GitHub is also a public portfolio that shows what you can do.

-----

## What Does the `-u` Flag Do?

The `-u` flag in `git push -u origin main` stands for **“set upstream”**. It tells Git to remember that the local `main` branch should track the remote `origin/main` branch. After running it once, you can simply type `git push` or `git pull` without specifying `origin main` every time. It is a shortcut that saves typing on every future push and pull.

-----

## How Do Local and Remote Repositories Stay Synchronised?

They stay synchronised through `git push` and `git pull`. When you make commits locally and run `git push`, those commits are uploaded to GitHub. When changes are made on GitHub (by you or a collaborator) and you run `git pull`, those commits are downloaded and merged into your local branch. The key is to push and pull regularly so your local and remote histories stay aligned and do not diverge.

-----

## What Challenges Did I Face?

The main challenge I faced was that my Week 1 and Week 2 work was done on a friend’s laptop and was not accessible on my HP laptop. I had to recreate the markdown files from memory and from my session slides. This taught me the importance of always working in my own repo and pushing regularly — if I had pushed after each session, the work would never have been lost.

-----

## What Did I Learn This Week?

This week I learned how to connect a local Git repository to GitHub using `git remote add origin`, push code for the first time using `git push -u origin main`, pull remote changes with `git pull`, and understand what tracking branches are. I also learned the difference between `git clone` (downloading a repo for the first time) and `git pull` (updating an existing local repo). Most importantly, I learned that pushing to GitHub regularly is a habit, not an afterthought.