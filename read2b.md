# what is Git?
Snapshots

Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

Local Operations

Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

Tracking Changes

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

Loss of Data

Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

States

Files in Git can reside in three main states: committed, modified and staged.

* Committed

Data is securely stored in a local database

* Modified

File has been changed but not committed to the database

 

Download Git
In order to use Git, your computer must have it available. If you already have Git on your computer, you should make sure you have the latest version.

Git can be installed in three ways:

Install as a package
Install via another installer
Download and compile the source code.
Mac OS X 
Terminal

The simplest method for installing Git on a Mac (for Mavericks 10.9 and above) is running Git from the Terminal. If Git is not installed, you will see a prompt for installation.

Git Website

You can also download Git by visiting this link and following the posted directions:

http://git-scm.com/download/mac (Links to an external site.)

GitHub

A third option is to install Git as part of the GitHub for Mac install. GitHub is repository hosting service, which we will discuss in a future section.

Download GitHub for Mac via the following link:

http://mac.github.com (Links to an external site.)

Windows
Git Website

You can download Git by visiting this link and following the posted directions:

http://git-scm.com/download/win (Links to an external site.)

GitHub

Install Git as part of the GitHub for Windows install.

http://windows.github.com (Links to an external site.)

Linux
Package Manager

You can try installing Git via your distribution’s inherent package management tool.

For Fedora:

$ sudo yum install git
For Ubuntu:

$ sudo apt-get install git
Git Website

To download Git for Linux, visit this link and follow the posted directions:

http://git-scm.com/download/linux (Links to an external site.)

Setting up a Git Repository
Importing
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

Switch to the target project’s directory
Example:

$ cd test (cd = change directory)
Use the git init command
$ git init
To start tracking these repository files, perform an initial commit by typing the following:
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”
Cloning
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

$ git clone https://github.com/test
By cloning the file, you have copied all versions of all files for a project. This command leads to the creation of a directory called “test,” with an initialized .git directory inside it, which has copies of all versions of all files for the specified project. The command also automatically checks out — or retrieves for editing — a copy of the newest version of the project.

To clone a repository into a directory with another name of your choosing, use the following command format:

$ git clone https://github.com/test mydirectory
The command above makes a copy of the target repository in a directory named “mydirectory.”

Committing a File
After staging one or multiple files, you should commit the changes and record what you did within the commit message:

$ git commit -m “made change x,y,z”
*This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.

Committing All Changes
$ git commit -a
*This command commits a snapshot of all modifications to tracked files in the working directory.

Pushing Changes
Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

Example:

$ git push origin master
*This command pushes changes from the local “master” branch to the remote repository named “origin”.

*For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.