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

Remove a default routing table

```bash
ip route del default via <GATEWAY IP>
ip route del default via 128.222.1.101
```
