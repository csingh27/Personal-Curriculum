**Installationb **   

*Installation of Git on Ubuntu 16.04*
1. Type *sudo apt-get install git* on the terminal  

**Initialize**  

*Turn an existing directory on your system to Git directory*   
1. Navigate to a directory in your system. E.g. GitHub  
2. Open terminal inside the directory 'GitHub' and type *git init* 
3. Create empty files in the directory using *touch* command  
E.g. *touch index.html*  
E.g. *touch app.js*  

**Configuration** 

*Configure your Git account*
1. Configure your git using *git config* command
E.g. git config --global user.name "csingh27"    
     git config --global user.email "s----------5@gmail.com"  
**Add files to git staging area**  
git add index.html  
git status  
git rm --cached index.html  
git status  
git add * .html 
**Add all files**  
git add .  
git commit  
initial commit  
exit  
edit a file   
git status  
git add .  
git commit -m "changed app.js"  
touch .gitignore  
touch log.txt  
add the file name (or * .txt if you want all text files to be ignored) that you do not want to be included in git to .gitignore   file  
create a directory with new file  
if you dont want a directory to be included add /dir2 to the .gitignore file  
git branch mybranch to create a branch  
to switch branches, git checkout mybranch  
git merge mybranch  
create new repository  
create new folder in repository   
move file from one repository  
git remote  
git remote add origin https://github.com/csingh27/ComputerVision.git  
git remote  
* git remote add gitcv https://github.com/csingh27/ComputerVision.git  
git remote  
git push -u origin master  
