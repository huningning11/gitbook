#温度传感器积木块区

![](/media/BD_temperature2_0.png)

##1.功能描述

###功能简介


温度传感器是指能感受温度并转换成可用输出信号的传感器。

###接线说明

####1-接线图

<div align="center">
    <img src="/media/BD_temperature2_1.png" alt="图1" width="884">
    <h4>（图1）温度传感器与树莓派扩展板的接线图</h4>
</div>  

####2-实物图

<div align="center">
    <img src="/media/BD_temperature2_2.png" alt="图2" width="557">
    <h4>（图2）温度传感器实物图</h4>
</div>

####3-接口定义

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | GND |GND|电源负极输入口|
| 2  | VCC |VCC|电源正极输入口|
| 3  | OUT |A0|模拟信号输出端口|



###返回值

* 返回值：测得温度值
* 数据类型：浮点型（数字）
* 输出范围：0-100





###产品特性

* 工作电压：直流4～30V；
* 工作电流：小于133μA
* 输出电压：+6V～-1.0V
* 输出阻抗：1mA负载时0.1Ω；
* 精度：0.5℃精度（在+25℃时）；
* 漏泄电流：小于60μA；
* 比例因数：线性+10.0mV/℃；
* 非线性值：±1/4℃；
* 校准方式：直接用摄氏温度校准；
* 额定使用温度范围：-55～+150℃。

###积木块应用

<div align="center">
    <img src="/media/BD_temperature2_3.png" alt="图3" width="920">
    <h4>（图3）温度传感器测试程序</h4>
</div>

##2.综合运用案例

<div align="center">
<img src="/media/BD_temperature2_4.png" alt="图4" width="439">
    <h4>（图4）通过温度传感器控制小灯</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/temperature_1.txt" download="" target="_blank">温度传感器测试程序</a>
* <a href="../download/积木块说明案例源代码/temperature_2.txt" download="" target="_blank">通过温度传感器控制小灯</a>