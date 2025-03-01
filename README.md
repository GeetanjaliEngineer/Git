
# Git Commands  
______________________________
 Using Git commands for version control and collaboration on GitHub.

## 📌 1. Configuration Commands
```sh
git config --global user.name "Your Name"   # Set the global username
git config --global user.email "youremail@example.com"   # Set the global email
git config --global core.editor "code --wait"   # Set default text editor
git config --list   # View current Git configuration
```

## 📌 2. Initialize or Clone Repository
```sh
git init   # Initialize a new Git repository
git clone <repo-url>   # Clone an existing repository
```

## 📌 3. Check Repository Status
```sh
git status   # Check the current status of the working directory
```

## 📌 4. Staging and Committing Changes
```sh
git add <file>   # Add a specific file to the staging area
git add .   # Add all modified files to the staging area
git commit -m "Commit message"   # Commit changes with a message
git commit --amend -m "New commit message"   # Modify the last commit message
```

## 📌 5. Branching
```sh
git branch   # List all local branches
git branch <branch-name>   # Create a new branch
git checkout <branch-name>   # Switch to an existing branch
git switch <branch-name>   # Alternative way to switch branches
git checkout -b <branch-name>   # Create and switch to a new branch
git merge <branch-name>   # Merge a branch into the current branch
git branch -d <branch-name>   # Delete a branch
```

## 📌 6. Remote Repository Management
```sh
git remote -v   # Show all remote repositories
git remote add origin <repo-url>   # Add a new remote repository
git push -u origin <branch-name>   # Push changes to the remote repository
git pull origin <branch-name>   # Fetch and merge changes from the remote repository
git fetch origin   # Fetch remote changes without merging
```

## 📌 7. Undoing Changes
```sh
git reset <file>   # Unstage a file (keep changes)
git reset --hard <commit-hash>   # Reset to a specific commit (deletes changes)
git revert <commit-hash>   # Revert a commit by creating a new commit
git restore <file>   # Discard local changes in a file
```

## 📌 8. Viewing Logs and History
```sh
git log   # View commit history
git log --oneline   # Compact commit history (one commit per line)
git diff   # Show unstaged changes
git diff --staged   # Show staged changes
```

## 📌 9. Stashing Changes
```sh
git stash   # Save changes without committing
git stash list   # View the list of stashed changes
git stash pop   # Apply the last stashed changes
git stash drop   # Remove the last stashed changes
```

## 📌 10. Tagging Versions
```sh
git tag   # List all tags
git tag -a v1.0 -m "Version 1.0"   # Create an annotated tag
git push origin --tags   # Push all tags to the remote repository
```

## 📌 11. GitHub Collaboration
```sh
git fork   # Copy a repository on GitHub
git clone <forked-repo-url>   # Clone the forked repository
git rebase <branch>   # Reapply commits on top of another base branch
git cherry-pick <commit-hash>   # Apply a specific commit from another branch
```

## 📌 12. Full Git Workflow
```sh
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
```

## 📖 Additional Resources
- 🔗 [Official Git Documentation](https://git-scm.com/doc)  
- 🔗 [GitHub Docs](https://docs.github.com/en/get-started/using-git)  

---
