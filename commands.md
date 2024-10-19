
# **Git Commands**

## **Basic Commands**

### **1. `git --help`**  
Displays help information about Git commands and options.

---

### **2. `pwd`**  
Prints the **current working directory** to show your current location in the filesystem.

---

### **3. `ls`**  
Lists **files and directories** in the current directory.

---

### **4. `mkdir <directory-name>`**  
Creates a **new directory**.  
Example:  
```bash
mkdir git-for-devops
```

---

### **5. `cd <directory-name>`**  
Changes the **current directory** to the specified one.  
Example:  
```bash
cd git-for-devops/
```

---

## **Working with Git**

### **6. `git init`**  
Initializes a **new Git repository** in the current directory. This creates a `.git` folder to track changes.

---

### **7. `git status`**  
Displays the **state of the working directory and staging area**, showing which files are modified, staged, or untracked.

---

### **8. `ls -a`**  
Lists **all files and directories**, including **hidden files** (e.g., `.git`).

---

### **9. `vim <file-name>`**  
Opens a file using the **Vim text editor**.  
Example:  
```bash
vim sample-file.txt
```

---

### **10. `cat <file-name>`**  
Displays the **content of a file**.  
Example:  
```bash
cat sample-file.txt
```

---

### **11. `touch <file1> <file2>`**  
Creates **empty files**.  
Example:  
```bash
touch nibba.txt nibbi.txt
```

---

## **Staging and Committing Changes**

### **12. `git add <file-name>`**  
**Stages changes** for the next commit.  
Example:  
```bash
git add nibbi.txt
```

---

### **13. `git rm --cached <file-name>`**  
**Removes a file from the staging area** without deleting it from the working directory.  
Example:  
```bash
git rm --cached nibba.txt
```

---

### **14. `git commit -m "<message>"`**  
Saves the staged changes with a **commit message**.  
Example:  
```bash
git commit -m "Added nibbi"
```

---

### **15. `git config`**  
Displays or modifies **Git configuration** (like username, email, etc.).

---

### **16. `git restore <file-name>`**  
**Discards changes** in the working directory, restoring the file to the latest committed state.

---

### **17. `git restore --staged <file-name>`**  
**Unstages a file**, moving it from the staging area back to the working directory.  
Example:  
```bash
git restore --staged nibbi.txt
```

---

### **18. `git rm <file-name>`**  
**Removes a file** from the working directory and stages the deletion.  
Example:  
```bash
git rm sample-file.txt
```

---

## **Viewing Logs and Branching**

### **19. `git log`**  
Displays the **commit history**.

---

### **20. `git log --oneline`**  
Shows a **condensed version** of the commit history with one line per commit.

---

### **21. `git branch`**  
Lists the **branches** in the repository.

---

### **22. `git checkout -b <branch-name>`**  
**Creates a new branch** and switches to it.  
Example:  
```bash
git checkout -b develop
```

---

### **23. `git checkout <branch-name>`**  
**Switches to an existing branch**.  
Example:  
```bash
git checkout master
```

---

## **History Management**

### **24. `history`**  
Displays the **list of previous commands** executed in the terminal.

---

# **Summary Workflow Example**

Here’s an example of a typical Git workflow using the commands listed above:

1. **Initialize a new repository**:  
   ```bash
   git init
   ```

2. **Create a new file and add it to the staging area**:  
   ```bash
   touch example.txt
   git add example.txt
   ```

3. **Commit the changes with a message**:  
   ```bash
   git commit -m "Initial commit"
   ```

4. **Create and switch to a new branch**:  
   ```bash
   git checkout -b feature-branch
   ```

5. **Make changes, stage, and commit again**:  
   ```bash
   vim example.txt  # Edit the file
   git add example.txt
   git commit -m "Updated example.txt"
   ```

6. **Switch back to the master branch**:  
   ```bash
   git checkout master
   ```

7. **View the commit history**:  
   ```bash
   git log --oneline
   ```
