# Git

This document is introduction to **Git**.

**Version Control System** of our choice is **Git**.

## Contents

- Git introduction
- Installation
- First setup
- GUI Clients and IDE addons
- How git works
- Ways of working with git
- Git vocabulary

## Git introduction

### Short version

**Git** is widely used **Distributed Version Control System**.

### Long version

**Git** is a mature, **actively maintained** [open source project](https://github.com/git/git). It was originally developed in 2005 by Linus Torvalds, the creator of the Linux operating system kernel.

It is **Distributed Version Control System**.

A staggering number of software projects rely on Git for version control, including commercial projects as well as open source.

It works well on a wide range of operating systems and IDEs (Integrated Development Environments) and has many addons.

## Installation

Git is preinstalled on school computers and it is ready to be used. This topic describes installation process for use on personal workstations.

TODO

## First setup

First thing to setup after installing **Git** is registration of its user. This can be done in few ways, easiest is via cmd/terminal. Just type in:

    $ git config --global user.name "John Doe"

and

    $ git config --global user.email johndoe@example.com

Of course with your **own** name and email.

These values will be stored in config file in you profile specifically in (for Windows):

    <drive>:/Users/<username>/.gitconfig

To check that correct values are stored use command:

    git config --list

## GUI Clients and IDE addons

**Git** is mostly command line tool. It comes with basic GUI which can be used, but it is not really intuitive and it does not provide all functionality.

For this reason many GUI client exists, some of them are free. Whole list is available on [git website](https://git-scm.com/downloads/guis).

For same reason most IDEs have some addons which are used to use **git** via GUI.

## How git works

Work files are stored in _repository_ (_repo_) which is directory on disk. In this directory we can see our files with which we work (**current version**) and some additional files which are use by **Git**. Most of them are stored in _.git_ directory (in root of repository), but there can be additional files like _.gitignore_, _.gitconfig_ and so on (this is advance topic).

History of repository can be understood as **node tree**. Where each node is a _commit_ and each branch is a _branch_.

Every repository has virtual layer where are stored _staged changes_ (files or parts of files).

## Ways of working with git

1. work is done by **one** person on one computer in one _branch_
2. work is done by **one** person on one computer in one _branch_ with connected _remote repository_
3. work is done by **one** person on one computer in multiple _branches_ with connected _remote repository_
4. work is done by **multiple** people on many computers in multiple _branches_ with connected _remote repository_ where data are _merged_ via _pull requests_
5. work is done by **multiple** people on many computers in multiple _branches_ with connected _remote repository_ where data are _merged_ via _pull requests_ and specific **workflow** is used

## Git vocabulary

- repo/repository: place where code lives
- local repo: repository on workstation
- remote repo: repository on remote server (like GitHub)
- staging area: virtual space where changes for next commit are stored
- commit: set of changes in given time, also contains author, timestamp and parent(s)
- node tree: (graphical) representation of commits
- branch: set of connected commits
- merge: merge of different change sets (for example merging two branches together)
- merge conflict: system is not able automatically merge changes together
