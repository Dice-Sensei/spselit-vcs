# Introduction

This document is introduction to VCS (Version Control System).

## Contents

- What is VCS?
- Why we need it?
- Where we use it?

## What is VCS?

### Short version

VCS or Version Control System is set of tools for managing changes of text files.

### Long version

VCS or Version Control System is set of tools which helps manage changes to text files mostly source code or documents. It can be used on binary files to but it will have reduced usability.

## Why we need it?

### Short version

- Collaboration: allows multiple people working on same file without overwriting their work
- History Tracking: keeps track of all changes
- Backup and Recovery: provides way to revert to previous version
- Branching: working separately on same file

### Long version

- Collaboration: allows simultaneously multiple people to work on same file or even same line of file without unknowingly overwriting each other work (there may be merge conflicts)
- History Tracking: keeps track of all changes done including author id, timestamp and commit message
- Backup and Recovery: provides way to revert to previous version which is useful in case of bugs and not just previous version but any
- Branching: working separately on same file; sometimes it is required to make changes to file without disturbing current work so we can work on same file in multiple isolated spaces before merging all work together

## Where we use it?

### Short version

- Software development
- Document management

### Long version

- Software development: management of codebase, database scheme versioning, Single source of truth
- Document management: writing projects, contract versioning
