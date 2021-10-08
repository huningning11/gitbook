#初次使用常见问题及解决方式

#### <a href="#knowInter">树莓派接口认识</a> 
#### <a href="#connectPi">如何连接树莓派?</a> 
#### <a href="#computerConPi">如何通过电脑连接树莓派?</a> 
#### <a href="#setPower">如何设置树莓派的显示分辨率?</a>
#### <a href="#solveConnect">连接设备显示3个或4个绿色√，如何解决?</a>
#### <a href="#uploadDown">如何保存、上传、下载和分享程序?</a>
#### <a href="#setIp">如何设置静态IP?</a>
#### <a href="#setStartUp">如何设置程序开机自启动?</a>
#### <a href="#handleProgram">运行程序卡死怎么办?</a>
#### <a href="#connectSound">如何连接蓝牙音箱?</a>
#### <a href="#soundOutput">连接音箱，没有声音输出怎么办?</a>
#### <a href="#configDiffer">树莓派不同配置的区别</a>
#### <a href="#system">系统备份与恢复</a>
#### <a href="#setAccount">如何配置账号?</a>
#### <a href="#systemBurn">如何烧录系统?</a>
#### <a href="#none">任务栏/菜单栏不显示了怎么办?</a>
#### <a href="#setTime">如何设置屏幕保护时间?</a>
#### <a href="#transFiles">传输文件没有权限怎么办?</a>
#### <a href="#remoteLogin">笔记本无法远程登录树莓派的Linux系统?</a>

## <a id="knowInter" name="knowInter">树莓派接口认识</a>

树莓派（Raspberry Pi）是一款为教学目的诞生的ARM架构的微型计算机，基于Linux系统。由美国树莓派基金会开发。

树莓派就是一个微型电脑，里面的操作系统为 Linux，Linux 和我们常见的 Windows 一样，用于操作电脑硬件，接受用户输入并输出反馈。

以下是树莓派的接口示意图。

<img src="/media/shumeipjiekou.png"  align = "center" width="80%">
<h5 align = "center">树莓派接口示意图</h5>


## <a id="connectPi" name="connectPi">如何连接树莓派?</a>

连接好鼠标键盘，插入 SD 卡。HDMI 连接显示器。最后插入电源。

## <a id="computerConPi" name="computerConPi">如何通过电脑连接树莓派?</a>

首先确保树莓派和电脑在同一个局域网内，即连接的是同一个WiFi，即可通过登录古德微平台使用账号进行登录，就进入如下界面

<img src="/media/shumeipailianjie.png"  align = "center" width="80%">
<h5 align = "center">树莓派连接图</h5>

然后点击设备控制，即可进入如下界面

<img src="/media/lianjietu2.png"  align = "center" width="80%">
<h5 align = "center">连接图2</h5>

然后将树莓派的电源接通，随后点击连接设备即可，这样就完成了树莓派与电脑的连接

## <a id="setPower" name="setPower">如何设置树莓派的显示分辨率?</a>

首先将树莓派的常规连接都连接完毕，即鼠标、键盘、显示器与电源，并记得插入SD卡，连接成功后，就点击首选项里Main Menu Edior这个选项，如下图所示

<img src="/media/fenbianlv1.png"  align = "center" width="80%">
<h5 align = "center">图1</h5>

然后点击首选项里的显示器设置，如下图所示

<img src="/media/fenbianlv2.png"  align = "center" width="80%">
<h5 align = "center">图2</h5>

然后再次进行第一步的操作，点击首选项，我们就可以看到多了一个显示器设置，如下图所示

<img src="/media/fenbianlv3.png"  align = "center" width="80%">
<h5 align = "center">图3</h5>

点击之后，这里就是设置分辨率的地方，就可以对树莓派进行分辨率的设置了，如下图所示。

<img src="/media/fenbianlv4.png"  align = "center" width="80%">
<h5 align = "center">图4</h5>

选择好之后，点击应用即可。

## <a id="solveConnect" name="solveConnect">连接设备显示3个或4个绿色√，如何解决?</a>

如果在连接设备的过程中，出现3个或者4个√的情况，一般是由于网络的原因，我们需要检查一下所处环境的网络是否畅通，也可能是树莓派在启动的时候，还没有完全启动，所以我们可以重启树莓派并灯带一两分钟，再次尝试连接设备即可。

## <a id="solveConnect" name="solveConnect">如何远程登录树莓派桌面?</>

