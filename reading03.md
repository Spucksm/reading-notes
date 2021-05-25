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
      * ![workflow chart](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)
