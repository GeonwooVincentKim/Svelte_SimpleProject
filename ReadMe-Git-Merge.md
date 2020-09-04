# How to merge your new branches to the original branch.

- 1. This is a project template for [Github-Merge] program.
- 2. To make unified-branch, makes sure you have to know about how to merge several branches.


## Process of create and merge several branches into unified branch.

### Current Commit History

```
git branch issue1
git checkout issue1
```

or, if you want to make this commands shortly,

```
git checkout -b issue1
```

### Create a new branch-pointer

```
vim index.html  
git commit -a -m "Your New Comments."
```
You don't have to do this, but if you have something that you modified or deleted some codes, it is good way to convert files by using 'vim' commands.

or you can only type this commands below.

```
git commit -a -m "Your New Comments."
```

### A branch name 'issue1' currently in progress.

You can starting from here if you want to merge several branches as a one-unified-branch.

```
git checkout master
```

And then generate new branch, 'hotfix'.

```
git checkout -b hotfix
vim index.html
git commit -a -m "Your New Comments."
```

### The 'hotfix' branch that have branched off from 'master' branch.

```
git checkout master
git merge hotfix
```

Before you deploy project, make sure you have to check several-branches merged well without [No-Errors].

### The 'master' branch that indicate some like 'hotfix' after Merge.

```
git branch -d hotfix
```

If the processing of 'merge' successfully finished, makes sure you have to delete branch that is not a [Master-Branch].

And what we need to after delete this branch, we should continue a process in [Master-branch].

```
git checkout master
vim index.html
git commit -a -m "Added new comments".
```

or you can omit those some step.
```
git checkout master
git commit -m "Added some new comments".
```


## Further information of merging several git-branches.

You can search futher information about how to merge several branches that above 2 or 3-branches.

```
https://git-scm.com/book/ko/v2/Git-%EB%B8%8C%EB%9E%9C%EC%B9%98-%EB%B8%8C%EB%9E%9C%EC%B9%98%EC%99%80-Merge-%EC%9D%98-%EA%B8%B0%EC%B4%88
```
