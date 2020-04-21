**Installation**   

***Installation of Git on Ubuntu 16.04***
1. Type *sudo apt-get install git* on the terminal  

**Initialize**  

***Turn an existing directory on your system to Git directory***   
1. Navigate to a directory in your system. E.g. GitHub  
2. Open terminal inside the directory 'GitHub' and type *git init*  

**Configuration** 

***Configure your Git account***
1. Configure your git using *git config* command  
E.g.  
*git config --global user.name "csingh27"*  
*git config --global user.email "s----------5@gmail.com"* 

**Add files to Git**  

***Create files in the directory***
1. Create empty files index.html and app.js in the directory using *touch* command  
E.g. *touch index.html* and *touch app.js*  

***Add files to git staging area***  
1. Add index.html file to the staging area
*git add index.html*  
2. Check the status of the *add* operation. It will show app.js as untracked files in red. 
*git status*  
3. Remove the file index.html from the staging area. .
*git rm --cached index.html*    
4. It will show app.js and index.html as untracked files
*git status*  
5. Add all html files at once.
*git add * .html* 
6. Check the status.
*git status*  
7. Add all files at once.
*git add .*  
8. Check status. No untracked files.
*git status*

***Commit files from the staging area to git***  

1. *git commit* or *git commit -m "changed app.js"* where "..." is a comment on the commit
2. Type *initial commit* in the text file that opens in the terminal and exit  
3. Check the status using *git status*  
It should display :  
*On branch master  
nothing to commit, working directory clean*  

***Ignore commit of specific files in the Git directory***  
1. Add .gitignore file   
*touch .gitignore*  
2. Add a txt file  
*touch log.txt*  
3. Add the file name  that you do not want to be included in Git to .gitignore file  
(or * .txt if you want all text files to be ignored)  
4. *git add . *  
5. Create a new directory *mkdir dir2*  
6. Add /dir2 to the .gitignore file if you do not want it to be included  
Note that .gitignore file would be hidden. So to edit it, you would need to 'Show hidden files'  

***Create a branch***  
1. Type *git branch mybranch* to create a branch 
2. Switch branches using *checkout* command  
*git checkout mybranch*  
To create a new branch and switch to it at the same time use *-b* (=branch+checkout)  
*git checkout -b mybranch*  
3. Work on a branch separately, make changes to the code, test it and merge when it is functional
*git merge mybranch*  
4. 
create new repository  
create new folder in repository   
move file from one repository  
git remote  
git remote add origin https://github.com/csingh27/ComputerVision.git  
git remote  
* git remote add gitcv https://github.com/csingh27/ComputerVision.git  
git remote  
git push -u origin master  

https://www.atlassian.com/git/tutorials/git-lfs
