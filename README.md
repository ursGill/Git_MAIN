# GOPI_MAIN
First repo
<br>
Author- Gill Saab


 <i><b>Configuring Git </b></i> :
```
git config --global user.name "MY NAME"   
git config --global user.email "someone@email.com"   
git config --list   
```
Clone & Status   <br>

<tb>Clone - Cloning a repository on our local machine <br>
```
git clone<-some link->   
```
Status - Displays the state of the code   <br>
```
git status  
```
   untracked : new files that git doesn't yet track

   modified : changed

   staged : file is ready to be committed

   unmodified: unchanged


change/modified    :-> add(staged) -> commit(unchanged)
newfile(untracked) 

Add & Commit :-
add -> adds new or changed files in your working directory to the Git Staging area.    <br>                                 
```
git add <-file name->
```                                                       
or (for more files at once)    <br>
``` 
 git add  
 ```
commit -> it is the record of change <br>
git commit -m "Some Message"  <br>

 Push Command :-
push -> upload local repo content to remote repo  <br>
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
```
git branch                       (to check branch) 
git branch -M main        (to rename branch)  
git checkout <- branch name->       (to navigate)  
git checkout -b <-new branch name->      (to create new branch) 

git branch -d <-branch name->          (to delete branch) 
```

<i>  <b> Merging Code:- </b></i> <br>
way 1:  
git diff <-branch name->  (to compare branches,comments,file & more) <br>
git merge<-branch name->  (to merge 2 branches ) <br>

way 2:
Create a PR
