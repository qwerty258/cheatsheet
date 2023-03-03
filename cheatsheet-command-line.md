command line
============

Search using grep

```sh
grep -rnw ./ -e "str"
```

Batch rename

```sh
rename "s/PNG/png" *
```

emmc check

```sh
mmc cid read /sys/class/mmc_host/mmc1/mmc1\:0001/
mmc extcsd read /dev/mmcblk1 | grep -i back
```

Reset gonme app picker layout

```sh
gsettings reset org.gnome.shell app-picker-layout
```

ARP scan

```sh
sodo arp-scan -I <interface> -l
```

images to pdf

```sh
img2pdf -S A4 -o output.pdf 1.jpg 2.png
```

serial log

```sh
nohup grabserial -Q -d /dev/ttyUSB1 -T --timeformat="%Y-%m-%dT%H:%M:%S.%f" -o "~/Serial.%Y-%m-%dT%H:%M:%S.log" &
```

gcc get default include path

```sh
gcc -xc -E -v -
gcc -xc++ -E -v -
```

find file end with extension

```sh
find . -type f -name *.rs
```
