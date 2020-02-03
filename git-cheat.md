# Github Cheat Sheet
Copy of [Github cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf).

## Setup
Configuring user information used across all local repositories. These
commands would be run only once.

Set a name that is identifiable for credit when review version history.
```
git config --global user.name “[firstname lastname]”
```

Set an email address that will be associated with each history marker.
```
git config --global user.email “[valid-email]”
```

Set automatic command line coloring for Git for easy reviewing.
```
git config --global color.ui auto
```

## Repo Initialization
Configuring user information, initializing and cloning repositories.

Initialize an existing directory as a Git repository.
```
git init
```

Retrieve an entire repository from a hosted location via URL.
```
git clone [url]
```

## Stage & Snapshot
Working with snapshots and the Git staging area.

Show modified files in working directory, staged for your next commit.
```
git status
```

Add a file as it looks now to your next commit (stage).
```
git add [file]
```

Unstage a file while retaining the changes in working directory.
```
git reset [file]
```

Get difference of what is changed but not staged.
```
git diff
```

Get difference of what is staged but not yet committed.
```
git diff --staged
```

Commit your staged content as a new commit snapshot.
```
git commit -m “[descriptive message]”
```

Transmit local branch commits to the remote repository branch.
```
git push [alias] [branch]
```

## Branch & Merge
Isolating work in branches, changing context, and integrating changes

List your branches. A * will appear next to the currently active branch.
```
git branch
```

Create a new branch at the current commit.
```
git branch [branch-name]
```

Switch to another branch and check it out into your working directory.
```
git checkout
```

Merge the specified branch’s history into the current one.
```
git merge [branch]
```

## Update
Retrieving updates from another repository and updating local repos.

Fetch down all the branches from that Git remote.
```
git fetch [alias]
```

Merge a remote branch into your current branch to bring it up to date.
```
git merge [alias]/[branch]
```

Fetch and merge any commits from the tracking remote branch.
```
git pull
```
