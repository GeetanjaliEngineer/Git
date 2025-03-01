# Git Commands Cheat Sheet

A comprehensive list of commonly used Git commands.

## 📌 Table of Contents
1. [Configuration Commands](#configuration-commands)
2. [Repository Commands](#repository-commands)
3. [Staging and Commit Commands](#staging-and-commit-commands)
4. [Branching Commands](#branching-commands)
5. [Remote Repository Commands](#remote-repository-commands)
6. [Undoing Changes](#undoing-changes)
7. [Logs and History](#logs-and-history)
8. [Stashing Commands](#stashing-commands)
9. [Tagging Commands](#tagging-commands)
10. [GitHub Collaboration](#github-collaboration)
11. [Git Workflow Summary](#git-workflow-summary)

---

## 1️⃣ Configuration Commands
```sh
git config --global user.name "Your Name"   # Set username
git config --global user.email "youremail@example.com"   # Set email
git config --global core.editor "code --wait"   # Set default editor
git config --list   # View configuration

2️⃣ Repository Commands
sh
Copy code
git init   # Initialize a new repository
git clone <repo-url>   # Clone an existing repository
3️⃣ Staging and Commit Commands
sh
Copy code
git status   # Check the current status
git add <file>   # Add a file to the staging area
git add .   # Add all changes to the staging area
git commit -m "Commit message"   # Commit changes with a message
git commit --amend -m "New message"   # Amend the last commit
4️⃣ Branching Commands
sh
Copy code
git branch   # List branches
git branch <branch-name>   # Create a new branch
git checkout <branch-name>   # Switch to a branch
git switch <branch-name>   # Another way to switch branches
git checkout -b <branch-name>   # Create and switch to a new branch
git merge <branch-name>   # Merge a branch into the current branch
git branch -d <branch-name>   # Delete a branch
5️⃣ Remote Repository Commands
sh
Copy code
git remote -v   # List remote repositories
git remote add origin <repo-url>   # Add a remote repository
git push -u origin <branch-name>   # Push changes to a remote branch
git pull origin <branch-name>   # Fetch and merge changes from a remote repository
git fetch origin   # Fetch changes without merging
6️⃣ Undoing Changes
sh
Copy code
git reset <file>   # Unstage a file
git reset --hard <commit-hash>   # Reset to a specific commit (deletes changes)
git revert <commit-hash>   # Revert a commit by creating a new commit
git restore <file>   # Discard local changes in a file
7️⃣ Logs and History
sh
Copy code
git log   # View commit history
git log --oneline   # Compact commit history
git diff   # Show unstaged changes
git diff --staged   # Show staged changes
8️⃣ Stashing Commands
sh
Copy code
git stash   # Save changes without committing
git stash list   # Show stashed changes
git stash pop   # Apply the last stashed changes
git stash drop   # Remove the last stashed changes
9️⃣ Tagging Commands
sh
Copy code
git tag   # List all tags
git tag -a v1.0 -m "Version 1.0"   # Create an annotated tag
git push origin --tags   # Push all tags to the remote repository
🔟 GitHub Collaboration
sh
Copy code
git fork   # Copy a repository on GitHub
git clone <forked-repo-url>   # Clone the forked repository
git rebase <branch>   # Reapply commits on top of another base branch
git cherry-pick <commit-hash>   # Apply a specific commit from another branch
✅ Git Workflow Summary
# Step 1: Setup Git
git config --global ...

# Step 2: Initialize or Clone
git init / git clone <repo-url>

# Step 3: Check Status
git status

# Step 4: Add & Commit
git add .  
git commit -m "message"

# Step 5: Create & Switch Branch
git branch new-branch  
git checkout new-branch

# Step 6: Merge Branches
git checkout main  
git merge new-branch

# Step 7: Connect Remote
git remote add origin <repo-url>

# Step 8: Push Changes
git push -u origin main

# Step 9: Pull Changes
git pull origin main

# Step 10: Undo Changes
git reset, git restore, git revert

# Step 11: Stash Changes (If Needed)
git stash

# Step 12: View Logs & Diff
git log  
git diff

# Step 13: Tag a Version
git tag -a v1.0 -m "Version 1.0"
