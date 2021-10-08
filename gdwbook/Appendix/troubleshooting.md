# 常用功能和故障排除

## 树莓派频繁无故重启

首先排除电源问题，使用稳定电源，5V2A

## 显示器无法显示

关闭电源，确保先连接 HDMI 再开启电源

## 如何格式化 SD 卡

<div align="center">
    <img src="/media/15621369504357.jpg">
</div>

## 如何烧录镜像

<div align="center">
    <img src="/media/15621369700021.jpg">
</div>

## 远程登录

Windows 下可使用 Windows Remote Desktop
其它系统可以使用 VNC Viewer

- 系统默认用户
    - 用户名： pi
    - 密码： 1

rdp 方式默认启用。vnc 方式如果无法连接，可远程登录后执行：

```bash
sudo raspi-config
```

选择 `5 Interfacing Options`

<div align="center">
    <img src="/media/15621383082637.jpg">
</div>

接下来选择 `P3 VNC` 进行配置

<div align="center">
    <img src="/media/15621383167898.jpg">
</div>

最后保存退出即可

## FTP

FileZilla
用户名：pi
密码：1
端口：22

