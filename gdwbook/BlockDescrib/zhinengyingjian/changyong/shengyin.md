#声音传感器积木块

![](/media/shengyin01.png)

##1.功能描述

###功能简介

* 声音传感器的作用相当于一个话筒（麦克风）。该传感器内置一个对声音敏感的电容式驻极话筒。声波使得话筒内的驻极体薄膜振动，导致电容的变化，而产生与之对应变化的微小电压。这一电压随后被转化成0-5V的电压，经过A/D转换被数据采集器接受，并传送给计算机。

###接线说明

####1-实物图

<div align="center">
    <img src="/media/shengyin1.png" alt="图1" width="300">
    <h4>（图1）声音传感器实物图</h4>
</div>  

####2-接线图

<div align="center">
    <img src="/media/shengyin04.jpg" alt="图2" width="400">
    <h4>（图2）一代扩展板声音传感器连接实物图</h4>
</div>

***

<div align="center">
    <img src="/media/shengyin05.jpg" alt="图3" width="400">
    <h4>（图3）二代扩展板声音传感器连接实物图</h4>
</div>

***

<div align="center">
    <img src="/media/shengyin06.jpg" alt="图4" width="400">
    <h4>（图4）集成扩展板声音传感器连接实物图</h4>
</div>

***
* 声音传感器有三个引脚，分别是VCC、GND、OUT，因为引脚顺序与扩展板的接口顺序一致，因此可以将声音传感器直接插入扩展板。如果我们只需要判断所处环境是否有噪音，我们可以只连接该模块，并将OUT 引脚连接到任意GPIO接口，获取其电平数值即可，当声音超过一定的强度时，输出低电平0，并且两盏小灯都亮起，反之当声音低于一定强度时，输出高电平1，只有右侧一盏小灯亮起；
* 如果我们需要进一步获取所处环境的噪音强度，那么我们还需要将OUT引脚连接到模拟接口（A0或A1），在连接A/D转换器，将得到的模拟器数值转换为数字数值并输出至调试窗口（此处的连接需要用到杜邦线）。

<div align="center">
    <img src="/media/shengyin07.jpg" alt="图5" width="400">
    <h4>（图5）声音传感器外接模数转换器测声音强度</h4>
</div>

* 如图（5）所示，如需测量环境声音的强度，只需在原先连接基础上添加一个模数转换器，并将输出端口从D改为A0,A1即可。
####3-接口定义

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | OUT |D或A0/A1|信号输出口|
| 2  | VCC |VCC|电源正极输入口|
| 3  | GND |GND|电源负极输入口|

###参数说明

* 积木输入参数表不同的信号输出端口；

###返回值

* 返回值：0表示声音达到一定强度，1表示声音没有达到一定强度；使用模数转换器时，输出数字信号；
* 输出范围：0，1；
* 数据类型：整型（数字）；



###积木块应用

<div align="center">
    <img src="/media/shengyin08.png" alt="图6" width="755">
    <h4>（图6）声音传感器测声音强度</h4>
</div>

***
<div align="center">
    <img src="/media/shengyin02.png" alt="图7" width="675">
    <h4>（图7）声音传感器测试</h4>
</div>

##2.综合运用案例
<div align="center">
<img src="/media/shengyin03.png" alt="图8" width="351">
    <h4>（图8）声音传感器控制小灯</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/shengyinanli3.txt" download="" target="_blank">声音传感器测声音强度</a>
* <a href="../download/积木块说明案例源代码/shengyinanli1.txt" download="" target="_blank">声音传感器测试</a>
* <a href="../download/积木块说明案例源代码/shengyinanli2.txt" download="" target="_blank">声音传感器控制小灯</a>