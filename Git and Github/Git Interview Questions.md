# Git and GitHub Interview Questions

## Table of Contents
1. [What is Git, and what is it used for?](#what-is-git-and-what-is-it-used-for)
2. [What is the difference between Git and GitHub?](#what-is-the-difference-between-git-and-github)
3. [What is the purpose of git init?](#what-is-the-purpose-of-git-init)
4. [What is the difference between git clone and git pull?](#what-is-the-difference-between-git-clone-and-git-pull)
5. [What is the purpose of the .gitignore file?](#what-is-the-purpose-of-the-gitignore-file)
6. [What is a commit in Git?](#what-is-a-commit-in-git)
7. [What is the difference between git fetch and git pull?](#what-is-the-difference-between-git-fetch-and-git-pull)
8. [What is a branch in Git, and why is it important?](#what-is-a-branch-in-git-and-why-is-it-important)
9. [How do you create and switch to a new branch in Git?](#how-do-you-create-and-switch-to-a-new-branch-in-git)
10. [What is git merge, and how does it work?](#what-is-git-merge-and-how-does-it-work)
11. [What is git rebase, and how does it differ from git merge?](#what-is-git-rebase-and-how-does-it-differ-from-git-merge)
12. [How do you resolve a merge conflict in Git?](#how-do-you-resolve-a-merge-conflict-in-git)
13. [What is git stash, and how is it used?](#what-is-git-stash-and-how-is-it-used)
14. [What is git reset, and how does it work?](#what-is-git-reset-and-how-does-it-work)
15. [How do you undo the last commit?](#how-do-you-undo-the-last-commit)
16. [What is git squash, and when would you use it?](#what-is-git-squash-and-when-would-you-use-it)
17. [What is a pull request (PR), and how is it used in GitHub?](#what-is-a-pull-request-pr-and-how-is-it-used-in-github)
18. [What is the difference between git fork and git clone on GitHub?](#what-is-the-difference-between-git-fork-and-git-clone-on-github)
19. [How would you handle version control for large binary files in Git?](#how-would-you-handle-version-control-for-large-binary-files-in-git)
20. [What are GitHub Actions, and how are they used?](#what-are-github-actions-and-how-are-they-used)

---

### What is Git, and what is it used for?
Git is a distributed version control system used to track changes in source code during software development. It allows multiple developers to work on the same project simultaneously, without overwriting each other's changes. Git maintains a complete history of all changes made to the code, allowing for easy rollback to previous versions.

### What is the difference between Git and GitHub?
Git is the version control tool that developers use to manage code locally, whereas GitHub is a cloud-based hosting service for Git repositories. GitHub provides collaboration features like pull requests, issues, and code reviews, making it easy for teams to work on the same project remotely.

### What is the purpose of git init?
The git init command is used to initialize a new Git repository in an existing directory or create a new, empty repository. It sets up the necessary .git directory to begin tracking changes to files in that directory.

### What is the difference between git clone and git pull?
- **git clone**: Used to create a local copy of a remote Git repository. It downloads the entire repository including its history.
- **git pull**: Fetches changes from a remote repository and merges them into your current branch. It is used when you already have a cloned repository and want to sync it with the latest changes from the remote.

### What is the purpose of the .gitignore file?
The .gitignore file specifies which files and directories Git should ignore and not track. This is useful for excluding unnecessary files (like build files, dependencies, or sensitive information) from being committed to the repository.

### What is a commit in Git?
A commit is a snapshot of the project at a particular point in time. Each commit represents a change made to the codebase, and it records the changes along with a message describing what was done. Commits form the backbone of version control in Git.

### What is the difference between git fetch and git pull?
- **git fetch**: Retrieves changes from the remote repository but does not merge them into your local branch. It updates your local tracking branches but keeps the working directory unchanged.
- **git pull**: Combines git fetch and git merge, fetching changes from the remote repository and merging them into your current branch.

### What is a branch in Git, and why is it important?
A branch in Git is a separate line of development that allows you to work on new features or bug fixes without affecting the main codebase. Branches enable parallel development, experimentation, and isolated work. Once the branch is ready, it can be merged back into the main codebase.

### How do you create and switch to a new branch in Git?
- To create a new branch: `git branch <branch-name>`
- To switch to a new branch: `git checkout <branch-name>`
- Alternatively, you can create and switch to a new branch in one command: `git checkout -b <branch-name>`

### What is git merge, and how does it work?
`git merge` is used to combine changes from one branch into another. It integrates the history of two branches, creating a new commit if there are no conflicts. In case of conflicts, Git will prompt you to resolve them manually before completing the merge.

### What is git rebase, and how does it differ from git merge?
`git rebase` moves or re-applies commits from one branch onto another. It creates a linear history by replaying commits on top of another branch. Unlike `git merge`, rebase doesn’t create a merge commit, making the history cleaner. However, it rewrites history, so it's best used carefully, especially on shared branches.

### How do you resolve a merge conflict in Git?
When Git encounters conflicting changes during a merge, it will pause the merge and mark the conflicts in the affected files. To resolve the conflict:
1. Open the conflicting files and decide which changes to keep.
2. After resolving conflicts, mark the conflict as resolved by using `git add <file>`.
3. Finally, complete the merge with `git commit`.

### What is git stash, and how is it used?
`git stash` temporarily saves your changes without committing them, allowing you to work on something else (like switching branches) and come back to your stashed changes later.
- To stash changes: `git stash`
- To apply stashed changes: `git stash apply`
- To remove stashed changes from the stash list after applying: `git stash drop`

### What is git reset, and how does it work?
`git reset` is used to undo changes. It can reset the current branch to a previous commit, modifying the staging area and/or the working directory depending on the options used:
- `--soft`: Moves the HEAD pointer without modifying the staging area or working directory.
- `--mixed`: Resets the staging area but keeps the changes in the working directory (default behavior).
- `--hard`: Resets both the staging area and the working directory, discarding all changes.

### How do you undo the last commit?
If you want to undo the last commit but keep the changes in your working directory:
```bash
git reset --soft HEAD~1
```
If you want to undo the last commit and discard the changes:
```bash
git reset --hard HEAD~1
```

### What is git squash, and when would you use it?
`git squash` is the process of combining multiple commits into a single commit. This is often done to clean up the commit history before merging a feature branch into the main branch. Squashing helps keep the commit history concise and meaningful. To squash commits, you can use interactive rebase:
```bash
git rebase -i <base-commit>
```

### What is a pull request (PR), and how is it used in GitHub?
A pull request is a feature in GitHub (and other Git hosting platforms) that allows developers to notify team members when they have completed work in a branch and want to merge it into the main branch. A PR facilitates code review, discussion, and collaboration before merging.

### What is the difference between git fork and git clone on GitHub?
- `git fork:` Creates a copy of a repository under your own GitHub account. This is used to propose changes to someone else's project.
- `git clone:` Downloads a copy of a repository to your local machine, which you can work on independently or contribute to if you have write access.

### How would you handle version control for large binary files in Git?
Git is not optimized for handling large binary files. However, Git LFS (Large File Storage) can be used to manage large files efficiently. Git LFS stores large files outside the repository and replaces them with small pointer files, reducing the repository size and improving performance.

### What are GitHub Actions, and how are they used?
GitHub Actions is a CI/CD (Continuous Integration/Continuous Deployment) feature that allows you to automate workflows directly in your GitHub repositories. You can create actions that run on specific events (like pushes, pull requests, etc.) to build, test, or deploy your code.