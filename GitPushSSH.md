# Step-by-Step Guide (with additional Git log)

Generate SSH Key Pair (with default options)

Open your terminal.

Run the following command to generate a new SSH key:
```bash
ssh-keygen
```

When prompted to "Enter file in which to save the key," press Enter to accept the default location (/home/your-user/.ssh/id_rsa).
You'll then be prompted for a passphrase. You can either set one or leave it empty.
This will generate two files: id_rsa (private key) and id_rsa.pub (public key).

## Verify SSH Key Location

List all files in the .ssh directory to ensure the keys were created:
```bash
ls -a ~/.ssh
```

You should see both id_rsa (private key) and id_rsa.pub (public key) listed.

## Copy the Public Key

Display the contents of the public key (id_rsa.pub) to copy it:

```bash
cat ~/.ssh/id_rsa.pub
```

This will print the public key on your terminal. Copy the entire output.

## Add SSH Key to GitHub

Go to GitHub and log in to your account.
In the upper-right corner, click on your profile picture and select Settings.
On the left sidebar, select SSH and GPG keys.
Click on New SSH Key.
Give the key a descriptive title (e.g., "Server SSH Key").
Paste the copied public key into the Key field.
Click Add SSH Key.

Clone the GitHub Repository

Copy the SSH URL of the repository you want to clone. It will look like this:

```scss
git@github.com:username/repository.git
```

Clone the repository to your local machine (or server) using this command:

```bash
git clone git@github.com:username/repository.git
```
## Navigate to the Repository

Change into the directory of the cloned repository:

```bash
cd repository
```
## Create a New File

Use the touch command to create a new .txt file or shell script (.sh file). For example:
```bash
touch script.sh
```
## Add, Commit, and Push the File

Add the newly created file to the staging area:
```bash
git add script.sh
```
Commit the changes with a message:

```bash
git commit -m "Add script.sh"
```

Push the changes to GitHub:

```bash
git push
```

Check Commit History with git log
After pushing your changes, you can use git log to check the commit history and confirm that your commit is present:

```bash
git log
```

This will show the commit history in reverse chronological order. You'll see the commit message you added ("Add script.sh") along with the commit hash, author, and timestamp.

To quit the git log view, press q.

Additional Commands for Status Check
Check Current Status of the Repository: If you want to see the status of your repository (untracked files, changes to be committed, etc.), you can use:

```bash
git status
```

View Detailed Commit Log: If you want more detailed information, including the changes in each commit, you can use:

```bash
git log --stat
```
Summary of Commands

```bash
# Step 1: Generate SSH key pair (default options)
ssh-keygen

# Step 2: Verify SSH keys are present
ls -a ~/.ssh

# Step 3: Copy the public key
cat ~/.ssh/id_rsa.pub

# Step 4: Add the SSH key to GitHub via the GitHub interface

# Step 5: Clone the repository
git clone git@github.com:username/repository.git

# Step 6: Navigate to the repository
cd repository

# Step 7: Create a new file
touch script.sh

# Step 8: Add, commit, and push the file
git add script.sh
git commit -m "Add script.sh"
git push

# Step 9: Check commit history
git log

# Additional: Check current status of the repository
git status

# Additional: View detailed commit history
git log --stat
Using the git log command allows you to confirm that your changes have been committed and pushed to GitHub successfully.
