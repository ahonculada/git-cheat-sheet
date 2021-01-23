# GIT CHEAT SHEET  

## Create a new repository on the command line  
` echo "# <repo name>" >> README.md`  
` git init`  
` git add README.md`  
` git commit -m "init commit"`  
` git branch -M master`  
` git remote add origin https://github.com/<user name>/<repo name>.git`  
` git push -u origin master`  

## Push an existing repository from the command line  
` git remote add origin https://github.com/<user name>/<repo name>.git`  
` git branch -M master`  
` git push -u origin master`  

## Configure Tooling   
Configure user information for all local repositories  
> `$ git config --global user.name "[name]"`  
> Sets the name you want attached to your commit transactions  

> `$ git config --global user.email "[email address]"`  
> Sets the email you want attached to your commit transactions  

> `$ git config --global color.ui auto`  
> Enables helpful colorization of command line output  

> `$ git config credential.helper store`  
> Set your credentials so you do not have to retype before 'git push'  

## Create Repositories  
Start a new respository or obtain one from an existing URL  
> `$ git init [project-name]`  
> Creates a new local repository with the specified name  

> `$ git clone [url]`  
> Downloads a project and its entire version history  

## Make Changes  
Review edits and craft a commit transation  
> `$ git status`  
> Lists all new or modified files to be committed  

> `$ git diff`  
> Shows file differences not yet staged  

> `$ git add [file]`  
> Snapshots the file in preparation for versioning  

> `$ git diff --staged`  
> Shows file differences between staging and the last file version  

> `$ git reset [file]`  
> Unstages the file, but presrve its contents  

> `$ git commit -m "[descriptive message]"`  
> Records file snapshots permanently in version history  

## Group Changes  
Name a series of commits and combine completed efforts  
> `$ git branch`  
> Lists all local branches in the current repository  

> `$ git branch [branch-name]`  
> Creates a new branch  

> `$ git checkout [branch-name]`  
> Switches to the specified branch's history into the current branch  

> `$ git merge [branch]`  
> Combines the specified branch's history into the current branch  

> `$ git branch -d [branch-name]`  
> Deletes the specified branch  

## Refactor Filenames  
Relocate and remove versioned files  
> `$ git rm [file]`  
> Deletes the file from the working directory and stages the deletion  

> `$ git rm --cached [file]`  
> Removes the file from the version control but preserves the file locally  

> `$ git mv [file-original] [file-renamed]`  
> Changes the file name and prepares it for commit  

## Supress Tracking  
Exclude temporary files and paths  
> `*.log`  
> `build/`  
> `temp-*`  

A text file names .gitignore supresses accidental versioning of  
files and paths matching the specified patterns  

> `$ git ls-files --other --ignored --exclude-standard`  
Lists all ignored files in this project  

## Save Fragments  
Shelve and restore incomplete changes  
> `$ git stash`  
Temporarily stores all modified tracked files  

> `$ git stash pop`  
> Restores the most recently stashed files  

> `$ git stash list`  
> Lists all stashed changesets  

> `$ git stash drop`  
> Discards the most recently stashed changeset  

## Review History  
Browse and inspect the evolution of project files  
> `$ git log`  
> Lists version history for the current branch  

> `$ git log -follow [file]`  
> Lists version hisotry for a file, including renames  

> `$ git diff [first-branch]...[second-branch]`  
> Shows content differences between two branches  

> `$ git show [commit]`  
> Outputs metadata and content changes of the specified commit  

## Redo Commits  
Erase mistakes and craft replacement history  
> `$ git reset [commit]`  
> Undoes all commits after [commit], preserving changes locally

> `$ git reset --hard [commit]`  
> Discards all hisotry and changes back to the specified commit  

## Synchronize Changes  
Registar a repository bookmark and exhange version history  
> `$ git fetch [bookmark]`  
> Downloads all history from the repository bookmark  

> `$ git merge [bookmark]/[branch]`   
> Combines bookmark's branch into current local branch  

> `$ git push [alias] [branch]`  
> Uploads all local branch commits to GitHub  

> `$ git pull`  
> Downloads bookmark hisotry and incorporates changes  




