efibootmgr
==========

# List Boot Info

```sh
efibootmgr -v
```

example:

```sh
BootCurrent: 0006
Timeout: 1 seconds
BootOrder: 0000,0006,0001,0002,0003
Boot0000* Windows Boot Manager  HD(1,GPT,32054706-21f8-495a-b99f-330a6b503d29,0x800,0x32000)/File(\EFI\MICROSOFT\BOOT\BOOTMGFW.EFI)WINDOWS.........x...B.C.D.O.B.J.E.C.T.=.{.9.d.e.a.8.6.2.c.-.5.c.d.d.-.4.e.7.0.-.a.c.c.1.-.f.3.2.b.3.4.4.d.4.7.9.5.}....................
Boot0001* debian        HD(1,GPT,7f7f5562-76d0-4deb-9953-55ae18d11df7,0x800,0x32000)/File(\EFI\DEBIAN\GRUBX64.EFI)..BO
Boot0002  debian        HD(1,GPT,c2d00cf1-d7a2-440d-9b19-4ef47e34ff16,0x800,0x18800)/File(\EFI\DEBIAN\GRUBX64.EFI)..BO
Boot0003  debian        HD(1,GPT,32054706-21f8-495a-b99f-330a6b503d29,0x800,0x32000)/File(\EFI\DEBIAN\GRUBX64.EFI)..BO
Boot0006* debian        HD(1,GPT,c2d00cf1-d7a2-440d-9b19-4ef47e34ff16,0x800,0x18800)/File(\EFI\DEBIAN\SHIMX64.EFI)
```

# Delete Bootnum

```sh
efibootmgr -b 0002 -B
```

# Set Boot Order

```sh
efibootmgr -o 0000,0001,0002,0003,0006
```

# Create New

```sh
efibootmgr -c -w -L "debian" -d /dev/sdb -p 1 -l \\EFI\\debian\\grubx64.efi
```

# Set Timeout

```sh
efibootmgr -t 10
```
