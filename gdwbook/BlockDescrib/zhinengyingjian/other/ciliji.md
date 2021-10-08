#磁力计积木块

![](/media/ciliji01.png)


##1.功能描述

###功能简介
* 采用GY-271三轴磁力传感器检测各轴数据和检验磁场大小。
***
![](/media/ciliji03.png)

功能简介：输出磁力计各轴的检测数据，可选择xyz三轴；

参数一：选择xzy三轴之一输出数据；

返回值：返回选择轴的磁力数据；数据类型：整型（数字）；
***
![](/media/ciliji04.png)

功能简介：获取磁力检测结果，当磁场大于3000时输出1，否则输出0；

返回值：0或1；整型（数字）；
###接线图

<div align="center">
    <img src="/media/ciliji02.png" alt="图1" width="687">
    <h4>（图1）磁力计连接图</h4>
</div>  



|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | VCC |VCC|电源正极输入口|
| 2  | GND |GND|电源负极输入口|
| 3  | SCL |CLK|I2C时钟信号输入口|
| 4  | SDA |DATA|I2C数据信号输入口|

###传感器参数
型号：GY-271

使用芯片：HMC5883L

供电电源：3-5v

通信方式：IIC通信协议

测量范围：±1.3-8 高斯


###积木块应用
<div align="center">
    <img src="/media/ciliji05.png" alt="图2" width="373">
    <h4>（图2）磁力计检测</h4>
</div>  





##2.案例代码下载
* <a href="../download/积木块说明案例源代码/cilijianli1.txt" download="" target="_blank">磁力计检测</a>
