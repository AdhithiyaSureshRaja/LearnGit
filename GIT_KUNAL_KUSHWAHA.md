
# List of Git Commands
Source : Complete Git essentials
Note: <> means have to write your own values (file names, branch names, URLs). [] means optional. // means comment.

---

## 1. Git Setup

### To set user name:
```
git config --global user.name "<your_name>"
```
**Note:** Sets your Git username globally.

### To set user email:
```
git config --global user.email "<your_email>"
```
**Note:** Sets your email globally.

### To check current configuration:
```
git config --list
```
**Note:** Displays all git configurations.

---

## 2. Initialize and Clone Repository

### To initialize a new repository:
```
git init
```
**Note:** Creates a new Git repository in the current directory.

### To clone an existing repository:
```
git clone <repository_url>
```
**Note:** Copies an existing repository from remote to your local machine.

---

## 3. Basic File Operations

### To check the status of files:
```
git status
```
**Note:** Shows the state of working directory and staging area.

### To add a file to staging:
```
git add <file_name>
```
**Note:** Adds the specified file to staging area.

### To add all files to staging:
```
git add .
```
**Note:** Adds all modified and new files to staging area.

### To unstage a file:
```
git reset <file_name>
```
**Note:** Removes file from staging but keeps changes in working directory.

### To remove a tracked file from the repo:
```
git rm <file_name>
```
**Note:** Deletes file from working directory and staging.

### To rename a file:
```
git mv <old_file> <new_file>
```
**Note:** Renames a file and stages the change.

---

## 4. Commit Changes

### To commit staged changes with a message:
```
git commit -m "<commit_message>"
```
**Note:** Saves staged changes permanently in history with a message.

### To amend the last commit:
```
git commit --amend
```
**Note:** Updates the last commit message or adds new changes to it.

---

## 5. Branching and Merging

### To create a new branch:
```
git branch <branch_name>
```
**Note:** Creates a new branch.

### To switch to a branch:
```
git checkout <branch_name>
```
**Note:** Switches to the specified branch.

### To create and switch to a branch:
```
git checkout -b <branch_name>
```
**Note:** Creates a new branch and switches to it immediately.

### To list all branches:
```
git branch
```
**Note:** Shows all branches.

### To delete a branch:
```
git branch -d <branch_name>
```
**Note:** Deletes the specified branch if merged.

### To merge a branch into current branch:
```
git merge <branch_name>
```
**Note:** Merges the specified branch into the current branch.

---

## 6. Remote Repositories

### To add a remote:
```
git remote add origin <repository_url>
```
**Note:** Links local repository to remote.

### To view remotes:
```
git remote -v
```
**Note:** Displays remote names and URLs.

### To remove a remote:
```
git remote remove <remote_name>
```
**Note:** Removes the specified remote.

### To change remote URL:
```
git remote set-url origin <new_repository_url>
```
**Note:** Updates the remote repository URL.

---

## 7. Fetch, Pull, and Push

### To fetch changes from remote:
```
git fetch origin
```
**Note:** Downloads changes from remote but does not merge.

### To pull changes from remote:
```
git pull origin <branch_name>
```
**Note:** Downloads and merges changes from remote.

### To push changes to remote:
```
git push origin <branch_name>
```
**Note:** Uploads your commits to the remote repository.

---

## 8. Logs and History

### To view commit history:
```
git log
```
**Note:** Shows detailed commit history.

### To view one-line history:
```
git log --oneline
```
**Note:** Shows compact commit history.

### To show details of a commit:
```
git show <commit_hash>
```
**Note:** Displays changes and info for a specific commit.

---

## 9. Stash

### To stash changes:
```
git stash
```
**Note:** Temporarily saves uncommitted changes.

### To list stashes:
```
git stash list
```
**Note:** Displays all stashed changes.

### To apply last stash:
```
git stash pop
```
**Note:** Applies the most recent stash and removes it from stash list.

### To clear all stashes:
```
git stash clear
```
**Note:** Deletes all stashed changes.

---

## 10. Reset and Revert

### To reset to a previous commit (keep changes):
```
git reset <commit_hash>
```
**Note:** Moves HEAD to a commit but keeps changes unstaged.

### To reset to a previous commit (remove changes):
```
git reset --hard <commit_hash>
```
**Note:** Moves HEAD to a commit and deletes all changes.

### To revert a commit:
```
git revert <commit_hash>
```
**Note:** Creates a new commit that undoes changes from a previous commit.

---

## 11. Tags

### To create a tag:
```
git tag <tag_name>
```
**Note:** Creates a tag for a specific commit.

### To list tags:
```
git tag
```
**Note:** Displays all tags.

### To push tags to remote:
```
git push origin --tags
```
**Note:** Uploads all tags to remote.

---

## 12. Ignoring Files

### To create `.gitignore`:
```
touch .gitignore
```
Add file names or patterns to ignore.
**Note:** Files listed in `.gitignore` will not be tracked by Git.

---
