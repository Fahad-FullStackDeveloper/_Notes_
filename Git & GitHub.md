GITHUB:
Website that allows developers to store and manage their code using Git.
https://github.com

open link: Governor-House-IT-Initiative-for-AI-Metaverse-/README.md at main · Fahad-FullStackDeveloper/Governor-House-IT-Initiative-for-AI-Metaverse- (github.com)



GIT: (SETUP)
    Version Control System is a tools that helps to track changes in code
Git is a Version Control System. It is: (i)popular  (ii)free & opensource  (iii)fast & scalable.

Check Git Version:
    {git --version} = 2.47.0.windows.2

Configuring Git through CMD/Terminal:
    (a)     {git config --global user.name "Fahad-FullStackDeveloper"}
    (b)     {git config --global user.email "fahad.dude2010@gmail.com"}
    (c)     {git config --list}


CLONE & STATUS:
    Clone - Cloning a repository on our local machine (remote= Github, local= laptop/PC) 
        For copy from remote to local. Go to GitHub Account> open repository> select "<> code" button> copy link from HTTPS of your file.
        And then follow below:
            {git clone <- insert link here-> 
            OR
            https://github.com/Fahad-FullStackDeveloper/Governor-House-IT-Initiative-for-AI-Metaverse-/new/main}
            NOW CLONING DONE FROM GITHUB TO LOCAL MACHINE.
            cd ->   Change Directory
            ls ->   List files
            ls-a -> All List (including hidden files)

    Status - displays the state of the code 
        (a)-Untracked(U)
            new files that git doesn't yet track
        (b)-Modified(M)
            changed
        (c)-Staged(S)
            file is ready to be committed
                (i)Add & (ii)Commit
        (d)-Unmodified()
            unchanged
        {git status}


ADD & COMMIT:
    Add - adds new or changed files in your working directory to the Git staging area.
        (a) git add <-file name->
        OR
        (b) git add .  (for adding all files to git and ready to commit)

    Commit - it is the record of change
        {git commit -m "some meaningful message about changes/ new record"}


PUSH COMMAND:
    Push - upload local repository(Laptop) content to remote repository(GitHub)
        {git push origin main}

INIT COMMAND:
    Init - used to create a new git repository
        * {cd ..}  (change directory from folder you are at to back folder.)
        * {mkdir LocalRepo/name related to the project}  (make new directory.)
        * {cd LocalRepo}  (change directory into folder of folder you are at.)
        * {git init}  (for making git repo to current folder)
        * {git ls -a}
        * {git add .}
        * {git commit -m "some meaningful message about changes/ new record"}
    Add new git repo    
        * {git remote add origin <-link->}
        * {git remote -v}  (to verify remote)
        * {git branch}  (to check branch)
        * {git branch -M main}  (to rename branch)
        * {git push origin main}  (push to git repo)
        * {git push -u origin main}  (for not typing again n again origin main)


ADVANCED WORK FLOW: (watch video from 0:49:10 - 1:00:44)
    Branch Commands (in/out)
        * {git branch}  (to check branch)
        * {git branch -M main}  (to rename branch)
        * {git chechout <-branch name->}  (to navigate)
        * {git chechout-b <-new branch name->}  (to create new branch)
        * {git chechout-d <-branch name->}  (to delete branch)

    Branch Merging Code
        Way 1
            * {git diff <-branch name->}  (to commpare commits, branches, file & more)
            * {git merge <-branch name->}  (to merge 2 branches)
        Way 2
            Create a PR (Pull Request - It lets you tell others about changes you've pushed to a branch in a repository to GitHub.)
        PULL COMMAND:
                {git pull origin main}
                (used to fetch and download from a remote repo and immediately update the local repo to match that content.)

    Resolving MERGE CONFLICTS: (watch video from 1:00:45 - 1:05:31)
        An event that takes place when Git is unable to automatically resolve diffrences in code between two commits.

    Undoing Changes: (watch video from 1:05:32 - 1:11:23)
        Case 1: stagged changes (add)
            git reset <-file name->
            git reset
    
    Case 2:git changes (for one commit)
        git reset HEAD~1

    Case 3: commited changes (for many commits)
        git reset <-commit hash->
        git reset --hard <-commit hast->


FORK: (watch video from 1:11:24 - 1:15:00)
    A fork is a new repository that shares code and visibility settings with the original "upstream" repository.
    Fork is a rough copy.
