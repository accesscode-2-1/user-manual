
# Git and Github Cheatsheet

This page has some quick info on git that you can use as a reference. This guide will be added to over the course of the semester. Please feel free to make a pull request with any additional information you think may be useful!

## Key terms

* __command line__: a tool for entering text commands into a computer (varies based on OS). For Mac we use the Terminal app. 

* __git__: a command line tool for storing and managing changes made to files in a project (usually code)

* __Github__: a web app that integrates with git and amplifies its functionality with a web-based interface and a social component

* __repository (repo)__: the place where the history of your work is stored (.git folder)

* __$__: The dollar sign is commonly used to represent the command line. Anything to the right of it is what you enter (ex. `$ ls` means you enter `ls`)

* __remote__: stored on another computer (usually a server or Github)

* __commit__: a single unit of changes to the project. Git works best when commits are small and frequent.


Local git repository consists of three “trees”:

1. __working directory__: where all of your files live in their current state

2. __index (staging area)__: where your changes are staged before you commit them

3. __git directory__: where the history of all your changes live (.git folder)


```
project/              <-- working directory
├── home.html         <-- files under version control
├── style.css        
└── .git/             <-- git directory
```

![](https://github.com/accesscode-2-1/user-manual/blob/master/git-trees.png)

## Command Line Basics

* `pwd`
  * print the directory (folder) where you currently are
* `ls`
  * list all files in the current directory
* `ls -a`
  * list all files in the current directory including hidden files (beginning with a dot)
* `cd your-directory-here`
  * move to the specified directory
* `cd ..`
  * move to the parent directory (up one level)
* `mkdir new-directory-name`
  * make a new directory
* `rm file-name`
  * remove specified file (FOREVER! Be careful with this)


## Initial git setup

* `git init`
  * initialize the current directory to be version controlled by git
* `git config --global user.name your-username`
  * set your git username (the same as Github username)
* `git config --global user.email your-email@mail.com`
  * set your git email (the same one you use for Github)


## Keeping track of where you are

*  `git log`
  * lists all of the commits in the repository, most recent ones first
*  `git status`
  * provides information on current changes to your files, and whether those changes have been staged (added to the index)


## Basic git workflow

Follow these steps to save your changes as a new version:

1. stage your files (add them to the index)
  * `$ git add -A .`
2. commit changes to files
  * `$ git commit -m “brief description of changes”`
3. pull changes made by other people
  * `$ git pull`
4. push your changes
  * `$ git push`
