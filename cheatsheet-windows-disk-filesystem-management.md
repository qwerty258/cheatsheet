Windows Disk and Filesystem Management
======================================

Open privileged command prompt.

Use SHIFT+F10 to open command prompt during windows installation.

Create EFI partition:

```bat
> DISKPART
DISKPART> LIST DISK
DISKPART> SELECT DISK #
DISKPART> CREATE PARTITION EFI SIZE=100
DISKPART> FORMAT QUICK FS=FAT32
DISKPART> ASSIGN LETTER=S
DISKPART> EXIT
> BCDBOOT X:\Windows /s S:
```

Remove assigned letter:

```bat
> DISKPART
DISKPART> REMOVE LETTER=S
DISKPART> EXIT
```

Create MSR partition:

```bat
> DISKPART
DISKPART> LIST DISK
DISKPART> SELECT DISK #
DISKPART> CREATE PARTITION MSR SIZE=16
DISKPART> EXIT
```

Delete partition:

```bat
> DISKPART
DISKPART> LIST DISK
DISKPART> SELECT DISK #
DISKPART> LIST PARTITION
DISKPART> SELECT PARTITION #
DISKPART> DELETE PARTITION [OVERRIDE]
DISKPART> EXIT
```

Format partition:

```bat
> DISKPART
DISKPART> LIST DISK
DISKPART> SELECT DISK #
DISKPART> LIST PARTITION
DISKPART> SELECT PARTITION #
DISKPART>  FORMAT  QUICK FS=NTFS UNIT=4096
DISKPART> EXIT
```

Convert to GPT:

```bat
> DISKPART
DISKPART> LIST DISK
DISKPART> SELECT DISK #
DISKPART> CONVERT GPT
DISKPART> EXIT
```

Filesystem info:

```bat
> FSUTIL FSINFO DRIVES
> FSUTIL FSINFO DRIVETYPE X:
> FSUTIL FSINFO SECTORINFO X:
LogicalBytesPerSector :                                 512
PhysicalBytesPerSectorForAtomicity :                    4096
PhysicalBytesPerSectorForPerformance :                  4096
FileSystemEffectivePhysicalBytesPerSectorForAtomicity : 4096
Device Alignment :                                      Aligned (0x000)
Partition alignment on device :                         Aligned (0x000)
No Seek Penalty
Trim Supported
Not DAX capable
Not Thinly-Provisioned
```
