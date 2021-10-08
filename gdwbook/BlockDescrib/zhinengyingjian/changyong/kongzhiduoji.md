#控制舵机积木块区

![](/media/kongzhiduoji1.png)

![](/media/kongzhiduoji6.png)

##1.功能描述

###功能简介

* 通过输入不同的PWM值控制舵机的转速，转向或位置等参数。

###舵机介绍

* 舵机分为两种，分别时180舵机和360舵机，根据特性的不同在不同的情况下使用。
* 180舵机是一种位置（角度）伺服的驱动器，适用于那些需要角度不断变化并可以保持的控制系统。

<div align="center">
    <img src="/media/servo3.png" alt="图1" width="1226">
    <h4>（图1）180°舵机控制原理图</h4>
</div> 

* 360舵机是一种连续旋转的舵机，在有些情况下，可以当作低转速的电机使用。

<div align="center">
    <img src="/media/servo4.png" alt="图2" width="1229">
    <h4>（图2）360°舵机控制原理图</h4>
</div> 

###接线说明

####1-接线图

<div align="center">
    <img src="/media/kongzhiduoji7.jpg" alt="图3" width="400">
    <h4>（图3）一代扩展板舵机实物接线图</h4>
</div>  

***
<div align="center">
    <img src="/media/kongzhiduoji8.jpg" alt="图4" width="400">
    <h4>（图4）二代扩展板舵机实物接线图</h4>
</div>  

***
<div align="center">
    <img src="/media/kongzhiduoji9.jpg" alt="图5" width="400">
    <h4>（图5）集成扩展板舵机实物接线图</h4>
</div>  

* 舵机引脚露出铁片的一面朝向树莓派USB接口一侧；

####2-接口定义

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | 红线 |VCC或5V|电源正极输入口|
| 2  | 棕色 |GND|地线|
| 3  | 黄色 |D（18或23号gpio口）|信号控制线|

###参数说明

![](/media/kongzhiduoji2.png)

* 参数一：控制舵机所用GPIO口；
* 参数二：控制舵机输出的PWM，输出范围：500-2500.

![](/media/kongzhiduoji3.png)

* 参数一：需要停止的舵机控制口。

### 使用场景

* 180舵机常用于机械臂，机械爪的控制及拟人多足机器人的动作设计中；
* 360舵机常用作智能小车的后轮驱动。

### 注意事项

* 180舵机的使用中有时会出现舵机抖动的情况，我们只需要在180舵机到达指定位置后及时关停舵机即可。
* 360舵机以PWM输出1500为中间值，但有时中间值可能会有偏差，我们只需要参照中间值相应改控制范围即可，例如一360舵机PWM输出1400时处于不动状态，参照于1500小了100，那么舵机的控制范围就变为400-2400，中间值为1400.

###积木块应用

<div align="center">
    <img src="/media/kongzhiduoji4.png" alt="图6" width="455">
    <h4>（图6）舵机控制小灯</h4>
</div>

* 随机获取一个PWM，当舵机控制信号大于1500则5号小灯亮。

##2.综合运用案例
<div align="center">
    <img src="/media/kongzhiduoji5.png" alt="图7" width="521">
    <h4>（图7）180舵机应用：滑杆控制机械爪</h4>
</div>



##3.案例代码下载
* <a href="../download/积木块说明案例源代码/duojikongzhianli1.txt" download="" target="_blank">舵机控制小灯</a>
* <a href="../download/积木块说明案例源代码/duojikongzhianli2.txt" download="" target="_blank">滑杆控制机械爪</a>