#LED小灯
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接
##一、基础知识
发光二极管简称为LED。由含镓（Ga）、砷（As）、磷（P）、氮（N）等的化合物制成。当电子与空穴复合时能辐射出可见光，因而可以用来制成发光二极管。在电路及仪器中作为指示灯，或者组成文字或数字显示。砷化镓二极管发红光，磷化镓二极管发绿光，碳化硅二极管发黄光，氮化镓二极管发蓝光。因化学性质又分有机发光二极管OLED和无机发光二极管LED。如图1所示。

<div align = "center">
    <img src="/media/xiaodeng1.jpg" width="80%">
    <h5>图1 LED 示意图</h5>
</div>
普通单色发光二极管具有体积小、工作电压低、工作电流小、发光均匀稳定、响应速度快、寿命长等优点，可用各种直流、交流、脉冲等电源驱动点亮。它属于电流控制型半导体器件，使用时需串接合适的限流电阻。 普通单色发光二极管的发光颜色与发光的波长有关，而发光的波长又取决于制造发光二极管所用的半导体材料。红色发光二极管的波长一般为650～700nm，琥珀色发光二极管的波长一般为630～650nm ，橙色发光二极管的波长一般为610～630nm左右，黄色发光二极管的波长一般为585nm左右，绿色发光二极管的波长一般为555～570nm。

##二、硬件连接
LED灯有长脚和短脚，长为正，短为负，在连接时需要注意，我们可以直接插入，也可以使用杜邦线进行连接。接通电源小灯就会亮起。如下图所示。

<div align = "center">
    <img src="/media/xiaodeng2.png" width="100%">
    <h5>图2 小灯连线</h5>
</div>

##三、基础应用（图形化）
1、测试小灯程序：控制小灯亮灭。通电后，16号小灯亮起，等待20秒，16号小灯熄灭。具体程序如下图所示。

<div align = "center">
    <img src="/media/xiaodeng3.png" width="100%">
    <h5>图3 控制小灯亮灭</h5>
</div>
2、控制小灯闪烁程序。在20秒内（重复10次*等待时间2秒），16号小灯亮—灭状态循环执行10次，即小灯闪烁10次。

<div align = "center">
    <img src="/media/xiaodeng4.png" width="100%">
    <h5>图4 控制小灯闪烁</h5>
</div>

3.此处为下载链接

4.小灯闪烁效果演示视频

[小灯闪烁效果演示视频](https://weibo.com/3264309324/JE2zpnlo7)

##四、基础应用（Python）

1、控制小灯亮—灭程序在Python环境中，具体代码如图所示。
<div align = "center">
    <img src="/media/xiaodeng5.png" width="100%">
    <h5>图5 控制小灯亮灭</h5>
</div>
2、控制小灯闪烁程序在Python环境中，具体代码如图所示。
<div align = "center">
    <img src="/media/xiaodeng6.png" width="100%">
    <h5>图6 控制小灯闪烁</h5>
</div>

##五、相关课程链接
1. [用树莓派点亮LED灯](https://mp.weixin.qq.com/s/YPKsdgknQozhu6Nc18yI9g)
2. [求救信号灯](https://mp.weixin.qq.com/s/Z0di6gZm36fCGzTaibXdzg)
3. [夜骑警示灯](https://mp.weixin.qq.com/s/0OHsrOX3tvGqcRjVf-VgZA)
4. [有趣的LED小灯](https://www.bilibili.com/video/BV1gv411j7CB/)