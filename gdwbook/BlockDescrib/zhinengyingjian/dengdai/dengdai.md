#灯带

![](/media/screenshot 1.png)

##1.功能描述

###功能简介
* 起到装饰以及烘托气氛的作用，塑造空间光环境。
* 通过更改RGB参数，可以设定灯带上灯的颜色。
* 可控制灯带上灯的亮度。
* 灯带柔软，可随意卷曲和伸张，也可制作图形、文字等造型。可随意剪切和延接。


###接线图

<div align="center">
    <img src="/media/screenshot2.png" alt="图1" width="1034">
    <h4>（图1）灯带-树莓派 接线图</h4>

</div>  
<div align="center">
    <img src="/media/screenshot3.png" alt="图2" width="1256">
    <h4>（图2）灯带-灯带 接线图</h4>
</div>  


###硬件连接

* 每段灯带上都有一些小箭头，箭头所指的方向为输出端，表示信号向前传递。箭头尾部方向则为输入端，即需要我们接线的方向。
* 以WS281X灯带为例，有GND、D0、5V三个接口，分别连接到树莓派的GND、VCC、D0（18号或12号）就可以实现对灯带的控制。
* 若需要更长的灯带，可以直接将多个灯带首尾相连使用。如果灯带过长，则需要为灯带进行独立供电，否则会出现供电不足，导致无法有效的控制信号或者树莓派重启。把灯带调暗则可以正常控制更多的灯。
<div align="center">
    <img src="/media/screenshot4.png" alt="图3" width="866">
    <h4>（图3）灯带细节图</h4>
</div>


###功能简介


![](/media/screenshot5.png)

* 设置GPIO口，可控制灯带上灯的个数，灯带亮度。

![](/media/screenshot7.png)

* 设置灯带上某个灯的RGB颜色列表。

![](/media/screenshot8.png)

* 通过调用本函数可使已经设置或更新灯带的数据生效。

![](/media/screenshot9.png)

* 设置灯带的亮度值。



###参数说明


![](/media/screenshot5.png)

* 参数一：GPIO端口号，范围为：1-27，此处只支持GPIO 12和18，变量类型：整型。
* 参数二：实际控制的灯带上的小灯数量，范围不超过灯带上的小灯总数，变量类型：整型。
* 参数三：灯带上小灯亮度，范围：0-255，变量类型：整型。亮度值为0表示熄灭。

![](/media/screenshot7.png)

* 参数一：小灯在灯带的实际位置，从第0个灯开始计数，范围：0-小灯总数，变量类型：整型。
* 参数二：RGB颜色列表，范围：0-255，变量类型：整型。

![](/media/screenshot8.png)

* 无参数。

![](/media/screenshot9.png)

* 参数一：灯带亮度，范围：0-255，变量类型：整型。


###使用场景

* 广泛应用于室内装修，街景装饰。


###积木块应用

<div align="center">
    <img src="/media/screenshot11.png" alt="图2" width="470">
    <h4>（图4）灯带测试-点亮第一个灯珠</h4>
</div> 

<div align="center">
    <img src="/media/screenshot10.png" alt="图2" width="455">
    <h4>（图5）依次点亮灯珠</h4>
</div>  


##2.综合运用案例


<div align="center">
    <img src="/media/screenshot12.png" alt="图3" width="504">
    <h4>（图6）相邻4个灯带为不同颜色</h4>
</div>


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/txt3.txt" download="" target="_blank">灯带测试-点亮第一个灯珠</a>
* <a href="../download/积木块说明案例源代码/yicidianliangdengzhu.txt" download="" target="_blank">依次点亮灯珠</a>
* <a href="../download/积木块说明案例源代码/xianglin4gedengdaibutongyanse.txt" download="" target="_blank">相邻4个灯带为不同颜色</a>