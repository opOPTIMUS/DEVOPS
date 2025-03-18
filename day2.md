DAY 02 
  
What is Git?
Git is a distributed version control system that tracks code changes and enables collaboration among developers. It allows you to commit, branch, merge, and revert code changes efficiently.

Key Git Concepts
  
Repository (Repo) – A directory containing your project and Git tracking files.
Commit – A snapshot of your project at a specific point in time.
Branch – A separate version of your code for independent development.
Merge – Combining changes from different branches.
Pull & Push – Syncing changes between your local and remote repositories.
Clone & Fork – Copying repositories for collaboration.



How to download and install the git ?  
  
🖥️ Windows Installation
  
Step 1: Download Git
Go to Git's official website.
Click on Windows to download the latest Git for Windows installer.
  
Step 2: Install Git
Run the downloaded .exe file.
Click Next and follow the setup wizard.
Choose Git Bash and Git GUI when prompted.
Select "Use Git from the Windows Command Prompt" (recommended).
Choose OpenSSH as the SSH client (default).
Select "Use the default branch name ‘main’".
Click Install and wait for the process to finish.
  
Step 3: Verify Installation
After installation, open Command Prompt (cmd) or Git Bash and type:
git --version
If Git is installed correctly, you’ll see the version number.
  


  
🐧 Linux Installation
  
Step 1: Install Git Using Terminal
Debian/Ubuntu:
sudo apt update
sudo apt install git -y

Step 2: Verify Installation
git --version
You should see output like git version 2.x.x.
  

Commamds for using git:

1. Check Git Version
git --version

2. to add file in staging area
git add <filename>

3. to verify staging area
git status

4. to commit the file 
git commit -m "msg"

5. to verify commits
git log

6. Configure Git (Only Once)
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"

7. to list the user info
git config --global --list

## Basic Git Commands

Here are some basic Git commands to help you get started:

### 1. `git init`
- Initializes a new Git repository in the current directory.

### 2. `git clone <repository-url>`
- Creates a local copy of a remote repository.

### 3. `git status`
- Shows the current state of the working directory and staging area (modified, added, or deleted files).

### 4. `git add <file>`
- Stages a specific file to be committed. To add all files, use `git add .`.

### 5. `git commit -m "commit message"`
- Commits the staged changes with a descriptive message.

### 6. `git log`
- Displays the commit history for the repository.

### 7. `git branch`
- Lists all branches in the repository. Use `git






  
  
  

  
