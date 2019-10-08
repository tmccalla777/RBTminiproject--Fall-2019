##Step1: Intitialize a New Project  
Create a new project/directory from the command line
	
 $ miniproject
 Go to Github and click the ‘+’ button in the top right corner and select ‘New Repository’

 Then fill out the Repository name and the Description fields (optional). 
Keep it public, and do not “Initialize this repository with a README”. Don’t change anything else.
	
Click “Create repository”.
:newRepo.png
	
 Next you’ll see the setup page.
	
And if you go to your Github Repo page, you’ll see the ReadMe that you initialized with and the reference to the first commit you made.
	
Now let’s get this Repo up to date.
	
Go back to your terminal and git add, git commit, and git push:
	
$ git add .$ git commit -m "Second commit"$ git push
	
Now check out your repo. It should have all the files you created your local directory with along with a new commit id
	
You’re initialized and ready to start working!

	
##Step 2: Setup Your Team
You’re going to need to add your team to your repo so they can collaborate.
	
Once your team is added as collaborators they’ll be able to push, merge, and a ton of other things so make sure you’re only adding your teammates.
	
Click on the “Settings” tab of your rep, then “Collaborators” then search for Github users and add them by clicking “Add Collaborator”:
	
They’ll receive an email letting them know you added them and will be listed as a collaborator.
	
	
If you’re a collaborator, go to the Github Repo page,
	
Git Clone the project, and cd into the directory.
	
Don’t fork it!
	
Forking will copy it in a new Repo to your Github page, but you don’t want that — you want to collaborate on the same Github Repo with your teammates.
	
	
$ git clone git@github.com:MinesJA/github_guide.git$ cd github_miniproject/
	
And now you’re ready to collaborate!

##Step 3: Collaborating
	
When you’re using git to work on the same project with multiple people, there’s one central rule you must follow:
	
**bold**THE MASTER BRANCH SHOULD ALWAYS BE DEPLOYABLE
	
The way to keep Master deployable is to create new branches for new features and merge them into Master when they’re completed.

	
**bold**Here’s how that works.

##Step 3a: Branches 
To start, branches should always represent features. For example, if you want to add the ability for a user to login you should probably create a branch called “user_authentication” and in that branch you should only update what you need to to enable a user to login.
	
It’s also important when collaborating that your team picks features that don’t have overlapping code. For example, you shouldn’t be working on a “user_login” branch at the same time that your teammate is working on a “user_logout” branch because the chances that you’re working on the same files and are writing overlapping code are very high.
	
In your terminal create a new branch:
 Adding the “-b” and a name at the end creates a new branch and then moves into that new branch.
Branches allow you to move back and forth between 'states' of a project. For instance, if you want to add a new page to your website you can create a new branch just for that page without affecting the main part of the project. Once you're done with the page, you can merge your changes from your branch into the master branch. When you create a new branch, Git keeps track of which commit your branch 'branched' off of, so it knows the history behind all the files.   
	
After running the above command, you can use the git branch command to confirm that your branch was created:
 Branching can lead to merge conflict. This is when there is a change in one file that conflicts with a change in another file and git can't figure out which version to use. You'll have to manually go in and tell git which version to use.
 
 ##Online tutorial [![Image]("https://i.ytimg.com/vi/LR5BYZjuXMU/maxresdefault.jpg)] (https://youtu.be/LR5BYZjuXMU)
