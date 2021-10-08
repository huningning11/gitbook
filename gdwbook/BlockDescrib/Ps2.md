#PS2手柄遥控器积木块区

![](/media/BD_PS2_bk.png)

##1.功能描述

###功能简介

![](/media/BD_PS2_init.png)

* 初始化手柄遥控器，获取数据前，须先调用该积木块，该积木块在整个程序中只需调用一次即可。

![](/media/BD_PS2_result.png)

* 获取手柄遥控器上的按钮操作结果。

###接线说明  

####1-端口介绍

<div align="center">
    <img src="/media/BD_PS2-1.png" alt="图1" width="1179">
    <h4>（图1）PS2接收器引脚介绍</h4>
</div>  

####2-实物图

<div align="center">
    <img src="/media/BD_PS2-2.jpg" alt="图2" width="2243">
    <img src="/media/BD_PS2-3.jpg" alt="图2" width="750">
    <h4>（图2）PS2手柄与接收器实物图</h4>
</div>

###参数说明

![](/media/BD_PS2_init.png)

* 参数一：DAT为接收器DAT引脚与树莓派上连接的GPIO口；
  * 数据范围：2-27；数据类型为：整型（数字）。
  * 引脚说明：信号流向，从手柄到树莓派，此信号是一个8bit 的串行数据，同步传送于时钟的下降沿。信号的读取在时钟由高到低的变化过程中完成。
  
* 参数二：CMD为接收器CMD引脚与树莓派上连接的GPIO口；
  * 数据范围：2-27；数据类型为：整型（数字）。
  * 引脚说明：信号流向，从主机到手柄，此信号和 DI相对，信号是一个 8bit 的串行数据， 同步传送于时钟的下降沿。
  
* 参数三：CS为接收器CMD引脚与树莓派上连接的GPIO口；
  * 数据范围：2-27；数据类型为：整型（数字）。
  * 引脚说明：用于提供手柄触发信号。在通讯期间，处于低电平。
  
* 参数四：CLK为接收器CMD引脚与树莓派上连接的GPIO口；
  * 数据范围：2-27；数据类型为：整型（数字）。
  * 引脚说明：时钟信号，由主机发出，用于保持数据同步。

###返回值

![](/media/BD_PS2_result.png)

* 返回值为按键组合值，数据类型为：整型（数字）；
<div align="center">
    <img src="/media/BD_PS2-4.png" alt="图3" width="826">
    <h4>（图3）PS2手柄按键返回值</h4>
</div>  

* **<font color=#FF00000> 注：</font> 上图为手柄按键单独返回值，若同时按下 `4`与 `5` ,则返回值为：45。**

###通信方式
* PS2采用的是SPI通信协议，SPI是串行外设接口的缩写，是一种高速的、全双工、同步的通信总线，并且在芯片的管脚上只占用四根线（DI、DO、CS、CLK），节约了芯片的管脚，同时为PCB的布局上节省空间。

###积木块应用

<div align="center">
    <img src="/media/BD_PS2-5.png" alt="图4" width="1120">
    <h4>（图4）输出PS2手柄按键值</h4>
</div>  

* **2、拍照、截屏保存到SD卡**

##2.综合运用案例
<div align="center">
<img src="/media/BD_PS2-6.png" alt="图3" width="486">
    <h4>（图5）通过手柄控制麦克纳姆轮小车移动</h4>
</div>  

###案例功能简介

* 功能一：麦克纳姆轮小车的运动。
* 功能二：PS2手柄的使用。

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/PS2-1.txt" download="" target="_blank">输出PS2手柄的按键值</a>
* <a href="../download/积木块说明案例源代码/PS2-2.txt" download="" target="_blank">通过手柄控制麦克纳姆轮小车移动</a>