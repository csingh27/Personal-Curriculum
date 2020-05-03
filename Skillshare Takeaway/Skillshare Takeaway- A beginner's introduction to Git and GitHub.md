Skillshare>  
**A beginner's introduction to Git and GitHub**  
Summary>  

**Setup**  

*Mac* : 
* Git is pre-installed
* Type *git --version* in terminal to check the version installed
*Linux* :  
* Type *sudo apt-get install git* in terminal  
*Windows* :  
* Type *git-scm.com* in the browser
* Download the *.exe* file and install
* Launch *GitBash* to use  

**Command-Line**  
*CLI* : Command Line Interface- faster and more efficient   
*GUI* : Graphic User Interface  
Basic commands :  
*pwd* : Print working directory  
*ls* : List the contents of the current folder  
Flags : Additional instructions to the commands to change the representation of the output  
e.g. *ls -l* tells it to print the output in a detailed list format  
*clear* : clears the screen  
*cd* : change working directory  
*touch* : Create a new file  
e.g. *touch file.txt* creates a file *file.txt* in the working directory  
*rm* : remove a file  
e.g. *rm file.txt*  
*mkdir* : creates a new folder  
*rm -r* : remove a directory  

**Basics**  
* Download "Skillshare Git Project.zip"  
* Extract the zip file at a conventient location, say /Desktop/Skillshare Git Project  
* Open Terminal at */Desktop/Skillshare Git Project/Skillshare Git Project*  
* Type *ls* in terminal to make sure that index.html, style.css files and "images" folder is inside it  
* Type *git init* to initialize the directory  
* Type *git status* to check the list of files to track (In Git we basically track files to check their updation)  
* Type *git add styles.css* to track this file  
* Type *git status*. You will still have two other files in the list of untracked files  
* Start tracking the untracked files using *git add*  
* To track all files use *git add .*
* Type *git status* to check if all files are being tracked  
* *git add* adds the files to the tracking list, or the so-called Staging Area  
* Open index.html and write your name instead of "Your Name" in Line no. 15  
* Save the file index.html and open in your browser. You should be able to see your name  
* Since you made the file to the working directory, it only reflects changes to the working directory.  
  The Staging Area is untouched. 
* Type *git status* and you will be able to see that the file index.html was modified  
* Type *git diff index.html* to check the chenges made between the file in the working directory   
  and the one in the staging area  

**Vim**  
* Vim is a text-editor  
* Create a file using *touch file.txt*  
* Type *vim file.txt*  
* Press *I* to use Vim in Insert mode- Works just like a normal text-editor  
* Press *ESC* to enter the command mode  
* To exit Vim, press *ESC* to exit the Insert mode, then press *SHIFT*+':', type 'wq' (write everything and exit)  
  and press 'ENTER'  
* Now type *vim file.txt*. You will notice that all changes were saved  
* Now press *SHIFT*+':', type 'q!' to quit without saving  changes  
* Type *vim file.txt* and you will notice that no changes were saved  

**Commit**  
* Open styles.css file and change the color in line #23 and save  
* Open the index.html file in the browser and the color will now be purple  
* Run *git status* or *git diff .* to see the changes made  
* Use *git add .* to stage the changes  
* Run *git status*  
* If you make some changes to one of the files by mistake, you can restore it by *git checkout .* command  
  It restores the version saved in the staging area  
* You can play with the files in the working directory as there is always a functional version present in the staging area  
* Type *git commit* to commit all the changes  
* Type *I* to enter into Insert mode and Enter a description of the changes made in this commit  
