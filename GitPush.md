# Git Setup and Push to GitHub

### Follow these steps to install Git, create a file, and push it to your GitHub repository.

---

## Step 1: Install Git

If Git is not already installed on your system, use the following commands:

```bash
sudo yum install git -y
git --version
```

## Step 2: Set Up Your Git Working Directory
Navigate to your desired directory:

```bash
cd ..
```

Switch to root user if needed:

```bash
sudo -i
```

Create a new directory for your project:

```bash
mkdir gitfile
```

Create a new file in the directory:

```bash
touch optimus.html
```

Navigate into the project directory:

```bash
cd gitfile
```

## Step 3: Initialize Git Repository

Initialize a new Git repository:

```bash
git init
```

Check the status of the repository (should show no files yet):

```bash
git status
```

Commit the changes with a message:

```bash
git commit -m "initial commit"
```
View the commit log:

```bash
git log
```

## Step 5: Configure Git User Details

Set your GitHub username (replace opoptimus with your actual GitHub username):

```bash
git config --global user.name "opoptimus"
```

Set your GitHub email (replace with your GitHub email):

```bash
git config --global user.email "your-email@example.com"
```
Verify the Git configuration:

```bash
git config --global --list
```
## Step 6: Add Remote Repository

Add the GitHub remote repository (replace with your actual repository URL):

```bash
git remote add origin https://github.com/opOPTIMUS/DEVOPS.git
```
Push your changes to the remote repository:

```bash
git push -u origin master
```
## Step 7: Create a GitHub Personal Access Token (PAT)

1 Go to GitHub and log in to your account.

2 Click on your profile icon in the top-right corner and go to Settings.

3 Scroll down and click on Developer settings.

4 In the left sidebar, select Personal access tokens under Developer settings.

5 Click Generate new token.

6 Provide a note (e.g., Git operations on my repo) and select repo scope.

7 Click Generate token and copy the token (you won’t be able to see it again).

## Step 8: Use the Personal Access Token (PAT)

1 After running git push, you’ll be prompted for your GitHub username and password.

2 Use your GitHub username as usual.

3 Paste the PAT as the password instead of your GitHub password.

Example:

```rust
Username for 'https://github.com': opoptimus
Password for 'https://opoptimus@github.com': <paste your PAT here>
```

## Step 9: Verify the Push on GitHub

1 After pushing, go to your repository on GitHub (https://github.com/opOPTIMUS/######).

2 Verify that the optimus.html file has been successfully pushed.

3 You may also see a link to create a pull request if needed.


# Final Recap of Commands:
```bash
# Step 1: Install Git
sudo yum install git -y
git --version

# Step 2: Set Up Your Project Directory
mkdir gitfile
cd gitfile

# Step 3: Initialize Git Repository
git init
git status

# Step 4: Add and Commit the File
touch optimus.html
git add optimus.html
git commit -m "initial commit"
git log

# Step 5: Configure User Info
git config --global user.name "opoptimus"
git config --global user.email "your-email@example.com"
git config --global --list

# Step 6: Add Remote Repo and Push
git remote add origin https://github.com/opOPTIMUS/DEVOPS.git
git push -u origin master
```
============================================================================================================================================================

Choosing Between main or master Branch in Git
Background:
master was the default branch name in Git repositories for many years.
main has become the default branch name for new repositories on GitHub since October 2020, as part of efforts to use more inclusive terminology.
Steps to Choose Between main or master:
If you're starting a new repository:

GitHub will use main by default for new repositories.
If you’re creating a repository from scratch on GitHub, the default branch will automatically be main.
