#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Sun Feb 14 10:37:17 2021

@author: thilzinger001
"""


# Practice repository to start learning Git

## commands used
- git init: create repo
- git status: compare working directory, staging area, and current branch
- git add: add changes from working directory to staging area
- git commit: commit changes from staging area to current branch
- git config: set or get configuration
- git log: show history of project commits
- git branch -c: create a branch
- git checkout: check out (switch to) a branch (or HEAD)
- git checkout -b: create branch, then check it out

## what's a branch?

a branch is a ref(erence) to a commit. 
when HEAD points to a branch, we say we're "on" that branch.
when we make a commit while we are on a branch, the branch is updated to ref(er) to the new commit

## what's a HEAD?

HEAD is a ref(erence) to the "current" branch (or sometimes a commit.. more on that later).
Git commands like "status", "log", and "branch" use HEAD. 
"git checkout" updates HEAD to ref(er) to a different branch.

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