rename
======

# replace strings in filenames

## perl-based rename (or prename) 

This version uses regular expressions to rename multiple files and is common on Debian/Ubuntu-based systems.

```sh
rename "s/PNG/png/g" *
```

## util-linux based rename

This version performs simple string replacement and is common on CentOS, Fedora, and Arch Linux systems.

```sh
rename jpg jpeg *.jpg
```
