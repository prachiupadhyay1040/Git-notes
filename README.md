# Git-notes

What is Git?

Git is a popular version control system. It was created by Linus Torvalds in 2005.
It is used for:
Tracking code changes
Tracking who made changes
Coding collaboration
What does Git do?
Manage projects with Repositories
Clone a project to work on a local copy
Control and track changes with Staging and Committing
Branch and Merge to allow for work on different parts and versions of a project
Pull the latest version of the project to a local copy
Push local updates to the main project
Why Git?
Over 70% of developers use Git!
Developers can work together from anywhere in the world.
Developers can see the full history of the project.
Developers can revert to earlier versions of a project.

Git installation :
https://linuxhint.com/git-source-code-management-system/

Check Git Version using command line: 
$ git --version
Configure Git

$ git config --global user.name "prachiupadhyay1040"
$ git config --global user.email "prachiupadhyay1040@gmail.com"

Note: Use global to set the username and e-mail for every repository on your computer.
If you want to set the username/e-mail for just the current repo, you can remove global.

Creating Git Folder
Now, let's create a new folder for our project:
Initialize Git
Once you have navigated to the correct folder, you can initialize Git on that folder:


1. Who created GIT and why the name GIT was chosen.
Answer. Git was created by Linus Torvalds and he is also a creator of Linux. Git
means a Foolish Person in British slang. He wanted something short and easy to
remember but he also wanted to disrespect the stupid version control system that he
had used before like bitkeeper.
2. Why do we need GIT?
Answer. We need git for collaboration, version control, Backup, Experimentation and
its open source.

3. What problems are solved by using GIT?
Answer. Git solves many of the challenges faced by software development teams,
including version control, collaboration, code quality, backup, and experimentation.
By using Git, teams can work more efficiently, produce higher quality code, and avoid
many of the common pitfalls of software development.
4. What are the areas in GIT staging?
Answer.
Working Directory: This is the directory on your local machine where you are
currently making changes to your files.
Staging Area: This is also known as the "index" and is where changes to files are
prepared to be committed to the Git repository. In this area, you can choose which
changes you want to include in the next commit.
Git Repository: This is the location where all of the committed changes are stored.
It contains the complete history of all changes made to the project.
5. Why is commit important in GIT?
Answer. A commit records changes to one or more files in your branch. Git assigns
each commit a unique ID, called a SHA or hash, that identifies: The specific
changes.
Commands executed :
To Configure :
● git config --global user.name "your user name"
● git config --global user.email "your email ID"
● git config --list

To use save, commit,tag,branch,push, pull,clone,revert,stash and reset
● git remote add http://10.247.166.154/root/dor.git
● git clone http://cf03p-git-001/root/dor.git
● git add . ⇒ To add files and folders into staging area
● git commit -m "add index file" ⇒ To commit the code will create an ID in hash value
● git status ⇒ Shows the status of git
● git log –oneline ⇒ shows the multiple commits with their tags and
messages
● git show <commit-id> ⇒ To check what is modified in the commit
● git push -u origin master ⇒ To push the code on central repository in master
branch
The branch concept is useful for parallel development
● git branch branch1 ⇒ To create a new branch
● git checkout branch1 ⇒ To change the branch
● git branch ⇒ To verify in which branch we present
● git branch -D branch1 ⇒ To delete a branch
● git merge <branch name> ⇒ To merge branch
● git push origin branch3
Git reset is used to undo local changes to state of a git repo
● git reset database.php ⇒ To revert back from staging area into workspace
● git reset . ⇒ Same as above
● git reset –hard ⇒ To clean from workspace and staging area as well
To remove untracked files
● git clean -f ⇒ To clear untracked files
To apply tags :
● Git tag -a <tagname> -m <message> <commit-id>
● Git tag ⇒ To check list of tags
● Git show <tagname> ⇒ shows the content in a tag
● Git tag -d <tagname> ⇒ To delete the tag
How to revert the commit-id
● git revert <commit-id> ⇒ To revert or undo the commit
Git Stashing is used when you want to started another work in the workspace
suddenly so you have stash the old code
● git stash

● git stash list
● git stash apply stash@{0}
● Git stash clear
