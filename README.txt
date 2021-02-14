#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Sun Feb 14 10:37:17 2021

"""


# Practice repository to start learning Git

## commands used
- git init: create a new git repo

- git status: compare working directory, staging area, and current branch

- git add: add changes from working directory to staging area

- git commit: commit changes from staging area to current branch
- git commit -m "<commit changes>": commits changes and adds one line description

- git config: set or get configuration

- git log: show a history (aka log) of project commits
- git log --oneline: show history of project commits in single line per commit
- git log --all: shows all commits
- git log --graph: shows graph view of all commits
- git log --oneline --all --graph: combines above
- git log <branch1>..<branch2>: log of commits in branch2 that don't exist in branch1
- git log <branch1>...<branch2>: log of commits in either branch but not both

- git branch: shows existing branches
- git branch -c: create a branch
- git branch -v: shows latest commit of all existing branches
- git branch --no-merged <branch1>: list of branches that have unmerged conflicts
- git branch --merged <branch1>: list of branches that have no unmerged conflicts

- git show: show a single commit

- git diff: show difference between commits, the working directory, and the staging area
- git diff <commit>: show diff b/w working dir and commit
- git diff --cached: show diff between staging area and HEAD
- git diff <commit>..<commit>: diff b/w two commits
- git diff <branch>..<branch>: diff b/w two branches

- git checkout: check out branch (update HEAD and apply chnages to working directory)
- git checkout -b: create branch, then check it out

- git stash: stash changes from working directory
- git stash list: list stashes
- git stash pop: apply stashed changes to working directory

- git merge: merge changes from different branches
- git merge --abort: abort an in-progress merge
- git merge --no-commit --no-ff: attempt to merge but don't create an auto or ff merge
    
- git remote -v: list remote repositories
- git push -u <remote><branch>: push <branch> to <remote> and set default upstream for <branch>

- git fetch: fetch changes from remote repository

## what's a branch?

a branch is a ref(erence) to a commit. 
when HEAD points to a branch, we say we're "on" that branch.
when we make a commit while we are on a branch, the branch is updated to ref(er) to the new commit

## what's a HEAD?

HEAD is a ref(erence) to the "current" branch (or sometimes a commit.. more on that later).
Git commands like "status", "log", and "branch" use HEAD. 
"git checkout" updates HEAD to ref(er) to a different branch.

## merging

merging means to bring the changes from one branch into another

- a fast forward (ff) merge happens when the target branch was branched from the current one,
and there are no new changes to the current branch since then.
- an automatic merge happens when the two histories have divereged, 
but git is able to reconcile them into one set of changes.
this creates a new commit on the current branch

## commit messages

default editor is vim (this can be changed)
    - 'i' to enter *insert* mode
    - type commit message
    - 'esc' -> ':wq' -> to write message and quit
or use 'git commit -m "<message>"'

- first line should be clear, accurate, and concise
- use proper grammar, spelling, and puncuation
- don't end with a '.'

for more advice, see: https://chris.beams.io/posts/git-commit/
