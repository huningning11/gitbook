#矩阵键盘积木块区

![](/media/BD_matrix%20keyboard_0.png)

![](/media/juzhenjianpan1.png)

##1.功能描述

###功能简介

矩阵键盘是单片机外部设备中所使用的排布类似于矩阵的键盘组。

###接线说明

####1-接线图

<div align="center">
    <img src="/media/juzhenjianpanlianjieshiyitu.png" alt="图1" width="1140">
    <h4>（图1）矩阵键盘与树莓派扩展板的接线图</h4>
</div>  

####2-实物图

<div align="center">
    <img src="/media/juzhenjianpanshiyit.png" alt="图2" width="903">
    <h4>（图2）矩阵键盘实物图</h4>
</div>

####3-工作原理

<div align="center">
    <img src="/media/juzhenjianpangongzuoyuanli.png" alt="图3" width="759">
    <h4>（图3）矩阵键盘工作原理示意图</h4>
</div>

###参数说明

前两个参数确定行和列数，后两个参数设置行和列对应的gpio口。

###返回值

* 返回结果：返回按键所在的列数和行数，如:按键8返回值为23;
* 变量类型：整型（数字）


###产品特性
* 1.16键输入
* 2.模块尺寸：60mm*60mm

###积木块应用

<div align="center">
    <img src="/media/juzhenjianpanceshi.png" alt="图4" width="817">
    <h4>（图4）矩阵键盘测试程序</h4>
</div>

##2.综合运用案例
<div align="center">
<img src="/media/juzhenjianpankongzhixiaod.png" alt="图5" width="838">
    <h4>（图5）矩阵键盘控制小灯</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/juzhenjianpanceshi.txt" download="" target="_blank">矩阵键盘测试程序</a>
* <a href="../download/积木块说明案例源代码/juzhenjianpankongzhixiaod.txt" download="" target="_blank">矩阵键盘控制小灯</a>