# GIT CHEAT SHEET  

## Create a new repository on the command line  
` echo "# <repo name>" >> README.md`  
` git init`  
` git add README.md`  
` git commit -m "init commit"`  
` git branch -M master`  
` git remote add origin https://github.com/ahonculada/<repo name>`  
` git push -u origin master`  

## Push an existing repository from the command line  
` git remote add origin https://github.com/<user name>/<repo name>`  
` git commit -m "init commit"`  
` git branch -M master`  
` git remote add origin https://github.com/<user name>/<repo name>.git`  
` git push -u origin master`  

## Push an existing repository from the command line  
` git remote add origin https://github.com/<user name>/<repo name>.git`  
` git branch -M master`  
` push -u origin master`  

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

