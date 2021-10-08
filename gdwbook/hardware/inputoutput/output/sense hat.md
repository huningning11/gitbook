#sense hat
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识

Sense hat即为点阵屏，树莓派主板40Pin GPIO接口提供电源和数据连接。Sense hat的常用功能有很多，sense hat集成了很多常用的传感器，有陀螺仪-角速度传感器、加速度计—线性加速度传感器、磁力计—磁力计传感器、气压计、温度传感器、湿度传感器、8*8RGB LED矩阵和五项摇杆，可以实现不同类型的实验，应用程序，甚至是游戏。Sense hat通过不同的积木实现不同的功能，它可以显示不同的字符、字符串以及点，还可以实现显示内容的清除和旋转。下图为sense hat 的示意图。

<img src="/media/sense%20hat.png"  align = "center" width="80%">
<h5 align = "center">sense hat 示意图</h5>

上图即为树莓派的多功能传感器扩展板sense hat，另外还附带了一些配件，主要用于与树莓派主板连接、固定，包括了40pin的排针插座以及一些固定柱和螺帽。


##二、硬件连接

Sense hat与树莓派的安装非常简单，我们只需借助上图中的排插即可将sense hat扩展板与树莓派主板进行连接，下面是结合后的实物图。

<img src="/media/shiwutu.png"  align = "center" width="100%">

<img src="/media/shiwutu1.png"  align = "center" width="100%">
<h5 align = "center">sense hat连接实物图</h5>

##三、基础应用（图形化）
1.	sense hat测试程序：在点阵屏上以红色点亮坐标为第三行第三列的点。

<img src="/media/sense%20hatceshi.png"  align = "center" width="100%">
<h5 align = "center">测试程序</h5>
此处我们需要注意点阵屏的坐标是从0开始的，一直到7结束，就好像我们的坐标轴一样，x轴为行，y轴为列。我们在使用积木块编写代码时需要注意。

2.	sense hat小案例
控制点阵屏上的小灯由列到行依次点亮，此处我们使用到了双层循环。

<img src="/media/shuangcengxunhuan.png"  align = "center" width="100%">
<h5 align = "center">双层循环</h5>


3.此处为程序代码下载链接

4.sense hat演示视频

[sense hat效果演示视频](https://weibo.com/3264309324/JE3ONiJvH)

##四、基础应用（Python）

暂无，后期需补充


##五、相关课程链接
[sense hat系列课程](https://mp.weixin.qq.com/s/IbySEli0unT-oFe0HJqN6Q)