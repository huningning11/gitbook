#sensehat传感器积木块区

![](/media/sensehat10.png)

##1.功能描述

###功能简介
* sense hat集成了很多常用的传感器，有陀螺仪-角速度传感器、加速度计—线性加速度传感器、磁力计—磁力计传感器、气压计、温度传感器、湿度传感器、8*8RGB LED矩阵和五项摇杆。
***
![](/media/sensehat11.png)
* 功能介绍：调用sensehat中的温度传感器，对环境温度进行测量；
* 返回值：返回温度值，单位为摄氏度，数据类型为浮点型（数字）；
***
![](/media/sensehat12.png)
* 功能介绍：调用sensehat中的湿度传感器，对环境湿度进行测量；
* 返回值：返回湿度值，数据类型为浮点型（数字）；
***
![](/media/sensehat13.png)
* 功能介绍：调用sensehat中的大气压传感器，对环气压进行测量；
* 返回值：返回大气压值，单位为mb，数据类型为浮点型（数字）；
***
![](/media/sensehat14.png)
* 功能介绍：调用sensehat中的指南针，陀螺仪，加速度计，对树莓派实时的姿态进行测量；
* 参数说明：参数一：输入真调用指南针模块；参数二：输入真调用陀螺仪模块；参数三；输入真调用加速度计模块；  
* 返回值：返回值一：返回指南针当前的角度，数据类型：浮点型（数字）；返回值二：获取当前欧拉角，数据类型为列表，分别显示各个方向轴上的角速度；参数三：获取加速度计x轴数据；参数四：获取加速度计y轴数据；参数五：获取加速度计z轴数据；
***
![](/media/sensehat15.png)
* 功能介绍：获取摇杆的数据，可以是方向和动作，方向有up，down，left，right，动作有pressed和released，获取摇杆数据的积木是阻塞的，也就是说当程序运行到这一步时会停下来，直到获取到摇杆数据才会执行下面的命令，如果阻塞不便于程序的编写，可以调用onStick函数来跳过阻塞，该程序只要检测到摇杆就会执行相应的程序。
* 返回值：返回字符串类型，分别是up，down，left，right，pressed和released，分别表示摇杆的上下左右按压和复位；




###积木块应用
<div align="center">
    <img src="/media/sensehat16.png" alt="图1" width="467">
    <h4>（图1）sensehat传感器测试</h4>
</div>  

##2.综合运用案例
<div align="center">
    <img src="/media/sensehat17.png" alt="图2" width="1041">
    <h4>（图2）贪吃蛇小游戏</h4>
</div>  



##3.案例代码下载
* <a href="../download/积木块说明案例源代码/sensehatanli2.txt" download="" target="_blank">sensehat传感器测试</a>
* <a href="../download/积木块说明案例源代码/sensehatanli3.txt" download="" target="_blank">贪吃蛇小游戏</a>