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
- git log --oneline: show history of project commits in single line per commit
- git show: show a single commit
- git diff: show difference between commits, the working directory, and the staging area
- git diff <commit>: show diff b/w working dir and commit
- git diff --cached: show diff between staging area and HEAD
- git diff <commit>..<commit>: diff b/w two commits
- git diff <branch>..<branch>: diff b/w two branches
- git checkout: check out branch (update HEAD and apply chnages to working directory)
- git branch: shows existing branches
- git branch -v: shows latest commit of all existing branches

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