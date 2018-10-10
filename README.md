# Git SSH Keys & Basic Git Commands

## Generating an SSH key
After creating an SSH key, and adding it to your GitHub account you will not have to do it again! You will be prompted for your SSH key passphrase later on for security reasons.. So don't forget that passcode!

If you do that's alright, you will have to create a brand new key and add it to your GitHub account again. 

[Directions to make one are provided by GitHub here](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)


## Adding a new SSH key to your GitHub account
[Directions on adding a new SSH Key provided by GitHub here](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)



## Creating a Repo For the *1st time*
Creating GitHub repos, saving changes to your github, and accessing folders and files through terminal is part of every Developer's essential tools. Navigating and using the terminal is not easy, but you can always find support with a quick google search. 

#### Terminal Commands
```sh
cd #this command Changes Directories, this is what you use to navagate through folders
cd ~ #this command Changes Directories to the home Directory
cd ~/Desktop/somefolder #this command Changes Directories to somefolder inside of your Desktop
ls #this command lists all the files in your current folder
ls -a #thi command lists all files and hidden files in your current directory

mkdir #this command Makes a new Directory (makes a new folder)
touch somefile.txt #this creates a new file named somefile and it's type of file
open . #this command opens your current directory in the finder

rm yourFile.psd #this command Removes (deletes) the file named yourFile.psd
rm yourFile.psd yourOtherFile.psd #this command Removes (deletes) the file named yourFile.psd as well as yourOtherFile.psd
rmdir folderName #this command deletes folders, note: this only deletes EMPTY directories
rm -R directoryName #this command will tell your Terminal to delete that folder, any files it contains, and any subfolders inside of it, and any directories inside of those subdirectories and so on this will delete everything, and you will NOT get this back. 

```