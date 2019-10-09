### Secton 2 : Git Commands and Terminology
 Description on the following Git commands and terminology:
 
 
 ## Repository
 A repository contains all of your project's files and stores each file's history.Also known as Repo. You can own it individually, or you can share it with other people in an organization/group.Repositories can be public or private. Public repositories are visible to everyone. Usually refers to a central place where data is stored and maintained. You can create a new repository by 
 > Go to the upper-right corner of any page, use the  drop-down menu, and select New repository.

## Clone
clone is used  to create a local copy on your computer and sync between the two locations. Cloning a repository means that you're downloading a copy of the source code from source control It requires a repository to be created before hand. Use can use it by:
> On GitHub, navigate to the main page of the repository, Under the repository name, click Clone or download.

## Fork
A fork is a copy of a repository. Forking a repository allows you to experiment with changes without interfearing the original project.It is mainly used to fix bug.Used to fetch updates from or submit changes to the original repository.
You can navigate by:
>In the top-right corner of the page, click Fork.

## Branch
It can be used to solve bug, experiment new ideas and develop other features. Each repository has one default branch, and can have multiple other branches. You can merge a branch into another branch. You can create or delete branches:
>On GitHub, navigate to the main page of the repository. Click the branch selector menu.Type a unique name for your new branch, then select Create branch.

## Commit
Commits usually contain a commit message which is a brief description of what changes were made. It that allows you to keep record of what changes were made when and by who.At the bottom of the page, type a short, meaningful commit message that describes the change you made to the file. You can attribute the commit to more than one author in the commit message.

## Merge
Merging takes the changes from one branch (in the same repository or from a fork), and applies them into another. A merge can be done automaticallyor can be done via the command line.Check out the branch you wish to merge to. Usually, you will merge into master.
> $ git checkout master
You can push the merge to your GitHub repository.
> $ git push origin master

## Checkout
The git checkout command lets you navigate between the branches created by git branch. it tells Git to record all new commits on that branch. It makes it easy to try new experiments without destroying existing functionality, and it makes it possible to work on many unrelated features at the same time.

## Push
Pushing refers to sending your committed changes to a remote repository, such as a repository hosted on GitHub. For instance, if you change something locally, you'd want to then push those changes so that others may access them.After creating a repository, copy the git commands under the “…or push an existing repository from the command line”, and paste them into the terminal. These commands will add a remote repository, and then push your local repository to the remote repository.

## Pull
Pull refers to when you are fetching in changes and merging them. For instance, if someone has edited the remote file you're both working on, you'll want to pull in those changes to your local copy so that it's up to date.A pull grabs any changes from the GitHub repository and merges them into your local repository.

## Remote Add / Remove / Show
To add a new remote, use the git remote add command on the terminal, in the directory your repository is stored at. The git remote add command takes two arguments: A remote name, for example, “origin” A remote URL, which you can find on the Source sub-tab of your Git repo.

## Status
A status is a type of status check on GitHub.Status checks are external processes, such as continuous integration builds, which run for each commit you make in a repository.The git status command displays the state of the working directory and the staging area. 

## Master Branch
The main branch — the one where all changes eventually get merged back into, and is called master. This is the official working version of your project, and the one you see when you visit the project repository at github. If you make changes to the master branch of a group project while other people are also working on it, it will affect everyone.


## [Click Here to Return to the README](https://github.com/tmccalla777/RBTminiproject--Fall-2019/blob/master/README.md)
