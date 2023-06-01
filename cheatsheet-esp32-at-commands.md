ESP32 AT Commands
=================

```bash
AT+RESTORE                                      # restores the factory default settings
AT+GMR                                          # checks version information
AT+RST                                          # restarts the module
AT+CWMODE_DEF=1                                 # set station mode
AT+CWLAP                                        # lists available APs
AT+CWJAP_DEF="SSID","Password"                  # connect to AP
AT+CWDHCP_DEF=1,1                               # set station mode with DHCP
AT+CWAUTOCONN=1                                 # auto connect
AT+CIFSR                                        # show local IP
AT+PING="10.0.1.1"                              # ping network gate


AT+CIPSTART="TCP","10.0.1.116",2048             # setup TCP to server
AT+CIPMODE=1                                    # set UART-WIFI passthrough mode
AT+CIPSEND                                      # enter UART-WIFI passthrough mode
AT+SAVETRANSLINK=1,"10.0.1.116",2048,"TCP"      # save configuration in WIFI mode

AT+UART_DEF=115200,8,1,0,0

AT+CIPSTART="TCP","10.0.1.99",3333

AT+SAVETRANSLINK=1,"10.0.1.99",3333,"TCP"

AT+CIUPDATE
```
