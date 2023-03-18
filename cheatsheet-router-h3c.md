Router H3C
==========

# 命令介绍

```sh
sys                                                     # 进入配置视图
dis cu                                                  # 查看当前配置
dis ip int b                                            # 查看当前所有端口地址
int vlan 1
ip address xxxx                                         # 掩码 配置管理地址及掩码
dhcp server ip-pool vlan1                               # dhcp相关配置 若路由器已配置可忽略
gateway-list 192.168.1.254
network 192.168.1.0 mask 255.255.255.0
dns-list 114.114.114.114
telnet server enable                                    # 开启telnet服务、
local-user admin class manage                           # 创建管理用户
password simple admin
service-type telnet http https                          # 服务类型
authorization-attribute user-role network-admin         # 设置管理员权限
wlan auto-ap enable                                     # 开启自动ap
wlan auto-persistent enable                             # 开启ap自动固化
dis wlan ap all                                         # 查看已经上线的ap
ip route-static 0.0.0.0 0 192.168.1.1                   # 配置到路由器的管理地址
wlan service-template wlan                              # 配置无线服务模板
ssid test                                               # 设置ssid
akm mode psk
preshared-key pass-phrase simple xxxxxxx                # 设置无线密码
cipher-suite tkip                                       # 加密方式
security-ie wpa
service-template enable                                 # 服务模板使能
wlan ap 48bd-3d98-1d60 model WA5320                     # 单个ap绑定模板
serial-id 219801A0YD8181E10472
vlan 1
radio 1                                                 # 绑定5g射频
    radio enable
    service-template wlan
radio 2                                                 # 绑定2.4G射频
    radio enable
    service-template wlan
gigabitethernet 1
gigabitethernet 2
wlan ap-group default-group                             # ap组里绑定无线服务模板
vlan 1
ap-model WA5320                                         # 设置使用的ap型号
    radio 1
    radio enable
    service-template wlan
    radio 2
    radio enable
    service-template wlan
save                                                    # 保存配置
reset saved-configuration                               # 清空配置（尖括号下）
```

# Display AP All Info

```sh
dis wlan ap al verbose
```

# H3C绑定IP地址（命令行）

以`10.0.3.1`为例，用telnet登录路由器

```sh
telnet 10.0.3.1
```

用户login和password都是admin

登录后输入sys，进入系统视图

```sh
sys
```

输入`dis ip int b`，查看当前路由器所有端口地址信息

```sh
dis ip int b
```

以`vlan 1`为例，输入`int Vlan-interface 1`，进入vlan1端口视图

```sh
int Vlan-interface 1
```

输入`dhcp server ip-pool vlan1`，进入`vlan1 dhcp`地址池

```sh
dhcp server ip-pool vlan1
```

以下列信息为例，输入`static-bind`命令，绑定 IP 和 MAC

```sh
static-bind ip-address 10.0.3.108 mask 255.255.255.0 hardware-address 8888-8888-8788
```

注：`mask`为子网掩码，`8888-8888-8788`为MAC地址且固定为`XXXX-XXXX-XXXX`格式

输入`undo static-bind`命令删除绑定的IP地址

```sh
undo static-bind ip-address 10.0.3.108
display dhcp server ip-in-use
```
