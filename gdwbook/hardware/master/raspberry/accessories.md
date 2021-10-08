#图解及配件选择

独木难成舟，虽说最简单的配置只需要一个树莓派、一个 TF 卡、一根充电线、一个充电头即可。可这样的”低配版”的实际使用效果并不理想。下面就简单的说一下树莓派接口情况以及配件的挑选要求。

<div align="center">
    <h4>3B 主板正面</h4>
    <img src="/media/rpi3B.jpg" width="80%">
    <hr width="80%">
</div>

<div align="center">
    <h4>3B 主板尺寸图</h4>
    <img src="/media/designRpi3B.jpg" width="80%">
    <hr width="80%">
</div>

<div align="center">
    <h4>3B+ 主板正面</h4>
    <img src="/media/rpi3B+.jpg" width="80%">
    <hr width="80%">
</div>

<div align="center">
    <h4>3B+ 主板尺寸图</h4>
    <img src="/media/designRpi3B+.jpg" width="80%">
    <hr width="80%">
</div>

<div align="center">
    <h4>4B 主板正面</h4>
    <img src="/media/rpi4B.jpg" width="80%">
    <hr width="80%">
</div>

<div align="center">
    <h4>4B 主板尺寸图</h4>
    <img src="/media/designRpi4B.jpg" width="80%">
    <hr width="80%">
</div>

4B除了性能提升，接口上有以下几点变化：

 1. 从4个USB 2 变成两个USB 2和两个USB 3。
 2. 从一个HDMI输出变成两个 Micro HDMI输出。
 3. 从Micro USB供电变成 USB-C（type-C）供电。
 
##树莓派主要配件列表

 * 树莓派

   各版本的树莓派安装系统过程和基本操作都差不多， Raspberry Pi 3 Model B容易上手，对供电或配件要求较低，容易上手。选用Pi4前建议先用3B练练手，反正玩树莓派一片肯定是不够的。

 * TF 卡

   TF 卡即 T-Flash 卡，又叫 Micro SD 卡，即微型 SD 卡。品牌的话网上一般都推荐闪迪，容量推荐 16G 以上，速度Class4 是最低要求，Class10 当然最好。 

   注意：SD 卡体积为 24mm*32mm2.1mm；TF(micro SD)卡为 15mm*11mm*1mm。

 * 充电线
   树莓派所需的充电线是 Micro USB 通用充电线，就是一般 Android 手机的电源线，建议还是买一根带开关的充电线。树莓派没有开关机按钮，只能通过连接
   /断开电源来开关机。每次都拔电源头确实很麻烦，而且可能会损坏树莓派主板的充电口。

 * 充电头

   充电头要求是 5V/(2~3A)，如果电流不足，可能会出现各种问题。所以建议买个符合标准的。

 * HDMI 线(HDMI 转VGA 线)

   HDMI 线可以说是PC 的标配，如果显示器没有 HDMI 接口，可以买一根[VGA转HDMI线](https://item.taobao.com/item.htm?spm=a1z10.3-c.w4002-22298106374.9.77e870c92n96gz&id=573042354423)， VGA 接口几乎每个显示器都有。Pi4 需要[Micro HDMI转HDMI线](https://item.taobao.com/item.htm?spm=a1z10.3-c.w4002-22298106374.12.77e870c92n96gz&id=605650092072)。

 * 显示器（HDMI 接口或者通过 GPIO 接口）

   个人推荐入手，虽然显示器不是必须的，但是刚入门的话，推荐还是加上显示器吧，特别对孩子来说有显示器简单很多。个人觉得 GPIO 口比较宝贵了，所以用的是 HDMI，接到台式机的显示屏上。另外注意，如果显示屏是 VGA 接口的话，需要HDMI 转VGA 的转接线。
   家里临时用下，用电视机也可以作为显示器的。有些一体机支持HDMI out

 * PC 外设

   USB键盘鼠标，这些有当然更好，没有也没关系，就是为了方便顺手。对于初学者建议第一次用显示器、鼠标键盘可以加快上手的进度。
 
 * PC
 
   台式机笔记本都可以，需要联网用于下载软件。PC 操作系统也是随意的， 当然我这里以使用最广泛的 Windows 为例（XP、7、8、10 都可以，我使用的是 Windows 10）。
 
 * 古德微树莓派扩展板
 
   该扩展板上面有标记各个引脚的引脚号，无需用户必需熟记树莓派上的引脚。另外，其引脚的布局是根据各种传感器的引脚而设计的，因此用户可以快速根据传感器的引脚与扩展板上的接口“对号入座”。

 * 摄像头

   树莓派自身没有集成摄像头模块，可以使用单独购买的摄像头连接到树莓派 CSI 接口。也可以购买USB摄像头。

 * 音频设备

   [USB全向麦克风](https://item.taobao.com/item.htm?spm=a230r.1.14.28.1f9553d6PWQCkO&id=607207560927&ns=1&abbucket=14#detail)，3.5mm音响

 * 各种传感器

   传感器是扩展树莓派时需要的。比如，检测声音有声音传感器； 测距避障使用超声波传感器；检测光线就得有光敏传感器；检测温度湿度需要使用温湿度传感器……

 * 外壳

   为了美观和安全着想，最好给它配个外壳避免其他小物件碰到树莓派主板而短路

 * 散热片

   若没有长时间连续使用树莓派可以不配用散热片

###树莓派必备配件

 * 树莓派
 * TF 卡
 * 充电线
 * 充电头

###树莓派作为微型电脑主机使用配件（初学者推荐）

 * HDMI 线(HDMI 转VGA 线)
 * 显示器（HDMI 接口或者通过 GPIO 接口）
 * PC 外设

###树莓派作为外部设备使用配件

 * PC（可连网）

###树莓派补充扩展配件

 * 古德微树莓派扩展板
 * 摄像头
 * 音频设备
 * 各种传感器
 * 外壳
 * 散热片
    
初次使用建议购买[古德微树莓派学习套件](https://item.taobao.com/item.htm?spm=a230r.1.14.1.1f9553d6PWQCkO&id=605097485186&ns=1&abbucket=14#detail),
套件配备了树莓派专用充电头、充电线、教学镜像、扩展板以及和课程配套的传感器。
 