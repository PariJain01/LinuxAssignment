## 📚 Introduction to Version Control and Git Basics

### 🔄 What is Version Control?

Version control is a system that records changes to a file or set of files over time. It allows multiple people to collaborate, tracks who made what change and when, and lets you roll back to previous versions when needed.

### 🧰 What is Git?

Git is the most widely used version control system. It's free, open-source, and designed to handle everything from small to very large projects with speed and efficiency.

---

## 🛠️ Git Installation and Configuration

### ✅ Step 1: Install Git

#### On Ubuntu/Debian:

```bash
sudo apt update
sudo apt install git
```
#### On Windows:

* Download and install from: [https://git-scm.com](https://git-scm.com)

---

### ✅ Step 2: Configure Git (Only once after install)

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Check config:

```bash
git config --list
```

---

## 💻 Basic Git Commands

### 1. **`git init`**

Initializes a new Git repository in your folder.

```bash
git init
```

---

### 2. **`git add`**

Stages changes (files) for commit.

```bash
git add filename.txt         # Add a specific file
git add .                    # Add all files in the directory
```

---

### 3. **`git commit`**

Records a snapshot of the staged changes.

```bash
git commit -m "Your commit message"
```

---

### 4. **`git push`**

Uploads your local commits to the GitHub repository.

```bash
git push origin main
```

---

### 5. **`git pull`**

Fetches and merges changes from the remote repository.

```bash
git pull origin main
```

---
### ✅ 3. Set Up Remote Repository (Local → GitHub)
Steps Followed:

Created a new repository on GitHub (without initializing README).

Initialized local Git repo and added files.

Connected remote repo:

```bash

git remote add origin https://github.com/username/project.git  
git push -u origin master 
```
Outcome: Code from the local system was successfully pushed to GitHub.

---

### ✅ 4. Merge Types & Branching

Branching is essential for managing multiple features or bug fixes.

Created a new feature branch, committed code, and pushed to GitHub.

Commands Used:

```bash

git checkout -b new-feature  
git add .  
git commit -m "Added new feature"  
git push origin new-feature
```
Merge via Pull Request:
 
Opened a pull request on GitHub and merged into the master branch.

---

### ✅ 5. Undo the Last Commit / Remove Files
Undo Last Commit but Keep Changes:

```bash

git reset --soft HEAD~
```
Undo and Discard Changes:
```bash

git reset --hard HEAD~1
```
Remove Specific File from Repo:
 
```bash

git rm filename  
git commit -m "Removed unwanted file"  
git push
```
Outcome: Gained confidence in rolling back changes and correcting mistakes.

---

### ✅ 6. Merge Conflict Resolution
Steps:

Created two branches and made conflicting edits to the same file.

Attempted a merge, which resulted in a conflict.

Resolved manually in VS Code, then:

``` bash
git add .  
git commit -m "Resolved conflict"  
git push
```
Learning: Understood how to identify conflict markers (<<<<, ====, >>>>) and resolve them effectively.

---

### ✅ 7. Practice: Additional Git Commands
Practiced:

Clone Repositories:

``` bash
git clone https://github.com/user/repo.git
```
View Commit History:

``` bash
git log  
git show HEAD
```
Revert Changes:

```bash
git revert <commit_hash>  # Creates a new commit to undo
```
Outcome: Developed a deeper understanding of Git workflows and gained hands-on experience with version control tools.

---

### ✅ Conclusion
This week’s Linux/Git module provided foundational knowledge crucial for DevOps.

I can now confidently manage repositories, branches, commits, and collaborate using Git.

Looking forward to applying these skills in Docker and Kubernetes modules in the coming weeks.
