# GIT

Definition: Git is a **Distributed Version Control System (DVCS)** used to track changes in files and source code locally without the internet.

GIT REPO: A Git repository is a location where Git manages your project files and their version history.

When we initialise Git in a project, it creates a hidden directory called `.git`, which stores Git’s internal information and repo history
cmd: git init

<u>**Architecture:</u>
1. Working Directory – Writing**

The place where we create, modify and delete project files.
⬇️
git add

**2. Staging Area – Selecting**

The place where we prepare selected changes before committing them.
⬇️
git commit

**3. Local Repository – Saving**

The place where Git stores committed snapshots and project history.

create new brach : git switch -c branch-name
switch - switches to another branch
-c - creates new branch

git branch - to check your current branch  (current branch is indicated with *)

always switch the branch that should receive changes before merging
master← branch
cmd on master branch: - git merge branchname

Delete a merged branch: git branch -d mergedbranch

**What is a merge conflict?**

A merge conflict occurs when Git cannot automatically combine changes made in different branches, usually because the same lines were modified differently. A developer must manually resolve the conflict, stage the resolved files, and commit the merge.

- **Local repository:** Git project on your computer.
- **Remote repository:** Git project hosted on a platform like GitHub.
- **Push:** Send your local commits to the remote.
- **Pull:** Download and integrate remote changes into your local branch.

| Command | Purpose |
| --- | --- |
| `git remote -v` | View remote connections |
| `git remote add origin URL` | Add a remote |
| `git remote remove origin` | Remove a remote connection |
| `git remote rename origin upstream` | Rename a remote |
| `git push origin master` | Push master to GitHub |
| `git push -u origin master` | Push and set upstream |
| `git push` | Push using configured upstream |
| `git fetch origin` | Download remote updates without integrating them |
| `git pull` | Fetch and integrate remote updates |

`git fetch`
Download only
Downloads the latest changes from GitHub but doesn't merge them into your current local branch.

`git pull`
Download + integrate
Downloads the latest changes and integrates them into your current local branch.

Command	Purpose
git clone URL	Downloads an existing repository
