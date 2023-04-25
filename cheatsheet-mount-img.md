Mount .img File
===============

# Get Partition Layout

```sh
sudo fdisk -l *.img
```

example:

```sh
$ sudo fdisk -l openwrt-22.03.4-x86-64-generic-ext4-combined-efi.img  
GPT PMBR size mismatch (246303 != 246334) will be corrected by write.
The backup GPT table is corrupt, but the primary appears OK, so that will be used.
The backup GPT table is not on the end of the device.
Disk openwrt-22.03.4-x86-64-generic-ext4-combined-efi.img: 120.28 MiB, 126123520 bytes, 246335 sectors
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes
Disklabel type: gpt
Disk identifier: 93FFDD41-3E4A-2AC5-91B9-53E979FB5900

Device                                                  Start    End Sectors  Size Type
openwrt-22.03.4-x86-64-generic-ext4-combined-efi.img1     512  33279   32768   16M Linux filesystem
openwrt-22.03.4-x86-64-generic-ext4-combined-efi.img2   33280 246271  212992  104M Linux filesystem
openwrt-22.03.4-x86-64-generic-ext4-combined-efi.img128    34    511     478  239K BIOS boot

Partition table entries are not in disk order.
```

# Mount *.img Partition

```sh
sudo mount -o loop,offset=<offset> *.img /mnt
```

example:

```sh
# the offset is partition (start sector) * (sector size)
# 512 * 512 = 262144
mount -o loop,offset=262144   openwrt-22.03.4-x86-64-generic-ext4-combined-efi.img /mnt/part1
```
