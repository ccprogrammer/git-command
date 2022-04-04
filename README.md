# GIT COMMAND

#### # Fact about branch
1. branch will clone the commit history of the branch that is selected to be clone and the new branch is not sub branch of the branch that are cloned before but it's sub branch from master but the new branch has the commit history from the old branch that are selected
2. if you want to work on other task just checkout to the branch that are doing the task not merging the task branch to your branch 
3. branch cannot be rename instead of renaming just do this clone the branch name as you like and delete the old branch

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
>1. ***git merge/rebase origin/(master / from branch name ~~without bracket~~)*** 
>2. ***git add .***
>3. ***git push*** 


#### # Undo all **Modified** but not removing new folder
>1. git checkout -- .

#### # Update branch if your branch have been updated by another user
This will update your code with new code that another user write to your branch
>1. git pull


<br />

---

<br />

# FLUTTER

<br />

## Upgrading/Downgrading flutter sdk/version

#### # Change Channel
Flutter has 4 channel stable(the latest stable version), master(on progress development like -pree version), beta, and dev
>1. flutter channel (will show the list of channel)
>2. flutter channel (channel name)
>3. flutter upgrade

#### # Upgrading sdk
>1. flutter upgrade (this command will upgrade the latest version your current channel)

#### # Upgrade/downgrade by changing repository
>1. locate flutter directory, for example **C:\flutter**
>2. run git bash
>3. git checkout (flutter version) / example git checkout 1.22.6 / example git checkout 2.10.2
>4. flutter doctor (to perform download and compile for the selected version)

<br />

## Things to do after cloning repo to prevent error


#### # Gradle problem
in **gradle.properties** path
>1. D:\Keep Out\Asal Ngoding\Development\WORKSPACE\Flutter\one-smile\android\gradle.properties
add or remove or change the path to you jdk path 
>2. org.gradle.java.home=C:/Program Files/Java/jdk-17.0.1

#### # Building apk in cloned repo
First change the **keystore.properties** path 
>1. D:\your-app-dir\android\keystore.properties
>2. inside **keystore.properties** change the storeFile= path with **D:\your-app-dir\android\app\keystore.jks**

#### # Things to do to remove red highlight in new opened cloned repo
Run this in flutter terminal (Administrator)
>1. flutter pub cache repair 
>2. flutter pub get

in **Administrator CMD** you can just type this command to enter project dir quick by copy you project dir path
>d:
>cd D:\project dir


## OneSmile


#### # Deeplink
>1. Add this code in routes with the widget constructor filled with settings.arguments so when pushNamed called and arguments: ... is filled it will pass to the constructor
```
 case '/surveyPage':
        return MaterialPageRoute(
            builder: (context) => SurveyConsentPage(
                  languageCode: settings.arguments,
                ));
        break;
```
>2. Make Function in helper 
```
  toSurvey({String languageCode}) async {
    return Navigator.of(context).pushNamed(
      '/surveyPage',
      arguments: languageCode,
    );
  }
```
>3. Add switch case in deeplink, here if languageCode is 'id' it will add arguments with 'id' and automatically pass it to the constructor languageCode: because languageCode: is filled with settings.arguments.
```
        case "survei":
          return toSurvey(languageCode: 'id');
          break;
        case "survey":
          return toSurvey(languageCode: 'en');
          break;
```









