# Introduction

This document is introduction to VCS (Version Control System).

## Contents

- What is VCS?
- Why we need it?
- Where we use it?

## What is VCS?

### Short version

VCS or Version Control System is set of tools for managing changes of files over time.

### Long version

VCS or Version Control System is set of tools for managing changes of files over time. It provides track of changes with options to revert to previous versions.

Normally it is used for managing (human readable) text files mostly source code or documents. But it can be used on binary files too, but it will have reduced usability.

## Why we need it?

### Short version

- Collaboration: allows multiple people working on same file without overwriting each other work
- History Tracking: keeps track of all changes
- Backup and Recovery: provides way to revert to previous version
- Branching: working separately on same file (more on this later)

### Long version

- Collaboration: allows multiple people working on same file or even same line without unknowingly overwriting each other work (there may be merge conflicts, but that is for later)
- History Tracking: keeps track of all changes - including author, timestamp and commit message
- Backup and Recovery: provides way to revert to previous version which is useful in case of bugs or incidents, it is possible to revert to any version
- Branching: working separately on same file; sometimes it is required to make changes to file without disturbing current work so we can work on same file in multiple isolated spaces before merging all work together (more on this later)

## Where we use it?

### Short version

- Software development
- Document management
- Design projects

### Long version

- Software development: management of codebase, database scheme versioning, Single source of truth
- Document management: collaborative writing projects, contract versioning
- Design projects: tracking project changes, keeping multiple versions available
