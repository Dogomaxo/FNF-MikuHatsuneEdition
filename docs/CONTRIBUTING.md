# Contributing to FNF: Miku Hatsune Edition

Thank you for your interest in contributing to **FNF: Miku Hatsune Edition**! This guide will help you get started with filing issues or opening pull requests.

## Table of Contents

- [Contributing to FNF: Miku Hatsune Edition](#contributing-to-fnf-miku-hatsune-edition)
  - [Table of Contents](#table-of-contents)
  - [1. Issues Guidelines](#1-issues-guidelines)
    - [1.1 Requirements](#11-requirements)
  - [1.2 Issue Types](#12-issue-types)
    - [Bug Report (view list)](#bug-report-view-list)
    - [Crash Report (view list)](#crash-report-view-list)
    - [Charting Issue (view list)](#charting-issue-view-list)
    - [Enhancement (view list)](#enhancement-view-list)
    - [Content Contribution (Not Implemented yet)](#content-contribution-not-implemented-yet)
  - [1.3 Before You Submit](#13-before-you-submit)
  - [2. Pull Request Guidelines](#2-pull-request-guidelines)
    - [2.1 Choosing a base branch](#21-choosing-a-base-branch)
    - [2.2 Maintaining your pull request](#22-maintaining-your-pull-request)
    - [2.3 Merge conflicts and rebasing](#23-merge-conflicts-and-rebasing)
    - [2.4 Code PRs](#24-code-prs)
    - [2.5 Code comments](#25-code-comments)
    - [2.6 Documentation PRs](#26-documentation-prs)
    - [2.7 GitHub PRs](#27-github-prs)
  - [2.8 Charting PRs](#28-charting-prs)
  - [3. Acknowledgments and Closing](#3-acknowledgments-and-closing)

## 1. Issues Guidelines

Use issues to report bugs or request features. This section provides guidelines to follow when opening an [issue](https://github.com/Dogomaxo/FNF-MikuHatsuneEdition/issues).

### 1.1 Requirements

Make sure you're playing:

- the latest version of the game (currently **v0.8.3**)
- the latest version of the mod (currently **v0.1.0-pre.alpha** or **Develop Build**)
- without any mod other than Miku's

## 1.2 Issue Types

Choose the appropriate template that bestsuits your needs:

### Bug Report ([view list](https://github.com/Dogomaxo/FNF-MikuHatsuneEdition/issues?q=is%3Aissue%20state%3Aopen%20label%3A"type%3A%20minor%20bug"))

   For minor bugs and general issues with the game. Choose this one if none of the others fit your needs.

### Crash Report ([view list](https://github.com/Dogomaxo/FNF-MikuHatsuneEdition/issues?q=is%3Aissue%20state%3Aopen%20label%3A"type%3A%20major%20bug"))

   For crashes and freezes

### Charting Issue ([view list](https://github.com/Dogomaxo/FNF-MikuHatsuneEdition/issues?q=is%3Aissue%20state%3Aopen%20label%3A"type%3A%20charting%20issue"))

   For misplaced notes, wonky camera movements, broken song events, and everything related to the game's charts.

### Enhancement ([view list](https://github.com/Dogomaxo/FNF-MikuHatsuneEdition/issues?q=is%3Aissue%20state%3Aopen%20label%3A"type%3A%20enhancement"))

   For suggestions to add new features or improve existing ones. (Since I am only one person on this project, I greatly appreciate enhancement.)

### Content Contribution (Not Implemented yet)

   propose new art sprites, audio, charts, or stages from WIP songs.

## 1.3 Before You Submit

Complete the Issue Checklist at the top of your template!

Be sure to use the search bar on the Issues page to check that your issue hasn't already been reported by someone else.
Duplicate issues make it harder to keep track of important issues with the mod.

Fill out all required fields in the template and attach screenshots or files if applicable.

Also only report one issue or enhancement at a time! If you have multiple bug reports or suggestions, split them up into separate submissions so they can be checked off one by one.

Once you're sure your issue is unique and specific, feel free to submit it.

> [!TIP]
> If none of the above Issue templates suit your inquiry (like questions about songs, mechanics, content, install, etc.), please [open a discussion](https://github.com/Dogomaxo/FNF-MikuHatsuneEdition/discussions).

**Thank you for opening issues! This helps me a lot with the development of the mod and avoiding future conflicts.**

## 2. Pull Request Guidelines

You are welcome to contribute changes by [opening pull requests](https://github.com/Dogomaxo/FNF-MikuHatsuneEdition/pulls).
This section covers guidelines for opening and managing pull requests (PRs).

### 2.1 Choosing a base branch

When creating a branch in your fork, base your branch on either the `main` or `develop` branch depending on the types of changes you want to make.

> [!CAUTION]
> Avoid using your fork's default branch (`main` in this case) for your PR. This is considered an [anti-pattern](https://jmeridth.com/posts/do-not-issue-pull-requests-from-your-master-branch/) by GitHub themselves!
> Instead, make a separate branch for your additions (ex. `docs/fix-typo` or `minor-bugfix`).

Choose the `main` branch if you modify:

- Documentation (`.md` files)
- GitHub files (`.yml` files or anything in the `.github` folder)

Choose the `develop` branch if you modify:

- Mod code (`Hscript (.hxc)` files)
- Any other type of file like images, sounds, songs metadata, etc.

> [!TIP]
> When in doubt, base your branch on the `develop` branch.

Choosing the right base branch helps keep your commit history clean and avoid merge conflicts.
Once you’re satisfied with the changes you’ve made, open a PR and base it on the same branch you previously chose.

### 2.2 Maintaining your pull request

Keeping your pull request clean and easy to review increases the chance that it will be accepted!

The maintenance policy is as follows::

- If I require changes to your PR, we will label your PR `status: needs revision`.
- I may also leave a comment under your PR specifying what changes you should make.
- If you receive a comment, you have 45 days to implement the requested changes.
- After this period, your PR will be closed due to inactivity and labeled `status: stale`.
- Even after your PR is closed, you may request for me to reopen it. Just be sure to address the issues!

This policy ensures that PRs awaiting review are up to date and ready to merge.

### 2.3 Merge conflicts and rebasing

Some mod updates may introduce significant breaking changes that may create merge conflicts in your PR. To resolve them, you will need to update or rebase your PR.

Most merge conflicts are small and will only require you to modify a few files to resolve them.
However, some changes are so big that your commit history will be a total mess!
In this case, you will have to perform a [**rebase**](https://docs.github.com/en/get-started/using-git/about-git-rebase).
This process reapplies your changes on top of the updated branch and cleanly resolves the merge conflicts.

> [!TIP]
> If your commit history becomes too long, you can use rebase to `squash` your PR's commits into a single commit.

### 2.4 Code PRs

Code-based PRs make changes such as **fixing bugs** or **implementing new features** in the mod.

This involves modifying one or several of the repository’s `.hxc` files, found within the `scripts/` folder.

### 2.5 Code comments

Code comments help others understand your changes, so the way you write them is important!
Here are some guidelines for writing comments in your code:

- **Explain the “why”, not the “what”**. Only add a comment when the intent or logic isn’t immediately clear.
- **Use DocBlocks** (`/** … */`) above functions or classes to describe their purpose, parameters, and any special behavior.
- **Inline comments** (`// …`) should be brief and only clarify edge cases or design decisions (e.g., “prevent negative time”).
- **Keep comments up to date** and remove any commented-out code or debug traces that are no longer needed.
- **Avoid opinions or signing every line**; only add your name when a non-trivial explanation might require follow-up.

### 2.6 Documentation PRs

Documentation-based PRs make changes such as **fixing typos** or **adding new information** in documentation files.

This involves modifying one or several of the repository’s `.md` files, found throughout the repository.

Make sure your changes are easy to understand and formatted consistently to maximize clarity and readability.

> [!CAUTION]
> DO NOT TOUCH THE `LICENSE.md` FILE, EVEN TO MAKE SMALL CHANGES!

### 2.7 GitHub PRs

GitHub-related PRs make changes such as **tweaking Issue Templates** or **updating the repository’s workflows**.

This involves modifying one or several of the repository’s `.yml` files, or any other file in the `.github` folder.

If you want to contribute improvements to the repository's GitHub workflows or templates (e.g., issue templates or GitHub Actions), please test them on your own fork first to avoid breaking anything in the main project.

## 2.8 Charting PRs

Charting PRs make changes such as **adjusting chart metadata**.

This involves modifying one or several of the `assets` repository's `*-metadata.json` files, found in the `data/songs/` directory.

> [!CAUTION]
> I **do not** accept changes to the chart `.json` file itself.
> If you find an error in the game's charts, please open an issue and I'll review it and make tweaks themselves as necessary.

## 3. Acknowledgments and Closing

Based on practices from [FunkinCrew's CONTRIBUTING.md](https://github.com/FunkinCrew/Funkin/blob/main/docs/CONTRIBUTING.md).

Thank you for reading the Contributing Guide.
I truly hope to receive contributions from you. You don't know how much it would mean to me and how grateful I will be.
