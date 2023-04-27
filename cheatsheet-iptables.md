iptables
========

# Show rules

```sh
sudo iptables  -L -v -n --line-numbers
```

# Add rules

```sh
sudo iptables -A OUTPUT -p udp -j ACCEPT
sudo iptables -A INPUT -p udp --dport 69 -j ACCEPT
sudo iptables -A INTERNAL_OUT -p udp -j ACCEPT
```

# Delete rule by number

```sh
sudo iptables -D INPUT 38
```
