# this file will be our cheetcheat for the commands
`git init`: start a new local repository 

`git add file_name`: add the file to the stagin area

`git commit -m "meaningful message"`: to save a version of the file on git (.git file in local repository). It should be followed by a meaningful message: 
  - why was the file changed
  - how this addresses the issue
  - effects 
  - limitations of the change
 
 Pressing commit without using -m will open the editor, which allow you to give a meaningful message on multiple lines.
 
 Commit can be used on multiple files that are in the staging area (we can `git add` files without directly `git commit`), to have one unified meaningful message for related changes in different files, so to reduce repetitive messages. 
 
 `git commit --amend`: if your commit has not been pushed yet, this command allow you to edit its message.

`git status`: chcek in which conceptual areas are the files: files have been modified but not staged (located in develop. area and local repo.), staged for commit (in staging area) and untracked (not added to git yet)

`git log -n`: list n last commits done to the project 






