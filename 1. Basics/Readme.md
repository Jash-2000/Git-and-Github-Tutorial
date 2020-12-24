# 1. Basics
Go to(or create) any empty directory through command line. Then, enter the command **git init** to initialize git. 

This will create a hidden .git object in the folder. You can view it by typing **ls -a**. This is also displayed below : 

---

## Working model of git

Once git has been initilized, the directory has the following items present in it 
  1. **Working tree** - The working tree is the location on your computer that contains the directories and files of a single commit. This is where you can view and edit the files of the project, preparing them for the next commit. We will learn later that you check out a commit to place its directories and files into the working tree.
  2. **Staging area/ Index** - The staging area contains a list of files that are planned to be included in the next commit that you make. You prepare the staging area just the way that you want it, so that the next commit is a meaningful snapshot of the project. You will learn later that you use the add command to add new or modified files to the staging area.
  3. **Local Repository** - The local repository contains all of the commits that have been made for the project. These commits represent the version history of the project. Next, we will discuss the project directory.

---

## Commiting to local repository

