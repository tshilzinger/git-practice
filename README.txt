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
- git checkout: check out branch (update HEAD and apply chnages to working directory)
- git branch: shows existing branches
- git branch -v: shows latest commit of all existing branches
- git merge: merge changes from different branches

## merging

merging means to bring the changes from one branch into another

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