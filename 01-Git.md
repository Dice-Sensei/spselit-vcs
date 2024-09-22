# Git

This document is introduction to **Git**.

**Version Control System** of our choice is **Git**.

## Contents

- Git introduction
- Installation
- First setup
- GUI Clients and IDE addons

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