远程登录树莓派桌面需要进行先行调试，我们需要将新建一个手机热点，名称为gdwteaching,密码为12344321，让电脑和树莓派处于同一个局域网即可，然后就进行正常的登录账号连接设备即可。

## <a id="uploadDown" name="uploadDown">如何保存、上传、下载和分享程序?</a>

保存文件点击界面右上角的保存按钮即可。如下图所示。

<img src="/media/baocun.png"  align = "center" width="50%">
<h5 align = "center">保存</h5>

下载程序即在代码库中选择相应的代码并进行下载即可

<img src="/media/xiazai.png"  align = "center" width="50%">
<h5 align = "center">下载</h5>

将下载的程序文件上传，即点击菜单栏右侧的上传按钮即可

<img src="/media/shangchuantu.png"  align = "center" width="50%">
<h5 align = "center">上传</h5>

分享程序即可在界面的右侧点击，输入分享的对象账户名，进行分享即可。

<img src="/media/fenxiang2.png"  align = "center" width="50%">
<h5 align = "center">分享</h5>

## <a id="setIp" name="setIp">如何设置静态IP?</a>

在把玩树莓派的过程中，有时需要手动给它设定一个静态的 IP 地址，一来可以防范 DHCP 自动分配的IP 来回变动，导致远程登陆时常无法连接；二来还可以提高树莓派的网络连接速度。

输入：sudo vim /etc/dhcpcd.conf，打开 dhcpcd.conf 文件后，找到如下图代码：

<img src="/media/yangliip1.png"  align = "center" width="80%">
<h5 align = "center">样例1</h5>

删除前面的注释符号”#”，指定无线接口wlan0，并修改为如下图所示：

<img src="/media/yangliip2.png"  align = "center" width="80%">
<h5 align = "center">样例2</h5>

注意：

手动静态 IP 要注意不能跟路由器 DHCP 所自动分配的 IP 冲突， 否则树莓派就有可能无法正常联网。

24位的意思就是24个二进制的1，是这样的：11111111.11111111.11111111.00000000，换算成十进制的表示就是：255.255.255.0

28位：11111111.11111111.11111111.11110000，换算成十进制为255.255.255.240

30位：11111111.11111111.11111111.11111100，换算成十进制为255.255.255.252

## <a id="setStartUp" name="setStartUp">如何设置程序开机自启动？</a>

1、	在Windows的文件资源管理器地址输入自启动文件夹地址；
C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp;
或者%programdata%\Microsoft\Windows\Start Menu\Programs\Startup二选一

<img src="/media/qidong1.png"  align = "center" width="80%">
<h5 align = "center">图1</h5>

2、	就可以在打开Windows10的程序启动文件夹，将要开机自动启动的程序软件创建开解方式；

<img src="/media/qidong2.png"  align = "center" width="80%">
<h5 align = "center">图2</h5>

3、	然后将程序快方式复制到StartUp文件夹下面；

<img src="/media/qidong3.png"  align = "center" width="80%">
<h5 align = "center">图3</h5>

4、	提示需要提供管理员权限才能移动此文件夹，当前登录账号操作需要有管理员权限，点击继续；

5、	这样的快捷方式就放在了StartUp文件夹下面，若要开机自动启动多个软件，就可以继续重复上面的操作；

<img src="/media/qidong4.png"  align = "center" width="80%">
<h5 align = "center">图4</h5>

6、	同样的在Windows任务管理器中也可以看到启动项，任务栏右键-任务管理器；

<img src="/media/qidong5.png"  align = "center" width="80%">
<h5 align = "center">图5</h5>

7、	在启动中可对已加入开机自动启动的程序进行管理，删除开机自动启动，或禁用开机自动启动软件。

<img src="/media/qidong6.png"  align = "center" width="80%">
<h5 align = "center">图6</h5>

以上即是win10系统设置某软件为开机自动启动的方法。

## <a id="handleProgram" name="handleProgram">运行程序卡死怎么办?</a>

如果遇到运行程序卡死的情况，最直接的方法就是重启树莓派

## <a id="connectSound" name="connectSound">如何连接蓝牙音箱?</a>

在显示器的右上端，点击蓝牙标志，打开蓝牙，然后与蓝牙音箱进行配置。

## <a id="soundOutput" name="soundOutput">连接音箱，没有声音输出怎么办?</a>

没有声音可能是音箱没电了，所以需要给音箱进行充电。

