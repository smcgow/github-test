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
  
  $git add .        -> This will add all files in folder.