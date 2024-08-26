# Git-Github-Tutorial

Day-1 :

What is GIT?

Git has multiple full forms but I will go with the standard "Global Information Tracker" which is a "Version Control System" used to manage and track the versions of our code locally. Typically we would not start a task and complete it within a day, it takes days or weeks to complete. So, to locally manage our code or to maintain each version of our code we use GIT.

GIT ----> Local source code management

Versions ----> Checkpoints for our code, like saving the progress of games played in video games, we use GIT for code progress and management.

GIT was founded by Linus Torvalds, the creator of Linux in 2005.


Day-2:

What is GitHub?

GitHub is a central repository for all the repos and commits you tend to do. GitHub is a cloud version of GIT with UI features, git manages the code locally and GitHub is a cloud tool that allows you to manage, share and collaborate code publically.

GitHub ----> web-based platform for version control and collaboration

GitHub was founded by Chris Wanstrath, P. J. Hyett, Tom Preston-Werner, and Scott Chacon in the year 2007.

Day-3:

Installing Git

Before you start using Git, you have to make it available on your computer. Even if it’s already installed, it’s probably a good idea to update to the latest version. You can either install it as a package or via another installer, or download the source code and compile it yourself.

Installing on Linux:

$ sudo dnf install git-all

If you’re on a Debian-based distribution, such as Ubuntu, try apt:
  $ sudo apt install git-all

Installing on Windows:

Visit this link :- https://git-scm.com/download/win

Download either 32-bit / 64-bit based on your system requirements.

Commands:


### **1. Beginner Commands**

- **`git init`**  
  Initializes a new Git repository in your project directory.
  ```bash
  git init
  ```

- **`git clone`**  
  Copies an existing Git repository to your local machine.
  ```bash
  git clone <repository_url>
  ```

- **`git status`**  
  Shows the status of the working directory and staging area (modified, added, deleted files).
  ```bash
  git status
  ```

- **`git add`**  
  Adds files to the staging area (preparing them for commit).
  ```bash
  git add <file_name>
  ```
  Add all files:
  ```bash
  git add .
  ```

- **`git commit`**  
  Records changes to the repository with a message.
  ```bash
  git commit -m "your commit message"
  ```

- **`git log`**  
  Displays a log of all commits in your repository.
  ```bash
  git log
  ```

- **`git branch`**  
  Lists all branches in your repository.
  ```bash
  git branch
  ```
  Create a new branch:
  ```bash
  git branch <branch_name>
  ```

- **`git checkout`**  
  Switches to another branch.
  ```bash
  git checkout <branch_name>
  ```
  Create and switch to a new branch:
  ```bash
  git checkout -b <new_branch_name>
  ```

- **`git merge`**  
  Merges changes from one branch into the current branch.
  ```bash
  git merge <branch_name>
  ```

- **`git remote add`**  
  Connects your local repository to a remote server.
  ```bash
  git remote add origin <repository_url>
  ```

- **`git push`**  
  Pushes committed changes from your local repository to a remote repository.
  ```bash
  git push origin <branch_name>
  ```

- **`git pull`**  
  Fetches and merges changes from a remote repository into your local repository.
  ```bash
  git pull origin <branch_name>
  ```

---

### **2. Intermediate Commands**

- **`git fetch`**  
  Retrieves updates from a remote repository without merging them into your working directory.
  ```bash
  git fetch origin
  ```

- **`git rebase`**  
  Reapplies commits on top of another base tip (useful for linearizing commit history).
  ```bash
  git rebase <branch_name>
  ```

- **`git stash`**  
  Temporarily saves changes that are not ready to be committed.
  ```bash
  git stash
  ```
  Apply the stashed changes:
  ```bash
  git stash apply
  ```

- **`git diff`**  
  Shows the differences between files in the working directory and the staging area.
  ```bash
  git diff
  ```

- **`git reset`**  
  Unstages changes (reverts files to previous states).
  ```bash
  git reset <file_name>
  ```
  Reset to a specific commit:
  ```bash
  git reset --hard <commit_id>
  ```

- **`git tag`**  
  Creates a tag for a specific commit (often used for versioning).
  ```bash
  git tag v1.0.0
  ```
  Push tags to a remote repository:
  ```bash
  git push origin --tags
  ```

---

### **3. Advanced Commands**

- **`git cherry-pick`**  
  Applies a specific commit from one branch into another.
  ```bash
  git cherry-pick <commit_id>
  ```

- **`git revert`**  
  Creates a new commit that undoes the changes of a previous commit.
  ```bash
  git revert <commit_id>
  ```

- **`git reflog`**  
  Shows a log of all references, including HEAD changes.
  ```bash
  git reflog
  ```

- **`git blame`**  
  Shows what revision and author last modified each line of a file.
  ```bash
  git blame <file_name>
  ```

- **`git submodule`**  
  Manages repositories inside other repositories.
  ```bash
  git submodule add <repository_url>
  ```

- **`git bisect`**  
  Helps find the commit that introduced a bug by performing a binary search through your commit history.
  ```bash
  git bisect start
  git bisect bad
  git bisect good <commit_id>
  ```

- **`git clean`**  
  Removes untracked files from the working directory.
  ```bash
  git clean -f
  ```

- **`git config`**  
  Configures Git settings, such as username and email.
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "your.email@example.com"
  ```

- **`git archive`**  
  Creates a zip or tar archive of your project.
  ```bash
  git archive --format=zip HEAD > archive.zip
  ```

- **`git hook`**  
  Manages client-side hooks (automate tasks like pre-commit, post-commit).
  Hooks are located in `.git/hooks/`.

