#获取颜色传感器数据

![](/media/BD_color0.png)

##1.功能描述

###功能简介
* 获取颜色传感器识别到的颜色数据和结果；
* 颜色传感器通信方式为IIC通信方式。

###接线图

<div align="center">
    <img src="/media/yanse01.jpg" alt="图1" width="400">
    <h4>（图1）一代扩展板颜色传感器的接线图</h4>
</div>  

***

<div align="center">
    <img src="/media/yanse02.jpg" alt="图2" width="400">
    <h4>（图2）二代扩展板颜色传感器的接线图</h4>
</div>  

***

<div align="center">
    <img src="/media/yanse03.jpg" alt="图3" width="400">
    <h4>（图3）集成扩展板颜色传感器的接线图</h4>
</div>  



###参数说明
* 无参数

###返回值
* 返回结果：获取颜色传感器的数据-RGB列表，如[100,60,40]，
* 结果范围：列表中的每个元素范围均为：0-255；
* 变量类型：列表；其中列表元素类型：整型（数字）。

###使用场景
* 识别物体表面颜色；
* 传感器需要贴紧要识别的物体上识别准确度才会比较高。
###注意事项
* 1.当无法明显区分RGB哪种颜色为主时，返回为c，当RGB中某一颜色打参数高于其他两颜色参数100时，能较好识别物体的颜色；如[200,50,30],那么此时输出为r，表示红色；
* 2.检测数据积木块和获取结果积木块并非同时进行，为了保证结果的准确性，需要在识别和获取结果的过程中将传感器固定在同一位置；

###积木块应用
<div align="center">
    <img src="/media/BD_color11.png" alt="图4" width="1454">
    <h4>（图4）输出颜色传感器的数据</h4>
</div>  
* 对比

##2.综合运用案例
<div align="center">
    <img src="/media/BD_color3.png" alt="图5" width="511">
    <h4>（图5）通过颜色传感器控制改变灯带的颜色</h4>
</div>  

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/color_sensor1.txt" download="" target="_blank">获取颜色传感器数据</a>
* <a href="../download/积木块说明案例源代码/color_sensor2.txt" download="" target="_blank">通过颜色传感器控制改变灯带的颜色</a>