# Introduction

This document is introduction to **VCS** (Version Control System).

## Contents

- What is VCS?
- Why we need it?
- Where we use it?
- Solutions
- Types and Architecture

## What is VCS?

### Short version

**VCS** or Version Control System is set of tools for managing changes of files over time.

### Long version

**VCS** or Version Control System is set of tools for managing changes of files over time. It provides track of changes with options to _revert_ to previous versions.

Normally it is used for managing (human readable) text files mostly source code or documents. But it can be used on binary files too, but it will have reduced usability.

## Why we need it?

### Short version

- **Collaboration**: allows multiple people working on same file without overwriting each other work
- **History Tracking**: keeps track of all changes
- **Backup and Recovery**: provides way to _revert_ to previous version
- **Branching**: working separately on same file (more on this later)
- **Traceability**: way to find when bug was introduced

### Long version

- **Collaboration**: allows multiple people working on same file or even same line without unknowingly overwriting each other work (there may be _merge conflicts_, but that is for later)
- **History Tracking**: keeps track of all changes, not just content of files but also their creation, removal and movement, also includes author, timestamp and _commit message_
- **Backup and Recovery**: provides way to _revert_ to previous version which is useful in case of bugs or incidents, it is possible to _revert_ to any version
- **Branching**: working separately on same file, sometimes it is required to make changes to file without disturbing current work so we can work on same file in multiple isolated spaces knows as _branches_ before _merging_ them all together (more on this later)
- **Traceability**: way to find when bug was introduced, who cause it (_blame_) and where it was fixed

## Where we use it?

### Short version

- **Software development**
- **Document management**
- **Design projects**

### Long version

- **Software development**: management of codebase, database scheme versioning, Single source of truth
- **Document management**: collaborative writing projects, contract versioning
- **Design projects**: tracking project changes, keeping multiple versions available

## Solutions

Currently there quite few **VCS** just to name some: [Git](https://git-scm.com/), [SVN](https://subversion.apache.org/), [Mercurial](https://www.mercurial-scm.org/), [Perforce](https://www.perforce.com/products/helix-core), ...

We are going to use **Git** - already decided.

## Types and Architecture

### Short version

- **Local**: changes are stored locally
- **Centralized / Client-Server architecture**: changes are stored on server and clients connect to it to interact with it, example: **SVN**
- **Distributed**: all copies are kept in a local codebase _repository_, and updates are made by sharing _patches_ or modifications across peers, example: **Git**

### Long version

- **Local**: changes are stored locally as _patches_ to base file
- **Centralized / Client-Server architecture**: changes are stored on server and clients connect to it to interact with it, only current _branch_ is available _locally_ switching to another requires connecting to server, synchronization between peers is not possible, example: **SVN**
- **Distributed**: all copies are kept in a local codebase _repository_, and updates are made by sharing _patches_ or modifications across peers, normally there is some entity (for example GitHub, GitLab, Azure DevOps) which acts as _remote repository_ with which all peers are communicating regularly but that is only to make synchronization easier between them, local work can be done without connecting to it so offline work is possible, example: **Git**
