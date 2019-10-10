# Setting up Github and Collaboraton

 ### Online video tutorial [![Image](/images/youtube.png)](https://youtu.be/LR5BYZjuXMU)

## Step1: Intitialize a New Project  
Create a new project/directory from the command line
eg. $ miniproject
Go to Github and click the ‘+’ button in the top right corner and select ‘New Repository’

 Then fill out the Repository name and the Description fields (optional).
Keep it public, and do not “Initialize this repository with a README”. Don’t change anything else.

Next you’ll see the setup page.

And if you go to your Github Repo page, you’ll see the ReadMe that you initialized with and the reference to the first commit you made.

Now let’s get this Repo up to date.

Go back to your terminal and git add, git commit, and git push:

$ git add .$ git commit -m "Second commit"$ git push

Now check out your repo. It should have all the files you created your local directory with along with a new commit id

You’re initialized and ready to start working!

## Step 2: Setup Your Team
You’re going to need to add your team to your repo so they can collaborate.

Once your team is added as collaborators they’ll be able to push, merge, and a ton of other things so make sure you’re only adding your teammates.

Click on the “Settings” tab of your rep, then “Collaborators” then search for Github users and add them by clicking “Add Collaborator”:

They’ll receive an email letting them know you added them and will be listed as a collaborator.


If you’re a collaborator, go to the Github Repo page,

Git Clone the project, and cd into the directory. Don’t fork it!

Forking will copy it in a new Repo to your Github page, but you don’t want that — you want to collaborate on the same Github Repo with your teammates.

And now you’re ready to collaborate!


 
## Step 3: Collaborating

When you’re using git to work on the same project with multiple people, there’s one central rule you must follow:

**THE MASTER BRANCH SHOULD ALWAYS BE DEPLOYABLE**

The way to keep Master deployable is to create new branches for new features and merge them into Master when they’re completed.
**Here’s how that works**

Adding a collaborator to a GitHub repository is the way to work with cloning. Since cloning creates a disconnected copy of the repository on the contributor's local computer, they will need a way to upload any changed they make to the original repository. By adding an authorized person as a contributor, the creator of the project gives permission to another person to push commits to the repository.

 
 ## Step 3a: Branches
To start, branches should always represent features. For example, if you want to add the ability for a user to login you should probably create a branch called “user_authentication” and in that branch you should only update what you need to to enable a user to login.

It’s also important when collaborating that your team picks features that don’t have overlapping code. For example, you shouldn’t be working on a “user_login” branch at the same time that your teammate is working on a “user_logout” branch because the chances that you’re working on the same files and are writing overlapping code are very high.

###In your terminal create a new branch:
Adding the “-b” and a name at the end creates a new branch and then moves into that new branch.
When you're working on a project, you're going to have a bunch of different features or ideas in progress at any given time – some of which are ready to go, and others which are not. Branching exists to help you manage this workflow.
Changes you make on a branch don't affect the master branch, so you're free to experiment and commit changes, safe in the knowledge that your branch won't be merged until it's ready to be reviewed by someone you're collaborating with.Your branch name should be descriptive (e.g., refactor-authentication, user-content-cache-key, make-retina-avatars), so that others can see what is being worked on.
 
Branches allow you to move back and forth between 'states' of a project. For instance, if you want to add a new page to your website you can create a new branch just for that page without affecting the main part of the project. Once you're done with the page, you can merge your changes from your branch into the master branch. When you create a new branch, Git keeps track of which commit your branch 'branched' off of, so it knows the history behind all the files.   

After running the above command, you can use the git branch command to confirm that your branch was created:
Branching can lead to merge conflict. This is when there is a change in one file that conflicts with a change in another file and git can't figure out which version to use. You'll have to manually go in and tell git which version to use.
 
 ## Resolve merge conflict
 Merge conflicts occur when competing changes are made to the same line of a file, or when one person edits a file and another person deletes the same file. For more information, see "About merge conflicts."

Tip: You can use the conflict editor on GitHub to resolve competing line change merge conflicts between branches that are part of a pull request. For more information, see "Resolving a merge conflict on GitHub."

Competing line change merge conflicts
To resolve a merge conflict caused by competing line changes, you must choose which changes to incorporate from the different branches in a new commit.

