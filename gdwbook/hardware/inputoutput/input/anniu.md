#按钮
##目录
一、基础知识(图文介绍)

二、硬件连接（图文介绍、注意事项等）

三、基础应用（图形化代码展示说明，附代码下载链接以及效果视频）

四、基础应用（Python）

五、相关课程链接

##一、基础知识
  按钮，是一种常用的控制元件，常用来接通或断开“控制电路”（其中电流很小），从而达到控制设备运行的一种开关，不仅如此，除去开关的用途，按钮还可以作为输入设备进行各种信息的输入，是一种非常实用的设备，如图1所示。
<div align="center">
    <img src="/media/button.png" width="80%">
    <h5>图1 按键实物图</h5>
</div>

按钮在使用中有独立式按钮和矩阵式按钮：当按钮作为开关使用，所需个数较少时，常用独立式按钮进行连接；当所需按钮个数较多时，为节省IO线数量，常用矩阵式按钮以代替独立式按钮。如图2所示
<div align="center">
    <img src="/media/buttonmatrix.png" width="80%">
    <h5>图2 矩阵式键盘</h5>
</div>

按钮的使用原理如下：按钮有两个状态：高—低电平，按钮松开时为低电平，按下时为高电平，高电平为1，低电平为0.具体状态如图3所示。
<div align = "center">
    <img src="/media/buttontest.png" width="100%">
    <h5>图3 按钮原理图</h5>
</div>

##二、硬件连接
按钮的连接方式与按钮的结构有关，按钮有三个引脚（如图4所示），分别为VCC（电源）、OUT（反馈，输出信息）、GND（地），在接入时，应遵循接口一一对应的原则。需注意，如若按钮的引脚顺序与扩展板顺序不一致，则不可直接插入，我们应使用杜邦线将按钮与树莓派对应的引脚连接，或通过古德微设计的扩展板，将按钮直接插入引脚排。以GPIO为25号的引脚排为例，如图5所示。
<div align = "center">
    <img src="/media/buttonfeetshow.png" width="100%">
    <h5>图4 按钮引脚示意图</h5>
</div>
<div align = "center">
    <img src="/media/buttonhardwareconnection.png " width="100%">
    <h5>图5 按键连线示意图</h5>
</div>

##三、基础应用（图形化）
1.按钮按下时：检测在20秒内（等待0.2秒*100次重复）用户是否按下按钮，当按钮被按下时LOG输出会显示为1，否则为0。如图6所示。
<div align = "center">
    <img src="/media/anniuanxiaceshi.png" width="100%">
    <h5>图6 按钮状态</h5>
</div>

2.按钮控制小灯：用户在10秒内（等待10秒*100次重复），当按下按钮时，小灯就会亮起来，当松开按钮或100次循环（超过10秒）结束时，小灯熄灭。积木块如图7所示。
<div align = "center">
    <img src="/media/anniukongzhixiaodeng.png" width="100%">
    <h5>图7 按钮控制小灯</h5>
</div>

3.此处为程序下载链接

4.按钮控制小灯亮灭效果演示

[按钮控制小灯亮灭效果演示](https://m.weibo.cn/status/4595043429519663?wm=3333_2001&from=10B1199020&sourcetype=qq&featurecode=newtitle)

##四、基础应用（Python）
1.按钮控制小灯程序在Python环境下具体代码如图8所示。

```python
import RPi.GPIO as GPIO
import time
LED=6 # 小灯GPIO号
KEY=25 # 按钮GPIO号
GPIO.setwarnings(Flase)
GPIO.setmode(GPIO.BCM) # 指定BCM引脚编号模式
GPIO.setup(LED,GPIO.OUT) # 设置小灯的GPIO为输出信号
GPIO.setup(KEY,GPIO.IN) # 设置按钮的GPIO为接收信号
while True：
    if GPIO.input(KEY)==1: # 判断按键是否被按下
        print('KEY=1')
        GPIO.output(LED,GPIO.HIGH) # 设置小灯GPIO为高电平
    else:
        print('KEY=0')
        GPIO.output(LED,GPIO.LOW) # 设置小灯GPIO为低电平
    time.sleep(0.5) # 等待0.5秒
```

<h5 align = "center">图8 按钮控制小灯python程序</h5>

##五、相关课程链接
1. [小按钮 大用处](https://mp.weixin.qq.com/s/5o9fUUpZfL1KMXlOVA8XhA)