# Week 2 Day 2 — Git Fundamentals

## What I Learned

- Initializing a Git repository using `git init`
- Checking repository status using `git status`
- Staging files using `git add`
- Creating commits using `git commit`
- Viewing commit history using `git log --oneline`
- Viewing unstaged changes using `git diff`
- Viewing staged changes using `git diff --cached`
- Discarding unstaged changes using `git restore`
- Unstaging changes using `git restore --staged`
- Working with branches using `git branch`
- Renaming the default branch to `main`
- Checking configured remote repositories using `git remote -v`

## Git Workflow

The basic Git workflow I practiced was:

```text
Working Directory
       ↓
    git add
       ↓
Staging Area
       ↓
   git commit
       ↓
Repository History
```

## Key Concepts

`git init` initializes a Git repository.

`git add` moves changes into the staging area.

`git commit` saves a snapshot of the staged changes.

`git status` shows the current state of the working directory and staging area.

`git diff` shows changes that have not been staged.

`git diff --cached` shows changes that have been staged.

## Branching Practice

I created and switched to a feature branch using Git.

The feature branch allows me to work on changes separately from the main branch.
`git restore` can discard unstaged changes.

`git restore --staged` removes a file from the staging area without deleting its changes.

## Professional Practice

I am organizing my DevOps learning into one portfolio repository so that my Linux, Git, development, DevOps, and QA work can be tracked as one continuous learning journey.
