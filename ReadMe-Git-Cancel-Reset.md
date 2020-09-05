# How to cancel you've already reseted.

- 1. This is a project template for [Githib-Cancel-Reset].
- 2. To cancel reseted branch, make sure you have to know about how to cancel-reset-branch.



## Process of cancel that you already 'reset'.


### Type 'git reflog' to check your own repository works well or not.

```
git reflog
```

And it will shows several commits that you've already pushed to your github-repository.

```
your_git_repo_id HEAD@{0}: HEAD~: updating HEAD 
your_git_repo_id HEAD@{1}: your_acts (Such as Checkout, Update something)
your_git_repo_id HEAD@{2}: your_acts (Such as Modify, add some comments or codes)
```


### Check the reflog of the previous work and see which 'HEAD' you want to move to.

Example

```
git reset --hard HEAD@{the number you want to move..}
```

Subsitution

```
git reset --hard HEAD@{1}
```