## <a id="configDiffer" name="configDiffer">树莓派不同配置的区别</a>

目前主要有以下型号的树莓派: the Pi 3 Model B, the Pi 2 Model B, the Pi Zero, the Pi Zero W and the Pi 1 Model B+ and A+.

<img src="/media/shumeipaipeiz.png"  align = "center" width="80%">
<h5 align = "center">树莓派的不同配置</h5>

Raspberry Pi Model A+是树莓派的低成本版本。它有512MB RAM（截至2016年8月：早期型号有256MB），一个USB端口，40个GPIO引脚，没有以太网端口。

Raspberry Pi Model B+是原始树莓派的最终修订版。它有512MB RAM，4个USB端口，40个GPIO引脚和一个以太网端口。

2015年2月，它被第二代Raspberry Pi 2 Model B取代。Raspberry Pi 2最初使用900MHz四核Arm Cortex-A7 CPU，并有1GB RAM。一些最新版本的Raspberry pi2（v1.2）现在使用900MHz的Arm Cortex-A53 CPU。

Raspberry Pi 3 Model B在2016年二月发布. 使用1.2GHz 64位4核Arm Cortex-A53处理器,有1GB的内存,集成了802.11n的无线网络以及4.1版本的蓝牙.

Raspberry Pi 3 Model B+在2018年3月发布.使用1.4GHz 64位4核Arm Cortex-A53处理器,有1GB的内存,千兆有线网口,集成了802.11ac/n无线网络和4.3版本的蓝牙.

Raspberry Pi 4 Model B在2019年6月发布.使用1.5GHz64位4核Arm Cortex-A72处理器,内存有不同大小的版本(2GB,4GB,8GB),千兆有线网络口,集成了802.11ac/n无线网络和5.0版本蓝牙.初始发布的版本使用的是1GB内存,后续使用2GB代替但价格不变.

Raspberry Pi Zero和Raspberry Pi Zero W/WH大小只有Model A+的一半,使用1GHz单核处理器和512M内存,以及mini-HDMI,USB OTG接口和摄像头连接器.Raspberry Pi Zero W还集成了802.11n无线网络和4.1版本蓝牙.Raspberry Pi Zero WH 和 Zero W是一样的,只是多了焊接好的插针而已.

Model A/A+只有一个USB接口,Model B有两个,而Model B+, Raspberry Pi 2 Model B, 和Raspberry Pi 3 Model B 有4个USB接口.因此可以连接大多数的USB2.0设备.像鼠标键盘,网课,外置存储卡都可以通过USB连接.Raspberry Pi Zero 和Raspberry Pi Zero W只有一个micro USB的接口,要用USB OTG的线去连接设备.

树莓派版本中还有Compute Module(没有在上面的列表中列车),用于工业应用,尺寸更小,可方便的嵌入主板中，例如工业产品中的电路板，为制造商提供了在自己的设备中使用树莓派生态系统的简单方法。

## <a id="system" name="system">系统备份与恢复</a>

为了大家更容易上手，古德微为大家准备好了系统镜像。以下介绍系统备份和恢复的方法。

1. 备份前准备

安装了系统的TF卡

在Windows系统下载安装 Win32DiskImager 软件

2. 使用 Win32DiskImager 备份

先新建一个空白的.img 后缀的文件(注意：路径名和文件名不能含有中文)。比如：我在 E 盘imageBack目录下新建了一个”raspberrypi.img”文件。

备份系统可以分为三步。第一步，选择含系统的TF 卡；第二步，选择下载好的镜像文件；第三步，点击“读取”（Read）。

<img src="/media/beifen1.png"  align = "center" width="80%">
<h5 align = "center">系统的备份与修复</h5>

镜像备份

注意：

使用 Win32DiskImager 备份属于全盘备份(无压缩)，即 16G TF 卡备份完成后的镜像文件也是 16G 左右；

备份时一定不要点击写入（Write），否则 TF 卡中的系统和文件将不复存在

3. 使用 win32DiskImager 恢复

恢复系统也可以分为三步。第一步，选择新的TF 卡/已格式化的TF 卡；第二步，选择之前备份的镜像文件；第三步，点击“写入”（Write）。

格式化 TF 卡

这里主要说一下格式化 TF 卡的方法。(注意：重新烧录其他系统需要先格式化，只使用 Windows 本身的格式化方法是不能解决问题的，格式化会清空SD卡的所有数据)

