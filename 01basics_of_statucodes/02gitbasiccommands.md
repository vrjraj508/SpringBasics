Here's a summarized list of all the Git commands we’ve discussed so far, along with detailed descriptions and their options:

---

### **1. `git --version`**
- **Description**: Checks the installed Git version on your system.
- **Example**:
  ```bash
  git --version
  ```

---

### **2. `git init`**
- **Description**: Initializes a new Git repository in the current directory. Creates a hidden `.git` folder to track version control.
- **Example**:
  ```bash
  git init
  ```

---

### **3. `git clone <repository-url>`**
- **Description**: Clones an existing repository from a remote URL to your local system.
- **Options**:
  - `--depth 1`: Clones only the latest commit to save time and space.
- **Example**:
  ```bash
  git clone https://github.com/username/repo-name.git
  git clone https://github.com/username/repo-name.git --depth 1
  ```

---

### **4. `git add <file>`**
- **Description**: Stages files for the next commit. Prepares files for tracking by Git.
- **Options**:
  - `.`: Adds all files in the current directory.
  - `<file>`: Adds a specific file.
- **Examples**:
  ```bash
  git add .
  git add file.txt
  ```

---

### **5. `git commit -m "<message>"`**
- **Description**: Records changes to the repository with a descriptive message.
- **Options**:
  - `-m "<message>"`: Adds a commit message.
- **Example**:
  ```bash
  git commit -m "Initial commit"
  ```

---

### **6. `git remote add origin <repository-url>`**
- **Description**: Links a local repository to a remote repository (commonly referred to as "origin").
- **Example**:
  ```bash
  git remote add origin https://github.com/username/repo-name.git
  ```

---

### **7. `git remote -v`**
- **Description**: Displays the current remote repository URLs (fetch and push URLs).
- **Example**:
  ```bash
  git remote -v
  ```

---

### **8. `git remote remove origin`**
- **Description**: Removes the existing remote origin URL from your repository.
- **Example**:
  ```bash
  git remote remove origin
  ```

---

### **9. `git push -u origin <branch>`**
- **Description**: Pushes the local branch to the remote repository for the first time and sets the upstream tracking branch.
- **Options**:
  - `-u`: Sets upstream tracking for the branch.
- **Example**:
  ```bash
  git push -u origin main
  ```

---

### **10. `git push -f origin <branch>`**
- **Description**: Forcefully pushes changes to the remote repository, overwriting the existing content.
- **Options**:
  - `-f`: Force push (use with caution).
- **Example**:
  ```bash
  git push -f origin main
  ```

---

### **11. `git branch -M <branch-name>`**
- **Description**: Renames the current branch to the specified name.
- **Example**:
  ```bash
  git branch -M main
  ```

---

### **12. `git rm -r --cached <file/folder>`**
- **Description**: Unstages a file or folder and stops tracking it in the repository while keeping it in the working directory.
- **Options**:
  - `-r`: Recursively removes files from subdirectories.
  - `--cached`: Removes files from Git tracking only.
- **Examples**:
  ```bash
  git rm -r --cached .
  git rm -r --cached folder-name
  ```

---

### **13. `git status`**
- **Description**: Displays the current status of your repository, including staged, unstaged, and untracked files.
- **Example**:
  ```bash
  git status
  ```

---

### **14. `git log`**
- **Description**: Shows the commit history of the repository.
- **Options**:
  - `--oneline`: Displays a concise version of the commit log.
- **Example**:
  ```bash
  git log
  git log --oneline
  ```

---

### **15. `git pull`**
- **Description**: Fetches updates from the remote repository and merges them into your local branch.
- **Example**:
  ```bash
  git pull origin main
  ```

---

### **16. `git add .gitignore`**
- **Description**: Adds a `.gitignore` file to the repository to exclude specific files/folders from tracking.
- **Example**:
  ```bash
  echo "node_modules/" >> .gitignore
  git add .gitignore
  git commit -m "Add .gitignore"
  git push
  ```

---

### **17. `cp -r <source> <destination>`**
- **Description**: Copies files and folders from a source directory to a destination (used for moving local files into the Git repository).
- **Example**:
  ```bash
  cp -r /path/to/local/files/* .
  ```

---

### **18. `git reset HEAD <file>`**
- **Description**: Unstages a file from the staging area but keeps it in the working directory.
- **Example**:
  ```bash
  git reset HEAD file.txt
  ```

---

These commands cover everything we’ve discussed so far, from initializing a repository to pushing changes, managing remotes, and cleaning up files. Let me know if you need more details about any specific command! 😊