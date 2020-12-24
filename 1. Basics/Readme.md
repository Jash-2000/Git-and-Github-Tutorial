# 1. Basics
Go to(or create) any empty directory through command line. Then, enter the command **git init** to initialize git. 

This will create a hidden .git object in the folder. You can view it by typing **ls -a**. This is also displayed below : 

![ls -a](https://github.com/Jash-2000/Git-and-Github-Tutorial/blob/main/1.%20Basics/git%20object.JPG)

Note that my PC name is Bhargav Pandya

---

## Working model of git

Once git has been initilized, the directory has the following items present in it 
  1. **Working tree** - The working tree is the location on your computer that contains the directories and files of a single commit. This is where you can view and edit the files of the project, preparing them for the next commit. We will learn later that you check out a commit to place its directories and files into the working tree.
  2. **Staging area/ Index** - The staging area contains a list of files that are planned to be included in the next commit that you make. You prepare the staging area just the way that you want it, so that the next commit is a meaningful snapshot of the project. You will learn later that you use the add command to add new or modified files to the staging area.
  3. **Local Repository** - The local repository contains all of the commits that have been made for the project. These commits represent the version history of the project. Next, we will discuss the project directory.

![git object](https://github.com/Jash-2000/Git-and-Github-Tutorial/blob/main/1.%20Basics/git_locations.JPG)

---

## Commiting to local repository

  1. git status - This shows our current status of the staging area. 
    * A file showing **??** means that it is unttracked (not added to staging area)
    * A file showing **A** means it has been added to staging area but has not been comitted
    * A file showing **M** means it has been modified after adding to the staging area but before commiting it.
  2. git add - This is used to add files to the staging area. You can use **git add .** if you want to add everything to the staging area. Or else type **git add /<filename/>**
  3. git commit - Used to finally commit the staged files to local repository. It is a good practice to write a short commit message to show what changes have been made. Using the code **git commit -m "This is ma first commit"**, you can add the commit message. If you wish to open the commit message in a text editor, do not use **-m** tag and git will open up your default editor. 
  4. git log - This message helps you in viewing the entire logging history of your commits. This log history would be better viewed if you are using GUI client or Web based services like github.  
  
  ![Git Basics](https://github.com/Jash-2000/Git-and-Github-Tutorial/blob/main/1.%20Basics/git_basics.JPG)

---

## Remote Repository
### One very important thing to note is that locally initialized repositories are aliased by **master** keyword while clonned repos are termed as **main**. This might give an error while pushing to the remote repository. The details for the same are given [here](https://github.com/github/renaming).

A remote repository is usually a professionally managed repository that is hosted in a data center or in the cloud. It often acts as the central source of truth or official state of the project. And it often integrates with other systems like issue trackers and continuous delivery pipelines.A remote repository is often a bare repository. Because nobody works with the repository locally, there is usually no working tree or staging area on a remote repository. The root directory of a remote repository is similar to the ".git" directory in a local repository. By convention, remote repository names end with **.git**. Tutorial for creating a remote repository can be found in the Github and Bitbucket tutorial links I provided in [Project Readmefile](https://github.com/Jash-2000/Git-and-Github-Tutorial/blob/main/README.md).
 
Once the remote repo has been created, you are ready to synch it to a local repository but there are 2 ways to do so :

  1. **__Clonning__** - This is done when we do not have a local repository but a remote one is present. So, we clone (i.e. create a copy of the entire repository on local machine). Doing this downloads each and every file from the remote repository and is very important task when working on an open-source project.
  
  The command used for clonning is **git clone /<url for cloning/> [ optional project name ]**. Note that the project name is the name with which your local project directory would be saved. In case you do not provide the project name, according to the default settings, git will name the local reposiotry with the same name given to the remote repository.
  
  The following figure would make this thing more clear. I have clonned this repository itself to add locally saved images in the repository.
  
  ![git clone](https://github.com/Jash-2000/Git-and-Github-Tutorial/blob/main/1.%20Basics/git_clone.JPG)
  
  2. **__Adding__** - In this case we add a remote repository to an already existing local repository. It is very interesting to note that you can not push the commits from local repo to remote repo before pulling them. This means that an local reposiory can only push if it is updated with the latest version of the remote repo.
  
  The command for doing this is **git remote add /<alias name for remote repo/> /<url/>** 
  

Once a remote repo has been clonned/added to a local repo, we can use the command **git remote -v** to view its status. 
![Verbose](https://github.com/Jash-2000/Git-and-Github-Tutorial/blob/main/1.%20Basics/verbose.JPG)

---

## Pushing to remote repository


