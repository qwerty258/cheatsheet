vim
===

# remove duplicated rows with sort

```vim
:sort u
```
# numeric sort, the 1, 2, 3, 4 ... 9, 10 way.

```vim
:sort n
```

# reindent the entire file

```vim
gg=G
```

# display the name of the current file

type `Ctrl` `g` (or press `1` then `Ctrl` `g` for the full path).

# replace string

```vim
:%s/string to replace/new string/g
```

# delete line with string

```vim
:g/string/d
```

# match for ascii characters

```vim
/[\x00-\x7F]
/[\d0-\d127]
```

# match for non-ascii characters

```vim
/[^\x00-\x7F]
/[^\d0-\d127]
```

# multiline modification

1. move the cursor to the character you want insert before
2. enter visual block mode (`Ctrl` `v`)
3. use `j`, `k`, `g`, `G` (`Shift` `g`) to move cursor around to select multiple lines
4. press `I` (`Shift` `i`)
5. type in characters you want to insert
6. press `Esc` twice

# open a file in a new buffer and vertically split window

```vim
:vs filename
```

# split window vertically

`Ctrl` `wv`

# switch windows

`Ctrl` `ww`
