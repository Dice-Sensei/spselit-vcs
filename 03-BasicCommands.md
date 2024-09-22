# Basic Git Commands

This document is introduction to basic commands for **Git**.

## Contents

- How it works
- Git commands
  - git init
  - git clone
  - git status
  - git add
  - git commit
  - git fetch
  - git pull
  - git push
- Git actions in Visual Studio Code
- Git vocabulary
- Practical task: ???

## How it works

Work files are stored in _repository_ (_repo_) which is directory on disk. In this directory we can see our files with which we work (**current version**) and some additional files which are use by **Git**. Most of them are stored in _.git_ directory (in root of repository), but there can be additional files like _.gitignore_, _.gitconfig_ and so on (this is advance topic).

## Git commands

**Git** has many commands which can be used, but only a fraction of them is used regularly. Whole list with example can be find [here](https://git-scm.com/docs/git#_git_commands).

To understand inner workings of GUI clients or IDE addons for **Git** some basic knowledge of **Git commands** is required. It is not just commands itself but also their meaning.

### git init

This command will crate **new empty** _repository_ of given name (it will contain only _.git_ directory).

    git init <repository name>

### git clone

This command will _clone_ **existing** _repository_ from given link (either _local_ or _remote_). This means it will contain all current files and whole history.

    git clone <repo> <directory>

### git status

This command will show status of repository.

TODO: how to read status

    git status

## Git vocabulary

- repo/repository: place where code lives
- local repo: repository on workstation
- remote repo: repository on remote server (like GitHub)
