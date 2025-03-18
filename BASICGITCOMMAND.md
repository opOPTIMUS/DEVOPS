2. git clone <repository-url>
Description: Creates a local copy of a remote repository.

bash
Copy
git clone https://github.com/username/repository-name.git
3. git status
Description: Displays the state of the working directory and staging area, showing which files are modified, added, or deleted.

bash
Copy
git status
4. git add <file>
Description: Stages a file to be included in the next commit. To stage all modified files, use git add ..

bash
Copy
git add <file-name>
To stage all files:

bash
Copy
git add .
5. git commit -m "commit message"
Description: Commits the staged changes with a descriptive message.

bash
Copy
git commit -m "Your commit message"
6. git log
Description: Shows the commit history for the repository.

bash
Copy
git log
7. git branch
Description: Lists all the branches in the repository. To create a new branch, use git branch <branch-name>.

bash
Copy
git branch
To create a new branch:

bash
Copy
git branch <branch-name>
8. git checkout <branch-name>
Description: Switches to the specified branch.

bash
Copy
git checkout <branch-name>
9. git merge <branch-name>
Description: Merges the changes from the specified branch into the current branch.

bash
Copy
git merge <branch-name>
10. git pull
Description: Fetches the latest changes from the remote repository and merges them into your current branch.

bash
Copy
git pull
11. git push
Description: Pushes your committed changes to the remote repository.

bash
Copy
git push
12. git remote -v
Description: Displays the URLs of remote repositories connected to your local repository.

bash
Copy
git remote -v
13. git reset <file>
Description: Unstages a file, removing it from the staging area.

bash
Copy
git reset <file-name>
14. git diff
Description: Shows the differences between the working directory and the staging area (files that are modified but not yet staged).

bash
Copy
git diff
