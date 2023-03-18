Firmware Backup and Burn
========================

# Backup

```bash
sudo avrdude -c stk500 -b 115200 -i 10 -p m2560 -P /dev/ttyACM0 -U flash:r:arduino_firmware.hex:I
```

- -c stk500: Arduino MEGA 2560 use the original STK500 protocol
- -b Baudrate: Baudrate
- -i 10:           ISP clock delay in ms
- -p m2560:        Chip type
- -P /dev/ttyACM0: Serial port
- -F: Overrides the signature check, do not use this
- -U flash:r:arduino_firmware.hex:i: <memtype>:r|w|v:<filename>[:format]:

`man avrdude` for more

**VERY IMPORTANT: Press the REST button immediately after running the command**

# Burn

```bash
sudo avrdude -D -c stk500 -b 115200 -p m2560 -P /dev/ttyUSB0 -U flash:w:arduino_firmware.hex
```

