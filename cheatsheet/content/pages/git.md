title: Git
slug: Git
category: Git
date: 2021-06-02 10:22
modified: 2017-06-09

#git init

This command turns a directory into an empty Git repository. This is the first step in creating a repository. After running git init, adding and committing files/directories is possible.

#git add

Adds files in the to the staging area for Git. Before a file is available to commit to a repository, the file needs to be added to the Git index (staging area). There are a few different ways to use git add, by adding entire directories, specific files, or all unstaged files.  
***git add < file or directory name >***

#git commit

Record the changes made to the files to a local repository. For easy reference, each commit has a unique ID.

It’s best practice to include a message with each commit explaining the changes made in a commit. Adding a commit message helps to find a particular change or understanding the changes.  
***git commit -m "Commit message in quotes"***

#git status

This command returns the current state of the repository.

git status will return the current working branch. If a file is in the staging area, but not committed, it shows with git status. Or, if there are no changes it’ll return nothing to commit, working directory clean.  

#git config

With Git, there are many configurations and settings possible. git config is how to assign these settings. Two important settings are user user.name and user.email. These values set what email address and name commits will be from on a local computer. With git config, a --global flag is used to write the settings to all repositories on a computer. Without a --global flag settings will only apply to the current repository that you are currently in.  
***git config <setting> <command>***  
  ***git config --global user.email "my@emailaddress.com"***  
  ***git config --global user.name "Brian Kerr"***  

#git branch

To determine what branch the local repository is on, add a new branch, or delete a branch.  

* Create a new branch  
***git branch <branch_name>***

* List all remote or local branches  
***git branch -a***

* Delete a branch  
***git branch -d <branch_name>***

#git checkout

To start working in a different branch, use git checkout to switch branches.  

* Checkout an existing branch  
***git checkout <branch_name>***

* Checkout and create a new branch with that name  
***git checkout -b <new_branch>***

#git merge

Integrate branches together. git merge combines the changes from one branch to another branch. For example, merge the changes made in a staging branch into the stable branch.  
***git merge <branch_name>***  

#git remote

To connect a local repository with a remote repository. A remote repository can have a name set to avoid having to remember the URL of the repository.  

* Add remote repository  
***git remote <command> <remote_name> <remote_URL>***

* List named remote repositories  
***git remote -v***  

#git clone

To create a local working copy of an existing remote repository, use git clone to copy and download the repository to a computer. Cloning is the equivalent of git init when working with a remote repository. Git will create a directory locally with all files and repository history.  
***git clone <remote_URL>***

#git pull

To get the latest version of a repository run git pull. This pulls the changes from the remote repository to the local computer.  
***git pull <branch_name> <remote_URL/remote_name>***

#git push

Sends local commits to the remote repository. git push requires two parameters: the remote repository and the branch that the push is for.  
***git push <remote_URL/remote_name> <branch>***   
Push all local branches to remote repository - ***git push —all***  

#git log

To show the chronological commit history for a repository. This helps give context and history for a repository. git log is available immediately on a recently cloned repository to see history.  
