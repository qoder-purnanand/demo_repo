Certainly! Below is the complete Markdown with all the points (1, 2, 3, etc.) properly formatted as bullet points along with the Git command explanations, in a way that can be directly copied into your README.md file:

markdown
Copy
# Git Commands Documentation

This document contains a collection of commonly used `git` commands, categorized and explained for easy reference.

---

## **Basic Git Commands**

- **1. `git init`**  
  **Description**: Initializes a new Git repository.  
  **Usage**:
  ```bash
  # Initialize a new Git repository
  git init
2. git clone
Description: Clones an existing repository into a new directory.
Usage:

bash
Copy
# Clone an existing repository into a new directory
git clone <repository_url>
3. git status
Description: Displays the state of the working directory and staging area.
Usage:

bash
Copy
# Check the status of your current repository
git status
4. git add
Description: Stages changes (add files to the staging area).
Usage:

bash
Copy
# Stage a single file
git add <file_name>       

# Stage all modified files
git add .                 
5. git commit
Description: Commits the staged changes to the repository.
Usage:

bash
Copy
# Commit changes with a message
git commit -m "Commit message"
6. git push
Description: Pushes local commits to a remote repository.
Usage:

bash
Copy
# Push changes to the remote repository
git push origin <branch_name>
7. git pull
Description: Fetches and merges changes from the remote repository into the current branch.
Usage:

bash
Copy
# Pull changes from the remote repository
git pull origin <branch_name>
Branching Commands
1. git branch
Description: Lists all local branches, or creates a new branch.
Usage:

bash
Copy
# List all branches
git branch                

# Create a new branch
git branch <branch_name>  
2. git checkout
Description: Switches to a different branch or commit.
Usage:

bash
Copy
# Switch to an existing branch
git checkout <branch_name>  

# Create a new branch and switch to it
git checkout -b <branch_name> 
3. git merge
Description: Merges changes from another branch into the current branch.
Usage:

bash
Copy
# Merge changes from another branch into the current branch
git merge <branch_name>
Remote Commands
1. git remote
Description: Manages remote repositories.
Usage:

bash
Copy
# Add a remote repository
git remote add <name> <url>       

# Remove a remote repository
git remote remove <name>          

# View remotes and their URLs
git remote -v                     
2. git fetch
Description: Fetches changes from the remote repository but doesn't merge them.
Usage:

bash
Copy
# Fetch changes from the remote repository
git fetch origin
3. git push --force
Description: Forcefully pushes changes to a remote repository (use with caution).
Usage:

bash
Copy
# Force push changes to the remote repository
git push --force origin <branch_name>
History & Log Commands
1. git log
Description: Shows the commit history.
Usage:

bash
Copy
# Show the commit history
git log              

# Show the log in a simplified format
git log --oneline     
2. git diff
Description: Shows the differences between changes.
Usage:

bash
Copy
# Show differences between the working directory and the index
git diff              

# Show differences between a commit and the working directory
git diff <commit>      
3. git revert
Description: Reverts a specific commit (creates a new commit to undo changes).
Usage:

bash
Copy
# Revert a specific commit
git revert <commit_hash>
Advanced Commands
1. git reset
Description: Resets the current branch to a specific commit.
Usage:

bash
Copy
# Reset to a specific commit and discard all changes
git reset --hard <commit_hash>  

# Reset but keep changes in working directory
git reset <commit_hash>         
2. git rebase
Description: Re-applies commits on top of another base commit.
Usage:

bash
Copy
# Rebase current branch onto another branch
git rebase <branch_name>   
3. git stash
Description: Stashes changes in the working directory to apply later.
Usage:

bash
Copy
# Save changes temporarily
git stash        

# Apply the last stashed changes
git stash apply  
Tagging Commands
1. git tag
Description: Adds a tag to a specific commit.
Usage:

bash
Copy
# Tag the current commit
git tag <tag_name>               

# Create an annotated tag with a message
git tag -a <tag_name> -m "Message" 

# Tag a specific commit
git tag <tag_name> <commit_hash>   
2. git push --tags
Description: Pushes all tags to the remote repository.
Usage:

bash
Copy
# Push all tags to the remote repository
git push --tags
Configuration Commands
1. git config
Description: Configures Git settings (user name, email, etc.).
Usage:

bash
Copy
# Set global username
git config --global user.name "Your Name"    

# Set global email
git config --global user.email "you@example.com" 

# View all Git configurations
git config --list                            
Undoing Changes
1. git checkout -- <file>
Description: Discards changes in a file (reverts to the last commit).
Usage:

bash
Copy
# Discard changes in a file
git checkout -- <file_name>
2. git reset <file>
Description: Unstages a file but keeps the changes in the working directory.
Usage:

bash
Copy
# Unstage a file but keep the changes in the working directory
git reset <file_name>
Miscellaneous Commands
1. git rm
Description: Removes a file from both the working directory and staging area.
Usage:

bash
Copy
# Remove a file from the working directory and staging area
git rm <file_name>
2. git mv
Description: Moves or renames a file.
Usage:

bash
Copy
# Rename or move a file
git mv <old_file_name> <new_file_name>
