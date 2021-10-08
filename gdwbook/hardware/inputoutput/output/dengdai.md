#灯带
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识

灯带是指把LED灯用特殊的加工工艺焊接在铜线或者带状柔性线路板上面，再连接上电源发光，因其发光时形状如一条光带而得名。应用广泛：建筑物、桥梁、道路、花园、庭院、地板、天花板、家具、汽车、池塘、水底、广告、招牌、标志等领域。如图1所示。

<div align = "center">
    <img src="/media/dengdai1.jpg" width="100%">
    <h5>图1 灯带示意图</h5>
</div>

##二、硬件连接

每段灯带上都有一些小箭头，箭头所指的方向为输出端，表示信号向前传递。箭头尾部方向则为输入端，即需要我们接线的方向。以WS281X灯带为例，有GND、D0、5V三个接口，分别连接到树莓派的GND、VCC、D0（18号或12号）就可以实现对灯带的控制。如果想要更长的灯带，就可以直接将多个灯带进行首尾相连使用。此处需要注意，如果灯带过长，则需要为灯带进行独立供电，否则会出现供电不足，从而导致无法有效的控制信号或者树莓派重启，这里有个小知识，把灯带调暗则可以正常控制更多的灯。灯带细节示意图如下。

<div align = "center">
    <img src="/media/dengdaishiyitu.png" width="100%">
    <h5>图2 灯带细节图/h5>
</div>

##三、基础应用（图形化）

1、	灯带指令介绍，灯带的指令可以从智能硬件的灯带模块里进行查找。如图3所示。灯带指令的具体含义如图4所示。
<div align = "center">
    <img src="/media/dengdai3.png" width="100%">
    <img src="/media/dengdai4.png" width="100%">
    <h5>图3 4 灯带指令介绍</h5>
</div>
2、	灯带测试程序。点亮第一个灯珠，程序如下。此处需注意灯带需要刷新显示。
<div align = "center">
    <img src="/media/dengdaidengzhu.png" width="100%">
    <h5>图5 点亮一个灯珠</h5>
</div>
3. 依次点亮灯珠,程序如下。
<div align = "center">
    <img src="/media/yicidianlingdengzhu.png" width="100%">
    <h5>图6 依次点亮灯珠</h5>
</div>

4、此处为下载链接

5、依次点亮灯珠效果演示视频

[依次点亮灯烛效果演示视频](https://weibo.com/3264309324/JE31lg8uu)

##四、基础应用（Python）

准备工作-安装rpi_ws281x包：

打开控制终端，命令行形式输入：
sudo pip3 install rpi_ws281x adafruit-circuitpython-neopixel
等待安装完成，确认一下：
pip3 show rpi_ws281x adafruit-circuitpython-neopixel
如果有显示版本等信息，则表示安装无误。
或者直接使用Thonny的包管理功能，分别搜索rpi_ws281x和adafruit-circuitpython-neopixel安装。

1. 依次点亮灯珠

以下程序为实现单向流水灯程序在Python环境中的代码：
<div align = "center">
    <img src="/media/danxiangliushuid.png" width="100%">
    <h5>图7 依次点亮灯珠</h5>
</div>
2. 注意事项
<div align = "center">
    <img src="/media/zhuyishix.png" width="100%">
    <h5>图8 注意事项</h5>
</div>

##五、相关课程链接
1. [闪亮圣诞树](https://mp.weixin.qq.com/s/u03z0i1-b-ckpP4FX8BXiQ)
2. [色彩奔跑](https://mp.weixin.qq.com/s/vCSRF4DAO95t5z3pWHFL_g)
3. [气象灾害预警信号灯](https://mp.weixin.qq.com/s/S9OVm0XeyCzhPw9PcgnQlA)
4. [拔河比赛](https://mp.weixin.qq.com/s/E03d8J6rGfsipomjVMJ_Kw)