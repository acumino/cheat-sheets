## Git Commands Cheat Sheet

**Table of Contents:**
- [Git Commands Cheat Sheet](#git-commands-cheat-sheet)
  - [Repository Setup and Cloning](#repository-setup-and-cloning)
  - [Working Directory and Staging Area](#working-directory-and-staging-area)
  - [Committing Changes](#committing-changes)
  - [Branching and Merging](#branching-and-merging)
  - [Remote Repositories](#remote-repositories)
  - [Stashing Changes](#stashing-changes)
  - [Submodules](#submodules)
  - [Advanced Commands](#advanced-commands)

### Repository Setup and Cloning

- `git init`: Initialize a new git repository.
- `git clone <repository>`: Clone an existing repository.
- `git config --global user.name "<name>"`: Set the name associated with all commits.
- `git config --global user.email "<email>"`: Set the email associated with all commits.

### Working Directory and Staging Area

- `git status`: Check the status of your working directory.
- `git add <file>`: Add a file to the staging area.
- `git add .`: Add all files in the working directory to the staging area.
- `git rm <file>`: Remove a file from the working directory and the staging area.
- `git mv <old-file> <new-file>`: Rename a file and update the staging area.
- `git clean -n`: Show files that would be removed.
- `git clean -f`: Remove untracked files.
- `git clean -fd`: Remove untracked files and directories.

### Committing Changes

- `git commit -m "<message>"`: Commit the staged changes with a descriptive message.
- `git commit --amend`: Amend the last commit with new changes.
- `git log`: View the commit history.
- `git log --oneline`: View the commit history in a compact format.
- `git log --graph`: View the commit history as a graph.
- `git diff`: Show the differences between the working directory and the latest commit.
- `git diff --staged`: Show the differences between the staging area and the latest commit.
- `git diff <commit1> <commit2>`: Show the differences between two commits.
- `git show <commit>`: Show the changes made in a specific commit.

### Branching and Merging

- `git checkout <branch>`: Switch to a different branch.
- `git checkout -b <new-branch>`: Create a new branch and switch to it.
- `git branch`: List all branches in the repository.
- `git branch -m <new-branch>`: Rename the current branch.
- `git branch -a`: List all branches, including remote branches.
- `git branch -r`: List remote branches.
- `git merge --abort`: Abort a merge in progress.
- `git merge --continue`: Continue a merge after resolving conflicts.
- `git branch -d <branch>`: Delete a branch (if it has been merged).
- `git branch -D <branch>`: Force delete a branch.
- `git merge <branch>`: Merge the specified branch into the current branch.
- `git merge --no-ff <branch>`: Merge the specified branch into the current branch without fast-forwarding.
- `git cherry-pick <commit>`: Apply the changes from a specific commit to the current branch.
- `git cherry-pick --continue`: Continue cherry-picking after resolving conflicts.
- `git cherry-pick --abort`: Abort the cherry-pick operation.
- `git revert <commit>`: Create a new commit that undoes the changes from a specific commit.

### Remote Repositories

- `git remote add <name> <url>`: Add a remote repository.
- `git remote -v`: List all remote repositories.
- `git remote remove <name>`: Remove a remote repository.
- `git fetch <remote>`: Fetch changes from a remote repository.
- `git fetch --all`: Fetch changes from all remote repositories.
- `git pull <remote> <branch>`: Fetch changes from a remote repository and merge them into the current branch.
- `git push <remote> <branch>`: Push changes to a remote repository.
- `git push --force <remote> <branch>`: Force-push changes to a remote repository, potentially overwriting existing history.
- `git push --set-upstream <remote> <branch>`: Push changes to a remote repository and set the remote branch as the upstream branch.
- `git push --all <remote>`: Push all branches to a remote repository.
- `git push --tags <remote>`: Push all tags to a remote repository.

### Stashing Changes

- `git stash`: Temporarily save changes in the working directory that are not ready to be committed.
- `git stash list`: List all stashed changes.
- `git stash apply`: Apply the stashed changes to the working directory.
- `git stash drop`: Remove a single stash.
- `git stash drop <stash>`: Remove a specific stash.
- `git stash clear`: Remove all stashes.
- `git stash pop`: Apply the stashed changes and remove them from the stash list.
- `git stash branch <branch>`: Create a new branch and apply the stashed changes.

### Submodules

- `git submodule add <repository> <path>`: Add a submodule to the repository.
- `git submodule init`: Initialize the submodules.
- `git submodule update`: Update the submodules.
- `git submodule foreach <command>`: Execute a command in each submodule.
- `git submodule sync`: Synchronize the submodule URLs.

### Advanced Commands

- `git blame <file>`: Show who last modified each line of a file.
- `git bisect start`: Start a binary search to find a specific commit.
- `git bisect good <commit>`: Mark a commit as good during the binary search.
- `git bisect bad <commit>`: Mark a commit as bad during the binary search.
- `git bisect reset`: Reset the binary search.
- `git reflog`: Show the reference log.
- `git rebase <base>`: Rebase the current branch onto a new base commit.
- `git rebase -i <base>`: Interactively rebase the current branch onto a new base commit.
- `git rebase --abort`: Abort the rebase process.
- `git rebase --continue`: Continue the rebase process after resolving conflicts.
- `git rebase --skip`: Skip applying a specific commit during a rebase.
- `git fsck`: Check the repository for integrity.
- `git gc`: Clean up the repository and optimize it.
- `git archive <commit>`: Create an archive of a specific commit.
- `git tag`: List all tags in the repository.
- `git tag -a <tag> -m "<message>"`: Create an annotated tag with a message.
- `git tag -d <tag>`: Delete a tag.
- `git push <remote> :<tag>`: Remove a tag from a remote repository.
- `git fetch --prune`: Fetch changes from a remote repository and remove any remote-tracking branches that no longer exist on the remote.
- `git remote prune <remote>`: Remove any remote-tracking branches that no longer exist on the specified remote repository.
