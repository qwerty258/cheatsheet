git
===

Remove file from history:

```sh
git filter-repo --force --invert-paths --path PATH-TO-YOUR-FILE-WITH-SENSITIVE-DATA
```

Force reset to remote branch:

```sh
git reset --hard origin/main
```

Rebase branch

```sh
git rebase --onto <new-parent> <old-parent>
```

Combine last 3 commits into one

```sh
git rebase -i HEAD~3
```
