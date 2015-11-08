# Useful aliases

## cane
Add all the things, amend the same commit and keep the same commit message

## pr 
Checkout a pull request from your upstream repository ex. `git pr 10`


## The config

```
[alias]
        cane = commit -a --amend --no-edit
        pr = "!f() { git fetch upstream refs/pull/$1/head:refs/remotes/upstream/pr/$1 && git checkout FETCH_HEAD && git remote prune upstream; }; f"
```
