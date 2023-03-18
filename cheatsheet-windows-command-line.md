Windows Command Line
====================

# Turn off Hibernate

```bat
@powercfg -h off
```

# Get all File Path

```bat
DIR /A /B /S > result.txt
```

We can make this command a bat file.

Just put the bat file in desired folder and run it.

# Mount/Unmount EXT4 Under Windows Linux Subsystem

```bat
wsl --mount \\.\PHYSICALDRIVE0 --partition 2 --type ext4
wsl --unmount \\.\PHYSICALDRIVE0
```
