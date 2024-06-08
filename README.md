# git-demo
## Git basic Commands

### Git version
    git –version

### Ls
    List of directory and folder

### Ls -a
    List of all directory and folder with hidden

### Pwd
    Pwd
    Working directory present

## SETUP
   Configuring user information used across all local repositories

### git config --global user.name "[firstname lastname]"
    set a name that is identifiable for credit when review version history 

### git config --global user.email “[valid-email]” 
set an email address that will be associated with each history marker 

### git config –list
    list of users

### git config --global color.ui auto 
    set automatic command line coloring for Git for easy reviewing

### SETUP & INIT 
    Configuring user information, initializing and cloning repositories 

## git init 
   initialize an existing directory as a Git repository
 
## git clone [url] 
   retrieve an entire repository from a hosted location via URL

### STAGE & SNAPSHOT 
   Working with snapshots and the Git staging area 

### git status 
    show modified files in working directory, staged for your next commit 

### git add [file] 
    add a file as it looks now to your next commit (stage) 

### git add .
    add all files as it looks now to your next commit(stage)

### git commit -m “[descriptive message]” 
    commit your staged content as a new commit snapshot

### git push [alias] [branch] 
    example: git push origin main
    Transmit local branch commits to the remote repository branch 


### git reset [file] 
    unstage a file while retaining the changes in working directory 

### git diff 
    diff of what is changed but not staged 

### git diff --staged 
    diff of what is staged but not yet commited 

##  BRANCH & MERGE
    Isolating work in branches, changing context, and integrating changes 

### git branch 
    list your branches. a * will appear next to the currently active branch
 
### git branch [branch-name] 
    create a new branch at the current commit 

### git checkout 
    switch to another branch and check it out into your working directory 

### git merge [branch] 
    merge the specified branch’s history into the current one 

### git log
    show all commits in the current branch’s history

## INSPECT & COMPARE 
    Examining logs, diffs and object information

### git log 
    show the commit history for the currently active branch 

### git log branchB..branchA
    show the commits on branchA that are not on branchB 

### git log --follow [file] 
    show the commits that changed file, even across renames 

### git diff branchB...branchA 
    show the diff of what is in branchA that is not in branchB 

### git show [SHA]  
    show any object in Git in human-readable format

## TRACKING PATH CHANGES 
   Versioning file removes and path changes 

### git rm [file] 
    delete the file from project and stage the removal for commit 

### git mv [existing-path] [new-path] 
    change an existing file path and stage the move 

### git log --stat -M 
    show all commit logs with indication of any paths that moved

## IGNORING PATTERNS 
   Preventing unintentional staging or commiting of files

    logs/ 
    *.notes 
    pattern*/ 

    Save a file with desired paterns as .gitignore with either direct string matches or wildcard globs.

### git config --global core.excludesfile [file] 
    system wide ignore patern for all local repositories

## SHARE & UPDATE 
   Retrieving updates from another repository and updating local repos 

### git remote add [alias] [url] 
    add a git URL as an alias 

### git fetch [alias] 
    fetch down all the branches from that Git remote 

### git merge [alias]/[branch] 
    merge a remote branch into your current branch to bring it up to date 

### git push [alias] [branch] 
    Transmit local branch commits to the remote repository branch 

### git pull 
    exambple: git pull origin main
    fetch and merge any commits from the tracking remote branch


## REWRITE HISTORY 
Rewriting branches, updating commits and clearing history

### git rebase [branch] 
    apply any commits of current branch ahead of specified one 

### git reset --hard [commit] 
    clear staging area, rewrite working tree from specified commit


## TEMPORARY COMMITS 
   Temporarily store modified, tracked files in order to change branches

### git stash 
    Save modified and staged changes 

### git stash list 
    list stack-order of stashed file changes 

### git stash pop 
    write working from top of stash stack 

### git stash drop 
    discard the changes from top of stash stackg

_______________________________________________________________________________________________________________________________

## Local to Git step by step
### mkdir
    1. create folder on local machine (example: git-commands)
    Create a new repository same name  (example: git-commands) on "https://github.com"
### git init
    initialized empty git repository  
### project
    create folder or files(one or many) inside project folder
    example: 
        1. index.html
        2. style.css
        3. script.js
        4. readme.md
### git status        
    1. show untracked / new files in working directory
    2. show modified / changed files in working directory   
### git add .
    1. add all files as it looks now to your next commit(stage)
    2. add single file (example: git add index.html)
### git commit -m "add initial files"
    1. commit your files and folder
    2. git status
       check status once commited files.
### all folder / files created and those changes add / commit on local machine / branch
### same folder / project upload on Github / other repository
### Create new repository on Github(https://github.com/new) / other repository (but make sure name should be same example: git-commands)

### git remote add origin [url] (https://github.com/balramkamble/git-commands.git)
    add a git URL as an alias
### git remote -v
    to verify remote
    esample: https://github.com/balramkamble/git-commands.git
### git branch
    to check branch current branch
    example: Master
### git branch -M main
    to rename branch "main"
    example master to main
### git branch
    to check branch name once after rename branch
    example: main
### git push origin main
    push changes in branch
    example: main branch
________________________________________________________________________________
## Git to Local to Git workflow
### Github Repository
    1. create new repository
    2. already created repository
### git clone [url] 
    1.  retrieve an entire repository from a hosted location via URL
    example: git clone https://github.com/balramkamble/git-commands.git
### project
    project folde add/modify/delete folder/files
### git status        
    1.  show untracked / new files in working directory
    2.  show modified / changed files in working directory   
### git add [file] 
    add a file as it looks now to your next commit (stage)
### git add .
    add all files as it looks now to your next commit(stage)
### git commit -m “[descriptive message]” 
    commit your staged content as a new commit snapshot
### git push [alias] [branch] 
    1example: git push origin main
    Transmit local branch commits to the remote repository branch 
_____________________________________________________________________________
## Git Branches
### Git branch
    to check current branch
### git branch -M main
    to rename branch
### git checkout [branch name] 
    shift one branch to another branch
### git checkout -b [new branch name]
    to create new branch
    eample: feature1
### git branch -d [branch name]
    eample: to delete branch
_____________________________________________________________________________

## Merge Code 2 options
## option 1
### git diff [branch name]
    to compare commits, branches, files and more
### git merge [branch name]
    to merge 2 branches
## option 2 
### create PR (pull request) from github
_____________________________________________________________________________

written by balram kamble

