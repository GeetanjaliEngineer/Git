# Git
 **Git Commands **

1. Configuration Commands

git config --global user.name "Your Name" → Set username
git config --global user.email "youremail@example.com" → Set email
git config --global core.editor "code --wait" → Set default editor
git config --list → View configuration

3. Repository Commands
git init → Initialize a new repository
git clone <repo-url> → Clone an existing repository

4. Staging and Commit Commands
git status → Check the current status
git add <file> → Add a file to the staging area
git add . → Add all changes to the staging area
git commit -m "Commit message" → Commit changes with a message
git commit --amend -m "New message" → Amend the last commit

5. Branching Commands
git branch → List branches
git branch <branch-name> → Create a new branch
git checkout <branch-name> → Switch to a branch
git switch <branch-name> → Another way to switch branches
git checkout -b <branch-name> → Create and switch to a new branch
git merge <branch-name> → Merge a branch into the current branch
git branch -d <branch-name> → Delete a branch

6. Remote Repository Commands
git remote -v → List remote repositories
git remote add origin <repo-url> → Add a remote repository
git push -u origin <branch-name> → Push changes to a remote branch
git pull origin <branch-name> → Fetch and merge changes from a remote repository
git fetch origin → Fetch changes without merging

7. Undoing Changes
git reset <file> → Unstage a file
git reset --hard <commit-hash> → Reset to a specific commit (deletes changes)
git revert <commit-hash> → Revert a commit by creating a new commit
git restore <file> → Discard local changes in a file

8. Logs and History
git log → View commit history
git log --oneline → Compact commit history
git diff → Show unstaged changes
git diff --staged → Show staged changes

9. Stashing Commands
git stash → Save changes without committing
git stash list → Show stashed changes
git stash pop → Apply the last stashed changes
git stash drop → Remove the last stashed changes

10. Tagging Commands
git tag → List all tags
git tag -a v1.0 -m "Version 1.0" → Create an annotated tag
git push origin --tags → Push all tags to the remote repository

11. GitHub Collaboration
git fork → Copy a repository on GitHub
git clone <forked-repo-url> → Clone the forked repository
git rebase <branch> → Reapply commits on top of another base branch
git cherry-pick <commit-hash> → Apply a specific commit from another branch


Final Summary of Git Workflow

Setup Git → git config --global ...
Initialize or Clone → git init / git clone
Check Status → git status
Add & Commit → git add . → git commit -m "message"
Create & Switch Branch → git branch new-branch → git checkout new-branch
Merge Branches → git checkout main → git merge new-branch
Connect Remote → git remote add origin <repo-url>
Push Changes → git push -u origin main
Pull Changes → git pull origin main
Undo Changes → git reset, git restore, git revert
Stash Changes (If Needed) → git stash
View Logs & Diff → git log, git diff
Tag a Version → git tag -a v1.0 -m "Version 1.0"
