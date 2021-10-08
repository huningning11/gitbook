#PS2手柄遥控器积木块区

![](/media/BD_motor0.png)

##1.功能描述

###功能简介

![](/media/BD_motorhat_enable.png)

* 设置电机驱动使能。控制电机转动前，须先是指定的电机驱动使能后，方可控制电机转动。

![](/media/BD_motorhat_control.png)

* 控制指定电机以指定速度正反转。

![](/media/BD_motorhat_stop.png)

* 关停指定电机。

###接线说明

<div align="center">
    <img src="/media/BD_motor1.png" alt="图1" width="1237">
    <h4>（图1）电机接线图</h4>
</div>  

###参数说明

![](/media/BD_motorhat_enable.png)

* 参数一：A/B或C/D，A/B为设置A和B两个电机使能或失效。C/D为设置C和D两个电机使能或失效；
* 参数二：设置使能或失效。设置为使能后方可控制电机转动，设置失效后，电机两端断开失电。

![](/media/BD_motorhat_control.png)

* 参数一：A-D，选择控制不同的电机；
* 参数二：控制电机转速，范围：0-3000；数据类型：整型（数字）；
* 参数三：正转或反转，控制电机的转动方向。

![](/media/BD_motorhat_stop.png)

* 参数一：A-D，关停制动指定电机；

###积木块应用

<div align="center">
    <img src="/media/BD_motor2.png" alt="图4" width="1245">
    <h4>（图2）控制电机过程</h4>
</div>

##2.综合运用案例
<div align="center">
    <img src="/media/BD_PS2-6.png" alt="图3" width="486">
    <h4>（图5）通过手柄控制麦克纳姆轮小车移动（部分代码）</h4>
</div>  

###案例功能简介

* 功能一：电机驱动板控制两轮子的转动。
* 功能二：PS2手柄的使用。

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/motorhat-1.txt" download="" target="_blank">电机驱动板控制电机转动</a>
* <a href="../download/积木块说明案例源代码/motorhat-2.txt" download="" target="_blank">通过手柄控制麦克纳姆轮小车移动</a>