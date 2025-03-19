```bash
# Configure Git
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
git config --global --list

# Create a New Repository
git init
git clone https://github.com/username/repository.git

# Checking Repository Status
git status

# Working with Files
git add filename
git add .  # Add all files
git commit -m "Commit message here"
git log

# Branching
git branch new-branch-name
git checkout branch-name
git checkout -b new-branch-name  # Create and switch to a new branch
git branch  # List all branches
git merge branch-name  # Merge a branch into the current branch

# Remote Repositories
git remote add origin https://github.com/username/repository.git
git fetch  # Fetch changes from remote repository
git pull origin branch-name  # Pull changes and merge from remote repository
git push origin branch-name  # Push local changes to remote
git remote -v  # Show current remotes

# Viewing Changes
git diff  # View changes before committing
git show commit-hash  # View changes after committing

# Undoing Changes
git reset filename  # Unstage a file (remove from staging area)
git checkout -- filename  # Undo local changes to a file
git rm --cached filename  # Remove a file from the repository (keep locally)

# Deleting Branches
git branch -d branch-name  # Delete a local branch
git branch -D branch-name  # Force delete a local branch (if not merged)
git push origin --delete branch-name  # Delete a remote branch

# Tagging
git tag v1.0.0  # Create a tag (marking a release)
git push origin --tags  # Push tags to remote repository
```