格式化 SD 卡

打开 SDFormatter 工具格式化 TF(MicroSD)卡，如下图所示：

<img src="/media/beifen2.png"  align = "center" width="80%">
<h5 align = "center">系统的备份与修复</h5>

格式化

格式化完成后，等待片刻，重新插上 SD 卡，即可在我的电脑看到 SD 卡原空间大小。

注意：

建议连续格式化两遍，第二遍格式化时请把 Volume Label里的文字清空，特别有时boot可能会变成乱码。这样可以确保格式化成功

## <a id="setAccount" name="setAccount">如何配置账号?</a>

###基本步骤：

1.	开机登录：首先确保需要配的账号已经开通好了，还没开账号的通知技术人员开通，然后拿需要配置账号的SD卡插到树莓派上，开机，单击左上角的浏览器；再单击浏览器左上角的书签GDWRobot，进入平台登录界面，输入要配置的账号和密码（初始密码为123456），单击登录。

<img src="/media/peizhi1.jpg"  align = "center" width="80%">
<h5 align = "center">图1</h5>

<img src="/media/peizhi2.png"  align = "center" width="80%">
<h5 align = "center">图2</h5>

登录之后界面如下:

<img src="/media/peizhi3.png"  align = "center" width="80%">
<h5 align = "center">图3</h5>

2.	新建设备：单击我的设备，可以看到新账号是没有设备的，需要新建设备（如果是旧账号就已经有设备存在，不需要新建设备，直接跳到第3步下载配置文件），单击左边的蓝色按钮“+设备”，会弹出弹窗，设备编号是要配置的账号，设备类型选择智能小车，单击确定，弹出创建成功的提示信息，并且设备栏显示已经建好的设备。

<img src="/media/peizhi4.png"  align = "center" width="80%">
<h5 align = "center">图4</h5>

<img src="/media/peizhi5.png"  align = "center" width="80%">
<h5 align = "center">图5</h5>

<img src="/media/peizhi6.png"  align = "center" width="80%">
<h5 align = "center">图6</h5>

3.	下载配置文件：在设备栏里点击蓝色按钮“配置文件”，浏览器会自动下载配置文件config.txt。

<img src="/media/peizhi7.png"  align = "center" width="80%">
<h5 align = "center">图7</h5>

4.	找到并检查配置文件：打开任务栏上的文件管理器，双击打开Downloads文件夹，看到有刚刚下载的config.txt文件（若文件夹里原先也有config.txt，那最新下载的文件为config(1).txt，需要将原来的config.txt删除，将config(1).txt重命名为config.txt），双击config.txt文件打开检查一下里面的账号信息是否正确，检查无误就关闭文件。

<img src="/media/peizhi8.png"  align = "center" width="80%">
<h5 align = "center">图8</h5>

<img src="/media/peizhi9.png"  align = "center" width="80%">
<h5 align = "center">图9</h5>

<img src="/media/peizhi10.png"  align = "center" width="80%">
<h5 align = "center">图10</h5>

<img src="/media/peizhi11.png"  align = "center" width="80%">
<h5 align = "center">图11</h5>

6.	更新配置文件：关闭config.txt之后，右键单击文件，选择剪切，返回上一层文件目录，找到back文件夹，将config.txt粘贴到back文件里，若已有同名文件，直接覆盖。

<img src="/media/peizhi12.png"  align = "center" width="80%">
<h5 align = "center">图12</h5>

<img src="/media/peizhi13.png"  align = "center" width="80%">
<h5 align = "center">图13</h5>

7.	将SD卡扩容（因为SD卡本身是32G大小的，但是我们烧录的镜像是16G的，这样还是16G的空间是不可用的，需要利用起来。）

7.1) 在命令行里输入sudo raspi-config, 然后回车，出现如下图，

<img src="/media/hh1.png"  align = "center" width="80%">
<h5 align = "center">图14</h5>

7.2)通过键盘的上下键移动到7 Advanced Options，然后点击Enter（回车）出现如下图

<img src="/media/hh2.png"  align = "center" width="80%">
<h5 align = "center">图15</h5>

7.3)再次点击Enter，等待屏幕命令行闪烁一下，出现如下图

<img src="/media/hh3.png"  align = "center" width="80%">
<h5 align = "center">图16</h5>

