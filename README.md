# Git_MAIN
**First repo**
<br>
Author- Gill Saab


 <i><b>Configuring Git </b></i> :
```
git config --global user.name "MY NAME"   
git config --global user.email "someone@email.com"   
git config --list   <-- to view configurations -->
```
**Clone & Status**

<tb>Clone - Cloning a repository on our local machine <br>
```
git clone<-some link->   
```
Status - Displays the state of the code
```
git status  
```
   untracked : new files that git doesn't yet track

   modified : changed

   staged : file is ready to be committed

   unmodified: unchanged


change/modified /newfile(untracked) :-> add(staged) -> commit(unchanged)
 

**Add & Commit :-**\
add -> adds new or changed files in your working directory to the Git Staging area.    <br>                                 
```
git add <-file name->
```
 __Or__
(for add more files at once)    <br>
``` 
 git add .
 ```
commit -> it is the record of change <br>
```
git commit -m "Some Message"  
```

 **Push Command :-**\
push -> upload local repo content to remote repo  <br>
```
git push origin main  or  git push origin -u main  
```
  **Init Command :-**

init -> used to create a new git repo 
```
   git init
   git add .
   git commit -m "Message"
   git remote add origin <-link->
   git remote -v  (to verify remote)
   git branch  (to check branch)
   git branch -M main  ( to rename current branch)
   git push origin main
```
  WorkFlow :-   
Local Git: Github repo -> clone -> changes -> add -> commit -> push

   Branch Commands :-
```
git branch                          (to check branch) 
git branch -M main                  (to rename current branch)  
git checkout <- branch name->       (to navigate)  
git checkout -b <-new branch name->     (to create new branch) 

git branch -d <-branch name->           (to delete branch) 
```

<i>  <b> Merging Code:- </b></i> <br>
__Way 1:__

 (to compare branches,comments,file & more)
 
```
git diff <-branch name-> 
```
(to merge current branch to <-branch name-> given )
```
git merge<-branch name->  
```
<br>

__Way 2:__\
Create a PR\
***Pull Command***:
Used to fetch and download content from a remote repo and immediately update the local repo to match that content
```
git pull origin main
```
***Undoing Changes***\
__Case 1__: staged changes
```
git reset <-file name->
git reset
```
__Case 2__: commited changes (for one commmit)
```
git reset HEAD~1
```
__Case 3__: commited changes (for many commits)
```
git reset <-commit hash->
git reset --hard <-commit hash->
```
***Fork***\
A fork is a new repository that shares code and visibility settings with original "upstream" (Fork is a rough copy)

***Creating .gitignore file***\
__Use Case__ : For ignoring sensitive ,unecessary files/folders

1. By Using git bash
   ```
   touch .gitignore
   nano .gitignore
   ```
2. By Using Editor
    * You can simply create .gitignore file by Naming .gitignore
    * And then you can edit it according to which files/folders you want to ignore
      
**Use following formats for ignore files/folders**
   * For files eg. ignoring all .log , .exe files
     ```
     *.log    <-ignore all .log files->
     *.exe    <-ingnore all .exe files->
     ```
     ,You can use extension of files to ignore them
  * For folders
    ```
    <-foldername->/      <-for single folder->
    build*/              <-ignore all folders starts with build->
    
    ```
 * For except file that you don't want to ignore
   use (!) for exclude file/folder to be ignored
   ```
   *.log
   !important.log     <-important file name->
   ```
    
