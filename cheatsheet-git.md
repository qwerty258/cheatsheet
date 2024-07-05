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

Rebase branch without commit time change

```sh
git rebase --committer-date-is-author-date --onto <new-parent> <old-parent>
```

Combine last 3 commits into one

```sh
git rebase -i HEAD~3
```

Git pull without fetch submodules

```sh
git pull --no-recurse-submodules
```

Modify last commit message

```sh
git commit --amend
```
