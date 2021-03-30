# Git Introduction

## Definitions

### Version Control
>Is a system that allows you to revisit various versions of a file or set of files by recording changes.Version Control System (VCS). And a Local VCS entails one database on your hard disk that stores changes to files.

### Centralized Version Control System (CVCS)
>This system entails a single server storing all changes and file versions, so a developer team can collaborate on a single file or set of files. And allowes programmers to have more knowledge of team members’ activities with certain files.

### Distributed Version Control systems (DVCS)
>Allows for multiple mirrored repositories, programmers working in teams can collaborate with each other in various ways to complete a joint project, which enables the use of various simultaneous workflows.
----------


## Git
>Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

>relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk

### Files in Git can reside in three main states :
![States](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

* Committed
    * Data is securely stored in a local database.
* Modified 
    * File has been changed but not committed to the database.
* Staged
    * Flagged a file’s changed version to be committed in the next snapshot.
---------------------
   ## Download Git
   In order to use Git, your computer must have it available. If you already have Git on your computer, you should make sure you have the latest version.

Git can be installed in three ways:
* Install as a package
* Install via another installer
* Download and compile the source code

### Installing on Mac OS X
* Terminal 
    * The simplest method for installing Git on a Mac (for Mavericks 10.9 and above) is running Git from the Terminal. If Git is not installed, you will see a prompt for installation.
* Git Website
    *    You can also download Git by visiting this link and following the posted directions [Here](http://git-scm.com/download/mac)
* GitHub 
    * A third option is to install Git as part of the GitHub for Mac install. GitHub is repository hosting service, which we will discuss in a future section. Download GitHub for Mac via [link](http://mac.github.com)    

### Installing on Windows
*  Git Website
    * You can download Git by visiting this [link](http://git-scm.com/download/win)
* GitHub
    * nstall Git as part of the GitHub for Windows install by visiting this [link](http://windows.github.com)    

### Installing on Linux
>You can try installing Git via your distribution’s inherent package management tool.
* For Fedora:
    * ```$ sudo yum install git```
* For Ubuntu:
    * ```$ sudo apt-get install git```
* Git Website
    * To download Git for Linux, visit this [link](http://git-scm.com/download/linux)    

### Graphical Clients
>Git includes inherent Graphical User Interface (GUI) tools. However, users can also utilize third-party tools created for particular platforms.

GUI Clients for Mac, Windows, and Linux via this [link](https://git-scm.com/downloads/guis)

----------------
## Initial Customization

1. Configuration of Variables
    * An inherent Git tool called ```git config``` allows the setting of configuration variables that control aspects of Git’s operation and look.
1. Identity Setting
    * Type the following
    ```
    git config --global user.name "Jane Smith"
    git config --global user.email "example@email.com"  
     ```  
    * To confirm that you have the correct settings, enter the following command:
    ```
    git config --global user.name (should return Jane Smith)
    git config --global user.email (should return example@email.com)

### Default Text Editor
To configure a different text editor, such as Emacs, type the following:
```
$ git config --global core.editor emacs
```
### Check Settings
To check settings, use the ```git config --list``` command

### Getting Help
There are three ways to get more information on a particular command, by accessing the manual:
1. ```git help command```
1. ```git command --help```
1. ```man git-command```

-------------------
## Setting up a Git Repository
* Importing
 To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:
    1. Switch to the target project’s directory 

       Example:

       ```$ cd test (cd = change directory)```

    1. Use the git init command 

       ```$ git init```

    1. To start tracking these repository files, perform an initial commit by typing the following:

       ```$ git add *.c```

       ```$ git add LICENSE```  

       ```$ git add LICENSE```

------------
## Cloning
use the clone command with a repository’s URL: 

```$ git clone https://github.com/test```     

By cloning the file, you have copied all versions of all files for a project. This command leads to the creation of a directory called “test,” with an initialized .git directory inside it, which has copies of all versions of all files for the specified project. The command also automatically checks out — or retrieves for editing — a copy of the newest version of the project.

To clone a repository into a directory with another name of your choosing, use the following command format:

```$ git clone https://github.com/test mydirectory```

--------------------
## Workflow

### Local Repository Structure
The local Git repository has three components:

![Workflow](https://blog.udemy.com/wp-content/uploads/2015/08/image036.png)

1. Working Directory: The actual files reside here.
1. Index: The area used for staging
1. Head: Points to the most recent commit

### Saving Changes
* Tracked
    * >Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
* Untracked    
    * >Untracked files were not in the last snapshot and do not currently reside in the staging area.

---------
## The Life Cycle of File Status
![The Life Cycle](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
1. You stage the modified file.
1. Then, you commit staged changes.

-------------
## Check File Status
Use Command:

```$ git status```

--------------
## Tracking and Staging a New File
* Single File

    ```git add filename```

* All Files

    ```$ git add *```

After adding a new file called EXAMPLE, you would see information regarding changes to be committed when using the ```git status``` command:
```
$ git status

On branch master

Changes to be committed:

  (use "git reset HEAD ..." to unstage) 
```  
```
new file: EXAMPLE
```

This information tells us that there are changes to be committed and that the file has been staged.

--------------
### Committing a File
Use:

```
$ git commit -m “made change x,y,z”
```

### Committing All Changes
use:
```
$ git commit -a 
```

### Pushing Changes
Example:
```
$ git push origin master
```

### Stashing Changes
When you are not ready to commit changes but do not want to lose them either use:
```git stash``` . This command temporarily removes changes and hides them, giving you a clean working directory. 

---------------
## Remote Repositories

### Cloned Repositories
Cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

### Seeing Your Remotes
By using ```git remote -v```, you can view all the remote URLs next to their corresponding short names.

----------------------------
  [Back to Home](README.md)