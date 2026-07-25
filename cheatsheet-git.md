git
===

Remove file from history:

```sh
git filter-repo --force --invert-paths --path PATH-TO-YOUR-FILE-WITH-SENSITIVE-DATA
```

Only keep directories or files:

```sh
git filter-repo --force --path PATH-1-TO-DIRECTORY-YOU-WANT-KEEP --path PATH-2-TO-DIRECTORY-YOU-WANT-KEEP --path PATH-TO-FILE-YOU-WANT-KEEP
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
git commit --amend --date="2008-01-01T00:00:00+08:00" --reset-author # change auther date and reset author to current git user
git commit --amend --author="Author Name <email@address.com>" # change auther
git commit --amend --date="2008-01-01T00:00:00+08:00" --author="Author Name <email@address.com>" # change auther and auther date
```

cherry-pick a commit from another git repository

```sh
git remote add other https://example.link/repository.git
git fetch other
git cherry-pick commit
git remote remove other
git gc
```

drop the root commit (first commit)

```sh
git rebase --committer-date-is-author-date -i --root # change the root commit to drop
```
