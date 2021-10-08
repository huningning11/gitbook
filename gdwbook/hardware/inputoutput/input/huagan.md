#滑杆电位器
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识

直线位移传感器的功能在于把直线机械位移量转换成电信号。为了达到这一效果，通常将可变电阻滑轨定置在传感器的固定部位，通过滑片在滑轨上的位移来测量不同的阻值。传感器滑轨连接稳态直流电压，允许流过微安培的小电流，滑片和始端之间的电压，与滑片移动的长度成正比。如图1所示。
<div align = "center">
    <img src="/media/huagan1.png" width="100%">
    <h5>图1 滑杆传感器</h5>
</div>

##二、硬件连接

由于滑杆输出的是模拟信号，而模拟信号只有通过A/D转化为数字信号后才能用软件进行处理，这一切都是通过A/D转换器（ADC）来实现的。因此在使用滑杆时，一般都再接上A/D转换器。
<div align = "center">
    <img src="/media/huagan2.png" width="100%">
    <img src="/media/huagan3.png" width="100%">
    <h5>图2 3 滑杆传感器连线</h5>
</div>

##三、基础应用（图形化）

1. 滑杆传感器的测试：检测在20秒内（等待1秒 x 20次重复）的滑杆位置（最小值：0 - 最大值32767）
<div align = "center">
    <img src="/media/huagan4.png" width="100%">
    <h5>图4 滑杆传感器的测试</h5>
</div>

2. 滑杆控制流水灯：永远运行程序（重复当真）直到中断或切断电源，每隔0.1秒在指定滑杆内点亮不同小灯。
<div align = "center">
    <img src="/media/huagan5.png" width="100%">
    <h5>图5 滑杆控制流水灯</h5>
</div>

##四、基础应用（Python）

A/D转换器的使用：
(1)在python编程中，要想成功使用A/D转换器，使滑杆的模拟信号转换成数字信号，首先需要下载安装此转换器的第三方库扩展包。
(2)通过相关的python语言代码，进行库的调用。
(3)进行相关调试，即可使用成功。

准备工作-A/D转换器（Adafruit-ADS1x15）第三方库的安装、卸载：
<div align = "center">
    <img src="/media/huagan6.png" width="100%">
    <img src="/media/huagan7.png" width="100%">
    <img src="/media/huagan8.png" width="100%">
    <img src="/media/huagan9.png" width="100%">
    <img src="/media/huagan10.png" width="100%">
    <img src="/media/huagan11.png" width="100%">
    <img src="/media/huagan12.png" width="100%">
    <h5>图6-12 A/D转换器（Adafruit-ADS1x15）第三方库的安装、卸载</h5>
</div>

##五、相关课程链接
1. [气象灾害预警信号灯](https://mp.weixin.qq.com/s/S9OVm0XeyCzhPw9PcgnQlA)
