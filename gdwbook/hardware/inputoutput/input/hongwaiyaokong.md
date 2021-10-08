#红外遥控
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识

红外遥控是一种无线、非接触控制技术，具有抗干扰能力强，信息传输可靠，功耗低，成本低，易实现等显著优点，被诸多电子设备特别是家用电器广泛采用，并越来越多的应用到计算机和手机系统中。如图1所示。

红外遥控的发射电路是采用红外发光二极管来发出经过调制的红外光波；红外接收电路由红外接收二极管、三极管或硅光电池组成，它们将红外发射器发射的红外光转换为相应的电信号，再送后置放大器。

发射机一般由指令键(或操作杆)、指令编码系统、调制电路、驱动电路、发射电路等几部分组成。当按下指令键或推动操作杆时，指令编码电路产生所需的指令编码信号，指令编码信号对载波进行调制，再由驱动电路进行功率放大后由发射电路向外发射经调制定的指令编码信号。

接收电路一般由接收电路、放大电路、调制电路、指令译码电路、驱动电路、执行电路(机构)等几部分组成。接收电路将发射器发出的已调制的编码指令信号接收下来，并进行放大后送解调电路，解调电路将已调制的指令编码信号解调出来，即还原为编码信号。指令译码器将编码指令信号进行译码，最后由驱动电路来驱动执行电路实现各种指令的操作控制（机构）.
<div align = "center">
    <img src="/media/hongwaiyaokong1.jpg" width="100%">
    <h5>图1 红外遥控器</h5>
</div>

##二、硬件连接
<div align = "center">
    <img src="/media/hongwaiyaokong2.jpg" width="100%">
    <h5>图2 红外遥控板连线</h5>
</div>

##三、基础应用（图形化）
1. 红外控制机械战警

<div align = "center">
    <img src="/media/hongwaiyaokong3.png" width="100%">
    <img src="/media/hongwaiyaokong4.png" width="100%">
    <img src="/media/hongwaiyaokong5.png" width="100%">
    <img src="/media/hongwaiyaokong6.png" width="100%">
    <img src="/media/hongwaiyaokong7.png" width="100%">
    <img src="/media/hongwaiyaokong8.png" width="100%">
    <h5>图3-8 红外控制机械战警</h5>
</div>

##四、基础应用（Python）
1. 红外控制机械战警


##五、相关课程链接
1. [会跳舞的机器人](https://mp.weixin.qq.com/s/cLXrt7ibQaorZUzkhCZi_A)
