#温湿度传感器积木块

![](/media/wenshidu01.png)

##1.功能描述

###功能简介

温湿度传感器是一种装有湿敏和热敏元件，能够用来测量温度和湿度的传感器装置，有的带有现场显示，有的不带有现场显示。温湿度传感器由于体积小，性能稳定等特点，被广泛应用在生产生活的各个领域。

###接线说明

####1-实物图

<div align="center">
    <img src="/media/wenshidu1.png" alt="图1" width="651">
    <h4>（图1）温湿度传感器实物图</h4>
</div>  

####2-接线图

<div align="center">
    <img src="/media/wenshidu02.png" alt="图2" width="1139">
    <h4>（图2）温湿度传感器接线图</h4>
</div>

####3-接口定义

<div align="center">
    <img src="/media/wenshidu2.jpg" alt="图3" width="750">
    <h4>（图3）温湿度传感器接线图</h4>
</div>

###参数说明

* 参数一：表示温湿度传感器输出的GPIO信号口；
* 参数二：是否需要返回温度值，需要输入真；
* 参数三：是否需要返回湿度值，需要输入真；

###返回值


* 返回值：返回包含温度值的湿度值的列表；
* 数据类型：列表（数字）；







###积木块应用

<div align="center">
    <img src="/media/wenshidu3.png" alt="图4" width="914">
    <h4>（图4）温湿度传感器基础应用</h4>
</div>




##2.案例代码下载
* <a href="../download/积木块说明案例源代码/wenshiduanli1.txt" download="" target="_blank">温湿度传感器基础应用</a>
