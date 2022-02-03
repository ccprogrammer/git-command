#### # Cloning repo will only clone the master and cannot choose spesific branch to clone but you can choose spesific branch with command
1. ***git checkout (branch name ~~without bracket~~)***

#### # Adding new code update / push
This will update your branch with your code that has been updated, it will only add new code or remove the code that you had remove in Text Editor not uploading all files but but only updated code/files
1. ***git add .*** (the . means adding all files that has changed)

2. ***git commit -m 'Commit message explaining what change you do to the code'***

3. ***git push origin*** or ***git push origin (your current branch name)***

#### # Move to spesific branch 
After you move to spesific branch you choose, all the code/files in your Text Editor/IDE will change to the branch you choose not updating your current branch
1. ***git checkout (branch name ~~without bracket~~)***

#### # Update your current Branch with master / from branch name
This will update your current branch content with master or from branch or whatever branch you choose
1. ***git merge origin/(master / from branch name ~~without bracket~~)*** or ***git rebase origin/(master / from branch name ~~without bracket~~)***  






