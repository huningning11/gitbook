#声音传感器
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化代码展示说明，附下载链接，效果视频）

四、基础应用（Python）

五、相关课程链接

##一、基础知识
声音传感器的作用相当于一个话筒（麦克风）。它用来接收声波，显示声音的振动图像，但是不能对噪声的强度进行测量。该传感器内置一个对声音敏感的电容式驻极话筒。声波使得话筒内的驻极体薄膜振动，导致电容的变化，而产生与之对应变化的微小电压。这一电压随后被转化成0-5V的电压，经过A/D转换被数据采集器接受，并传送给计算机。声音传感器的具体图像如图1所示。
<div align="center">
    <img src="/media/shengyin1.png" width="40%">
    <h5>图1 声音传感器</h5>
</div>

##二、硬件连接
声音传感器有三个引脚，分别是VCC、GND、OUT，因为引脚顺序与扩展板的接口顺序一致，因此可以将声音传感器直接插入扩展板。如果我们只需要判断所处环境是否有噪音，我们可以只连接该模块，并将OUT 引脚连接到任意GPIO接口，获取其电平数值即可，当声音超过一定的强度时，输出低电平0，并且两盏小灯都亮起，反之当声音低于一定强度时，输出高电平1，只有右侧一盏小灯亮起；如果我们需要进一步获取所处环境的噪音强度，那么我们还需要将OUT引脚连接到模拟接口（A0或A1），在连接A/D转换器，将得到的模拟器数值转换为数字数值并输出至LOG（此处的连接需要用到杜邦线）。如下图所示。
<div align="center">
    <img src="/media/shengyin2.png" width="100%">
    <h5>图2 声音传感器的连接示意图</h5>
</div>

##三、基础应用（图形化）
1.声音传感器测试：永远运行程序（重复值为真）直到强行中断程序或切断电源，每隔0.1秒通过获取传感器输出的电平数值，并输出到LOG中。我们可以旋转电位器调节声音传感器的灵敏度，以确保数值发生变化，如图3所示。
<div align="center">
    <img src="/media/shengyin3.png" width="100%">
    <h5>图3 声音传感器测试</h5>
</div>

2.声控小灯程序：永远运行程序（重复值为真）直到强行中断程序或切断电源，每隔0.1秒直接通过获取声音传感器输出的电平数值，以控制小灯的亮灭。如若声音传感器的值为1，即所处环境的声音较强时，小灯亮起；反之，当声音传感器的输出电平数值为0，即所处环境的声音较弱时，小灯熄灭，具体程序如图4所示。
<div align="center">
    <img src="/media/shengyinchuanganqikongzhixiaodeng.png" width="100%">
    <h5>图4 声控小灯程序</h5>
</div>

3.此处为下载链接

4.声控小灯演示视频

[声控小灯演示视频](https://weibo.com/3264309324/JDTY46KC3)
##四、基础应用（Python）
1.声音控制小灯程序在Python环境下的具体代码如下：

```python
import RPi.GPIO as GPIO
import time
SOUND=23 # 声音传感器GPIO引脚
LED=6 # 小灯GPIO号
GPIO.setwarnings(Flase)
GPIO.setmode(GPIO.BCM) # 指定BCM引脚编号模式
GPIO.setup(SOUND, GPIO.IN) # 设置声音传感器的GPIO为接收信号
GPIO.setup(LED,GPIO.OUT) # 设置小灯的GPIO为输出信号
while True：
    if GPIO.input(SOUND)==1: # 判断所处环境是否有噪音
        print('SOUND=1')
        GPIO.output(LED,GPIO.HIGH) # 设置小灯GPIO为高电平
    else:
        print('SOUND=0')
        GPIO.output(LED,GPIO.LOW) # 设置小灯GPIO为低电平
    time.sleep(0.5) # 等待0.5秒
```

##五、相关课程链接
1. [声控灯](https://mp.weixin.qq.com/s/Kr42Yq3xOEmgdFXyJH42JA)
