Git Hub:
Git is a version control software.

Git Hub is a platform which is used to store project related files / source codeat one place.

In git hub, we can create source code repository to store project code.

All the developers can connect to project repository to store all the source code.(Code Integration will become very easy)

Git Hub repository will monitor all code changes.

who modified
when modified
what modified
why modified


Environment Setup:

Create account in www.github.com

Download & Install 'git client' software in our system

 URL : https://git-scm.com/downloads

Open Git bash and configure your name and your email

 $ git config --global user.name "your-name"

$ git config --global user.email "your-email"

Note: Configuring name and email is just one time process in git bash


What is Git Hub Repository ?

=> Repository is a place where we can store project source code / files.

=> For every project one repository will be created.

=> We can create 2 types of repositories in git hub

  1) Public Repo (anybody can see & you choose who can commit)

  2) Private Repo (you choose who can see & who can commit)

Project Git Repo URL : https://github.com/ashokitschool/sbi_loans_app.git

=> Project team members will connect with git repository using its URL.

Flow Diagram:

Developer → Working Tree → Staging Area → Local Repo → Central Repo (GitHub)

1. Working Tree — your actual project folder
   
 When you code—adding, editing, or deleting files—all of that happens in the Working Tree.

To turn your project into a Git repository for the first time:

git init

After this, Git can track your project.

2. Working Tree → Staging Area: git add

You modified `Login.java`. Now, you decide to include this change in the next commit: git add Login.java

Or, to stage all changed files:git add .

The changes are now in the Staging Area.

The Staging Area simply means:

"I want to save these changes in the next commit."

3. Status check: git status

git status

It shows:

which files are modified
which are staged
which are untracked

Important: In the diagram, `git status` is shown near the staging area, but technically, `git status` does not move any files. It simply displays the current Git state.

4. Staging Area → Local Repository: git commit

Now, you permanently save the staged changes to the Git history:

git commit -m "Add login functionality"

A commit has now been created and is stored in your computer's local repository.

At this stage, the code has not yet been sent to GitHub.

5. Local Repo → GitHub/Central Repo: git push

To send local commits to GitHub:

git push

Or commonly:

git push origin main

Your commit has now reached the GitHub Central Repository.

Flow Diagram :Coding / File Changes
                ↓ 
            Working Tree
                ↓
            git add .
               ↓
           Staging Area
              ↓
           git commit -m "message"
               ↓
           Local Repository
               ↓
           git push
              ↓
           GitHub Repository


