# Basic Commands

`git add`  <file>
The changes in this file go from your local folder to the staged area, which is one step before committing the changes to your local remote repository

`git commit -m "message"`
with this command the changes go from the staged area to the local repository (note: the local repository is captured in .git file in the folder)
`git commit`
you will get a message that no commit can be done if you don't specify a message, therefore an editor will open to add a message to the commit

`git status`
this gives you the status of your changes, which ones are not yet committed, which ones are not yet added or are completely new files 

`git log`
this gives you the history of your timeline
options: --help, --abbrev (smaller ids), -n number (limits the. number of commits to go back)
press q for quit, to go back to your terminal

`git diff commit1 commit2`
gives you a comparison between the 2 commits, note oldest file first and newest file after

`git show commit1 commit2`
shows you both commits so that you can see more information but the changes are separately presented and not line by line

`git remote add origin` <adress>
create the bridge between local repository and github repository, copy the adress from your github page after you created a new repository, the name of the bridge is origin

`git push`
to get your timeline and changes to the repository of github

`git push --set-upstream origin main`
to set the push for the first time

`git pull` 
to get the lastest update from github

`git revert`
get to your previous git if you don`t want the last commit
e.g if you made a mistake, but commited that mistake, you can git revert, and then go back to the previous version, if you then still want to go back further then you can revert once more, note that it does keep the history of the revert commits, every revert is a new commit

`git reset`
erasing all your commits, note: this mostly not prefered as this erases your history

`git clone`
it will recover the full project in case you lost the folder locally
or when you start locally from scratch 

`git branch` <new branch>
to create a separate branch

`git branch -a`
list branches that exists, with the -a option you will see which branches are in the remote area

`git checkout`
to checkout the branch you would like to adjust

`git checkout -b <new name>`
this is to create a new branch and checkout immediately in one step

`git tag`
tags the current commit

`git tag <name> <commitID>`
tag a previous commit