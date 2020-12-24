# Git-and-Github-Tutorial
If you are very new to git, read through the readme first. If you want to revise a topic, than you can go to any of the above topics. They contain detailed instrudtions for use.
This tutorial is specifically for using Git using command line tools. Although, I have added links for using it with GUI tools and Web- based serveces as well.

## About VCS and Git

We can think of version control from the perspectives of content, teams, and agility. Version control manages a collection of changing and improving files which we can call a project. The complete history of the project is tracked and available at any time. Version control also supports teams working on that collection of files. Teams work in many different ways, and a good version control system will support many of their workflows or ways of getting work done. Version control helps support collaboration on the project and improves quality through facilitating team communication and reviews. Finally, version control enables agility, the ability to adapt quickly and constructively to a changing environment.

Version control enables team to manage a collection of files in an agile way. This collection of files is called a project and Git is flexible enough to manage many types of projects. Git is a distributed version control system. Thos means that users work with local copies of the repository enabling them to work while offline and synchronize with other repositories at a later time. A repository contains the project history as commits. A commit is a snapshot of the entire project at a point in time.

---

## Why Git

Git is a distributed version control system. We've seen that this means each user has a local copy of the repository and that repositories can easily be synchronized. Git is a free and open source software project meaning that the code that implements Git is publically available. No single company owns Git, and anyone can make contributions to improve it. Git has a vibrant community of support and an ecosystem in which many other technologies are integrated with it.


---
## Tutorial for using git client, GUI clients and remote VCS websites
These clients helps the users in maintain a git based Version control and also help developing a synchronized connection between a local and a remote repository (fancy term for a folder). 

  1. **Git can be used with command line using Git client**. The exact installation details are available [here](https://git-scm.com/downloads).

  2. Other than this command line tool, there exist many **GUI tools for using git client**. The most famous ones are:
    * Github Desktop (For windows) - This is usually recomended if you are using Github as you remote repository(configurations are done in default for github). However, you can connecct it with any remote VCS website by pasting the repository's URL and entering your login credentials every time you switch. A very basic and flawed piece of code to show how Github GUI works. The accompanied tutorial can be found [here]( https://learn.sparkfun.com/tutorials/using-github).
    * Sourcetree (Fow Windows) - This one is  recomendded for connecting with Bitbucket. A desciptive guide for installation and set up is available [here](https://www.coursera.org/learn/version-control-with-git/lecture/COD2g/sourcetree-installation-and-getting-started).
    * GitKraken (For MAC and Linus) - The [documentation](https://www.gitkraken.com/) is self explaining.
   
  3. **Remote VCS Websites** are web services hosting remote version control systems. These can be thought of as cloud services for VCS mannagement. Usually, companies have their own remote repositories for confidential work, but the entire open-source community relies on free services offered by sites like [Github](https://github.com/) for personal use and [BitBucket](https://bitbucket.org/product) for professional use.   

---
## Getting Started

The fisrt thing you do after installing git is to configure your username, email, and the default editor.

  * git config --global user.name <Your name>. 
    For example :  git config --global user.name "Jash Shah"

Here, the tag **--global** means that username has been configured for all the repository for a particular user. You can use the tags **--local** or **--system** instead.

  * Similalry configure the email address as well. If you are installing git client after installing github desktop, this setting gets configured by default -

git config --global user.email "jashshah0801@gmail.com"

git config --global user.email "7563883+Jash-2000@users.noreply.github.com"  <This is the default configuration>


Now that you are ready with basic configurations, follow the order number of the files present in this repository.
