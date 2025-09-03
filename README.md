# GOPI_MAIN
First repo
<br>
Author- Gill Saab


Configuring Git

git config --global user.name "MY NAME"
git config --global user.email "someone@email.com"
git config --list

Clone & Status

Clone - Cloning a repository on our local machine
git clone<-some link->

Status - Displays the state of the code
git status

   untracked : new files that git doesn't yet track

   modified : changed

   staged : file is ready to be committed

   unmodified: unchanged


change/modified    :-> add(staged) -> commit(unchanged)
newfile(untracked) 

      Add & Commit :-
add -> adds new or changed files in your working directory to the Git Staging area.  git add <-file name-> or git add .(for more files at once)

commit -> it is the record of change
git commit -m "Some Message"

     Push Command :-
push -> upload local repo content to remote repo
git push origin main  or  git push origin -u main

  Init Command :-

init -> used to create a new git repo
   git init
   git remote add origin <-link->
   git remote -v  (to verify remote)
   git branch  (to check branch)
   git branch -M main  ( to rename branch)
   git push origin main

  WorkFlow :-
Local Git: Github repo -> clone -> changes -> add -> commit -> push

   Branch Commands :-

git branch  (to check branch)
git branch -M main  (to rename branch)
git checkout <- branch name->  (to navigate)
git checkout -b <-new branch name-> (to create new branch)

git branch -d <-branch name->  (to delete branch)


   Merging Code:-
way 1:  
git diff <-branch name->  (to compare branches,comments,file & more)
git merge<-branch name->  (to merge 2 branches )

way 2:
Create a PR
