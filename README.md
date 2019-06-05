一键脚本安装shadowsocks/shadowsocksR/V2Ray + 开启bbr
---

一键脚本搭建shadowsocks/shadowsocksR/V2Ray + 设置开启自启动 + 升级内核&开启bbr加速。

## 教程
1.下载一键搭建ss脚本文件，只需要执行一次，卸载ss后也不需要重新下载

git clone https://github.com/lissh/ss-fly.git

2.运行搭建ss脚本代码

ss-fly/ss-fly.sh -i [password] 1024

3.开启一键加速

ss-fly/ss-fly.sh -bbr

4.判断BBR加速有没有开启成功。输入以下命令：

sysctl net.ipv4.tcp_available_congestion_control

如果返回值为：

net.ipv4.tcp_available_congestion_control = bbr cubic reno

后面有bbr，则说明已经开启成功了。





## 支持系统
CentOS 6+

Debian 7+

Ubuntu 12+

## 使用教程
一键搭建ss/ssr：[一键脚本搭建shadowsocks+开启bbr](https://www.flyzy2005.com/fan-qiang/shadowsocks/install-shadowsocks-in-one-command/)

一键搭建V2Ray：[一键脚本搭建V2Ray+配置与优化](https://www.flyzy2005.com/v2ray/how-to-build-v2ray/)

或者参考：[Wiki](https://github.com/flyzy2005/ss-fly/wiki)

## 交流群
flyzy小站交流群：http://t.me/flyzyxiaozhan

搬瓦工用户交流群：https://t.me/banwagongusers

## 推荐的VPS
### 国外VPS
[Vultr优惠网](https://www.vultryhw.cn/)

[搬瓦工优惠网](https://www.bwgyhw.cn/)

### 国内VPS
[阿里云优惠网](https://www.aliyunyhw.com)

[腾讯云优惠网](https://www.tengxunyunyhw.com)

### VPS信息汇总
[VPS GO](https://www.vpsgo.com)
