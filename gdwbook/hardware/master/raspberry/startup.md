#树莓派开机连接

简单的说一下吧，第一次使用树莓派有屏幕（显示器）的话使用自然方便。没有显示器，怎么愉快的玩树莓派？古德微的图形化编程是网页版，所以只要设置树莓派连上WIFI，在同一局域网就可以在普通电脑上打开浏览器对树莓派进行编程。

另外我们可以通过远程登陆的方式来操作你的树莓派。远程连接也必须和树莓派在同一局域网络下。

远程连接树莓派的的方法有三种：SSH 远程连接、windows远程连接、VNC 远程连接。先说有屏幕玩转树莓派的方法。

##有屏幕

这里将 TF 卡插入树莓派，注意卡的金手指应该面向 PCB。对于树莓派3B/4B， 推到底就行了。先连鼠标和键盘，再接显示器，然后打开显示器，最后插上 micro USB 电源（建议5V 3A）。

<div align="center">
    <img src="/media/piconnect.gif" width="80%">
    <h4>树莓派开机连接动画演示</h4>
</div>

树莓派开机连接上电源后，树莓派上的绿色指示灯会闪烁，说明系统正常，
显示器很快会有显示，是操作系统的加载过程。等待启动了Linux系统，会显示如下桌面。

<div align="center">
    <img src="/media/20200519142859.jpg" width="80%">
    <h4>树莓派开机后桌面</h4>
</div>

单击右上角网络图标，找到WIFI网络，输入无线网络密码，就能将树莓派连接到网络了。需要用到鼠标、键盘相配合，输入WIFI 密码。注意：如果WIFI的用户名是汉字将不能连接到网络，一定是 英文字母或数字，不能有汉字。如果没有键盘，可以单击鼠标右键，在快捷菜单中就能找到可以使用的软键盘。

用户登录在线编程平台 如下图所示，点击浏览器图标，点击左上角GDWRobot 标签进入登陆页面，登录名称见板上标签，一般为用户姓名的汉语拼音（小写），初始密码为123456。

<div align="center">
    <img src="/media/20200519143232.jpg" width="80%">
    <h4 >登陆编程平台</h4>
</div>

登陆成功后点击我的设备，选择相应设备点击连接设备，看到5个绿色对勾的提示信息表示设备连接成功，并能看到树莓派IP，即可进行接下来的图形编程操作，实现多种功能。如下图

<div align="center">
    <img src="/media/20200519143411.jpg" width="80%">
    <h4>连接设备</h4>
</div>

