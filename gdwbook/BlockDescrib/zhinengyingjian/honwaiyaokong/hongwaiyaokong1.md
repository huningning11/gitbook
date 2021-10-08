#红外遥控扩展板积木块区

![](/media/hongwaiyaokong01.png)

##1.功能描述

###功能简介
* 红外遥控是一种无线、非接触控制技术，具有抗干扰能力强，信息传输可靠，功耗低，成本低，易实现等显著优点，被诸多电子设备特别是家用电器广泛采用，并越来越多的应用到计算机和手机系统中。


###实物图

<div align="center">
    <img src="/media/hongwaiyaokong1.jpg" alt="图1" width="1385">
    <h4>（图1）红外遥控扩展板实物图</h4>
</div>  

<div align="center">
    <img src="/media/hongwaiyaokong2.jpg" alt="图2" width="3301">
    <h4>（图2）红外遥控扩展板实物连接图</h4>
</div>  



###工作原理

* 红外遥控的发射电路是采用红外发光二极管来发出经过调制的红外光波；红外接收电路由红外接收二极管、三极管或硅光电池组成，它们将红外发射器发射的红外光转换为相应的电信号，再送后置放大器。

* 发射机一般由指令键(或操作杆)、指令编码系统、调制电路、驱动电路、发射电路等几部分组成。当按下指令键或推动操作杆时，指令编码电路产生所需的指令编码信号，指令编码信号对载波进行调制，再由驱动电路进行功率放大后由发射电路向外发射经调制定的指令编码信号。

* 接收电路一般由接收电路、放大电路、调制电路、指令译码电路、驱动电路、执行电路(机构)等几部分组成。接收电路将发射器发出的已调制的编码指令信号接收下来，并进行放大后送解调电路，解调电路将已调制的指令编码信号解调出来，即还原为编码信号。指令译码器将编码指令信号进行译码，最后由驱动电路来驱动执行电路实现各种指令的操作控制（机构）.


###积木块说明

![](/media/hongwaiyaokong02.png)

功能简介：接收下一个红外信号。

返回值：返回红外信号的键名；数据类型：文本
***
![](/media/hongwaiyaokong03.png)

功能简介：在树莓派终端执行一句命令语句。

参数一：输入语句命令，如重启树莓派命令：sudo reboot
***
![](/media/hongwaiyaokong04.png)

功能简介：设置红外扩展板的模式及数据发射输入gpio口；（本积木调用后树莓派会重启，所以需要断开设备后重新连接）

参数一：选择需要设置的红外模式（有发射模式和接收模式）；

参数二：选择发射和接收数据的gpio口；发射模式选择17号gpio口，接收模式选择18号gpio口；
***
![](/media/hongwaiyaokong05.png)

功能简介：获取当前红外遥控模块的模式和端口。

返回值：由模式和端口信息组成的列。
***
![](/media/hongwaiyaokong06.png)

功能简介：控制红外机器人（机械战警）运动。

参数一：选择红外遥控机器人需要执行的动作，有前进，后退，左转，右转，滑行前进，滑行后退，滑行左转，滑行右转和停止。
***
![](/media/hongwaiyaokong07.png)

功能简介：控制红外机器人（机械战警）的手做动作。

参数一：选择红外遥控机器人需要执行的动作，有左手上，左手下，右手上和右手下；
***
![](/media/hongwaiyaokong08.png)

功能简介：控制红外机器人（机械战警）的实现各种功能。

参数一：选择红外遥控机器人需要执行的动作，有讲科普，跳舞，战斗，讲故事，学英语和唱歌；
***
![](/media/hongwaiyaokong09.png)

功能简介：控制红外机器人（机械战警）的模拟发射导弹。

参数一：选择红外遥控机器人需要执行的动作，有发射导弹和连续发射导弹；
***
![](/media/hongwaiyaokong10.png)

功能简介：控制红外机器人（机械战警）的音量。

参数一：选择红外遥控机器人音量的大小，有调高音量和调低音量；

###积木块应用
<div align = "center">
    <img src="/media/hongwaiyaokong3.png" width="414">
    <img src="/media/hongwaiyaokong4.png" width="597">
    <img src="/media/hongwaiyaokong5.png" width="1007">
    <img src="/media/hongwaiyaokong6.png" width="1115">
    <img src="/media/hongwaiyaokong7.png" width="1056">
    <img src="/media/hongwaiyaokong8.png" width="1108">
    <h5>图3 红外控制机械战警</h5>
</div>

##2.综合运用案例
<div align="center">
    <img src="/media/hongwaiyaokong11.png" alt="图4" width="1208">
    <h4>（图4）机器人跳舞</h4>
</div>  



##3.案例代码下载
* <a href="../download/积木块说明案例源代码/hongwaiyaokonganli1.txt" download="" target="_blank">机器人跳舞</a>