7.4)然后通过键盘的右箭头按键，移动光标到Finish，按Enter，会出现下图，确实是否要立即重启，选择是，按Enter，重启树莓派。（这样第8步就可以跳过了，重启后打开文件夹，查看总空间是否已经变为28.9G，如下图）

<img src="/media/hh4.png"  align = "center" width="80%">
<h5 align = "center">图17</h5>

<img src="/media/hh5.png"  align = "center" width="80%">
<h5 align = "center">图18</h5>

8.	重启树莓派：粘贴好之后，点击左上角的树莓图标，在下拉菜单里点击最后一项Shutdown，弹框选项选择点击Reboot，将树莓派重启。

<img src="/media/hh6.png"  align = "center" width="80%">
<h5 align = "center">图19</h5>

<img src="/media/hh7.png"  align = "center" width="80%">
<h5 align = "center">图20</h5>

9.	检测连接设备：等待树莓派重启完成，然后重新点击浏览器登录古德微编程平台，登录之后点击我的设备，单击蓝色按钮“控制”，进入到图形化编程页面，点击连接设备，看看是否会弹出5个√，只有出现5个√才能进行后面的测试；若不是5个，刷新一下网页，断开重连几次，若依旧不是5个√，证明账号没有配成，需要将前面步骤再来一遍，直到登录后能连接成功。

<img src="/media/hh8.png"  align = "center" width="50%">
<h5 align = "center">图21</h5>

10.	检测基本功能：在树莓派上安插一个小灯，左侧的积木区大致点击几个部分，检查是否都能弹出子菜单，然后在积木区的基础里，拖出输出调试信息和获得版本号的语句并拼接，以及在智能硬件的常用里，拖出控制点亮小灯的语句，点击右边的绿色箭头打开黑色调试框，点击运行程序，检查调试信息框是否输出相应的SD卡版本（若无需检查SD卡版本时可忽略这一部分），以及树莓派上小灯是否点亮；

<img src="/media/qw1.png"  align = "center" width="80%">
<h5 align = "center">图22</h5>

<img src="/media/qw2.png"  align = "center" width="80%">
<h5 align = "center">图23</h5>

若一切都正常，证明账号已配置完成，再将小灯熄灭，就可以关闭树莓派了。

###稍微快一点的方法：
（进行这一步操作前提是保证当前没有未关闭的文件，以防数据丢失）

在上述步骤进行到第6步之后，不用重启树莓派，打开任务栏上的Linux终端，用命令行代码开启关闭服务替代重启的步骤（能节省些许等待树莓派重启的时间），输入sudo systemctl stop reikrobot（可以按↑键找到这句代码，向上翻不到记录就手动输入），回车，再输入sudo systemctl start reikrobot（也可以按↑键找到这句代码，向上翻不到记录就还是手动输入），再回车，返回到程序编写界面，刷新网页，再继续第8步操作往后。

<img src="/media/kyd1.png"  align = "center" width="80%">
<h5 align = "center">图1</h5>

<img src="/media/kyd2.png"  align = "center" width="80%">
<h5 align = "center">图2</h5>

<img src="/media/kyd3.png"  align = "center" width="80%">
<h5 align = "center">图3</h5>

### <a id="systemBurn" name="systemBurn">如何烧录系统?</a>

一、搭建树莓派系统

###1、下载镜像

准备好 raspbian 系统，进入官网 下载https://www.raspberrypi.org/downloads/raspbian/

有三个选项可选，分别是桌面环境+推荐软件、桌面环境、最小运行环境（目前最新的是Buster版本，如果官网更新了就下载最新的即可，要注意后面修改软件源的时候要选择Buster的源）

此处下载的是带有桌面环境的 Raspbian 系统（不需要其他推荐软件，按需下载即可）,下载的文件名是 “2019-07-10-raspbian-buster.img“。

###2、格式化TF卡

准备一张 32G TF 卡（官方建议大于4G，有条件当然越大越好），下载 SDFormatter V4.0(绿色) 或者 FormatTool 来格式化 TF 卡为 FAT32 格式。不要用 win 系统自带的格式化工具，不能够还原出原本的大小。

【2020.04.09 更新】：各位关注该文章的伙伴们，不好意思下载链接失效了，有人私信说链接指向了个病毒文件，因此将原工具的下载链接替换成指向对应的百度搜索内容。

###3、烧录镜像

下载 Win32DiskImager ，选择刚才下载的镜像，write 到已格式化好的 TF 卡中。

###4、开机！

