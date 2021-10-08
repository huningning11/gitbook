#超声波传感器积木块

![](/media/chaoshengbo1.png)

![](/media/chaoshengbo01.png)

##1.功能描述

###功能简介
* 使用超声波传感器测距，单位是厘米。


###接线图

<div align="center">
    <img src="/media/chaoshengbo1.jpg" alt="图1" width="500">
    <h4>（图1）超声波传感器实物图</h4>
</div> 

***
<div align="center">
    <img src="/media/csb02.jpg" alt="图2" width="400">
    <h4>（图2）一代扩展板超声波传感器接线图</h4>
</div>  

***

<div align="center">
    <img src="/media/csb03.jpg" alt="图3" width="400">
    <h4>（图3）二代扩展板超声波传感器接线图</h4>
</div>  

***

<div align="center">
    <img src="/media/csb04.jpg" alt="图4" width="400">
    <h4>（图4）集成扩展板超声波传感器接线图</h4>
</div>  

***

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | VCC |Vcc|电源正极输入口|
| 2  | Trig |Trig|触发信号输入口（控制口）|
| 3  | Echo |Echo|回响信号输出口（接收口）|
| 4  | GND |Gnd|电源负极输入口|

###工作原理

* 1.给脉冲触发引脚（trig）输入一个长为10us的高电平方波；
* 2.输入方波后，模块会自动发射8个40KHz的声波，与此同时回波引脚（echo）端的电平会由0变为1；（此时应该启动定时器计时）；
* 3.当超声波返回被模块接收到时，回波引 脚端的电平会由1变为0；（此时应该停止定时器计数），定时器记下的这个时间即为超声波由发射到返回的总时长；
* 4.根据声音在空气中的速度为344米/秒，即可计算出所测的距离；测试距离=（高电平时间*声速）/2

<div align="center">
    <img src="/media/csb05.png" alt="图5" width="913">
    <h4>（图5）超声波传感器时序原理图</h4>
</div> 

###参数说明
* 无参数

###返回值
* 返回结果：返回超声波传感器于物体之间的距离，单位厘米（cm）；
* 变量类型：浮点型（数字）。


###积木块应用
<div align="center">
    <img src="/media/csbyy1.png" alt="图3" width="652">
    <h4>（图3）超声波传感器积木块应用</h4>
</div>  

##2.综合运用案例
<div align="center">
    <img src="/media/csbyy2.png" alt="图4" width="323">
    <h4>（图4）超声波测距警告</h4>
</div>  

* 5号小灯为红灯，6号小灯为黄灯，12号小灯为蓝灯，16号小灯为绿灯，当检测物体在一定距离外时，表示安全的绿灯亮，当物体逐渐靠近时，绿灯依次切换为蓝灯，黄灯，红灯来表示物体的远近程度。

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/chaoshengboanli1.txt" download="" target="_blank">超声波传感器积木块应用</a>
* <a href="../download/积木块说明案例源代码/chaoshengboanli2.txt" download="" target="_blank">超声波测距警告</a>