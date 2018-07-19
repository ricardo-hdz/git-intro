# Git Introduction

## Quickstart
```
git clone https://github.com/ricardo-hdz/git-intro.git
cd git-intro
git pull
```

## Git Basics

### 1. git checkout <branch>
- `git checkout feature_ab`
- Make changes to function ab()
- `git status`
- push changes to feature_ab branch `git push origin <branch>`

### 2. git rebase <branch>
- `git rebase master`
- resolve conflicts
- commit merge (after resolving conflicts, do `escape :`)

### 3. git stash, git apply
- Make changes to function ab()
- `git checkout master`
- `git stash`
- `git checkout master`
- `git checkout feature_ab`
- `git apply`

### Fork
- Create a fork of repo
- Make changes
- Create PR to main repo

### Create your own branch
`git checkout -b <branch_name>`
