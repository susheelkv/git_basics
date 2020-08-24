## Installation

### MacOS
Use the git package that comes with Xcode or download from
git-scm.com
### Windows 
Download from git-scm.com/download. It will install "Git Bash" & this
article assumes that you are working off of this bash


## One time setup
- Commands shown below are for macOS
-- Choose a passphrase (you will be prompted for this when pushing code)
```
susheel {gitrepo}$ ssh-keygen 
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/susheel/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /Users/susheel/.ssh/id_rsa. 
Your public key has been saved in /Users/susheel/.ssh/id_rsa.pub. 
```
- Copy the public key to your git account. (Account -> settings -> SSH keys)
-- make sure to provide read/write access
```
susheel {gitrepo}$ cat ~/.ssh/id_rsa.pub <br/>
ssh-rsa xxxxxxx........
.... 
.... 
.... 
```

## Working on an existing repository

- Create a directory for local repo, navigate to the dir & initialize git
```
$ git init
```
- Add remote URL
```
$ git remote add origin ssh://git@github.com/susheelkv/git_basics.git 
```

- Set username & email (will show up on your commits)

```
$ git config --global user.name "Your Username" 

$ git config --global user.email "user@userdomain.com" 

```

- Pull code to local repo
```
$ git pull origin master 
```

- Add file for commit (README in this case), make your changes
```
$ git add README.md 
[master 98a85c0] adding missed commands to readme
 1 file changed, 9 insertions(+), 5 deletions(-)
```

- Add a commit comment
```
$ git commit "Changes to README" 
```
- Push your changes
```
$ git push origin master <br/>
```
