#常用功能

* KVM共享显示器和鼠标键盘
* 文件交换
* 静态IP设置
* 截图


##KVM共享显示器和鼠标键盘

为了更好的兼容现有机房，低成本的开展树莓派人工智能编程教育，可通过KVM共享显示器和鼠标键盘。具体请参考连接示意图：

<div align="center">
    <img src="/media/KVMconnect.png" width="80%">
    <h4>KVM连接示意图</h4>
</div>

##文件交换
可以通过FTP或U盘读取/写入数据。

###FTP
推荐一个免费好用的FTP工具： FileZilla（可支持SFTP传输）
输入树莓派IP，用户名密码点击登陆即可，其中：
     
       连接地址：以“sftp://”开头 + 树莓派IP地址 
       用户名：pi
       密码：1
       端口：22
<div align="center">
    <img src="/media/ftpconnect.png" width="80%">
    <h4>SFTP连接</h4>
</div>

###U盘

1. 插入U盘看到提示后点确定

<div align="center">
    <img src="/media/UPANinform.png" width="50%">
    <h4>U盘提示</h4>
</div>

2. 打开后可以看到U盘在media/pi/DATA目录下。

<div align="center">
    <img src="/media/mediadata.png" width="80%">
    <h4>U盘地址</h4>
</div>

3. 可以通过该目录复制粘贴文件了。

* 注意：
   如果没有看到弹出窗口，也可以到改目录下进行查找

## 静态IP设置

在把玩树莓派的过程中，有时需要手动给它设定一个静态的 IP 地址，一来可以防范 DHCP 自动分配的IP 来回变动，导致远程登陆时常无法连接；二来还可以提高树莓派的网络连接速度。

1. 输入：sudo vim /etc/dhcpcd.conf，打开 dhcpcd.conf 文件后，找到如下图代码：

<div align="center">
    <img src="/media/staticipsample.png" width="80%">
    <h4>静态IP样例 </h4>
</div>

2. 删除前面的注释符号”#”，指定无线接口wlan0，并修改为如下图所示：

<div align="center">
    <img src="/media/staticipwlan.png" width="80%">
    <h4>修改样例</h4>
</div>

* 注意：

   手动静态 IP 要注意不能跟路由器 DHCP 所自动分配的 IP 冲突， 否则树莓派就有可能无法正常联网。

   24位的意思就是24个二进制的1，是这样的：11111111.11111111.11111111.00000000，换算成十进制的表示就是：255.255.255.0
   
   28位：11111111.11111111.11111111.11110000，换算成十进制为255.255.255.240

   30位：11111111.11111111.11111111.11111100，换算成十进制为255.255.255.252   
   
## 截图
在树莓派里可以使用 scrot 命令在命令行截图。如果是远程登陆，也可以用Windows的截图工具。
截取全屏执行：

     sudo scrot

用鼠标选区域截取执行：

      sudo scrot -s

20秒后截取，参数可以自定义：

      sudo scrot -d20
   
* 注意：
  
  图片保存在/home/pi目录