Git Commands
============

_A list of my commonly used Git commands_

*If you are interested in my Git aliases, have a look at my `.bash_profile`, found here: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
| `git checkout origin/master filename` | to a copy a single file from remote or from other branch |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branchName]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git diff [source branch] [target branch]` | Preview changes before merging |

### stash & Commands

| Command | Description |
| ------- | ----------- |
| `git stash` | git stash is used to save the changes in present working directory |
| `git stash apply` | this command is used to apply the changes which you have saved before with the command git stash |
| `git stash list` | this command list all the stashed changes |
| `git stash drop` | this command delete the recent stashed chnages.|
| `git remote -v` | List all currently configured remote repositories |
| `git push --all origin` | Push all branches to your remote repository |
| `git push origin :<branchname>` | Delete a branch on your remote repository |
| `git tag 1.0.0 <commitID>` | You can use tagging to mark a significant changeset, such as a release |
| `git push --tags origin` | Push all tags to remote repository |
| `git fetch origin` | fetch the remote changes to local |
| `git reset --hard <sha-value>` | this command is used to switch from one commit -id to another [This command discards all history and goes back to the specified commit.] |
| `git reset --mixed` <sha-value> |  this command is used to switch from one commit to another but ....local changes will remain. |
| `git reset --soft` <sha-value> | this command is also used to switch but stage area changes will remain. |
| `git reset <filename>` | this command is used to unstage the file |
| `git reset <commit-id>` | This command undoes all the commits after the specified commit and preserves the changes locally [unstage all the chnages whatever files poresent in this commit-id] |
| `git log –follow [filename]` | This command lists version history for a file, including the renaming of files also |
| `git show [commit id]` | This command shows the metadata and content changes of the specified commit. |
| `git tag [commitID]` | This command is used to give tags to the specified commit. |
| `git revert <commitid>` | this command is used to remove/delete the commitid and it will create a new commited for history |
| `git rebase -i <commitid>` | this command is used to delete the commit id but it will not create a history |
| `git cherry-pick <commit id>` | this command is used to copy a sha-value from one branch to other |
