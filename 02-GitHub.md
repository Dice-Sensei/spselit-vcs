# GitHub

This document is introduction to **GitHub**.

## Contents

- What is GitHub?
- How we use it?
- Registration
- Showcase
- Creating repository

## What is GitHub?

### Short version

**GitHub** is service with [website](https://github.com/) which allows hosting of repositories. **GitHub** also provides additional service like project management, CI/CD and collaboration tools.

### Long version

**GitHub** is service with [website](https://github.com/) which allows hosting of repositories. On top of that **GitHub** is providing many additional services, like project management (issue, project boards, roadmap, wiki), CI/CD (GitHub actions, package hosting, GitHub pages, deployment), collaboration tools (pull request, code reviews, Codespaces, GitHub Copilot) and many more.

## How we use it?

In school we will use it to store your code, to provide you with assignments, to share school resources, to host your projects, to grade your work and so on.

In practice this really depends on team/company. Some have full workflow on GitHub from project management (creating issue), through code repository, code reviews, CI/CD (building software), deployment, documentation. Some have just part of workflow mostly code repository and code reviews.

## Registration

To use GitHub you need an account - obviously.

If you don't have one, please sing up [here](https://github.com/signup). You will just need an email, password and some nickname.

As this account will be yours and you will have all you school stuff there which can be later used when searching for work. Take this seriously and make a permanent account for you future self.

It is recommended to fill in you profile data (public profile).

## Showcase

What others can see from your profile and what it means.

### Profile

Profile dashboard `https://github.com/<username>` is publicly available (if not set otherwise). For example [Dice-Sensei](https://github.com/Dice-Sensei)'s dashboard.

Dashboard shows **contribution stats** to repositories hosted on GitHub. Only publicly available repositories are listed, but statistics can be provided for private too. Only to public repositories will be provided with links for activities like opening **Pull Request**.

Points of interest on dashboard are contribution matrix and contribution activity.

### Public repositories

Public repositories are your business card. Your potential new employer will be looking to these, checking your contributions and interests.

As already mention only public repositories will be shown, so if you wan't to work on something that is not ready to be seen by world have that repository as private.

## Creating repository

Repository can be created either **empty** or from **existing template** (this option will be used for tests and providing examples).

Repository can be **public** or **private**. Public means that code will be visible to everyone, but owner of repository will have control of who can contribute. Also **GitHub** will provide more tools to work on it with, for example pages or wiki. Private repository will not be publicly available, but it possible to specify which GitHub users will have access to it.

### Readme

Every _repository_ is **expected** but it is **not required** to contain `README.md` file. In this file you can describe you project in more detail then in description on **GitHub**. Also this file will be automatically show when looking at main page of _repository_.

### Ignore

Every _repository_ should contain `.gitignore` file. This file provides information to **git** which files should be ignored (not tracked - included in changes).

Which files should be ignored depends on programming language and used tool chain. As some languages and tools are producing large number of temporary or personal files.

**Best practice** is to create this ignore file on start of _repository_ (as already _tracked_ files are not automatically removed when ignore file is added). For that reason there is option to select template form which `.gitignore` will be crated.

### License

Every _repository_ should contain license file. GitHub provides option to pick license file on creation.

_Licensing problematic is really broad topic and it is out of scope for this learning resource._
