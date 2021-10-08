#矩阵键盘
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识

矩阵键盘是单片机外部设备中所使用的排布类似于矩阵的键盘组。矩阵式结构的键盘显然比直接法要复杂一些，识别也要复杂一些，列线通过电阻接正电源，并将行线所接的单片机的I/O口作为输出端，而列线所接的I/O口则作为输入。矩阵键盘示意图如下所示。
<div  align = "center">
    <img src="/media/juzhenjianpanshiyit.png" width="100%">
    <h5>图1 矩阵键盘</h5>
</div>

##二、硬件连接
矩阵键盘有8个引脚，在连接时直接插入集成板。插入方法如下图所示。
<div align = "center>
    <img src="/media/juzhenjianpanlianjieshiyitu.png" width="100%">
    <h5>图2 矩阵键盘连接示意图</h5>
</div>

矩阵键盘的内在工作原理如下图所示，一共有四行四列，汇聚成8个引脚接口，所以我们在确定每一按钮时，需要通过两个引脚进行确认。示意图如下。
<div align = "center>
    <img src="/media/juzhenjianpangongzuoyuanli.png" width="100%">
    <h5>图3 矩阵键盘内在工作机理示意图</h5>
</div>

##三、基础应用（图形化）

1.矩阵键盘测试程序。程序永远执行（条件为真，强行中断程序和切断电源除外），每隔一秒获取一次矩阵键盘的值。具体代码如下。

<div align="center">
    <img src="/media/juzhenjianpanceshi.png" width="100%">
    <h5>图4 矩阵键盘测试程序</h5>
</div>
2.矩阵键盘控制小灯亮灭程序：当矩阵键盘的”8”号案件被按下时，小灯亮起，再次按下时，小灯熄灭
<div align="center">
    <img src="/media/juzhenjianpankongzhixiaod.png" width="100%">
    <h5>图5矩阵键盘控制小灯程序</h5>
</div>

3.此处为下载链接

4.矩阵键盘控制小灯亮灭演示视频

[矩阵键盘控制小灯亮灭效果演示视频](https://weibo.com/3264309324/JE1HQowbV)

##四、基础应用（Python）
暂无，需要后期补充

##五、相关课程链接
暂无，需要后期补充

