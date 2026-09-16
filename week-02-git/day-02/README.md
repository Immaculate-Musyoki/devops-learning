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

## Rewriting Git History

I practiced rewriting Git history using interactive rebase.

### Interactive Rebase

I used:

```text
git rebase -i HEAD~N
```

Interactive rebase allows me to review and modify a range of commits.

Common interactive rebase commands include:

* `pick` — keep the commit unchanged
* `reword` — change the commit message
* `edit` — stop and modify the commit
* `drop` — remove the commit
* `squash` — combine the commit with the previous commit and edit the message
* `fixup` — combine the commit with the previous commit while keeping the previous message

### Finding Commit History

I used:

```text
git log --oneline --decorate
```

to view my commit history and identify commits I may want to modify.

I also learned that:

```text
HEAD
```

represents my current position in the Git history.

Examples:

```text
HEAD~1
HEAD~2
HEAD~3
```

refer to commits progressively further back from `HEAD`.

### Changing an Old Commit Message

I practiced changing an older commit message using:

```text
git rebase -i HEAD~3
```

I changed:

```text
pick
```

to:

```text
reword
```

for the commit I wanted to rename.

I then entered the new commit message when Git opened the commit message editor.

### Amend vs Rebase

I learned that:

```text
git commit --amend
```

is used to replace or correct the latest commit.

For older commits, interactive rebase can be used:

```text
git rebase -i HEAD~N
```

### Commit IDs

I learned that rewriting a commit can change its commit ID (hash).

For example:

```text
Old commit: 9127f52
New commit: ff69ccf
```

The commit ID changes because Git creates a rewritten version of the commit.

### Reviewing Changes

I practiced reviewing my work before committing:

```text
git status
git diff
git add <file>
git status
git diff --cached
git diff --cached --check
git commit -m "Clear commit message"
```

This helps me review changes before they become part of my Git history.

### Important Lesson

Rewriting Git history should be done carefully, especially after commits have already been pushed to a shared remote repository.

For my personal learning repository, I am practicing these commands before publishing my work to GitHub.

## Git Workflow

My Git workflow is:

```text
Edit files
    ↓
git status
    ↓
git diff
    ↓
git add
    ↓
git status
    ↓
git diff --cached
    ↓
git diff --cached --check
    ↓
git commit
```

This practice is helping me maintain a clean and professional Git history.
