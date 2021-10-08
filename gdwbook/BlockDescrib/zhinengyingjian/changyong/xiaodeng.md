#控制小灯积木块

![](/media/xiaodeng1.png)

##1.功能描述

###功能简介
* 通过设置对应GPIO口电平的高低来控制LED小灯的亮灭。


###接线图

<div align="center">
    <img src="/media/xiaodeng01.jpg" alt="图1" width="400">
    <h4>（图1）一代扩展板小灯实物连接图</h4>
</div>  

***

<div align="center">
    <img src="/media/xiaodeng04.jpg" alt="图2" width="400">
    <h4>（图2）二代扩展板小灯实物连接图</h4>
</div>  

* 与一代扩展板的连接方式相同

***

<div align="center">
    <img src="/media/xiaodeng05.jpg" alt="图3" width="400">
    <h4>（图3）集成扩展板小灯实物连接图</h4>
</div>  

* 集成扩展板5，6，12，16号接口自带小灯，可以直接调用；
* 任意GPIO口都可控制小灯，只需将LED小灯长脚端输入高电平，短脚端接地即可。



###参数说明
* 无参数




###积木块应用
<div align="center">
    <img src="/media/xiaodeng02.png" alt="图2" width="229">
    <h4>（图2）小灯测试程序</h4>
</div>  

##2.综合运用案例
<div align="center">
    <img src="/media/xiaodeng03.png" alt="图3" width="237">
    <h4>（图3）流水灯</h4>
</div>  



##3.案例代码下载
* <a href="../download/积木块说明案例源代码/xiaodenganli1.txt" download="" target="_blank">小灯测试程序</a>
* <a href="../download/积木块说明案例源代码/xiaodenganli2.txt" download="" target="_blank">流水灯</a>