
# Cheat Sheet #

## Terms ##

* Directory -> Folder
* Terminal or Command Line -> Interface for text commands
* CLI -> Command line interface
* cd -> Change directory
* Code Editor -> Word processor for writing code
* Repository -> Project, or the folder/place where your project is kept
* GitHub -> A website to store your repositories online

## Git Commands ##

All commands are to be used inside a Terminal or Bash.

### General Commands ###

* git version -> In order to check current version of Git
* git clone -> Bring a repository that is hosted somewhere like GitHub into a folder on your local machine
* git status -> Shows all the files which were created, edited or deleted, but haven't been saved to a commit yet
* git add -> Track your files and changes in Git
* git commit -> Save your files in Git
* git push -> Upload Git commits to a remote app, like GitHub
* git pull -> Download changed from repote repo to your local machine, the opposite from push

### Creating a repository on local machine and then uploading it to GitHub ###

* git init -> Initialize a Git repository - make the folder you are in a Git repository
* git remote add origin ```URL``` -> In order to push into a repository made on local machine (wasn't pulled from GitHub). Make sure a GitHub repository with the same name was created
* git remote -v -> Shows any remote repositories we have connected to the local repository

### Branch Commands ###

* git branch -> Shows all current branches. The branch with the ```*``` is the current branch
  * You can delete a branch with the flag ```-d``` like so ```git branch -d BRANCH NAME```
* git checkout ```BRANCH NAME``` -> Used to switch between branches
* git diff ```BRANCH NAME``` -> Compares the differences between the current selected branch and the ```BRANCH NAME``` entered
* git merge ```BRANCH NAME``` -> Merges the ```main``` branch and the ```BRANCH NAME``` entered
  * It's best practice to push the branch to GitHub and merge in GitHub rather than merging the different branches on your local machine so others may review your changes

### Undoing Git ###

* git reset ```FILE NAME``` -> Unstages changes (works like Ctrl + Z)
  * ```FILE NAME``` is optional
  * In order to undo a commit, you need to type ```HEAD~1``` as ```FILE NAME```
  * When using ```git log``` you can enter the commit hash as ```FILE NAME``` and reset to a specific point
  * You can use the ```--hard``` flag in order to not only unstage but undo changes in the files (Actually Ctrl + Z the commit history as well as the code itself)
* git log -> Shows a log of entire commit history

### Commands' Syntax ###

* git clone ```URL```
* git add ```FILE NAME``` 
  * Type ```.``` as ```FILE NAME``` in order to select all files
* git commit -m ```"TITLE TEXT"``` -m ```"DESCRIPTION TEXT"```
 * When writing the text, make sure to wrap with double ```"```
* git push ```origin``` ```main```
  * ```origin``` is the location of our Git repository
  * ```main``` is the branch we want to push into. If main doesn't work, try typing ```master``` instead
  * You are able to write ```git push -u origin main``` in order to set the main branch as default. After that you will be able to type only ```git push```
* git checkout ```-b``` ```BRANCH NAME```
  * ```-b``` in order to create a new branch
