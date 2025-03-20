1. Git Setup & Configuration
```
git config --global user.name "Your Name"    # Set your Git username
git config --global user.email "your@email.com"  # Set your Git email
git config --list    # View current Git configurations
```
2. Initializing & Cloning a Repository
```
git init   # Initialize a new Git repository
git clone <repo_url>   # Clone an existing repository
```
3. Checking the Status & Tracking Changes
```
git status   # Show the status of files in the repo
git add <file>   # Add a specific file to staging
git add .   # Add all modified files to staging
git reset <file>   # Unstage a file (remove from staging)
```
4. Committing & Viewing History
```
git commit -m "Your commit message"   # Commit staged changes
git commit -am "Your commit message"   # Add & commit changes in one step
git log   # Show commit history
git log --oneline --graph --all   # Compact commit history
```

🔄 Working with Remote Repositories

Commands to push, pull, and fetch updates from a remote repository.

5. Connecting & Updating Remote Repos
```
git remote add origin <repo_url>   # Connect to a remote repository
git remote -v   # View remote repository details
git fetch origin   # Get the latest changes from remote (does not merge)
git pull origin main   # Fetch & merge latest changes from main branch
```
6. Pushing Changes to Remote
```
git push origin main   # Push local commits to remote main branch
git push -u origin main   # Push and set upstream tracking for the branch
```

🌿 Branching & Merging

7. Working with Branches
```
git branch   # List all branches
git branch <branch_name>   # Create a new branch
git checkout <branch_name>   # Switch to a different branch
git checkout -b <branch_name>   # Create and switch to a new branch
git branch -d <branch_name>   # Delete a branch (merged)
git branch -D <branch_name>   # Force delete a branch (even if not merged)
```
8. Merging Branches
```
git merge <branch_name>   # Merge another branch into the current branch
git merge --no-ff <branch_name>   # Merge with a commit history
```

🚀 Advanced Git Commands

9. Undoing & Reverting Changes
```
git checkout -- <file>   # Discard changes in a file
git reset HEAD <file>   # Unstage a file
git reset --soft HEAD~1   # Undo last commit but keep changes staged
git reset --hard HEAD~1   # Undo last commit and discard changes
git revert <commit_hash>   # Create a new commit to undo a previous commit
```
10. Stashing Changes (Temporary Save)
```
git stash   # Stash changes for later
git stash list   # Show all stashed changes
git stash pop   # Apply the most recent stash and remove it
git stash apply   # Apply the most recent stash but keep it
git stash drop   # Remove the most recent stash
```
11. Handling Merge Conflicts
```
git merge <branch_name>   # Attempt to merge (may cause conflicts)
# Resolve conflicts manually, then:
git add <file>   # Mark conflict as resolved
git commit -m "Resolved merge conflict"   # Commit resolved conflict
```

💡 Additional Useful Commands

12. Tagging Releases
```
git tag <tag_name>   # Create a tag
git tag   # List all tags
git show <tag_name>   # Show details of a tag
git push origin <tag_name>   # Push a tag to remote
```
13. Viewing Differences
```
git diff   # Show unstaged differences
git diff --staged   # Show staged differences
git diff <branch1> <branch2>   # Show differences between branches
```
14. Cleaning Untracked Files
```
git clean -n   # Show untracked files that will be removed
git clean -f   # Force delete untracked files
```

🔄 Git Rebase & Cherry-Pick

Advanced commands to manage commits efficiently.

15. Rebasing Commits
```
git rebase <branch_name>   # Reapply commits from one branch onto another
git rebase -i HEAD~3   # Interactive rebase for last 3 commits
```
16. Cherry-Picking Specific Commits
```
git cherry-pick <commit_hash>   # Apply a specific commit to another branch
```

🎯 Git Shortcuts & Aliases

Speed up your workflow with Git aliases.
```
git config --global alias.st "status"
git config --global alias.cm "commit -m"
git config --global alias.br "branch"
git config --global alias.co "checkout"
git config --global alias.lg "log --oneline --graph --all"
```

🔥 Summary 

Command	Description:

git init:	Initialize a repository

git clone <repo_url>:	Clone a repository

git status:	Check current repo status

git add <file>:	Stage a file

git commit -m "msg":	Commit changes

git log:	View commit history

git branch <name>:	Create a new branch

git checkout <branch>:	Switch branches

git merge <branch>:	Merge a branch

git pull origin <branch>:	Fetch & merge changes

git push origin <branch>:	Push changes to remote

git reset --hard HEAD~1:	Undo last commit (permanently)

git stash:	Temporarily save changes

git rebase <branch>:	Move commits to a different base

git cherry-pick <commit>:	Apply a specific commit


