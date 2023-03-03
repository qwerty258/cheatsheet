git
===

Remove file from history:

```
git filter-repo --force --invert-paths --path PATH-TO-YOUR-FILE-WITH-SENSITIVE-DATA
```

Force reset to remote branch:

```
git reset --hard origin/main
```

Rebase branch

```
git rebase --onto <new-parent> <old-parent>
```
