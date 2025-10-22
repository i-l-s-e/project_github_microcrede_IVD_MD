# this file will be our cheetcheat for the commands
## starting a repository
`git init`: start a new local repository 

`git clone <ssh>`: initiate a link between the remote repository and your computer : automatically create a .git local repository and bridge it to the remote repository.

## commits
`git add file_name`: add the file to the staging area

`git commit -m "meaningful message"`: to save a version of the file on git (.git file in local repository). It should be followed by a meaningful message: 
  - why was the file changed
  - how this addresses the issue
  - effects 
  - limitations of the change
 
 Pressing commit without using -m will open the editor, which allow you to give a meaningful message on multiple lines.
 
 Commit can be used on multiple files that are in the staging area (we can `git add` files without directly `git commit`), to have one unified meaningful message for related changes in different files, so to reduce repetitive messages. 
 
 `git commit --amend`: if your commit has not been pushed yet, this command allow you to edit its message.

`git show <commit ID>` and `git diff <commit ID1 (old)> <commit ID2 (new)>`: show the difference in the files between two different commits

## push and pull
`git remote add origin <ssh>`: create the bridge between my local git repository and the remote github repository 
  
`git push`: to send the local git repository to github, after bridging the two.

`git pull` to retrieve remote repository to local repository (if someone else changed the github repository, *i.e.* update to the software)

## check-up
`git status`: check in which conceptual areas are the files: files have been modified but not staged (located in develop. area and local repo.), staged for commit (in staging area) and untracked (not added to git yet)

`git log -n`: list n last commits done to the project 

## go back
`git revert <commit ID>`: go back to a commit

`git reset --hard <commit ID>`: permanently delete further commits

## branches

`git checkout -b <branch name>`: create a new branch 

`git push -u origin <branch name>`: link the new branch to main

`git merge <branch_name>`

`git stash` and `git stash pop`: temporally save changes in a branch locally w/o needing to add, commit and push

## tags

`git tag <current branch-commit tag>`: to tag the current commit and branch where you are located, will be available on github with its corresponding zip file once pushed. It is used to tag different versions of a project (v1, v1.2 etc). You can add many tag to the same commit.

`git tag <tag> <commit ID>`

`git push --tag` 



