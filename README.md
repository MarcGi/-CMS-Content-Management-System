# Version-Control-System
Local CMS built in Bash for use on Linux Distributions

Second Year Bash project at the University of Dundee

How to Use:
1. Place script in /usr/local/bin
2. Go to terminal and run cms -help to retrieve all commands


--------------------------
Help for VCS Script
--------------------------

Notes:  
1.The creation of a repository should always be done before using any other commands.  
2.If patching fails replace file with file.prev (should be the file before the last made changes)  
3.Do not manually modify any .cfg .repo .prev .patch files unless you know the consequences  
4.Log of repo activity is stored at repo.log  
5.User needs sudo access in order to use CMS | CMS will fail to operate correctly if not  
6.This script has been checked and tested for bugs , none were found during this however use of this script is at your own risk  
7.This project is no longer being worked upon  
  
Commands:  
cms -adduser (path of repo folder) (Username of user to add) Add User to the repository in order to allow editing  
cms -removeuser (path of repo folder) (Username of user to remove) Remove user from the repository  
cms -createrepo (path of repo folder to be created) Create a repository at the given location  
cms -removerepo (path of repo folder to be deleted) Remove a repository at the given location  
cms -addfile    (path of file to be added to repo) Add file to a repository at the given location  
cms -removefile (path of file to be removed from repo) Remove file to a repository at the given location  
cms -checko	    (path of file to be checked out from repo) Check file out , allows user to edit only  
cms -checkin    (path of file to be checked in from repo) Check file in, saves changes to repo.log  
cms -revert	    (path of file to be reverted from last changes) Reverts file from last changes made to it  
cms -archive    (path of repo folder to be archived) Archive the whole repo as of current  
cms -unpacktar  (path of archived/tar file) Unpack a previous version of the repo and replace current with it(archives folder             unchanged)  
cms -compilesource	(path of repo folder) Compile all c files in the repo and outputs compiledFiles