现在可以自由的进行图形化编程了。
具体的操作过程可以[观看微课](https://mp.weixin.qq.com/s/wMBOO5gH_Ks3cD1izhLXqg)


###注意
  * WIFI连接过一次后，下次开机可自动连上
  * PI4的电源接口是 Type C
  * PI4的显示器接口是micro HDMI，且支持连接两个显示器。优先连接靠近充电口这个micro HDMI，连接第二个显示器有些功能不能显示，比如摄像头预览界面
 
##无屏幕

古德微的图形化编程是网页版，所以只要设置树莓派连上WIFI，在同一局域网就可以在普通电脑上打开浏览器对树莓派进行编程。

有三种比较方便的连接WIFI方法
  * 使用古德微默认WIFI
  * 使用网线，有线连接
  * 修改配置文件

###使用古德微默认WIFI
1. 树莓派默认连接的是：名称为gdwteaching
                 密码为12344321  的网络。
2. 将手机热点修改为名称为gdwteaching
                      密码为12344321
树莓派供电之后就会自动连接上这个热点名称的wifi
                      
3. 笔记本也同样连接该热点；保证两个设备（树莓派和你的笔记本）都在同一个网络环境下；
                      
4. 笔记本使用谷歌浏览器(chrome)登录gdwrobot的平台（http://www.gdwrobot.cn/robot_system/）

5. 连接设备后获得树莓派IP

6. 电脑远程登陆树莓派；搜索程序远程桌面连接；登陆后，修改树莓派的无线网络为家里的无线网络；

北京回龙观第二小学 王婧老师写了一篇[详细的手顺文档](https://mc.dfrobot.com.cn/thread-304201-1-1.html)，大家可以参考。

###使用网线，有线连接
1. 用网线连接树莓派，树莓派供电之后就会自动连接网络

2. 笔记本也同样连接这一网络（wifi或者网线连接皆可）；保证两个设备（树莓派和你的笔记本）都在同一个网络环境下；

3. 参考“使用古德微默认WIFI” 4-6步。



###修改配置文件

1. 先用windows的记事本复制一下文字，
       ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
       update_config=1
       country=CN

       network={
            ssid="修改为你WIFI的名称"
            psk="修改为你WIFI的密码"
            key_mgmt=WPA-PSK
       }

2. 将文件保存为 wpa_supplicant.conf,并copy到 古德微镜像SD 卡根目录（boot 中）
      PS：如果不会修改后缀名的童鞋，可以在保存的对话框中，用英文的双引号括住文件名，文件就会按照双引号内的文件名强制保存

3. 树莓派供电之后就会自动连接上这个热点名称的wifi

4. 参考“使用古德微默认WIFI” 4-6步。

广东清远市华侨中学 余宇宙老师写了一篇[详细的手顺文档](https://www.jianshu.com/p/4912b491e44e)，大家可以参考。

##远程登陆

远程登陆有三种（同一局域网）：
1. Windows 远程桌面连接

2. VNC 远程连接树莓派

3. SSH 远程连接树莓派

比较常用的是 1 和 2，Windows 远程桌面连接的优点是不用安装额外的软件，但是速度慢一点，连显示器时远程登陆的界面和显示器的界面是不同的session。
VNC 远程连接树莓派需要在windows安装额外软件，树莓派上需要启用VNC，优点是速度快一点，且连显示器时远程登陆的界面和显示器的界面同屏，包括摄像头预览。

###Windows 远程桌面连接

1. 打开电脑，Win+r 打开运行的窗口，输入：mstsc。就可以看到远程桌面的连接窗口，我们输入树莓派的 IP 地址。树莓派IP地址在古德微编程平台点连接设备后可以看到。
    
    <div align="center">
        <img src="/media/winremote.png" width="80%">
        <h4>远程登陆</h4>
    </div>

2. 选择”是”连接到该计算机，为了避免每次连接都看到这个提示，我还勾选了”不再询问我是否连接到此计算机”。
    
    <div align="center">
        <img src="/media/remoteconfirm.png" width="80%">
        <h4>验证确认</h4>
    </div>

3. 输入树莓派用户名:pi，密码：1。
    
    <div align="center">
        <img src="/media/remoteinput.png" width="80%">
        <h4>输入用户名密码 </h4>
    </div>

4. 点击”OK”(或回车)，即可连接。


某些Windows版本不支持远程登陆功能，浙江舟山的俞含盛老师写了一篇手顺供参考[用WIN10家庭版的笔记本远程登录树莓派的Linux系统](https://mc.dfrobot.com.cn/thread-302138-1-1.html)

###VNC 远程连接树莓派
VNC 是啥？VNC 是一款使用 RFB 协定的屏幕画面分享及远程操作软件，VNC 允许您访问和控制您的桌面应用程序，无论你在世界的哪一端。VNC 远程控制软件最大的特色莫过于它的平台无关性，你可以用 Windows 电脑控制 Linux 系统或苹果的 Mac OS，反之亦同。

简单的说，使用 VNC 可以登录树莓派，并看到图形化界面。以前树莓派官方的系统并没有自带 VNC，需要单独安装，但是现在新版的官方系统已经自带VNCserver，只需要在设置里启用一下就可以用啦。这里提供两种树莓派开启VNC 的方法：

* 方法一

开启系统，在图形化界面下，依次打开 菜单(Menu) > 首选项(Preferences)> Raspberry Pi Configuration。然后点击 Interfaces 栏，选择“enable” VNC 服务。
（windows远程登陆启用VNC时，请用方法二）

* 方法二

开启系统，在命令行输入：sudo raspi-config，然后回车。在弹出的界面中，选择第五项：“5 Interfacing Options”，回车。然后选择第三项：“VNC” 并开启(enable)它。

####连接过程
1. VNC 客户端推荐使用 VNC Viewer。

2. 输入ip后，弹出窗口输入用户名密码，点OK即可

<div align="center">
    <img src="/media/VNCinput.png" width="80%">
    <h4>输入用户名密码</h4>
</div>

开启摄像头预览同步功能：
1. 在树莓派桌面右上角的VNC图标右键，选择options
    
    <div align="center">
       <img src="/media/VNCoptions.png" width="50%">
       <h4>选择options</h4>
    </div>

2. 在Troubleshooting选项启用 “启用hardware JPEG encoding”后点OK。

    <div align="center">
       <img src="/media/vncJpgcoding.png" width="50%">
       <h4>启用hardware JPEG encoding</h4>
    </div>


###SSH 远程连接树莓派

1. 在树莓派启用 SSH （和启用VNC类似）

2. 打开 PuTTY 工具后，输入IP，端口选22，然后点open连接

3. 输入用户名和密码 （密码输入时看不见的，输入密码1后直接回车即可）


###注意事项
远程 SSH/VNC 连接首先需要确认的是：
1.	你的树莓派有没有连接到网络；（古德微编程平台连接设备是否出现5个勾）
2.	使用软件时，填写的 ip、用户名和密码是否正确；(5个勾出现后，会显示ip地址)
3.	树莓派有没有开启 SSH/VNC。