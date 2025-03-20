Use of .gitignore File in Git

The .gitignore file is used to tell Git which files and directories to ignore in a repository. This helps keep the repository clean and prevents unnecessary or sensitive files from being tracked.

Why Use .gitignore?

1. Avoid Tracking Unnecessary Files – Example: Temporary files, logs, compiled code.

2. Improve Performance – Prevent large files from slowing down Git operations.

3. Security – Avoid committing sensitive files like API keys or passwords.

4. Reduce Conflicts – Exclude OS-specific or personal environment files.

Example .gitignore File
```
# Ignore node_modules folder (for Node.js projects)
node_modules/

# Ignore Python compiled files
__pycache__/
*.pyc

# Ignore log files
*.log

# Ignore environment files
.env

# Ignore IDE-specific files
.vscode/
.idea/

# Java  
*.class  
*.jar  
```


How to Use .gitignore?

1. Create a .gitignore file in your project root.

2. Add the files/directories you want to ignore.

3. Save the file and commit it to your repository.
