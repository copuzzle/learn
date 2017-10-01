## 1 概述

### 1.3 TCP/IP 分层
 - 链路层 ARP
 - 网络层 IP(不可靠), ICMP
 - 运输层 TCP(可靠), UDP 
 - 应用层  

### 1.4 互联网的地址
 - A 类 0xxxxxxx(7位网络号).xxxxxxxx.xxxxxxxx.xxxxxxx (24位 主机号)
 - B 类 10xxxxxx.xxxxxxxx(14位网络号).xxxxxxxx.xxxxxxx (16位 主机号)
 - C 类 110xxxxx.xxxxxxxx.xxxxxxxx(21位网络号).xxxxxxx (8位 主机号)
 - D 类 1110xxxx.xxxxxxxx.xxxxxxxx.xxxxxxx (28位 多播组号)
 - E 类 11110xxx.xxxxxxxx.xxxxxxxx.xxxxxxx (27位 留着后用)

### 1.6 封装
当应用程序用TCP传送数据时，数据被送入协议栈中，然后逐个通过每一层直到被当作一串比特流送入网络。其中每一层对收到的数据都要增加一些首部信息（有时还要增加尾部信息）

### 1.7 分用 
就是反封装

### 1.9 端口号
16 bit的端口号来识别应用程序(2^16 个)， 类 UNIX  系统 1~1024 需要 root 权限，/etc/services 有常用服务。

## 2 链路层

### 2.1 引言
（1）为IP模块发送和接收IP数据报；
（2）为ARP模块发送ARP请求和接收ARP应答；
（3）为RARP发送RARP请求和接收RARP应答。TCP/IP支持多种不同的链路层协议，这取决于网络所使用的硬件，如以太网、令牌环网、FDDI（光纤分布式数据接口）及RS-232串行线路等。

### 2.2 以太网和IEEE 802封装
以太网和IEEE 802封装差异，还好长度一样。

