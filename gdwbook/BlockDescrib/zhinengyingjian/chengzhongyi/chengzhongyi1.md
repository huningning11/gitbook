#称重仪积木块区

![](/media/chengzhongyi01.png)

##1.功能描述

###功能简介
* 称重传感器通常用于重量测量，是我们日常生活的一个组成部分。其随处可见，例如在超市柜台或在高速公路上。称重仪最基础的原理就是压力传感器，当力施加于物体时使物体发生轻微的形变，再通过对应的方法测量形变的不同程度并记录下相应的力，从而达到称重的目的。本积木块所用称重仪使用的是应变式压力传感器和HX711AD模块。

![](/media/chengzhongyi03.png)
* 参数说明：参数一为数据gpio口，即引脚DT对应接口，参数二为时钟gpio口，即SCK对应接口，参数三为过滤的字节，可设置为32，64，128，默认为128.

![](/media/chengzhongyi04.png)
* 对称重仪进行去皮处理

![](/media/chengzhongyi05.png)
* 功能介绍：获取称重仪上物体的净重，单位为克（g），物体重量不超过5千克（kg）
* 返回值：返回物体净重，数据类型为整型（数字）

![](/media/chengzhongyi06.png)
* 通过调用本函数对称重仪gpio口进行重置



###实物图

<div align="center">
    <img src="/media/chengzhongyi1.jpg" alt="图1" width="800">
    <h4>（图1）称重仪实物图</h4>
</div>  

###接线图

<div align="center">
    <img src="/media/chengzhongyi2.jpg" alt="图2" width="300">
    <h4>（图2）称重仪接线图</h4>
</div>  

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | VCC |VCC|电源正极输入口|
| 2  | Trig(20) |SCK|时钟gpio口|
| 3  | Echo(21) |DT|数据gpio口|
| 4  | GND |GND|电源负极输入口|

###工作原理

<div align="center">
    <img src="/media/chengzhongyi4.png" alt="图3" width="1229">
    <img src="/media/chengzhongyi5.png" alt="图4" width="718">
    <img src="/media/chengzhongyi6.png" alt="图5" width="727">
    <h4>（图3）称重仪原理图</h4>
</div>  




###积木块应用

<div align="center">
    <img src="/media/chengzhongyi02.png" alt="图6" width="944">
    <h4>（图4）称重仪积木块应用</h4>
</div>  



##2.案例代码下载
* <a href="../download/积木块说明案例源代码/chengzhongyianli1.txt" download="" target="_blank">称重仪积木块应用</a>
