#滑杆积木块

![](/media/huagan01.png)

##1.功能描述

###功能简介

* 滑杆实质上是一种滑动变阻器，通过滑动改变接入电路中电阻的大小从而改变输出信号的大小。

###接线说明

####1-接线图

<div align="center">
    <img src="/media/huagan2.png" alt="图1" width="1087">
    <h4>（图1）滑杆连接图</h4>
</div>  

* 由于滑杆输出的是模拟信号，而模拟信号只有通过A/D转化为数字信号后才能用软件进行处理，这一切都是通过A/D转换器（ADC）来实现的。因此在使用滑杆时，一般都要接上A/D转换器。
* 如果使用的扩展板自带模数转换器，则可直接链接滑杆使用。
***
<div align="center">
    <img src="/media/huagan3.png" alt="图2" width="821">
    <h4>（图2）一代扩展板滑杆连接实物图</h4>
</div> 

***

<div align="center">
    <img src="/media/huagan03.jpg" alt="图3" width="400">
    <h4>（图3）二代扩展板滑杆连接实物图</h4>
</div> 

***

<div align="center">
    <img src="/media/huagan04.jpg" alt="图4" width="400">
    <h4>（图4）集成扩展板滑杆连接实物图</h4>
</div> 


####3-接口定义

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | OTA |A0-A3|模拟信号输出口|
| 2  | VCC |VCC|电源正极输入口|
| 3  | GND |GND|电源负极输入口|

###参数说明

* 积木输入参数范围为0-3，表不同的信号输出端口

###返回值


* 返回值：返回表示控制信号的数字；
* 输出范围：0-32767；
* 数据类型：整型（数字）；


###积木块应用

<div align="center">
    <img src="/media/huagan02.png" alt="图5" width="759">
    <h4>（图5）滑杆测试程序</h4>
</div>

##2.综合运用案例
<div align="center">
    <img src="/media/kongzhiduoji5.png" alt="图6" width="521">
    <h4>（图6）滑杆应用程序：滑杆控制机械爪</h4>
</div> 


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/huagananli1.txt" download="" target="_blank">滑竿测试程序</a>
* <a href="../download/积木块说明案例源代码/duojikongzhianli2.txt" download="" target="_blank">滑杆应用程序</a>