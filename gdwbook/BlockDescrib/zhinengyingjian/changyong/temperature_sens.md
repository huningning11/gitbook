#获取红外温度传感器数据

![](/media/2021.7.5.png)

##1.功能描述

###功能简介
* 使用mlx90614红外非接触式模块读取温度，单位是℃，读取的温度是红外模块朝向的位置的温度。测量值是传感器视场中所有物体的平均温度，所以越靠近温度检测口，测量值越准确。


###接线图

<div align="center">
    <img src="/media/hongwaiwendu01.jpg" alt="图1" width="400">
    <h4>（图1）一代扩展板红外温度传感器接线图</h4>
</div>  

***

<div align="center">
    <img src="/media/hongwaiwendu02.jpg" alt="图2" width="400">
    <h4>（图2）二代扩展板红外温度传感器接线图</h4>
</div>  

***

<div align="center">
    <img src="/media/hongwaiwendu03.jpg" alt="图3" width="400">
    <h4>（图3）集成扩展板红外温度传感器接线图</h4>
</div>  

###参数说明
* 无参数

###返回值
* 返回结果：获取红外温度传感器的数据，如27.35；
* 结果范围：-70—380；
* 变量类型：浮点型（数字）。

###通信方式
* 标准IIC通信协议。
###积木块应用
<div align="center">
    <img src="/media/2021.7.5.2.t.png" alt="图4" width="748">
    <h4>（图4）输出红外温度传感器的数据</h4>
</div>  

##2.综合运用案例
<div align="center">
    <img src="/media/2021.7.5.3.t.png" alt="图5" width="338">
    <h4>（图5）人体温度过高警告</h4>
</div>  

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/temperature_sensor-1.txt" download="" target="_blank">获取红外温度传感器数据</a>
* <a href="../download/积木块说明案例源代码/temperature_sensor-2.txt" download="" target="_blank">人体温度过高警告</a>