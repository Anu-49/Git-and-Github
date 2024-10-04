# About Git Github

## Local folders/repo - git bash

Git is a popular version control system. It was created by Linus Torvalds in 2005, and has been maintained by Junio Hamano since then.
It is used for:
  + Tracking code changes
  + Tracking who made changes
  + Coding collaboration
+ Manage projects with Repositories
+ Clone a project to work on a local copy
+ Control and track changes with Staging and Committing
+ Branch and Merge to allow for work on different parts and versions of a projec
+ Pull the latest version of the project to a local copy
+ Push local updates to the main project

### Working with Git
+ Initialize Git on a folder, making it a Repository
+ Git now creates a hidden folder to keep track of changes in that folder
+ When a file is changed, added or deleted, it is considered modified
+ You select the modified files you want to Stage
+ The Staged files are Committed, which prompts Git to store a permanent snapshot of the files
+ Git allows you to see the full history of every commit
+ You can revert back to any previous commit
+ Git does not store a separate copy of every file in every commit, but keeps track of changes made in each commit!


## Remote repositories - github

Git is not the same as GitHub.</br>
GitHub makes tools that use Git.</br>
GitHub is the largest host of source code in the world, and has been owned by Microsoft since 2018.</br>

## Git

To check version:
```
git --version
```

Configure git:
```
git config --global user.name "yourusername"
git config --global user.email "yourmailid@email.com"
``` 
Make directory (say directory name : myproject), change directory path, Work inside the newly created directory:
```
mkdir myproject
cd myproject
```
Initialized empty Git repository in /Users/user/myproject/.git/
```
git init 
```
Create new file let's say first.html and check the list of files and folders using:
```
ls
```
Check the Git status and see if the file is a part of our repo:
```
git status
```
Git is aware of the file, but has not added it to our repository!</br>
Files in your Git repository folder can be in one of 2 states:
+ Tracked - files that Git knows about and are added to the repository
+ Untracked - files that are in your working directory, but not added to the repository</br>

 When you first add files to an empty repository, they are all untracked. To get Git to track them, you need to stage them, or add them to the staging environment. </br>One of the core functions of Git is the concepts of the Staging Environment, and the Commit.</br>
 As you are working, you may be adding, editing and removing files. But whenever you hit a milestone or finish a part of the work, you should add the files to a Staging Environment.
</br>Staged files are files that are ready to be committed to the repository you are working on. When we are done with a editing a file we need to add it to Staging environment.
```
git add first.html
```
To add all files to staging environment:
```
git add --all
OR
git add --A
```
File should be staged. Check for git status now:
```
git status
```
Now ready to move from stage to commit for our repo. </br> When we commit, we should always include a message.
By adding clear messages to each commit, it is easy to see what has changed and when.
```
git commit -m "Commit my first html file"
```
Sometimes, when you make small changes, using the staging environment seems like a waste of time. It is possible to commit changes directly, skipping the staging environment. The -a option will automatically stage every changed, already tracked file.
```
git commit -a -m "Updated index.html with a new line"
```
To view the history of commits for a repo use the log command:
```
git log
```
Trouble remembering commands or options for commands??? use Git help.
</br>
There are a couple of different ways you can use the help command in command line:
</br>See all the available options for the specific command
```
git command -help
```
See all possible commands
```
git help --all
```

### Branches
Branches allow you to work on different parts of a project without impacting the main branch. When the work is complete, a branch can be merged with the main project.
create a new branch where branch name is 'hello-world-images:
```
git branch hello-world-images
```

