#手势控制


![](/media/screenshot38.png)

##1.功能描述

###产品特性
* 1.9种手势识别
* 2.接口：**IIC接口通讯协议**
* 3.工作电压：3.3V-5.0V
* 4.手势速度在正常模式下为60°/S至600°/S，游戏模式为60°/S至1200°/S
* 5.环境光免疫力：＜100K Lux
* 6.工作电流：3mA-10mA
* 7.模块尺寸：20mm*15mm

###接线说明


####1-接线图

<div align="center">
    <img src="/media/BD_gesture1.png" alt="图1" width="1178">
    <h4>（图1）手势传感器与树莓派扩展板的接线图</h4>
</div>  

####2-实物图

<div align="center">
    <img src="/media/BD_gesture2.jpg" alt="图2" width="427">
    <h4>（图2）手势传感器实物图</h4>
</div>


###功能简介


![](/media/screenshot39.png)

* 新建的ontouch函数需要带一个参数用以接收touch的位置信息。

![](/media/screenshot40.png)

* 输入的函数需要带两个参数用以接收位置信息：起始位置、结束位置。

![](/media/screenshot41.png)

* 输入函数名，该函数需要带一个参数用以接收圆位置信息。

![](/media/BD_get_gesture.png)

* 获取手势传感器的手势信息，该积木块为**阻塞操作**；
  *** **<font color=#FF00000> 何为阻塞操作：</font>在执行设备操作时，若不能获得资源或数据，则进程挂起直到满足可操作的条件再进行操作。即：该积木块获取到手势信息后才继续执行后面的积木块。**

![](/media/BD_getsture_init.png)

* 初始化手势传感器，在获取手势之前，须先调用该积木块。



###返回值

![](/media/BD_get_gesture.png)

* 返回值为手势的英文全拼，数据类型为：字符串（文本），

* **手势动图展示：**

* forward：
<div align="center">
    <img src="/media/BD_gesture_forward.gif" alt="图2" width="300">
    <h4>手掌向下移动</h4>
</div>

* backward：

<div align="center">
    <img src="/media/BD_gesture_backward.gif" alt="图2" width="300">
    <h4>手掌向上移动</h4>
</div>

* right：

<div align="center">
    <img src="/media/BD_gesture_right.gif" alt="图2" width="300">
    <h4>从左向右挥手</h4>
</div>

* left：

<div align="center">
    <img src="/media/BD_gesture_left.gif" alt="图2" width="300">
    <h4>从右向左挥手</h4>
</div>

* up：

<div align="center">
    <img src="/media/BD_gesture_up.gif" alt="图2" width="300">
    <h4>从前向后挥手</h4>
</div>

* down：

<div align="center">
    <img src="/media/BD_gesture_down.gif" alt="图2" width="300">
    <h4>从后向前挥手</h4>
</div>

* clockwise：

<div align="center">
    <img src="/media/BD_gesture_clockwise.gif" alt="图2" width="300">
    <h4>顺时针画圈圈</h4>
</div>

* anti-clockwise：

<div align="center">
    <img src="/media/BD_gesture_anti-clockwise.gif" alt="图2" width="300">
    <h4>逆时针画圈圈</h4>
</div>

* wave：
<div align="center">
    <img src="/media/BD_gesture_wave.gif" alt="图2" width="300">
    <h4>从上到下画圈</h4>
</div>



###积木块应用

<div align="center">
    <img src="/media/BD_gesture2.png" alt="图2" width="469">
    <h4>（图2）输出手势传感器结果</h4>
</div>

##2.综合运用案例
<div align="center">
<img src="/media/BD_gesture3.png" alt="图3" width="478">
    <h4>（图3）通过手势识别传感器控制灯带显示不同的效果</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/gesture-1.txt" download="" target="_blank">输出手势传感器结果</a>
* <a href="../download/积木块说明案例源代码/gesture-2.txt" download="" target="_blank">通过手势识别传感器控制灯带显示不同效果</a>


