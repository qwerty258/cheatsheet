wsl
===

# List distribution ans state

```bat
wsl --list --verbose
wsl -l -v
```

# Shutdown

```bat
wsl --shutdown
```

```bat
wsl --terminate Ubuntu
```

# Mount/Unmount EXT4 Under Windows Linux Subsystem

```bat
wsl --mount \\.\PHYSICALDRIVE0 --partition 2 --type ext4
wsl --unmount \\.\PHYSICALDRIVE0
```
