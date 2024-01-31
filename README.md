1. git status
2. git add <filename> EX: git add index.html --> this will be added to the staging are.
3. git rm --cached index.html --> if you want to unstaged
4. git add . ---> this will add all the files (this command you can actually know what you are adding to the staging area)
5. git rm -r cached . --> this will unstaged all the files.
6. git add A --> if you want to add everything with downwards and afterwards directory

Configure Git
=============
git config --global user.name "masudbappy"
git config --global user.email "masud.bappy90@gmail.com"
git config --global color.ui auto

Repositories in GIT contain a collection of files of various differenct versions of a project.


7. git show baf55113aa82568cf52216c164538602e444b215  --> show the diff of everything wich is commited.

8. git diff --> to show what i have changed.
9. # Check existing remotes
git remote -v

# If "origin" already exists, you can either update its URL or remove it
git remote set-url origin <new-remote-url>

# OR

git remote remove origin
git remote add origin <new-remote-url>
Branches
========
git branch --> to show local branches
git branch -r --> to show remote branches
git branch -a --> all local and remote branches
git branch feature-a --> create local branch
git checkout feature-a --> this will switch a particular branch
git checkout - "this will checkout to the previous branch"
git checkout -b feature-b --> create branch and checout to that branch
git branch -d feature-a  --> to delete a branch

Rebase:
=======
You have a branch which should checkout from main branch and main branch may have multiple commits. Now in a scenario  the main branch has moved on and you don't have the commits from the main or master branch. So what rebase does, it's going to bring all the changes from whatever branch that you want i am going to bring the changes and the changes will be underneath your new branch. it brings all the commits from master into your branch and i am going to try and apply Your changes on top of it. That's what rebase does.
after applying rebase you need to force push
