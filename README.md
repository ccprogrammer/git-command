## JUST SOME REMINDER NOTE 
#### # After cloning repo
in **gradle.properties** path
>D:\Keep Out\Asal Ngoding\Development\WORKSPACE\Flutter\one-smile\android\gradle.properties
add or remove or change the path to you jdk path 
>org.gradle.java.home=C:/Program Files/Java/jdk-17.0.1

#### # Building apk in cloned repo
First change the **keystore.properties** path 
>D:\your-app-dir\android\keystore.properties
inside **keystore.properties** change the storeFile= path with **D:\your-app-dir\android\keystore.properties**

#### # After cloning
Run this in flutter terminal (Administrator)
>1. flutter pub cache repair 
>2. flutter pub get

in **Administrator CMD** you can just type this command to enter project dir quick by copy you project dir path
>cd D:\project dir

<br />

---

<br />

## GIT COMMAND

#### # Fact about branch
1. branch will copy the commit history of the branch that is selected to be copy and the new branch is not sub branch of the branch that are copied before but it's sub branch from master
2. if you want to work on other task just checkout to the branch that are doing the task not merging the task branch to your branch 
3. 



#### # Cloning repo will only clone the master and cannot choose spesific branch to clone but you can choose spesific branch with command
>1. ***git checkout (branch name ~~without bracket~~)***

#### # Adding new code update / push
This will update your branch with your code that has been updated, it will only add new code or remove the code that you had remove in Text Editor not uploading all files but but only updated code/files
>1. ***git add .*** (the . means adding all files that has changed)

>2. ***git commit -m 'Commit message explaining what change you do to the code'***

>3. ***git push*** 

#### # Move to spesific branch 
After you move to spesific branch you choose, all the code/files in your Text Editor/IDE will change to the branch you choose not updating your current branch
>1. ***git checkout (branch name ~~without bracket~~)***

#### # Update your current Branch with master / from branch name
This will update your current branch content with master or from branch or whatever branch you choose
>1. ***git merge origin/(master / from branch name ~~without bracket~~)*** 
>2. ***git add .***
>3. ***git push*** 


#### # Undo all **Modified** but not removing new folder
>1. git checkout -- .







