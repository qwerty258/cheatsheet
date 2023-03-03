Bringing CAN interface up
=========================

https://elinux.org/Bringing_CAN_interface_up

# Introduction

SocketCAN provides several CAN interface types:

- virtual interfaces like vcan0
- native (real hardware) interfaces like can0
- SLCAN based interfaces like slcan0

# Virtual Interfaces

Virtual CAN interfaces will be brought up via iproute2 ip utility:

```sh
modprobe vcan
sudo ip link add dev vcan0 type vcan
sudo ip link set up vcan0
```
modprobe is needed in the case the driver is sill not loaded.

# Native Interfaces
In most cases you won't need to load the kernel driver for your real hardware. So let us concentrate on ip invocation:

```sh
sudo ip link set can0 type can bitrate 125000
sudo ip link set up can0
```

Aside from bringing interface up it is important to specify bitrate (assumes that CONFIG_CAN_CALC_BITTIMING is enabled in kernel)

# SLCAN based Interfaces

SLCAN based device provide a serial interface. At first you'll need a special daemon (slcand from can-utils), that will link this serial interface with a virtual CAN device. By default these devices get slcan name base. This is an example for a USB-to-CAN adapter working at 3Mbit/s:

```
sudo slcand -o -s8 -t hw -S 3000000 /dev/ttyUSB0
sudo ip link set up slcan0
```

So far there is no way to set bitrate for SLCAN based devices via ip tool, so you'll have to do this by slcand invocation: -sX parameter. -s8 in the above example will set adapter's bitrate to 1Mbit/s. See the table below for further CAN bitrates:

| ASCII Command | CAN Bitrate   |
|---------------|---------------|
| s0            | 10 Kbit/s     |
| s1            | 20 Kbit/s     |
| s2            | 50 Kbit/s     |
| s3            | 100 Kbit/s    |
| s4            | 125 Kbit/s    |
| s5            | 250 Kbit/s    |
| s6            | 500 Kbit/s    |
| s7            | 800 Kbit/s    |
| s8            | 1000 Kbit/s   |
