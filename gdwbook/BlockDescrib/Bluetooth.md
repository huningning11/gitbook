#蓝牙积木块区

![](/media/BD_bluetooth0.png)

##1.功能描述

###功能简介

![](/media/BD_bluetooth_getaddr.png)

* 获取设备的蓝牙地址，设备需打开蓝牙。

![](/media/BD_bluetooth_conx.png)

* 连接/断开指定蓝牙设备。

###参数说明

![](/media/BD_bluetooth_getaddr.png)

* 参数一：填入设备的蓝牙名称，数据类型为：字符串（文本）。

![](/media/BD_bluetooth_conx.png)

* 参数一：连接或断开，即：连接或断开指定蓝牙地址设备；
* 参数二：蓝牙的地址，可由上方积木块获取指定设备的地址，数据格式为：88:88:12:A2:CA:2B，数据类型：字符串（文本）。

###返回值

![](/media/BD_bluetooth_getaddr.png)

* 返回值为指定设备的蓝牙地址，如：88:88:12:A2:CA:2B。

###积木块应用

<div align="center">
    <img src="/media/BD_bluetooth1.png" alt="图2" width="434">
    <h4>（图2）连接蓝牙设备</h4>
</div>

##2.综合运用案例
<div align="center">
<img src="/media/BD_bluetooth2.png" alt="图3" width="525">
    <h4>（图3）如何使用蓝牙音箱</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/bluetooth-1.txt" download="" target="_blank">连接蓝牙设备</a>
* <a href="../download/积木块说明案例源代码/bluetooth-2.txt" download="" target="_blank">如何使用蓝牙音箱</a>