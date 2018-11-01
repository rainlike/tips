Git
===

**helpful links**
* [git-config documentation][1]

**Push only the current branch (permanently)**
```
git config --global push.default {option}
```
_possible options_
```
nothing: do not push anything
matching: push all matching branches
upstream: push the current branch to its upstream branch (tracking is a deprecated synonym for upstream)
current: push the current branch to a branch of the same name
simple: (since 1.7.11) like upstream, but refuses to push if the upstream branch's name is different from the local one
```

**Push only the current branch (without global settings)**
```
git push origin HEAD
```

**Abort last merge**
```
git merge --abort
```

**Cancel last commit**
```
git reset HEAD~1 (not pushed)
git reset HEAD (already pushed)
```

**Delete local branch**
```
git branch -D {branch}
```

**Delete remote branch**
```
git push origin :{branch}
git push origin --delete {branch} (since v1.7)
```

[1]: https://git-scm.com/docs/git-config
