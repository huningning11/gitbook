
#电子开关的使用方法
##一、基础知识

电子开关可以通过树莓派上的PWM信号控制输出电压的高低，达到调节电机转速，灯的亮度的功能。通过树莓派最高可以输出5V，输出驱动能力比单纯的GPIO口的3.3V更强。

<img src="/media/switch.png" width="60%">

电子开关的参数如下：

<img src="/media/switch_params.jpg" width="60%">

##二、硬件连接
电子开关的一般接线方法如下图所示：

<img src="/media/switch_lines.png" width="60%">

##三、基础应用
下面以通过电子开关驱动TT马达为例，给大家展示具体如何使用。

1、连线

<img src="/media/switch_connect.jpg" width="60%">

其中：

DC+  ——  VCC

CTL   ——  24号引脚（其他GPIO引脚也可以）

GND  ——  GND

OUT+ ——  TT马达正极

OUT- ——  TT马达负极

2、程序

<img src="/media/switch_code.png" width="60%">

当改变PWM输出值时，马达的转速会改变。
