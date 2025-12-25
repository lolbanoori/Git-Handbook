# Basic Git Operations

## Installation & GUIs

- **GitHub for Windows**: [https://windows.github.com](https://windows.github.com)
- **GitHub for Mac**: [https://mac.github.com](https://mac.github.com)
- **Git for All Platforms**: [http://git-scm.com](http://git-scm.com)

## Setup
Configuring user information used across all local repositories.

```bash
git config --global user.name "[firstname lastname]"
# Set a name that is identifiable for credit when reviewing version history

git config --global user.email "[valid-email]"
# Set an email address that will be associated with each history marker

git config --global color.ui auto
# Set automatic command line coloring for Git for easy reviewing
```

## Create & Initialize
Creating and cloning Git repositories.

```bash
git init
# Initialize an existing directory as a Git repository

git clone [url]
# Retrieve an entire repository from a hosted location via URL
```

## Stage & Snapshot
Working with snapshots and the Git staging area.

```mermaid
graph LR
    WD[Working Directory] -- git add --> SA[Staging Area]
    SA -- git commit --> LR[Local Repo]
    LR -- git push --> RR[Remote Repo]
    
    style WD fill:#ff9999,stroke:#333,stroke-width:2px
    style SA fill:#ffff99,stroke:#333,stroke-width:2px
    style LR fill:#99ff99,stroke:#333,stroke-width:2px
```

```bash
git status
# Show modified files in working directory, staged for your next commit

git add [file]
# Add a file as it looks now to your next commit (stage)

git reset [file]
# Unstage a file while retaining the changes in working directory

git diff
# Diff of what is changed but not staged

git diff --staged
# Diff of what is staged but not yet committed

git commit -m "[descriptive message]"
# Commit your staged content as a new commit snapshot
```

## Undoing Changes
Mistake recovery and safe rollback options.

```bash
git checkout <branch>
# Switch to another branch (e.g., git checkout main)

git reset
# Unstage staged files (after git add)

git reset --hard [commit]
# Reset to specific commit (dangerous — loses local changes)

git stash
# Temporarily shelve your changes to clean your working directory

git commit --amend
# Modify the most recent commit (do not use on published commits)

git revert [commit]
# Revert changes by creating a new commit that undoes a specific commit
```

\newpage