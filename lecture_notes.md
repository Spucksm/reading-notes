# 102 May 25, 2021 Tuesday
## Table of Contents
  1. [Home](README.md)
  2. [Markdown](markdown.md)
  3. [Text-Editor](text-editor.md)
  4. [Reading 02 Day 1](reading02.md)
  5. [Reading 03 Day 2](reading03.md)
  6. [Reading 04 Day 2](reading04.md)

## What is git
  * Is the engine under the hood for GitHub
      * A version control system
      * lets multiple devs work on same code simo without crashing
      * Keeps a history of my files
      * Allows users to keep track, change, and revert to previous changes
    * "commit"= save as ( to keep track of changes in order to go back in time to previos builds) keeps the same title with save points  to keep track of, like save points in a game
  * each "commit" (snapshot) has a label that points to it
  * "HEAD" = the label meaning "you are here"
  * Can assign messages to commits
      * messages are like writing a caption for your snapshot.
  * make "COMMIT" often. make small changes to my code and save as= "commit"
## What is GitHub?
  * A way to share code 
  * An online code saved in the cloud as well as on my local directory
  * Version tracking
  * Reviewing changes
  * Keep changes seperate until you want to add them in
## git + GitHub= awesome
  * allows sep dev work on same code without messing each other up
repositories
### what is it?
  * is a collection of files and folders that I told "Git" to pay attention to
    * usually, one project= one repository
    * really large project might have multiple
    
 ## Git Clone
  (clones repository from GitHub saving it from the cloud to my system)
 * Follow code:
    * "code ."     (opens "VS Code" in file directory)
  
## APC process- Add, Commit, Push
  * Way of getting changes from my computer to the repository (in this case GitHub)
  * code- 
    * git status
    * git add (file name)
      * git add readme.md
    * git commit -m "added info to the readme file"
    * git push origin name
    * 
## These are the ACP Steps
* uploading my changes from my computer to the cloud
  * git add (nameoffile) (*note- for one file*) _*OR*_
  * "git add ." (*note for all files*)
  * git commit -m "your message here"
  * git push origin main
