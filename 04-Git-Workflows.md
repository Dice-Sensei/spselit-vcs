#Git Workflows

This document is introduction to **Git workflows**.

## Contents

- What is Git workflow?
- One person working with git
- Team working with git
- Git workflows

## What is Git workflow?

Git workflow is guideline or a recipe how to work with **Git** either by **yourself** (one man show) or in **team**. So that work is consistent and productive without unnecessary problems.

There is quite few workflows which can be applied but not all are good choice for given project complexity, team size and skill of team members.

## One person working with git

Working with git as one person is easy. Because only one person is editing files so keeping track of what work is being done, what files are edited in which branch is easy.

There are 3 ways how to work with git:

1. work is done by **one** person on one computer in one _branch_
2. work is done by **one** person on one computer in one _branch_ with connected _remote repository_
3. work is done by **one** person on one computer in multiple _branches_ with connected _remote repository_

### ad 1)

This is easiest way of working with _git_ as it is nearly same as just having files on disk. When something happens to disk or folder itself everything is lost. But at least it is possible to return to any commit in project history (not just Ctrl-Z buffer).

Used commands: **git init**, **git add**, **git commit**

### ad 2)

This will on top of **ad 1)** adds another advantage and remove a problem, that is if something happens to disk or folder you can always return to version which is available in _remote repository_. Of course that means that you have to **synchronize** your work from time to time.

Used commands: **git init**/**clone**, **git add**, **git commit**, **git push**

Possible workflows: **Centralized workflow**

### ad 3)

This will add another advantage on top of **ad 2)**, that is you can switch to another _branch_ do there some unrelated work or fix a bug and return back to previous _branch_.

Used commands: **git init**/**clone**, **git add**, **git commit**, **git push**, **git checkout**, **git merge**

Possible workflows: **Centralized workflow**, **Feature branching**

## Team working with git

Working with git as a team is more challenging on other hand there is a git which guards and helps when multiple people edit/move or remove same file. As one person does not have a problem to track which files are modified by him, team members sometimes does not know who is working on what, left alone which files may another team member need to modify.

There are 2 ways how to work with git:

1. work is done by **multiple** people on many computers in multiple _branches_ with connected _remote repository_
2. work is done by **multiple** people on many computers in multiple _branches_ with connected _remote repository_ where data are _merged_ via _pull requests_

### ad 1)

In this setup there is one shared _remote repository_ with which every team member will be synchronizing their work. Then each member will have _local repository_ on their own machine. They can work in multiple _branches_. When is time to **put work together** (specific part on which given member was working to connect/merge to main work) it will be _merged_ in _local repository_ by given member then _pushed_ to _remote repository_.

Note: Given that **git** is **distributed** then every team member will have available work of every other team member as long they **synchronized** through _remote repository_. Which means even if machine of team member dies and remote is lost it is still possible to recover work.

Used commands: **git init**/**clone**, **git add**, **git commit**, **git push**, **git checkout**, **git merge**

Possible workflows: **Centralized workflow**, **Feature branching**,

### ad 2)

Difference between this and **ad 1)** is only in way how work is _merged_ together. And that is via _Pull Request (PR)_ which means it will be _merged_ in _remote repository_ and there will space for other team members to **comment** on it via _Pull Request Review_ - which gives way more control over what, how and with which quality is _merged_.

Used commands: **git init**/**clone**, **git add**, **git commit**, **git push**, **git checkout**, **git merge**
