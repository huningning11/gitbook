#指纹传感器积木区

![](/media/BD_finger0.png)

##1.功能描述

###功能简介

![](/media/BD_fingerprint_init.png)

* 初始化指纹传感器，并选择指纹传感器的通信端口,使用指纹传感器时，须先调用该积木块。

![](/media/BD_fingerprint_delete.png)

* 删除指纹传感器内存中，已录制的指定ID的指纹。

![](/media/BD_fingerprint_enroll.png)

* 录制指纹，将指纹保存至指纹传感器中。

![](/media/BD_fingerprint_search.png)

* 获取指纹传感器上的指纹ID或相似度，可用来判断当前指纹是否已录制。

![](/media/BD_fingerprint_saveImg.png)

* 保存指纹传感器上的指纹图片，保存至树莓派本地中的指定路径；
* 将指纹录制可视化，可用来观察录制的指纹纹路。

![](/media/BD_fingerprint_getnum.png)

* 获取指纹传感器中已录制的指纹数量。

![](/media/BD_fingerprint_getresult.png)

* 用来判断是否有可识别的指纹放置在指纹传感器上；
* **注：该积木块并非用来判断放置的指纹是否已录制至传感器**。

![](/media/BD_fingerprint_getdevice.png)

* 获取USB设备列表，等价于命令行 `ls /dev/ttyUSB*` 返回值

###接线图

<div align="center">
    <img src="/media/BD_finger1.jpg" alt="图1" width="1682">
    <h4>（图1）指纹传感器的接线图（USB转串口方式）</h4>
</div>  

###参数说明

![](/media/BD_fingerprint_init.png)

* 参数一：指纹传感器串口通信端口，GPIO：GPIO口通信方式，可直接与树莓派串口连接；USB0-USB4：USB串口通信方式，通过USB转TTL模块转接。

![](/media/BD_fingerprint_delete.png)

* 参数一：传感器中已录制的指纹ID，范围为：0-300。类型为：整型（数字）

![](/media/BD_fingerprint_search.png)

* 参数一：ID或置信度，ID:为指纹在录制时的ID；置信度：为与指纹传感器中最相似的指纹置信度。

![](/media/BD_fingerprint_saveImg.png)

* 参数一：树莓派本地路径，路径需为树莓派本地绝对路径下的图片文件格式，如：/home/pi/imageTemp/temp.jpg。变量类型为：字符串。


###返回值

![](/media/BD_fingerprint_enroll.png)

* 返回指纹的ID，ID范围为：0-300，类型为：整型（数字）
* 录制成功返回对应的ID，ID在原有的数量上累加一；若录制失败则返回-1；

![](/media/BD_fingerprint_search.png)

* 若参数一为ID：返回值范围为：0-300，类型为：整型；
* 若参数一为置信度：返回值范围为：0-100，类型为：整型；
* 若识别失败则返回值为：-1。

![](/media/BD_fingerprint_saveImg.png)

* 如果保存成功：返回值为参数一；
* 失败：返回值为：’‘（空字符串）。

![](/media/BD_fingerprint_getnum.png)

* 返回已录制的指纹数量，取值范围：0-300；变量类型：整型（数字）。

![](/media/BD_fingerprint_getresult.png)

* True或False；如果指纹传感器上检测到指纹（录制与未录制均可），则返回True,否则返回False;数据类型：bool(布尔类型)。

![](/media/BD_fingerprint_getdevice.png)

* 返回树莓派上的USB设备列表；
* 若检测到设备，则列表元素为”/dev/ttyUSB0“-"/dev/ttyUSB3",列表元素类型为：string(字符串);
* 若没检测到任何USB设备，则返回空列表（即：[]）；

###使用场景
* 指纹传感器为串口通信设备，若使用的GPIO串口模式，则需先设置树莓派为串口模式方可正常通信。

###积木块应用
<div align="center">
    <img src="/media/BD_finger2.png" alt="图2" width="1735">
    <h4>（图2）指纹传感器的简单使用</h4>
</div>  

##2.综合运用案例
<div align="center">
    <img src="/media/BD_finger3.png" alt="图3" width="727">
    <h4>（图3）基于指纹传感器的门禁系统</h4>
</div>  

###案例功能简介

* 功能一：指纹录制功能，通过矩阵键盘输入正确密码后，可进行指纹录制；
* 功能二：指纹识别功能，人体感应传感器感应到人体后，指纹传感器进行指纹识别。

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/finger_printer1.txt" download="" target="_blank">指纹传感器的简单使用</a>
* <a href="../download/积木块说明案例源代码/finger_printer2.txt" download="" target="_blank">基于指纹传感器的门禁系统</a>