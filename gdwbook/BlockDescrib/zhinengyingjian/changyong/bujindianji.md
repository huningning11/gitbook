#步进电（丝杆）积木块区

![](/media/bujindianji1.png)

##1.功能描述

###功能简介

![](/media/bujindianji2.png)

* 初始化设置控制42型步进电机的4个GPIO口，分别对应接入驱动板4个输入引脚（IN），驱动板上的输入口分别按顺序接入步进电机即可；如果为控制丝杆，驱动板的输出口按顺序分别对应丝杆的黄红黑蓝顺序线。

![](/media/bujindianji3.png)

![](/media/bujindianji4.png)

* 控制步进电机（丝杆）正反向运动，第一个参数可以调整速度，第二个参数为步进电机旋转的圈数，路径仅由第二参数控制，与第一参数无关。

###接线说明

####1-实物图

丝杆一般指滚珠丝杠，滚珠丝杠是将回转运动转化为直线运动，或将直线运动转化为回转运动的理想的产品。

<div align="center">
    <img src="/media/sigan1.png" alt="图1" width="913">
    <h4>（图1）丝杆实物图</h4>
</div>  

####2-接线图

<div align="center">
    <img src="/media/sigan2.png" alt="图2" width="654">
    <h4>（图2）丝杆（步进电机）连线图</h4>
</div>

<div align="center">
    <img src="/media/sigan3.png" alt="图3" width="710">
    <h4>（图3）丝杆控制方式</h4>
</div>





###积木块应用

<div align="center">
    <img src="/media/bujindianji5.png" alt="图4" width="484">
    <h4>（图4）步进电机基础控制</h4>
</div>

##2.综合运用案例
<div align="center">
<img src="/media/bujindianji6.png" alt="图5" width="484">
    <h4>（图5）按钮控制丝杆上下楼</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/bujindianjianli1.txt" download="" target="_blank">步进电机基础控制</a>
* <a href="../download/积木块说明案例源代码/bujindianjianli2.txt" download="" target="_blank">按钮控制丝杆上下楼</a>