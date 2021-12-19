Cheatsheet For GitHub / GitLab
===
## Configure Git
- ### For the configuration we have two commands which are most important at first time git setup in any new device.

    `git config --global user.name "[name]"`
    - Set the global name which is used in commit transations into your git repository and also it will attach into your every commit
 
    `git config --global user.email "[email]"`
    - Set the global email which is used in commit transations into your git repository and also it will attach into your every commit
---
## Repositories
- ### When you want to setup the new project git repository or you want to setup the existing project repository then you have to go with the below commands.

    `git init`
    - This command will turn to current directiory into git repository
        - Example:
            - My current project directiory is 'D:/git_projects/project'
            - Open the git bash
            - Go to the project directiory
            - Now run the `git init`
            - So, now your directiory is not only directiory but it's git repository too. Now you can do other oprations for handling the git repository for current directiory.

    `git clone [clone url]`
    - This command will clone the existing git repository and then you can do other oprations for handling the git repository
---
## The .gitignore File
- ### This file is very important file for the any project which contains the file / folder path for exclude the tracking into commit transations or exclude to upload extra files / folder into git repository.
    - Example:
        - If you are using android studio or vscode then you don't need to upload editer related file which are in project directiory in local so, you can define that editor related file / folder path into the `.gitignore` file which will not going to track into commit transations
- ### One more thing is like if you wants to upload any file or folder explicitly then you don't need to remove the file / folder path from the `.gitignore`. You can upload without changing the `.gitignore`
---
## Branches
- Git Branches are the most important part for the working with git. It will create the different route than main route. For that there is some commands which is helping you for work with different branches.

    `git branch [branch-name]` or `git checkout -b [new-branch-name]`
    - For Creating the new branch for the particular branch then you use the above command. First command is just creating the branch and second command is creating the branch and take you into that new branch (checkout into that new branch).

    `git checkout [branch-name]`
    - Above command is used for the changing the branch from current to another branch.

    `git merge [branch-name]`
    - Above command is used for the merging the branch into development / stagging / production server branch.
    
    `git merge --abort`
    - Above command is used for the abort merge request which is used by the cli
    
    `git branch -d [branch-name]`
    - Above command is used for the delete branch from local
    
    `git branch -D [branch-name]`
    - Above command is used for the delete branch forcefully from local
    
    `git push origin :[branch-name]`
    - Above command is used for the delete branch from remote
---
## Synchronization
- ### For any new changes which is needed to share with team or For any changes which is needed to take from any team member then you need to synchronize local with the git repository. For that there are many commands with different purpose which are following.

    `git fetch`
    - This command will fetch all the branches which are on the remote server

    `git pull origin --prune`
    - This command will fetch all the branches with update code code which are on the remote server

    `git pull origin [branch_name]`
    - This command will take updated code in local for the specific branch

    `git push origin [branch_name]`
    - This command will upload all the commits into remote specific branch
---