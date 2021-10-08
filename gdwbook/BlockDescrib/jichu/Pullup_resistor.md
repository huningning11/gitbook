#获取（1-27）号上拉电阻按钮检测结果  

![](/media/BD_up0.png)

##1.功能描述

###功能简介
* 读取相应GPIO口的电平结果，且设置相应GPIO口的初始电平为高电平，读取结果为GPIO口的电平状态。
* 上拉就是将不确定的信号通过一个电阻嵌位在高电平，上拉的电阻同时起限流作用。

<div align="center">
    <img src="/media/BD_up1.png" alt="图1" width="280">
    <h4>（图1）上拉电阻GPIO口电路原理图</h4>
</div>  

###参数说明
* 参数一：GPIO端口号，范围为：1-27，变量类型为：整型。  

###返回值
* 返回结果：0或1。当GPIO口电平为低时，返回值为：0；当电平为高时，返回值为：1。

###使用场景
* 硬件上没有上拉电阻的按钮；
* 按钮按下状态为低电平；
* 若情况满足以上两点，使用该积木块，通过软件设置上拉电阻，使按钮未按下悬空时的电平稳定为高电平。

###积木块应用
<div align="center">
    <img src="/media/BD_up2.png" alt="图2" width="640">
    <h4>（图2）输出按钮的检测结果</h4>
</div>  

##2.综合运用案例
<div align="center">
    <img src="/media/BD_up3.png" alt="图3" width="508">
    <h4>（图3）按钮按下灯亮，松开灯灭</h4>
</div>  

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/BD_up1.txt" download="" target="_blank">输出按钮结果</a>
* <a href="../download/积木块说明案例源代码/BD_up2.txt" download="" target="_blank">控制小灯亮灭</a>