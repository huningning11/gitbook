#红外传感器积木块

![](/media/hongwai01.png)

##1.功能描述

###功能简介

红外传感器是一种能够感应目标辐射的红外线，并利用红外线的物理性质来进行测量的传感器。

###接线说明

####1-实物图

<div align="center">
    <img src="/media/hongwaichuanganqi.png" alt="图1" width="606">
    <h4>（图1）红外传感器实物图</h4>
</div>  

####2-接线图

<div align="center">
    <img src="/media/hongwai04.jpg" alt="图2" width="400">
    <h4>（图2）一代扩展板红外传感器实物连接</h4>
</div>


***
<div align="center">
    <img src="/media/hongwai05.jpg" alt="图3" width="400">
    <h4>（图3）二代扩展板红外传感器实物连接</h4>
</div>

***

<div align="center">
    <img src="/media/hongwai06.jpg" alt="图4" width="400">
    <h4>（图4）集成扩展板红外传感器实物连接</h4>
</div>

* 红外传感器的连接方式与红外传感器的结构有关，红外传感器有三个引脚，分别为OUT、GND、VCC，在红外线传感器与扩展板连接时，应遵循接口一一对应的原则，该红外线传感器可以直接插入古德微扩展板24号的右侧三个接口，还可以使用杜邦线与其他接口进行连接。
* 红外线传感器上有一个接收管和一个发射管，黑色为接收管，白色为发射管，还有一个旋钮可以进行旋转，以调节检测距离的长短，顺时针旋转检测距离增加，反之，逆时针旋转检测距离则减少，其检测距离为2-30cm。
* 红外线传感器接入扩展板后，需注意，当检测范围内无障碍物时，检测结果0，且右侧一盏小灯亮起，当检测范围内有障碍物时，检测结果为1，且左右两盏小灯同时亮起。



####3-接口定义

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | OUT |D|信号输出口|
| 2  | VCC |VCC|电源正极输入口|
| 3  | GND |GND|电源负极输入口|

###参数说明

* 积木输入参数表不同的信号输出端口；

###返回值


* 返回值：0表示没有检测到障碍物，1表示有检测到障碍物；
* 输出范围：0，1；
* 数据类型：整型（数字）；





###积木块应用

<div align="center">
    <img src="/media/hongwai02.png" alt="图5" width="839">
    <h4>（图5）红外传感器测试</h4>
</div>

##2.综合运用案例
<div align="center">
<img src="/media/hongwai03.png" alt="图6" width="351">
    <h4>（图6）红外传感器控制小灯</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/hongwaianli1.txt" download="" target="_blank">红外传感器测试</a>
* <a href="../download/积木块说明案例源代码/hongwaianli2.txt" download="" target="_blank">红外传感器控制小灯</a>