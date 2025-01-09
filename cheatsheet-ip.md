IP
===

Interface up/donw

```bash
sudo ip link set <INTERFACE> up
sudo ip link set <INTERFACE> down
```
Show link details, can be used to show can interface parameters

```bash
ip -details link show <INTERFACE>
ip -details link show can0
```

Show all ip table info

```bash
ip rule list
ip route show table <table>
ip route show table all
```

Remove a default routing table

```bash
ip route del default via <GATEWAY IP>
ip route del default via 128.222.1.101
```

Add IP to interface

```
ip address add 192.168.1.100 dev eth0
```

Add route

```bash
ip route add 192.168.2.0/24 via 192.168.2.254 dev eth0
ip route add default via 192.168.1.254
```
