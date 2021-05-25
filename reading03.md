# Revisons and the Cloud
## Git Tutorial: A Comprehensive Guide
* TOC
  * Version control  
    * local Version
    * Centralized Version Control
    * Distributed Version Control
    * So, What is Git?
  * History of Git
  * Getting Started
    * Download Git
    * Graphical clients
    * Initial Customization
    * Default text editor
    * Check Settings
    * Getting Help
  * Setting up a Git Repository
    * importing
    * cloning
  * Workflow
    * local Repository
    * Saving Changes
    * The lifecycle of File Status
    * Check File Status
    * Tracking and Stagging a new file
    * Committing a file
    * committing all changes
    * pushing changes
    * stashing changes
  * Remote REpositories
    * cloned Repositories
    * Seeing your remote

## Version control
  * Is a system that allows me to revisit various systems of a file or set of files by recording changes. 
    * I can revert a file or a project to a previos version
    * track modifications and modifying individuals
    * compare changes.
    * Version Control system- VCS
      * mistakes with files can easily be rectified
* Local version Control
  * entails one database on my hardisk that stores changes to files
  * early years, devs created these local VCS
* Centalized Version
  * the need for collaboration withing a dev team on a single file or set of files led to the advent of the CVCS
    * CVCS- Centralized Version control System
  * single system entailing a single server to store all changes and file versions
  * can be acessed by various clients
  * streamlined collab process
* Distributed Version Control
  *  Distributed Version Control systems- DVCS
  *  addresses major vulnerability of the CVS
    * server is the single point of failure. if CVS goes down, all collabs cannot work with each other.
    * to prevent- DVCS allows clients to create mirrored repositories to create backups
    * DVCS allows for multiple mirrored repositories
* So, What is Git?
  * Snapshots
    * Git is a DVCS that stores data ina file system of snapshots.
    * everytime a save changes a version of the project (called a "_**COMMIT**_")
    * Git creats a snapshot of the file and stores a reference to it.
      * If no changes, Git only stores a reference to the already stored identical version.
  * Local Operations
    * Git mostly relies on local ops, as most nexessaery info can found in local resources.
    * allows for expediency, because a project's history resides on the local dick
    * eliminating the need to fetch history info from the server, allowing work to continue offline
  * tracking Changes
    * every change applied to any file or dir is tracked by Git.
    * Git is a "gatekeeper"?
      * will always detect file corruption or loss fo info in transit
  * Loss of Data
    * Git- Set up to minimize the possibility of irrevesible damage to files like accidentially lost data
    * extremely diffivult for a snapshot of my file that is _**committed**_ to be lost.
  * States
    * Files in Git can rside in three main states:
      * committed
        * data is securely stored in a local database 
      * modified
        * File has been changed but not committed to the database
      * staged  
        * Flagged a file's changed version to be committed in the next snapshot 
       ![workflow chart](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)
 
## History of Git
* traces its roots to the open source software project Linux Kernel.
* devs of this project began with a DVCS call "_**BitKeeper**_" in 2002
* 2005- many of the devs stopped this DVCS due to tension between Linux Kernel community and the company behind "_**BitKeeper**_"
 * resulted in revocation of the DVCS' gratis status.
 * Linus Torvald- Chief architect of Linux Kernel, began creating Git.
  * Intention of creating a DVCS with workflow design similar to "_**BitKeeper**_".
   * fast
   * nonlinear development w/multiple branches
   * can support large projects
   * stong mechanisms prventing corruptiong
   * simple design
 ## Getting Started
 * Download Git
   * to use, my computer must hae it available. If i have used Git on my computer, make sure i have latest and greatest ver
  * Git install 3 ways
   1. Install as a package
   2. install via another installer
   3. Download and compile the source code
 * Mac OS X
   * Terminal
     * Simplest method ( Mavericks 10.9 and above)- running Git form the terminal
   * Git website
     * http://git-scm.com/download/mac
   * GitHub
     * Install Git as park of the Github for Mac install
     * http://mac.github.com
 * Windows
   * Git website
     * http://git-scm.com/download/win
   * Github 
     * http://windows.github.com
   * Linux
     * Package manager
       * Fedora: 
         * $ sudo yum install git
       * Ubuntu:
         * $ sudo apt-get install git
      * git webstie
        * http://git-scm.com/downloads/guis
## Graphical Clients
 * Git includes inherent Graphical User Interface- (GUI) tools.
 * can use third-party tools 
   * [list of GUI clinets for all OS](https://git-scm.com/downloads/guis) 
## Initial Customication
* after ensuring Git instal, preform some customization steps (should only need to be done once on any machine. To change settings, repeat steps
 * Configuration of Variables
   * git config - allows the setting of the configuration variables that control aspects of Git's ops and look.
 * Identity Setting
   * after install, immediatly set the user name and email addres, used for every Git commit
     * git config --global user.name (should return "my name")
     * git config --global user.email (should return "my email")
   * to confirm that i have correct settings
     * git config --global user.name (should return "my name")
     * git config --global user.email (should return "my email")
   * by using global option, these Git settings apply system wide. To use a different identity settings for a specific project, change working directory to the desired local Git repo and repeat steps w/o using --global
## Default text editor
* w/o config of a default text editor, Git will use the system default, most likely Vim
* to change this (to emacs):  in terminal:
  * $ git config --global core.editor emacs 
  * Note- some editors, I msut find specific instrustions for the default config
## Check settings
* check settings- use the ```git config --list``` command
  * $ git config --list
    user.name=Jane Smith
    user.email=example@email.com
    color.status+auto
    color.branch=auto
    color.interactive=auto
## Getting Help
* three ways to get more info on a paticular command, accessing the manual:
 * git help command
   git command --help
   man git-command
## Setting up a Git Repository
 * Imporitng
  * to import and exsisting project or directory into Git, type into terminal
   *  
 
