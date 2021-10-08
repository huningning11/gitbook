#光敏传感器积木块

![](/media/guangmin01.png)

##1.功能描述

###功能简介

* 光敏传感器又叫光敏电阻器或者光感电阻，其工作原理是基于内光电效应。光敏传感器是利用光电元件作为检测元件的传感器。它首先把被测量的变化转化成光信号的变化，然后借助光电元件进一步将光信号转化成电信号。

###接线说明

####1-实物图

<div align="center">
    <img src="/media/guangmin04.png" alt="图1" width="400">
    <h4>（图1）光敏传感器实物图</h4>
</div>  

####2-接线图

<div align="center">
    <img src="/media/guangmin05.jpg" alt="图2" width="400">
    <h4>（图2）一代扩展板光敏传感器连接图</h4>
</div>

***

<div align="center">
    <img src="/media/guangmin06.jpg" alt="图3" width="400">
    <h4>（图3）二代扩展板光敏传感器连接图</h4>
</div>

***

<div align="center">
    <img src="/media/guangmin07.jpg" alt="图4" width="400">
    <h4>（图4）集成扩展板光敏传感器连接图</h4>
</div>

* 集成扩展板自带光敏传感器；

***
* 光敏传感器可同时输出高/低电平数值（即通过DO引脚输出0或1）以及亮度模拟数值（即通过AO引脚输出0-32767）。如果我们只需要简单的判断所处环境是否明亮，我们可以只连接光敏传感器获得其电平数值，如若所处环境明亮，则电平数值为1，反之，则电平竖直为0；但是如果我们需要进一步获取所处环境的亮度值，那么仅有光敏传感器就不够，还需要再接入A/D转换器，将得到的模拟数值转换成数字数值并输出至调试窗口。

####3-接口定义

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | A0 |A0|模拟信号输出口|
| 2  | D0 |D|数字信号输出口|
| 3  | GND |GND|电源负极输入口|
| 4  | VCC |VCC|电源正极输入口|

###参数说明

* 积木输入参数表不同的信号输出端口；

###返回值


* 返回值：0表示环境没达到一定亮度，1表示环境达到一定亮度；
* 输出范围：0，1；
* 数据类型：整型（数字）；




###积木块应用

<div align="center">
    <img src="/media/guangmin02.png" alt="图5" width="800">
    <h4>（图5）光敏传感器测试</h4>
</div>

##2.综合运用案例
<div align="center">
<img src="/media/guangmin03.png" alt="图6" width="395">
    <h4>（图6）光敏传感器控制小灯</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/guangminanli1.txt" download="" target="_blank">光敏传感器测试</a>
* <a href="../download/积木块说明案例源代码/guangminanli2.txt" download="" target="_blank">光敏传感器控制小灯</a>