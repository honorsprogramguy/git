# Git SSH Keys, Terminal Commands and Basic Git Commands

#### Generating an SSH key
After creating an SSH key, and adding it to your GitHub account you will not have to do it again! You will be prompted for your SSH key passphrase later on for security reasons.. So don't forget that passcode!

If you do that's alright, you will have to create a brand new key and add it to your GitHub account again. 

[Directions to make one are provided by GitHub here](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)


#### Adding a new SSH key to your GitHub account
[Directions on adding a new SSH Key provided by GitHub here](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)


## Terminal Commands

| Key/Command | Description |
------------ | -------------
| Tab | Auto-complete files and folder names |
| Ctrl + A | Go to the beginning of the line you are currently typing on |
| Ctrl + E | Go to the end of the line you are currently typing on |
| Ctrl + U | Clear the line before the cursor |
| Ctrl + K | Clear the line after the cursor |
| Ctrl + W | Delete the word before the cursor |
| Ctrl + T | Swap the last two characters before the cursor |
| Esc + T | Swap the last two words before the cursor |
| Ctrl + R | Lets you search through previously used commands |
| Ctrl + L or Command + K | Clears the Screen |
| Ctrl + C | Kill whatever you are running |


#### CORE COMMANDS

| Key/Command | Description |
------------ | -------------
| cd | Home directory |
| cd [folder] | Change directory |
| cd ~ | Home directory, e.g. 'cd ~/folder/' |
| cd / | Root of drive |
| ls | Short listing |
| ls -l | Long listing |
| ls -a | Listing incl. hidden files |
| ls -lh | Long listing with Human readable file sizes |
| ls -R | Entire content of folder recursively |
| open [file] | Opens a file |
| open . | Opens the directory |
| top | Displays active processes. Press q to quit |
| nano [file] | Opens the Terminal it's editor |
| pico	[file] | Opens the Terminal it's editor |
| q | Exit |
| clear | Clear screen |


#### COMMAND HISTORY
| Key/Command | Description |
------------ | -------------
| history n | Shows the stuff typed - add a number to limit the last n items |
| ctrl-r | Interactively search through previously typed commands |
| ![value] | Execute the last command typed that starts with 'value' |
| !! | Execute the last command typed |


#### FILE MANAGEMENT
| Key/Command | Description |
------------ | -------------
| touch [file] | Create new file |
| pwd | Full path to working directory |
| .. | Parent/enclosing directory, e.g. |
| ls -l .. | Long listing of parent directory |
| cd ../../ | Move 2 levels up |
| . | Current folder |
| cat | Concatenate to screen |
| rm [file] | Remove a file, e.g. rm [file] [file] |
| rm -i [file] | Remove with confirmation |
| rm -r [dir] | Remove a directory and contents |
| rm -f [file] | Force removal without confirmation |
| rm -i [file] | Will display prompt before |
| cp [file] [newfile] | Copy file to file |
| cp [file] [dir] | Copy file to directory |
| mv [file] [new filename] | Move/Rename, e.g. mv -v [file] [dir] |


#### DIRECTORY MANAGEMENT
| Key/Command | Description |
------------ | -------------
| mkdir [dir] | Create new directory |
| mkdir -p [dir]/[dir] | Create nested directories |
| rmdir [dir] | Remove directory ( only operates on empty directories ) |
| rm -R [dir] | Remove directory and contents |

#### HELP
| Key/Command | Description |
------------ | -------------
| [command] -h | Offers help |
| [command] --help | Offers help |
| [command] help | Offers help |
| reset | Resets the terminal display |
| man [command] | Show the help for 'command' |
| whatis [command] | Gives a one-line description of 'command' |



## Git Commands
Creating GitHub repos, saving changes to your github, and accessing folders and files through terminal is part of every Developer's essential tools. 

#### Creating your First Repository 

```sh
#navigate to the folder you want to put on GitHub
$ touch README.md #this creates a file called README.md this is a markdown file. Developers use this for a place to put instructions, a description about the project you can scroll to the top of this page, hit raw and see exactly how I wrote this MarkDown file
$ git add . #this adds everything changed in this repo from local to staging
$ git commit -m 'first commit' #this commits everything in staging to be ready to be pushed into GitHub it's important to include a -m (message) with this commit because it's for you and future developers to understand what happened during this commit. What changes happened at this point in time
$ git remote add origin git@github.com:yourGitHubUserName/yourRepoName.git #this links your github repo to your local folder on your machine. 
$ git push origin master # this pushes from staging to the repo on github
```
#### Whenever you wanna add changes to your repository online

```sh
$ git add . 
$ git add -u #when you have deleted a local file and you want to remove from your repository 
$ git commit -m 'what has changed'
$ git push origin
```

#### When you want to get someone else's repo onto your machine

```sh
# first fork the repo you want to work on, forking will take the repo, and make an exact copy onto your personal GitHub account
$ git clone git@github.com:yourUsername/yourReponame.git
```

#### When 
