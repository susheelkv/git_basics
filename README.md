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
susheel {gitrepo}$ ssh-keygen <br/> 
Generating public/private rsa key pair.<br/>
Enter file in which to save the key (/Users/susheel/.ssh/id_rsa): <br/> 
Enter passphrase (empty for no passphrase): <br/>
Enter same passphrase again: <br/>
Your identification has been saved in /Users/susheel/.ssh/id_rsa. <br/>
Your public key has been saved in /Users/susheel/.ssh/id_rsa.pub. <br/>
```
- Copy the public key to your git account. (Account -> settings -> SSH keys)
-- make sure to provide read/write access
```
susheel {gitrepo}$ cat ~/.ssh/id_rsa.pub <br/>
ssh-rsa xxxxxxx........<br/>
.... <br/>
.... <br/>
.... <br/>
```

## Working on an existing repository

- Set username & email (will show up on your commits)

```
git config --global user.name "Your Username" <br/>

git config --global user.email "user@userdomain.com" <br/>

```

- Add remote URL
```
git remote add origin ssh://git@github.com/susheelkv/git_basics.git <br/>
```

- Pull code to local repo
```
git pull origin master <br/>
```

- Add file for commit (README in this case)
```
git add README.md <br/>

- Once your changes are done & you are ready to commit
-- Add a commit comment
```
git commit "Changes to " <br/>
```
- Push your changes
```
git push origin master <br/>
```
