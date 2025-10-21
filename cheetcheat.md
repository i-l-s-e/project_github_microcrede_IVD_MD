# this file will be our cheetcheat for the commands

# Fork and Clone
You can fork a remote repository for which you are not a collaborator directly on the GitHub page of such repo. You will then be able to clone it to your local repository using `git clone <repo link>`on your terminal. 

# Conceptual areas
- developing area: in your computer, the folder where the project is developed
- staging area: place to prepare the commit (transition between develop. area and local repo. via `git add`). it allows to commit file A and B that are related in the project at the same time, as you can wait for file A and B to be in the staging area before commiting. 
- local repository: where the file version is saved on git after `git commit`.

# Managing sensitive files on your local repo
Using `.gitignore` file, you can list the different files of the project that should be ignored by git (*i.e.* not tracked), *e.g.* datasets, intermediate files

This is non-sense !!!!
And this is also non-sense common !!!