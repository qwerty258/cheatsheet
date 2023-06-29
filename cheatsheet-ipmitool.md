ipmitool
========

Set boot device

```bash
ipmitool -I lanplus -H <HOST or IP> -U <USER> -P <PASSWORD> chassis bootdev none
ipmitool -I lanplus -H <HOST or IP> -U <USER> -P <PASSWORD> chassis bootdev pxe
ipmitool -I lanplus -H <HOST or IP> -U <USER> -P <PASSWORD> chassis bootparam get 5
```

Trigger NMI

```sh
ipmitool -I lanplus -H <HOST or IP> -U <USER> -P <PASSWORD> chassis power diag
```
