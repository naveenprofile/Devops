Git is the free and open-source distributed version control systems that’s responsible for everything GitHub related that happens locally on your computer.

Understanding Version Control

Version control, also known as source control, is the technique of tracking and managing changes to codes and these are the systems that are software tools that enable software teams to manage modifications to source code as time passes.

What is GitHub?

GitHub is a widely-used Free-to-use cloud Storage platform with version control and many other essential features that specifically helps developers to manage and deploy their projects on GitHub.

Benefits of Using Git

History Tracking: 

Git allows you to track every change made in your project, including: who made the change and when it was made.

Collaboration: 

Multiple developers can be able work on the same project at the same time, and Git efficiently manages the merging of changes in code.

Branching and Merging: 

Git enables developers to create branches to work on new features or bug fixes and later merge them back into the main codebase.

Offline Work: 

Git works offline, which means you can commit changes and work on your project even without an internet connection.

Git Configuration & Setup

#git config –global user.name “Your Name”
#git config –global user.email “youremail@example.com”
#git config --list

#git remote add origin https://github.com/naveenprofile/Devops.git
#git remote set-url origin https://<token>2@github.com/naveenprofile/Devops.git
#git remote -v

GitHub -> Settings  -> Developer Settings -> Personal access tokens (classic) - Generate new token

git init - Initializes a new Git repository in the current directory.

git init <directory> - Creates a new Git repository in the specified directory.

git clone <repository_url> - this Clones a repository from a remote server to your local machine.

git clone –branch <branch_name> <repository_url> - Clones a specific branch from a repository.

git add <file> - Adds a specific file to the staging area.

git add . or git add –all	 - Adds all modified and new files to the staging area.

git status	 - Shows the current state of your repository, including tracked and untracked files, modified files, and branch information.

git status –ignored	 - Displays ignored files in addition to the regular status output.

git diff	- Shows the changes between the working directory and the staging area (index).

git diff <commit1> <commit2>	 - Displays the differences between two commits.

git diff –staged or git diff –cached - Displays the changes between the staging area (index) and the last commit.

git diff HEAD - Display the difference between the current directory and the last commit

git commit	- Creates a new commit with the changes in the staging area and opens the default text editor for adding a commit message.

git commit -m “<message>” or git commit –message “<message>”	- Creates a new commit with the changes in the staging area and specifies the commit message inline.

git commit -a or git commit –all	 - Commits all modified and deleted files in the repository without explicitly using git add to stage the changes.


git restore <file>	 - Restores the file in the working directory to its state in the last commit.


git reset <commit>	 - Moves the branch pointer to a specified commit, resetting the staging area and the working directory to match the specified commit.


git reset –soft <commit>	- Moves the branch pointer to a specified commit, preserving the changes in the staging area and the working directory.


git reset –hard <commit> - Moves the branch pointer to a specified commit, discarding all changes in the staging area and the working directory, effectively resetting the repository to the specified commit.


git rm <file>	- Removes a file from both the working directory and the repository, staging the deletion.

git mv	- Moves or renames a file or directory in your Git repository.


Branching and Merging

git branch	 - Lists all branches in the repository.

git branch <branch-name>	- Creates a new branch with the specified name.

git branch -d <branch-name>	 - Deletes the specified branch.

git branch -a - Lists all local and remote branches.

git branch -r	- Lists all remote branches.

git checkout <branch-name>	- Switches to the specified branch.

git checkout -b <new-branch-name>	 - Creates a new branch and switches to it.

git checkout — <file>	- Discards changes made to the specified file and revert it to the version in the last commit.

git merge <branch>	- Merges the specified branch into the current branch.

git log	 - Displays the commit history of the current branch.

git log <branch-Id>	 - Displays the commit history of the specified branch.

git log –follow <file>	 - Displays the commit history of a file, including its renames.

git log –all	 - Displays the commit history of all branches.

git stash	-  Stashes the changes in the working directory, allowing you to switch to a different branch or commit without committing the changes.

git stash list	- Lists all stashes in the repository.

git stash pop	 - Applies and removes the most recent stash from the stash list.

git stash drop	 - Removes the most recent stash from the stash list.

git tag	- Lists all tags in the repository.

git tag <tag-name>	 - Creates a lightweight tag at the current commit.

git tag <tag-name> <commit>	 - Creates a lightweight tag at the specified commit.

git tag -a <tag-name> -m “<message>”	 - Creates an annotated tag at the current commit with a custom message.


Remote Repositories

git fetch	 - Retrieves change from a remote repository, including new branches and commit.

git fetch <remote>	 - Retrieves change from the specified remote repository.

git fetch –prune	- Removes any remote-tracking branches that no longer exist on the remote repository.

git pull	- Fetches changes from the remote repository and merges them into the current branch.

git pull <remote>	 - Fetches changes from the specified remote repository and merges them into the current branch.

git pull –rebase	- Fetches changes from the remote repository and rebases the current branch onto the updated branch.

git push	- Pushes local commits to the remote repository.

git push <remote>	 - Pushes local commits to the specified remote repository.

git push <remote> <branch>	- Pushes local commits to the specified branch of the remote repository.

git push –all - Pushes all branches to the remote repository.

git remote	- Lists all remote repositories.

git remote add <name> <url>	 - Adds a new remote repository with the specified name and URL.





