GRUB2
=====

# openSUSE

```sh
sudo grub2-set-default  # set default boot menu
sudo grub2-once --list  # list all boot menu
sudo grub2-mkconfig     # update grub2 config file for boot
```

## set default example

```sh
> sudo grub2-once --list
     0 openSUSE Leap 15.5
     1 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 6.5.8-150500.55.31-default
     2 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 6.5.8-150500.55.31-default (recovery mode)
     3 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.55.31-default
     4 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.55.31-default (recovery mode)
     5 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.53-default
     6 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.53-default (recovery mode)
     7 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150400.24.88-default
     8 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150400.24.88-default (recovery mode)
     9 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.3.18-150400.24.81-default+
    10 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.3.18-150400.24.81-default+ (recovery mode)
> sudo grub2-set-default "Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.55.31-default"
```

## set boot once

```sh
> sudo grub2-once --list
     0 openSUSE Leap 15.5
     1 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 6.5.8-150500.55.31-default
     2 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 6.5.8-150500.55.31-default (recovery mode)
     3 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.55.31-default
     4 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.55.31-default (recovery mode)
     5 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.53-default
     6 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150500.53-default (recovery mode)
     7 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150400.24.88-default
     8 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.14.21-150400.24.88-default (recovery mode)
     9 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.3.18-150400.24.81-default+
    10 Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 5.3.18-150400.24.81-default+ (recovery mode)
> sudo grub2-once "Advanced options for openSUSE Leap 15.5>openSUSE Leap 15.5, with Linux 6.5.8-150500.55.31-default"
```
