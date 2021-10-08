#输入输出设备

输入输出设备（IO设备），是数据处理系统的关键外部设备之一，可以和计算机本体进行交互使用。

而树莓派之所以好玩，就在于其除了像电脑一样可以通过USB或HDMI等接口实现与各种电子设备的接连外，其还可以通过开放的IO引脚与其他各种电路模块、电子元件及各类传感器，实现智能化控制。

##树莓派引脚介绍

<div align="center">
    <img src="/media/GPIO-BCM.jpg.jpg" width="80%">
    <h4>树莓派引脚BCM编号模式（常用）</h4>
    <img src="/media/GPIO-BOARD.jpg" width="80%">
    <h4>树莓派引脚BOARD编号模式</h4>
</div>

树莓派一共有40个引脚，可分为6种：

 * 电源输出引脚
 
 3v3、5v分别代表3.3伏特和5伏特，是输出供电的正极，也就是我们常说的Vcc
 
 GND代表接地和输出供电的负极
 
 * GPIO
 
 GPIO（General Purpose I/O Ports）意思为通用输入/输出端口。树莓派有26个GPIO接口，其中有一部分是复用接口。
 
 * IC总线
 
 IC的正确读法为"Inter－Integrated Circuit"，主要有SDA（数据线）及SCL（时钟线）两种。
 
 * SPI总线
 
 SPI是串行外设接口（Serial Peripheral Interface）的缩写，主要有MISO（数据输入）、MOSI（数据输出）、SCLK（时钟信号）、SS（使能信号）。
 
 * UART总线
 
 UART是一种通用串行数据总线，用于异步通信，主要有RX（接收），TX（发送）。
 
 * PWM脉冲宽度调制
 
 脉冲宽度调制是一种模拟控制方式，其根据相应载荷的变化来调制晶体管基极或MOS管栅极的偏置，来实现晶体管或MOS管导通时间的改变，从而实现开关稳压电源输出的改变。