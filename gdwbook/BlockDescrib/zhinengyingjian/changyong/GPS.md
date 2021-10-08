#GPS积木块区

![](/media/GPS01.png)

##1.功能描述

###功能简介

全球定位系统(Global Positioning System，GPS)是一种以人造地球卫星为基础的高精度无线电导航的定位系统，它在全球任何地方以及近地空间都能够提供准确的地理位置、车行速度及精确的时间信息。本模块USB-Port-GPS 模块使用L80-39模组方案 。

###接线说明

####1-实物图

<div align="center">
    <img src="/media/GPS1.jpg" alt="图1" width="1001">
    <h4>（图1）GPS模块实物图</h4>
</div>  

####2-接线图

<div align="center">
    <img src="/media/GPS2.jpg" alt="图2" width="1001">
    <h4>（图2）GPS实物连接图</h4>
</div>



###参数说明

* 无

###返回值

![](/media/GPS02.png)

* 返回值：返回通过GPS定位后得到的经度纬度坐标列表；
* 数据类型：列表（数字）；

![](/media/GPS03.png)

* 由于通过获取位置信息积木返回值为经纬度坐标列表，为了更好的表述当前的位置，常用此积木块将经纬度坐标转化为具体位置信息。
* 参数说明：参数一输入经度，参数二输入纬度；
* 返回值：具体位置信息；
* 数据类型：文本。




###积木块应用

GPS基本使用方法  
1.常用模块下，找到初始化GPS模块

<img src="/media/GPS4.jpg" width="790">

2.创建变量：位置信息  

<img src="/media/GPS5.jpg" width="1229">

3.赋值为位置信息为：获取gps当前位置信息

<img src="/media/GPS6.jpg" width="702">

<img src="/media/GPS7.jpg" width="729">

4.基础模块下，选择输出调试信息命令

<img src="/media/GPS8.jpg" width="701">

5.人工智能基础模块中，选择通过纬度经度获取当前位置信息命令

<img src="/media/GPS9.jpg" width="716">

6.在列表模块中，选择列表取得命令

<img src="/media/GPS10.jpg" width="860">

7.程序编写完成后，如下图

<img src="/media/GPS3.png" width="1368">




##2.案例代码下载
* <a href="../download/积木块说明案例源代码/GPSanli1.txt" download="" target="_blank">GPS基本使用方法</a>
