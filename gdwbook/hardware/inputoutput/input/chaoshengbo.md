#超声波传感器
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识
超声波传感器是将超声波信号转换成其他能量信号（通常是电信号）的传感器。超声波是振动频率高于20kHz的机械波。它具有频率高、波长短、绕射现象小，特别是方向性好、能够成为射线而定向传播等特点。超声波对液体、固体的穿透本领很大，尤其是在阳光不透明的固体中。常用的超声波传感器由压电晶片组成，既可以发射超声波，也可以接收超声波。如图1所示。
<div align = "center">
    <img src="/media/chaoshengbo1.jpg" width="80%">
    <h5>图1</h5>
</div>

##二、硬件连接

使用古德微扩展板，我们可以通过专门为超声波模块所设计的接口，快速与树莓派连接。
<div align = "center">
    <img src="/media/chaoshengbo2.png" width="100%">
    <h5>图2 超声波连接方式</h5>
</div>

##三、基础应用（图形化）
1. 测试超声波传感器：检测在6秒内（等待0.3秒 x 20次重复），是否有障碍物，并且返回LOG输出障碍物的距离。
<div align = "center">
    <img src="/media/chaoshengbo3.png" width="100%">
    <h5>图3 超声波传感器的测试</h5>
</div>

2. 超声波测距并通过不同的小灯来指示：检测在30秒内（等待0.3秒 x 100次重复），是否有障碍物，在指定范围内点亮不同小灯。
<div align = "center">
    <img src="/media/chaoshengbo4.png" width="100%">
    <h5>图4 超声波测距</h5>
</div>

##四、基础应用（Python）
1. 测试超声波传感器
<div align = "center">
    <img src="/media/chaoshengbo5.png" width="100%">
    <h5>图5 超声波测距函数</h5>
    <img src="/media/chaoshengbo6.png" width="100%">
    <h5>图6 超声波测试</h5>
</div>

2. 超声波测距并通过不同的小灯来指示
<div align = "center">
    <img src="/media/chaoshengbo7.png" width="100%">
    <h5>图7 超声波测距</h5>
</div>

##五、相关课程链接
1. [测距仪](https://mp.weixin.qq.com/s/4-yTx2UiEDCLmoCQUgURMQ)
2. [坐姿提醒器](https://mp.weixin.qq.com/s/Nd6WJVBe6yo3mxRw9hVliA)
3. [智能视力测试仪（上）](https://mp.weixin.qq.com/s/-3PwAOlAULrNESi4N4OCaQ)
4. [智能视力测试仪（下）](https://mp.weixin.qq.com/s/GP9lSImdNFz2zUetaMI2FA)
5. [智能停车场](https://mp.weixin.qq.com/s/y8r2pbIMUL1xHIxC4kkoZQ)