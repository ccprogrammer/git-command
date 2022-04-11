# GIT COMMAND

### # Fact about branch
1. branch will clone the commit history of the branch that is selected to be clone and the new branch is not sub branch of the branch that are cloned before but it's sub branch from master but the new branch has the commit history from the old branch that are selected
2. if you want to work on other task just checkout to the branch that are doing the task not merging the task branch to your branch 
3. branch cannot be rename instead of renaming just do this clone the branch name as you like and delete the old branch


#### # Simplified Git Command, Create Read Delete
```
Common Command 
1. git add . (the . means adding all files that has changed)
2. git commit -m 'Commit message explaining what change you do to the code
3. git push 

Adding new branch
> git branch <branch_name>

To see all branch
> git branch / git branch -a

Delete Local Branch
> git branch -D (branch name)

Move to another branch
> git checkout (branch name)

Updating branch
> git pull

Cancel all modified file
> git checkout -- .

Show all commit in branch
> git log --oneline

# More explanatory

Merge branch with another branch (must be in the branch that you want to recieve a merge from another branch)
> git merge/rebase (branch name)

Reset/go back to the commit you select and the commit after the selected commit is deleted
> git reset (commit id)           //all code remain in the code editor
> git reset (commit id) --hard    //all code remove/reset back to the commit selected

Reverting to spesific commit (remove speific commit)
> git revert (commit id)

Delete Remote Branch (i recommend to delete it from the Git version control / web service like Github)
> git push [remotename] :[branch]
> example: git push origin :serverfix

Annoying ':' after running some command to cancel it just enter
> wq

```

#### # Cloning repo will only clone the master and cannot choose spesific branch to clone but you can choose spesific branch with command
```git checkout (branch name ~~without bracket~~)```

#### # Forking Git Repository
What is forking? it is copying other people repo with all the history to our repo it's just like making new repo but the repo is from other people repo. To do it just press 'Fork' in the repo you want to fork

#### # Add new branch from Github Website
If you want to add new branch from another branch, just select the branch first then add new branch
![image](https://user-images.githubusercontent.com/90954993/162657746-d4e99e72-5b77-403b-98f5-fcdb13f18af1.png)


#### # Adding new code update / push
This will update your branch with your code that has been updated, it will only add new code or remove the code that you had remove in Text Editor not uploading all files but but only updated code/files
```
1. git add  (the . means adding all files that has changed)
2. git commit -m 'Commit message explaining what change you do to the code
3. git push 
```

#### # Move to spesific branch 
After you move to spesific branch you choose, all the code/files in your Text Editor/IDE will change to the branch you choose not updating your current branch

```git checkout (branch name ~~without bracket~~)```

#### # Update your current Branch with master / from branch name
This will update your current branch content with master or from branch or whatever branch you choose
```
1. git merge/rebase origin/(master / from branch name ~~without bracket~~)
2. git add .
3. git push 
```

#### # Undo all **Modified** but not removing new folder

```git checkout -- .```

#### # Update branch if your branch have been updated by another user
This will update your code with new code that another user write to your branch

```git pull```







