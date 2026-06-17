# Remote Notes - Week 3

## What Is a Remote Repository?

A remote repository is a version of your project that is hosted on the internet or a network, separate from your local machine. It allows you to back up your work, share it with others, and collaborate on the same codebase from different computers.

The most common place to host a remote repository is **GitHub**.

-----

## What Is Origin?

`origin` is the default name Git gives to the remote repository you cloned from or connected to. It is simply a shortcut — instead of typing the full URL every time, you type `origin`.

```bash
# View what origin points to
git remote -v
```

You will see something like:

```
origin  git@github.com:Rosieeee344/my-repo.git (fetch)
origin  git@github.com:Rosieeee344/my-repo.git (push)
```

-----

## Why Do Developers Use GitHub?

Developers use GitHub because it:

1. **Stores code safely in the cloud** — your work is backed up even if your laptop is lost or damaged
1. **Enables collaboration** — multiple developers can work on the same project using branches and pull requests
1. **Tracks the full history** — every change is recorded with who made it and why
1. **Supports open source** — developers can share projects publicly and contribute to others’ work
1. **Integrates with tools** — GitHub connects to deployment platforms, CI/CD pipelines, and project management tools

-----

## Difference Between Local and Remote Repositories

|Local Repository                      |Remote Repository                                 |
|--------------------------------------|--------------------------------------------------|
|Stored on your computer               |Stored on GitHub (or similar)                     |
|Only you can access it                |Anyone with permission can access it              |
|Works offline                         |Requires internet connection                      |
|Changes stay local until pushed       |Changes are visible to collaborators after push   |
|Created with `git init` or `git clone`|Created on GitHub and linked with `git remote add`|
