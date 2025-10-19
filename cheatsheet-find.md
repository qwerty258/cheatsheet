find
====

```sh
find . -name test.txt                           # find file
find . -type f -name *.rs                       # find file end with extension
find . -type f -name "*.txt" -delete;           # find file and delete 
find . -type f -name "*.txt" -exec mv "{}" . \; # find file and move to current directory
```
