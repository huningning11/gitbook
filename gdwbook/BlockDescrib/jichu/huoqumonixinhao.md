#从ADS（0-3）获取模拟信号

![](/media/huoquads.png)

##1.功能描述

###功能简介

* ADS(0-3)为模拟端口
* 从模拟端口获取模拟信号


###参数说明

* 参数一：模拟端口号，范围为：0-3，变量类型为：整型，0对应A0，GPIO24端口，1对应A1，GPIO25端口。  

###返回值

* 返回结果：模拟信号的电压估值。-1表示出错了，-32767——32767对应电压-4.096——4.096v；

###使用场景

* 一般情况下需要配合ADS1115模数转换器（ADC）使用； ADC，Analog-to-Digital Converter的缩写，指模/数转换器或者模数转换器。是指将连续变化的模拟信号转换为离散的数字信号的器件。真实世界的模拟信号，例如温度、压力、声音或者图像等，需要转换成更容易储存、处理和发射的数字形式。模/数转换器可以实现这个功能，在各种不同的产品中都可以找到它的身影。
* 需要获得传感器模拟电压的值；

###模数转换器连接图

<div align="center">
    <img src="/media/moshu.png" alt="图1" width="636">
    <h4>（图1）模数转换器实物图</h4>
</div>  

<div align="center">
    <img src="/media/moshujiekou.png" alt="图2" width="1026">
    <h4>（图2）模数转换器一代扩展板连接图</h4>
</div>  
* 注意事项：模数转换器不要接反，容易烧毁；如器件因短路而发热请及时关闭电源；

***
* 二代及集成扩展板皆自带模数转换器（ADC）不需要外接

<div align="center">
    <img src="/media/mszhq01.jpg" alt="图3" width="400">
    <h4>（图3）二代扩展板模数转换器</h4>
</div>  

<div align="center">
    <img src="/media/mszhq02.jpg" alt="图4" width="400">
    <h4>（图4）集成扩展板模数转换器</h4>
</div>  

###积木块应用

<div align="center">
    <img src="/media/mszhq04.png" alt="图5" width="730">
    <h4>（图5）积木块应用</h4>
</div>  

<div align="center">
    <img src="/media/mszhq03.jpg" alt="图6" width="400">
    <h4>（图6）光敏传感器模数转换器应用</h4>
</div>  

* 选择一个需要使用模数转换器，能够输出数字信号的传感器模块（以上选择光敏传感器），如上图所示，可以在输出调试信息中得到从A0口读取到的数字信号数值；


###案例代码下载

* <a href="../download/积木块说明案例源代码/mszhq1anli.txt" download="" target="_blank">应用案例代码下载</a>