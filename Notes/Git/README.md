# Git
Some notes for git commands, it usually used in daily work

## Some basic command
```Javascript
git branch -a //check remote branch
git branch //check local branch
git branch test //create local branch "test"
git push origin test //push local branch "test" to remote branch
git checkout test //checkout the local branch "test"
//Please make sure your current branch's changes is committed or put in stash before checkout other branch
git branch -d test //delete local branch "test"

//pull remote branch to local
//initial git, can jump this steps
cd /path-to-folder //go to the folder for git local folder
git init //initialize git
git remote add origin clone-https-url //connect to remote origin master
//start here if already connected git repo
git fetch origin remote-branch //fetch remote branch to local
git checkout -b local-branch origin/remote-branch //create local branch and checkout the new branch
git pull origin remote-branch //pull the remote branch codes to local branch

//rebase remote branch to local branch
git remote -v //check remote
git fetch origin master:rebase_master //fetch remote master to local in rebase_master branch
git diff temp //check the different
git merge rebase_master //merge local branch rebase_master to current local branch
//Sometimes needs check the conflicts and re-submit
git branch -d rebase_master //delete temp rebase_master branch

```

## [Cherry-pick](https://github.com/MiaXIA/ProjectUtils/tree/master/Notes/Git/Cherry-pick.md)
It is used when you want to pick 1 or more commits from one branch to another, and the codes will live in both branch.

## [Reset](https://github.com/MiaXIA/ProjectUtils/tree/master/Notes/Git/Reset.md)
It is used when you want to revert some commits from remote branch.