For example, if you and another person both edited the file styleguide.md on the same lines in different branches of the same Git repository, you'll get a merge conflict error when you try to merge these branches. You must resolve this merge conflict with a new commit before you can merge these branches.

Open Git Bash.

Navigate into the local Git repository that has the merge conflict.

cd REPOSITORY-NAME
Generate a list of the files affected by the merge conflict. In this example, the file styleguide.md has a merge conflict.

$ git status
> On branch branch-b
> You have unmerged paths.
> (fix conflicts and run "git commit")
> Unmerged paths:
> (use "git add ..." to mark resolution)
>
> both modified:      styleguide.md
> no changes added to commit (use "git add" and/or "git commit -a")
Open your favorite text editor, such as Atom, and navigate to the file that has merge conflicts.

To see the beginning of the merge conflict in your file, search the file for the conflict marker.
When you open the file in your text editor, you'll see the changes from the HEAD or base branch after the line< < HEAD. 
Next, you'll see =======, which divides your changes from the changes in the other branch, followed by >>>>>>> BRANCH-NAME. 
In this example, one person wrote "open an issue" in the base or HEAD branch and another person wrote "ask your question in IRC" in the compare branch or branch-a.

If you have questions, please
<<<<<<< HEAD open an issue
=======
ask your question in IRC.
 branch-a
Decide if you want to keep only your branch's changes, keep only the other branch's changes, or make a brand new change, which may incorporate changes from both branches. Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge. In this example, both changes are incorporated into the final merge:

If you have questions, please open an issue or ask in our IRC channel if it's more urgent.
Add or stage your changes.

$ git add .
Commit your changes with a comment.

$ git commit -m "Resolved merge conflict by incorporating both suggestions."
You can now merge the branches on the command line or push your changes to your remote repository on GitHub and merge your changes in a pull request.

Removed file merge conflicts
To resolve a merge conflict caused by competing changes to a file, where a person deletes a file in one branch and another person edits the same file, you must choose whether to delete or keep the removed file in a new commit.

For example, if you edited a file, such as README.md, and another person removed the same file in another branch in the same Git repository, you'll get a merge conflict error when you try to merge these branches. You must resolve this merge conflict with a new commit before you can merge these branches.

Open Git Bash.

Navigate into the local Git repository that has the merge conflict.

cd REPOSITORY-NAME
Generate a list of the files affected by the merge conflict. In this example, the file README.md has a merge conflict.

$ git status
> On branch master
> Your branch and 'origin/master' have diverged, and have 1 and 2 different commits each, respectively.
> (use "git pull" to merge the remote branch into yours)
> You have unmerged paths.
> (fix conflicts and run "git commit")
> Unmerged paths:
> (use "git add/rm ..." as appropriate to mark resolution)
> 
> deleted by us:   README.md
>
> no changes added to commit (use "git add" and/or "git commit -a")
Open your favorite text editor, such as Atom, and navigate to the file that has merge conflicts.

Decide if you want keep the removed file. You may want to view the latest changes made to the removed file in your text editor.

To add the removed file back to your repository:

$ git add README.md
To remove this file from your repository:

$ git rm README.md
> README.md: needs merge
> rm 'README.md'
Commit your changes with a comment.

$ git commit -m "Resolved merge conflict by keeping README.md file."
> [branch-d 6f89e49] Merge branch 'branch-c' into branch-d

## 1. Forking vs. Cloning
### Forking
Forking a repository is essentially creating a linked copy of a repo where you can make whatever changes you wish without having any effect on the original project. Once you make changes to your *forked* version of the repository, you can then submit a pull request which will allow you to contribute your proposed changes to the original project. A forked copy has a real connection to its original repo as opposed to a cloned copy.

### Cloning
Cloning a repository is like downloading an offline copy of the project that is not connected to the original in any way. You are downloading a specific iteration of the repository at a specific point in time and that is your local copy. When you make changes to this clone, you can then push the changes back to the original project, but only if you are added as an official contributor by the creator of the repository.

## 2. Pull Request
A pull request is how a contributor can share his changes to a repository with the rest of the group and to discuss what parts should be kept and added to the main repository and what should be discarded. This is a good way for the whole team to review the propose changes of a contributor and discuss how to proceed.
