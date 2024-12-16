# Learnable Git Task

A Learnable to task to access our knowledge on Git and GitHub.

## Version Control

Version Control is a system that helps developers manage changes to source code or files over time. It tracks changes and modifications on file and saves these changes and modifications over time to allow easy access to passed modifications of your file in case you want to go back to previous versions for whatever reason. It also facilitates collaboration among team members by ensuring that everyone works on the latest version of the project and changes made to the code can be seen in the history of the file/project.

### Advantages of Version Control?

    1. Track Changes: It records who made changes, when, and what changes they made.
    2. Collaborate Effectively: Enables multiple developers to work on the same project without overwriting each other's work.
    3. Revert Mistakes: You can roll back to a previous version if a bug or error occurs or for whatever reason.
    4. Branching and Merging: Allows experimentation with features in isolated branches and merging them later.
    5. Audit and Documentation: Keeps a log of project/file history for accountability and easier debugging.

## Git vs GitHub

Git is a distributed version control system that enables developers to track changes in their source code or file (repositories). It works locally on your computer (offline) and does not require an internet connection aside when it is to be downloaded onto your computer. It is majorly used as a command-line interface (CLI) tool to track changes on ones local computer.  GitHub on the other hand is a platform for hosting git repositories online. It makes it easy to share and work on same code as it is hosted in the cloud. It provides an online backup for your repositories. Github also provides other tools to help improve collaboration and version control.


## Github Alternative
    1. GitLab
    2. BitBucket
    3. SourceForge

## Git fetch vs Git pull

Git fetch downloads/fetches the changes from a remote repository but doesn't change or modify your working or local branch. It stores those changes on another branch outside the working branch, allowing you to inspect them effectively before merging. Git pulls essentially downloads/fetches changes from the remote repository and immediately merges them into your local branch. It performs a git fetch and a git merge.

## Git rebase
It reapplies commits on top of another base tip. Let's say you have been working on a project with other developers, you create a new branch to work on a new feature while commits are still being made to the main branch. Git rebase essentially lets you reapply commits on your feature branch as though you branched off after the most recent commit to the main branch.

```bash
    git checkout feature
    git rebase main
```
this command checksout into your feature branch and reapplies commits as the tip of the base (main) branch.

##Git cherry-pick
As the name "cherry-pick" it allows you to pick specific commits on one branch to apply to another. It CHERRY-PICKS commits :). To cherry-pick a commit

```bash
    git checkout <target branch>
    git cherry-pick <commit hash>
```
To cherry-pick commits over a continuous range of commits, excluding the start commit.

```bash
    git checkout <target branch>
    git cherry-pick <stat commit hash>..<end commit hash>
```
symbols like ~ and ^ are added after the first commit to include or remove it from the commit.


To cherry-pick a non-continuous range of commit

```bash
    git checkout <target branch>
    git cherry-pick <commit hash>
```

to apply all commits from a branch

```bash
    git cherry-pick <branch name>
```
