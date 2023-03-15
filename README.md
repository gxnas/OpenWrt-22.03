<h1 align="center">OpenWrt 22.03 云编译</h1>
<p align="center">
<a href="https://github.com/gxnas/OpenWrt-22.03/actions/workflows/OpenWrt-22.03-X86-64.yml">
    <img src="https://github.com/gxnas/OpenWrt-22.03/actions/workflows/OpenWrt-22.03-X86-64.yml/badge.svg?style=flat" />
</a>
<p>



### 特性

- 基于原生 OpenWrt 22.03 编译，默认管理地址192.168.1.1
- 默认开启了 Software Offload
- 内置升级功能可用，物理 Reset 按键可用
- 预配置了部分插件<b>(注意，使用MosDNS同时作为广告过滤手段及dns分流措施。)</b>
- 可无脑 opkg kmod
- R2C/R2S核心频率1.6（交换了LAN WAN），R4S核心频率2.2/1.8（建议使用5v4a电源，死机大多数情况下，都是因为<b>你用的电源过于垃圾</b>，另外，你也可以选择使用<b>自带的app限制最大频率</b>，茄子🍆）
- O3 编译，CFLAG优化
- 插件包含：SSRP，PassWall，OpenClash，微信推送，网易云解锁，SQM，DNSProxy，网络唤醒，DDNS，迅雷快鸟，UPNP，FullCone(防火墙中开启，默认开启)，流量分载，irq优化，京东签到，Zerotier，FRPC，FRPS，无线打印，流量监控，过滤军刀，R2S-OLED
- ss协议在armv8上实现了aes硬件加速（请<b>仅使用aead加密</b>的连接方式）
- 集成并默认启用了BBRv2，LRNG
- 集成了Docker，并针对特殊问题做了一些workaround（关于如何挂载剩余空间到 /opt/docker 的姿势请自行研究） ，从非Docker版本升级至Docker版本请执行恢复出厂设置，并手动重新配置路由器；请勿在Docker版上恢复非Docker版的备份配置
- 如有任何问题，请先尝试ssh进入后台，输入fuck后回车，等待机器重启后确认问题是否已经解决 

### 下载

- 选择自己<b>设备对应的固件</b>，并[下载](https://github.com/gxnas/OpenWrt-22.03/releases)