将烧录完成的 TF 卡插入到树莓派中，同时接上 HDMI 显示器、键鼠，最后接上电源即可开机。

正常情况下，开机是直接进入到桌面环境，网络连接可以选择接入网线或者连接 wifi。

## <a id="none" name="none">任务栏/菜单栏不显示了怎么办?</a>

树莓派不小心删除/隐藏了任务栏？当找不到设定档时，LXPanel 会读取系统默认的设定。那么利用这一点，重置任务栏。

命令行输入：rm -rf ~/.config/lxpanel/LXDE-pi，删除配置文件，其中后面-pi 为用户名 如果没有改过用 户名就不管他。完成后执行 sudo reboot， 重启即可。

如果还不能解决可以直接输入：rm -rf ~/.config，将.config 目录直接删了，然后输入：sudo reboot 重启。

## <a id="setTime" name="setTime">如何设置屏幕保护时间?</a>

树莓派默认10分钟进入黑屏状态,就是我们常说的suspend状态

使用xset工具设置 : 

xset     s     off    
xset    dpms  0  0  0

在使用此命令的时候,可能会出现 xset : unable to open display "" 的问题 .

解决方案 : 

sudo vi /etc/profile

设置环境变量

export DISPLAY=:0.0 

sudo reboot 

重启后,通过xset命令执行 .

设置完成 .

## <a id="transFiles" name="transFiles">传输文件没有权限怎么办?</a>

执行以下命令即可：

sudo chown root:root /var/www/ -R

sudo find /var/www/ -type d -exec chmod 755 {} \;

sudo find /var/www/ -type f -exec chmod 644 {} \;

## <a id="remoteLogin" name="remoteLogin">笔记本无法远程登录树莓派的Linux系统?</a>

远程登录时出现"由于安全设置错误，客户端无法连接到远程计算机"，如图所示

<img src="/Appendix/issues-picture/remote-issues1.png" width="80%">

解決方法如下：

一、取得超级管理员的权限

   1、在搜索输入框中输入cmd,右键以管理员方式运行；
   
   <img src="/Appendix/issues-picture/remote-issues2.png" width="60%">
   
   
   2、出现命令提示符窗口
   
   <img src="/Appendix/issues-picture/remote-issues3.jpg" width="80%">
   
   3、运行命令net user administrator /active:yes
   
   <img src="/Appendix/issues-picture/remote-issues4.png" width="80%">
   
   4、关闭窗口，可看到已有administrator账户，需要重新注销才可切换成；
   
   <img src="/Appendix/issues-picture/remote-issues5.png" width="80%">
   
   5、点击注销，点击Administrator;
   
   6、第一次登录时会出现欢迎加载数据的过程，大约2-3分钟；
   
   7、可看到当前已是Administrator账户登录了；
   
   <img src="/Appendix/issues-picture/remote-issues6.jpg" width="80%">
   
   8、关闭的话可使用命令完成；
   
   <img src="/Appendix/issues-picture/remote-issues7.jpg" width="80%">
   
二、通过安全策略设置

   1、Win+R打开"运行"，输入secpol.msc打开"本地安全策略"（或者在"管理工具"中打开）；
   
   <img src="/Appendix/issues-picture/remote-issues8.png" width="80%">
   
   2、在本地安全策略中，打开"本地策略"下的"安全选项"；
   
   <img src="/Appendix/issues-picture/remote-issues9.jpg" width="80%">
   
   3、在右边的策略中，找到"系统加密"；将FIPS算法用于加密、哈希和签名，点击右键属性；
   
   <img src="/Appendix/issues-picture/remote-issues10.jpg" width="80%">
   
   4、将"本地安全设置"；设置为"已禁用"，在单击"应用"，后"确定"，即可实现远程控制。
   
   <img src="/Appendix/issues-picture/remote-issues11.png" width="80%">
   
三、登录远程桌面

   1、在搜索框中输入"远程桌面连接"。
     
   <img src="/Appendix/issues-picture/remote-issues12.png" width="80%">
   
   2、输入在古德微平台复制的IP,点击"连接"。
   
   <img src="/Appendix/issues-picture/remote-issues13.png" width="80%">
   
   3、在登录窗口输入用户名"pi",密码"1",点击"OK"。
   
   <img src="/Appendix/issues-picture/remote-issues14.png" width="80%">
   
   4、远程桌面连接成功。
   
   <img src="/Appendix/issues-picture/remote-issues15.png" width="80%">
   
