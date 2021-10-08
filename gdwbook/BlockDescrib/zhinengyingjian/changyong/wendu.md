#获取温度反馈积木块

![](/media/wendu01.png)

##1.功能描述

###功能简介
* 通过配置相应的参数，调用温度传感器DS18B20来测量环境的温度，单位为摄氏度。

###配置文件


* 1.进入树莓派桌面，点击进入终端，输入命令**sudo nano /boot/config.txt**按下enter进入配置文件。（注意命令nano后有空格）

![](/media/wendu06.png)

![](/media/wendu07.png)

* 2.进入配置文件后寻找**dtoverlay=w1-gpio-pullup,gpiopin=4**这样的代码，如果没有找到则在文件的最后加上这段代码，最后的gpiopin=4为DS18B20温度传感器控制信号接入口，如有需要可以改为其他口，如本例中以24号gpio口为控制口则最后数字改为24即可。

![](/media/wendu08.png)

* 3.改好配置文件后，按下ctrl+o，下方弹出保存文件名称后，再按下enter键即可保存。

###接线图


<div align="center">
    <img src="/media/wendu02.png" alt="图2" width="823">
    <h4>（图2）DS18B20温度传感器接线图</h4>
</div>  

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | VCC |Vcc|电源正极输入口|
| 2  | DQ |4号gpio|数字信号输入口（文件中为几号此处就接几号gpio）|
| 3  | GND |Gnd|电源负极输入口|

###工作环境

* 测温范围： －55℃～+125℃，固有测温误差1℃；
* 工作电源: 3.0~5.5V/DC （可以数据线寄生电源）；
* 在使用中不需要任何外围元件；

###参数说明
* 无参数

###返回值
* 返回结果：返回温度传感器所测数字，单位摄氏度℃；
* 变量类型：浮点型（数字）。


###积木块应用
<div align="center">
    <img src="/media/wendu09.png" alt="图3" width="632">
    <h4>（图3）温度传感器积木块测试</h4>
</div>  



##2.案例代码下载
* <a href="../download/积木块说明案例源代码/wenduanli1.txt" download="" target="_blank">温度传感器积木块案例</a>
