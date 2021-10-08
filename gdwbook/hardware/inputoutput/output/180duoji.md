#180°舵机
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识
舵机是一种位置（角度）伺服的驱动器，适用于那些需要角度不断变化并可以保持的控制系统。在高档遥控玩具，如飞机、潜艇模型，遥控机器人中已经得到了普遍应用，此处我们涉及的是180°舵机，如下图所示。
<img src="/media/180°duoji.png"  align = "center" width="80%">
<h5 align = "center">180°舵机</h5>
舵机作为机器人的执行器，其实与电机的功能非常的像，为机器人提供动力。它和肌肉与关节搭配起来的功能一样，手就是有了肌肉与关节的存在，才能完成“握住”与“释放”物体的动作。常见的机械爪，动力提供使用的就是舵机，如图2所示。
<img src="/media/servo2.jpg"  align = "center" width="80%">
<h5 align = "center">180°舵机控制原理图</h5>
<img src="/media/servo3.png"  align = "center" width="100%">
<h5 align = "center">图3 180度舵机</h5>

##二、硬件连接

舵机有三个接口，分别对应三种颜色的电线，红色接VCC，供5V电源；棕色接GND地线；黄色接D控制信号，常用的有18和23号引脚，具体示意图如下所示。
<img src="/media/servo5.png"  align = "center" width="100%">
<h5 align = "center">图5 舵机连线</h5>

##三、基础应用（图形化）
1.测试舵机程序：控制舵机转向0°
<img src="/media/ceshiduojichengxu.png"  align = "center" width="100%">
<h5 align = "center">图6 测试舵机程序</h5>
2.舵机的旋转数为500到2500之间的随机数，如果旋转数小于1500，则小灯两起，反之，小灯熄灭。
<img src="/media/duojikongzhixiaodeng.png"  align = "center" width="100%">
<h5 align = "center">图7 舵机控制小灯亮灭</h5>


3.此处为程序代码下载链接

4.舵机控制小灯亮灭程序演示效果视频

[舵机控制小灯亮灭演示视频](https://weibo.com/3264309324/JDTEimn53)

##四、基础应用（Python）
1. 控制180°舵机在Python环境中的具体代码如图所示。
<img src="/media/servo8.png"  align = "center" width="100%">
<h5 align = "center">图8 180度舵机控制</h5>


##五、相关课程链接
1. [趣味转盘](https://mp.weixin.qq.com/s/qZjesLvHQcxz6g5dB_h0KQ)
2. [智能停车场](https://mp.weixin.qq.com/s/y8r2pbIMUL1xHIxC4kkoZQ)