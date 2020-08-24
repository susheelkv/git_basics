Installation

MacOS: either use the git package that comes with Xcode or download from
git-scm.com
Windows: download from git-scm.com/download. It will install "Git Bash" & this
article assumes that you are working off of this bash

Commands shown below are on macOS

One time setup
====
susheel {gitrepo}$ ssh-keygen 
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/susheel/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /Users/susheel/.ssh/id_rsa.
Your public key has been saved in /Users/susheel/.ssh/id_rsa.pub.
susheel {gitrepo}$ cat ~/.ssh/id_rsa.pub 
ssh-rsa xxxxxxx........
....
....
....

Working on an existing repository
==

git config --global user.name "Your Username"

git config --global user.email "user@userdomain.com"

git remote add origin ssh://git@github.com/susheelkv/git_basics.git

git pull origin master

make code changes

git add <filename>

git commit "Add a comment here"

 git push origin master


Additional commands
==
git status

