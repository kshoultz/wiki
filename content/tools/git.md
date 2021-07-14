---
title: "git"
date: 2020-01-13T14:11:32-06:00
draft: false
---

### Why should I use Github.com?

* I can store my code there for free. 
* I can host my web pages there for free.
* One of my projects can be a template or starter set of files for a new website. 
* You can create a repo that holds a site that you created and understand. This can be good for holding your notes and learning code.
* You can use Github Desktop to make a lot of actions easier create visibility of your projects and repos.

### Credentials and Logging In

* Set up an SSH Key with github.com (Find a youtube video that walks you through this).
* Find process for using the github CLI to log in with a token (Gitbash or terminal).
* docs: https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-

### Creating a repository

1. You can create a repo on the github website UI. That's typically what I do.
1. I then follow the steps below to add code to the new empty repository.

### Initializing a repo locally

1. Navigate to the workspace directory you want your project to live.
1. Create a new direactory for the project name you want.
1. Navigate to the new directory.
1. git init
1. This project is now ready to execute git commands and work with a remote repository.

### Committing your code

1. git add .
1. git commit -m 'message for commit.'
1. git push origin master
1. git push heroku master (if you are committing to heroku for publish)

### Downloading an existing repository

1. Get the url for the repo you want to download (clone).
1. In your terminal, navigate to the directory you want to download the project.
1. git clone <http://github.com/targetproject.git> newprojectfolder
1. The project should download and fill the directory.
1. git remote add origin git@github.com:kshoultz/TEST.git
1. Go to github.com to see your code to verify it's all up there.
1. Here is some documentaion on this: <https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository>.

### Updating your local from github

1. Navigate to your project directory in the terminal.
1. git pull origin master
1. All of the changes from the server should download to your project and you should be up to date.

### Removing files from github

1. git rm file1.txt
1. git commit -m "remove file1.txt"

But if you want to remove the file only from the Git repository and not remove it from the filesystem, use:

1. git rm --cached file1.txt
1. git commit -m "remove file1.txt"
