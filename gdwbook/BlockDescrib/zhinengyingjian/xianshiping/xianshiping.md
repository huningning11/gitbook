#显示屏

![](/media/screenshot23.png)

##1.功能描述

###基础知识
* OLED（Organic Light-Emitting Diode）即有机发光二极管，是一种常见的显示器屏幕类型，
* OLED显示技术与传统的LCD显示方式不同，无需背光灯，采用非常薄的有机材料涂层和玻璃基板(或柔性有机基板)，当有电流通过时，这些有机材料就会发光。
* OLED显示屏幕可以做得更轻更薄，可视角度更大，并且能够显著的节省耗电量。

###硬件连接

<div align="center">
    <img src="/media/screenshot24.png" alt="图1" width="1035">
    <h4>（图1）OLED示意图</h4>
</div>

<div align="center">
    <img src="/media/screenshot36.png" alt="图1" width="1035">
    <h4>（图2）OLED连接图</h4>
</div>

###使用场景

* 在商业领域当中，POS机、复印机、ATM机中会安装小尺寸的OLED屏幕。
* 大屏幕可以用作商务宣传屏，也可以用作车站、机场等广告投放屏幕。
* 电子产品领域中，OLED应用最为广泛的就是智能手机，其次是笔记本、显示屏、电视、平板、数码相机等。

###功能简介

![](/media/screenshot25.png)

* 初始化OLED显示屏。

![](/media/screenshot26.png)

* 把图片显示到OLED显示屏。

![](/media/screenshot27.png)

* 关闭OLED显示屏。

![](/media/screenshot28.png)

* OLED显示屏显示。

![](/media/screenshot29.png)

* 清空OLED显示屏显示，使屏幕显示黑色。

![](/media/screenshot30.png)

* 以列表形式返回OLED屏幕的尺寸。

![](/media/screenshot31.png)

* LCD显示屏初始化。

![](/media/screenshot32.png)

* 在LCD屏上显示字符串。

![](/media/screenshot33.png)

* 清空CLD显示屏显示，使屏幕显示背景颜色。

###参数说明


![](/media/screenshot25.png)

* 参数一：显示屏设备型号。
* 参数二：使用接口名称。
* 参数三：屏幕像素（分辨率）宽度，变量类型：整型。
* 参数四：屏幕像素（分辨率）高度，变量类型：整型。

![](/media/screenshot26.png)

* 参数一：图片对象。

![](/media/screenshot27.png)

* 无参数。

![](/media/screenshot28.png)

* 无参数。

![](/media/screenshot29.png)

* 无参数。

![](/media/screenshot30.png)

* 无参数。

![](/media/screenshot31.png)

* 参数一：i2c设备地址，默认是1号设备

![](/media/screenshot32.png)

* 参数一：行，范围：1-2，变量类型：整型。
* 参数二：列，范围：1-16，变量类型：整型。
* 参数三：要显示的字符串。

![](/media/screenshot33.png)

* 清空CLD显示屏显示，使屏幕显示背景颜色。

###积木块应用

1、 测试OLED 屏幕，显示背景图片
<div align="center">
    <img src="/media/screenshot34.png" alt="图3" width="694">
    <h4>（图3）在OLED屏幕上显示背景图片</h4>
</div>  
2、在OLED 屏幕上显示文字
<div align="center">
    <img src="/media/screenshot35.png" alt="图3" width="694">
    <h4>（图4）在OLED屏幕上显示文字</h4>
</div>  


##2.综合运用案例


<div align="center">
    <img src="/media/screenshot37.png" alt="图3" width="363">
    <h4>（图5）OLED屏幕同时显示图片和文字</h4>
</div>


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/OLED3.txt" download="" target="_blank">在OLED屏幕上显示背景图片</a>
* <a href="../download/积木块说明案例源代码/OLED2.txt" download="" target="_blank">在OLED屏幕上显示文字</a>
* <a href="../download/积木块说明案例源代码/OLED1.txt" download="" target="_blank">OLED屏幕同时显示图片和文字</a>