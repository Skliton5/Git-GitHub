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

Project Git Repo URL : https://github.com/Skliton5/Git-GitHub.git

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

1. git init:

Creates a Git repository in your current folder.

Example:
Normal folder → git init → Git repository ✅

2. git status:

Shows the current status of your files — for example, new, modified, staged, etc.

3. git add :
git add liton.txt

Moves a specific file to the Staging Area.

Or:

git add .

Adds all changed files to the Staging Area.

4. git commit
git commit -m "liton file added"

Saves the staged changes as a commit in your Local Repository.

Think of it as creating a checkpoint of your work.

5. git push
git push

Sends your local commits to the GitHub/central repository.

Direction:

Local Repository → GitHub

6. git restore
git restore liton.txt

Used to unstage changes or discard changes, depending on how the command is used.

⚠️ Be careful with git restore because some options can permanently discard your changes.

7. git log:

Shows your commit history.

Example:

commit 790df17
liton file added

commit abc1234
first commit

8. git rm
git rm liton.txt

Deletes the file and stages the deletion.

Then:

git commit -m "delete liton file"
git push

Now the file will also be deleted from GitHub.

9. git clone
git clone <repository-url>

Downloads the complete GitHub repository to your computer.

Direction:

GitHub → Computer

Example:

git clone https://github.com/username/project.git

10. git pull:

Downloads the latest changes from GitHub to your local repository.

Direction:

GitHub → Local Repository

In your previous situation:

git pull --rebase origin main

means: Get the latest changes from GitHub and place your local commits on top of those changes.

11. .gitignore

.gitignore tells Git which files and folders should not be tracked.

Example:

target/
.classpath
.project
.settings/

For a Java/Spring Boot project, target/ is commonly ignored.


