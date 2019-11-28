Git and Git Hub

git --version       -> to get version

$ git init          -> Sets repository at the path you are in.
Initialized empty Git repository in C:/Users/35385/Documents/Courses/2. The Web Developer Bootcamp/projects/webDevBootCamp/GitAndGitHub/.git/

$ ls -a             -> Lists all files including hidden ones
.  ..  .git  readme.txt

rm -rf              -> to remove folder with .git


$ git status        -> Do before add. shows changes.
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)

$ git add app.js    -> Adds the app file

35385@LAPTOP-B51PEBFB MINGW64 ~/Documents/Courses/2. The Web Developer Bootcamp/projects/webDevBootCamp/GitAndGitHub (master)
$ git status
On branch master

No commits yet

Changes to be committed:        -> Status shows there is one file yet to be committed
  (use "git rm --cached <file>..." to unstage)
        new file:   app.js

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

## Need to set config before committing
$ git config --global user.email "stepeneoinmcgowan@gmail.com"
$ git config --global user.name "Stephen"

$ git commit -m "Committing the app file"   -> commit dir contents that have been added.
[master (root-commit) b4ba0d2] Committing the app file
 1 file changed, 1 insertion(+)
 create mode 100644 app.js
  
  $ git add .        -> This will add all files in folder.

  $ git add *.html      -> Wildcard used to match file types for add.

  $ git log            -> Shows log history. Enter 'q' to quit
  

  $ git checkout b4ba0d2e6312ff9dd9f8cd8536f3cc3195196d03      -> This moves the repo back to that revision. Now on HEAD branch.

  $ git revert --no-commit b4ba0d2e6312ff9dd9f8cd8536f3cc3195196d03..HEAD  -> Reverts repo back to that version. --no-commit means, apply to all files and don't prompt.

  $ git checkout master      -> Brings back to master branch.

  $ git reset HEAD file1.txt          -> If file was added, this removes it.

  Create .ignore file in directory and add file names to it for git to ignore them

  $ git branch              -> Lists all the branches in the repo

  $ git checkout -b Feature1    -> Adds a new Feature1 branch and switches to it
  $ git checkout master         -> Switches back to master branch.

  $ git merge Feature1          -> This merges all changes back to master when on master.

  $ git branch -d Feature1      -> This will delete the Feature1 branch.
  
$ git branch -add           -> lists all branches including remote ones

$ git remote add origin https://github.com/smcgow/github-test.git   -> this will link your repository to the remote github repository
$ git push -u origin master         -> This will synch the master branch with remote folder. Repeat for other branches.
$ git pull              -> This will update brnach or master 
#This downloads and checks out the git repo
$ git clone https://github.com/smcgow/github-test.git

  Sign in to github and git hub desktop.


  