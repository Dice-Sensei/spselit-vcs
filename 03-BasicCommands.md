# Basic Git Commands

This document is introduction to basic commands for **Git**.

## Contents

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
- Practical task: ???

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

### git add

This command will add given file to _staging area_.

    git add <file name>

It is possible to take out files from _staging area_ but that can be done in many ways and it is advance topic.

### git commit

This command will _commit_ files from _staging area_ with given message.

    git commit -m <message>

Message should contain descriptive info what was done in given _commit_ (more on this later). Message is not strictly necessary but nobody wants to guess what was done in given _commit_ and for that reason **message is very important**.

### git fetch

This command will download information from given _repository_.

    git fetch <remote repository>

Provided information will be stored in _.git_ directory but will **not affect current working directory**.
