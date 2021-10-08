#蜂鸣器积

![](/media/screenshot14.png)

##1.功能描述

###基础知识
* 有源蜂鸣器与无源蜂鸣器的区别（“源”是指震荡源），有源蜂鸣器内部带震荡源，一通电就会响；而无源内部不带震荡源，用直流信号无法令其鸣叫，必须用2K-5K的方波去驱动。本积木块均使用无源蜂鸣器。
* 蜂鸣器电源接口需要接3.3v，而非通用5v电源，如果接到5v电源，蜂鸣器会一直发声而无法正常使用。
* 蜂鸣器是一种一体化结构的电子讯响器，采用直流电压供电，是一种发声器件。
* 蜂鸣器主要分为压电式蜂鸣器和电磁式蜂鸣器两种类型。蜂鸣器在电路中用字母“H”或“HA”表示。


###接线图

<div align="center">
    <img src="/media/screenshot13.png" alt="图1" width="1035">
    <h4>（图1）蜂鸣器接线图</h4>
</div>

###功能简介
![](/media/screenshot21.png)

* 蜂鸣器测试，设为没电时，测试蜂鸣器鸣叫；设为有电时，测试蜂鸣器鸣叫停止。

![](/media/screenshot15.png)

* 初始化蜂鸣器播放音乐，默认初始化频率523(do声)。

![](/media/screenshot16.png)

* 调节整体奏乐速度。

![](/media/screenshot18.png)

* 调节音调。

![](/media/screenshot19.png)

* 蜂鸣器暂停奏乐。

![](/media/screenshot20.png)

* 蜂鸣器停止奏乐，在音乐末尾结束奏乐。

###参数说明


![](/media/screenshot21.png)

* 参数一：GPIO端口号，范围为：1-27，变量类型：整型。
* 参数二：设置GPIO口的电平高（1），低（0）.

![](/media/screenshot15.png)

* 参数一：GPIO端口号，范围为：1-27，变量类型：整型。

![](/media/screenshot16.png)

* 参数一：设定弹奏速度大小，默认为60，即每分钟60拍，变量类型：整型。

![](/media/screenshot18.png)

* 参数一：音调频率。
* 参数二：节拍数（时间长短）。

![](/media/screenshot19.png)

* 参数一：休止时间，单位是拍。

![](/media/screenshot20.png)

* 无参数。


###使用场景

* 报警、提示音。


##2.综合运用案例


<div align="center">
    <img src="/media/screenshot22.png" alt="图3" width="363">
    <h4>（图6）蜂鸣器模拟”蝈蝈“叫声</h4>
</div>


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/fengmingqi.txt" download="" target="_blank">蜂鸣器模拟”蝈蝈“叫声</a>
