journalctl
==========

```sh
journalctl --list-boots
```

```sh
journalctl -f -t <syslog identifier>
```

```sh
journalctl -f _COMM="process name" -g "string to match"
```

```sh
journalctl --vacuum-time=2d
```

```sh
journalctl -o short-iso-precise
```
