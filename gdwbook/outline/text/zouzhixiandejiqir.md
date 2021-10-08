##实验一：机器人小车走直线

###1、情景引入

控制机器人走直线，从A点到B点，根据机器人的速度和AB的距离，计算行走的时间。

###2、使用材料清单

组装好的机器人小车

###3、实验步骤：

####①　主要积木块

<div align="center">
    <img src="/media/test/lineCar-pic1.png" width="80%">
</div>

####②　实现程序

树莓派端接收端程序：

<div align="center">
    <img src="/media/test/lineCar-pic2.png" width="80%">
</div>

备注：360度舵机pwm范围在500-2500之间。以pwm=1500为转速最小（0），大于和小于1500分别为正转和反转，偏离1500越大转速越快。由于每个舵机的细微差异，不同舵机相同PWM值转速会有微小差异，需要通过不断调试，使得两个舵机转速达到一致。需要注意的是，由于镜像对称的原因，左右两个轮子分别为顺时针和逆时针旋转，才能直行，因此两个舵机的pwm值要在1500两侧。


###4:课后拓展

####①如何将实现直行及停止的功能封装为函数，更方便重复使用？

<div align="center">
    <img src="/media/test/lineCar-pic3.png" width="80%">
</div>

###5:源码下载

- <a href="../../download/微课源代码/机器人小车走直线.txt" download="" target="_blank">机器人小车走直线</a>