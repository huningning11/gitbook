#按钮检测积木块

![](/media/anniu1.png)

##1.功能描述

###功能简介
* 从指定相应的GPIO口获取按钮的检测结果。

###接线图

<div align="center">
    <img src="/media/buttonfeetshow.png" alt="图1" width="335">
    <h4>（图1）按钮引脚示意图</h4>
</div>  



***
<div align="center">
    <img src="/media/anniu5.jpg" alt="图2" width="400">
    <h4>（图2）一代扩展板按钮接线图</h4>
</div>

***
<div align="center">
    <img src="/media/anniu6.jpg" alt="图3" width="400">
    <h4>（图3）二代扩展板按钮接线图</h4>
</div>

***
<div align="center">
    <img src="/media/anniu7.jpg" alt="图4" width="400">
    <h4>（图4）集成扩展板按钮接线图</h4>
</div>

* 如图所示，集成扩展板自带按钮，无需外接，直接调用即可。

###参数说明
* 输入检测按钮信号的GPIO口。

###返回值
* 返回结果：返回0，1，-1；0表示未按下，1表示按下，-1表示出错；
* 结果范围：0，1，-1；
* 变量类型：整型（数字）。


###积木块应用
<div align="center">
    <img src="/media/anniu2.png" alt="图5" width="694">
    <h4>（图5）按钮输出结果</h4>
</div>  

##2.综合运用案例
<div align="center">
    <img src="/media/anniu3.png" alt="图6" width="351">
    <h4>（图6）按钮控制小灯1</h4>
</div>  

* 按钮按下时小灯亮，按钮松开时小灯灭；

<div align="center">
    <img src="/media/anniu4.png" alt="图7" width="351">
    <h4>（图7）按钮控制小灯2</h4>
</div>  

* 按钮按1下小灯亮，按钮按2下小灯灭，以此类推。
* **注意：由于按钮在按下到回弹的过程中需要一定的时间，所以需要合理设置按钮检测中的时间间隔，避免按钮检测不及时或一次按键多次反应的情况发生；**

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/anniuanli1.txt" download="" target="_blank">按钮输出结果</a>
* <a href="../download/积木块说明案例源代码/anniuanli2.txt" download="" target="_blank">按钮控制小灯1</a>
* <a href="../download/积木块说明案例源代码/anniuanli3.txt" download="" target="_blank">按钮控制小灯2</a>