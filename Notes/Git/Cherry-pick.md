# Cherry-pick

It is used when you want to pick 1 or more commits from one branch to another, and the codes will live in both branch. Usually I am using it when I commit some codes into dev branch, and then cherry-pick it to an early project version so that it can release as soon as possible to IT or Production version.

## Usage
When the codes are in branch A, and you want to put them into branch B
```Javascript
git checkout A
git log //You need to find out the commit ID you want to pick
git checkout B
git cherry-pick 'commit ID'
git push
```

It will pick the codes from branch A to branch B, and the codes will be both in A and B.

## References
[CSDN: git cherry-pick 把提交到A分支的部分commit 再提交到B分支上](https://blog.csdn.net/liu0808/article/details/79158980)