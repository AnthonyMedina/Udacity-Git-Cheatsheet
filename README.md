# Udacity-Git-Cheatsheet

This is a "cheat sheet" of all the Git commands used in the Udacity course:
[How to Use Git and GitHub](https://www.udacity.com/course/how-to-use-git-and-github--ud775).

<h3>Some Useful Console Commands</h3>

Command | Description | Options
------------ | ------------- | -------------
`cd <directory path>` | "change directory" -<br>changes the folder you are operating in. | `~` - to home directory<br>`../` - up one folder
`mkdir <folder name>` | "make directory" -<br>creates a new folder. |
`pwd` | "print working directory" -<br>displays the file path of the folder you are working in. |
`ls` | "list" -<br>lists files and folders in the folder you are working in | `-a` - list hidden files too
`touch <filename>` | creates a new file |

<h3>Setting Up Your Workspace</h3>

* Save [this file](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash) in your home directory with the name `git-completion.bash`.
* Save [this file](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh) in your home directory with the name `git-prompt.sh`.
* Download `bash_profile_course` [here](https://www.udacity.com/api/nodes/3341718587/supplemental_media/bash-profile-course/download?_ga=1.37232743.672083044.1467344711).
If you already have a file in your home directory named `.bash_profile`, copy the content from `bash_profile_course` and paste it at the bottom of `.bash_profile`. Otherwise, move `bash_profile_course` to your home directory and rename it to `.bash_profile`.

<h5>Making Git Configurations</h5>

Run the following Git configuration commands. The first one will need to be modified if you are using a text editor other than Atom.
See [this page](https://help.github.com/articles/associating-text-editors-with-git/#platform-mac) for the correct command for a couple of other popular text editors.

>`git config --global core.editor "atom --wait"`<br>
>`git config --global push.default upstream`<br>
>`git config --global merge.conflictstyle diff3`

<h2>Lesson 1 - Navigating a Commit History</h2>

Command | Description | Options
------------ | ------------- | -------------
`git help` | Prints the synopsis and a list of the most commonly used commands | `-a` prints all commands
`git clone <repo-url>` | Clone a repository into a new directory | `directory` - create a new folder for the clone<br>
`git log` | Show commit history | `--oneline` - display on one line<br>`--graph` - show a graph of the branch, merge history<br>`-<n>` - show `n` commits
`git diff` | Show changes between commits, commit and working tree, etc | (no arguments) - view the changes you made relative to the index<br>`--staged` - view the changes you staged for the next commit relative to the latest commit<br>`<commit1> <commit2>` - compare two commits
`git checkout <branch-name>` | Switch branches or restore working tree files | `-b <new-branch-name>` - create and switch to new branch

<h2>Lesson 2 - Creating and Modifying a Repository</h2>

Command | Description | Options
------------ | ------------- | -------------
`git init` | Create an empty Git repository |
`git status` | Show the working tree status |
`git add <filename>` | Add file contents to the index |
`git commit` | Record changes to the repository | `-m` - add message in terminal<br>`-a` - automatically stage files that have been modified and deleted
`git reset` | Reset current HEAD to the specified state | `HEAD <filename` - unstage file
`git branch` | List, create, or delete branches | `<branch-name>` - switch to branch<br>`-d <branch-name>` - delete branch
`git merge <branch1> <branch2>` | Join two or more development histories together | `--abort` - abort merge if there are unexpected conflicts
`git show <commit-ID>` | Show various types of objects |

<h2>Lesson 3 - Using GitHub to Collaborate</h2>

Command | Description | Options
------------ | ------------- | -------------
`git remote` |  |
`git push` |  |
`git pull` |  |
`git fetch` |  |
