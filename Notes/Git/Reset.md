# Revert committed changes
When I am working on multiple branchs sometimes I will push my code to a wrong branch, then I need to revert my committed changes inside wrong branch.

## Usage
```JavaScript
git reset --hard versionID(commit ID)
//--hard will lost the comitted codes you revert
//--soft will keep the reverted code for you to re-commit

//git push origin branchName
//This command will alert you that the version is behind the remote branch

git push origin branchName --force
//It will force push the codes and revert the changes, so please check if others working on this branch and needs something keep updated
```

## References
[CSDN: git撤销已经push到远端的commit](https://blog.csdn.net/xs20691718/article/details/51901161)