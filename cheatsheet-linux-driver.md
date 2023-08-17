Linux Driver Related Command
============================

# Insert a Module only

```sh
insmod *.ko
insmode *.ko <KEY>=<VALUE> <KEY>=<VALUE>    # insert a module with parameters
```

# Remove a Module

```sh
rmmod <MODULE NAME>
rmmod -f <MODULE NAME>  # force remove
```

# List Dynamically Loaded Modules

```sh
lsmod
```

# Process Dependency Information

```sh
depmod -n   # show dependency information only
```

# Load/Remove Module with Dependencies

```sh
modprobe <MODULE NAME>
modprobe -r <MODULE NAME>   # remove a module
```

# Print Info About Modules

```sh
modinfo <MODULE NAME>
modinfo -p <MODULE NAME>    # list modules parameters
```

# Module Info in sysfs

```sh
ls /sys/module/<MODULE NAME>/*
```
