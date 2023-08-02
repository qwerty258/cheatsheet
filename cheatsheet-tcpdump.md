tcpdump
=======

# Dump on specific interface

```sh
tcpdump -i <interface>
```

# Dump as a file for Wireshark

```sh
tcpdump -i <interface> -s 65535 -w <file>
```
# To capture any traffic sent to or from a given MAC address,

```sh
tcpdump ether host e2:a0:71:60:e5:2a

```
