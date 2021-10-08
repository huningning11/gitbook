#打印机

![](/media/screenshot42.png)

##1.功能描述


###基础知识
热敏打印机的原理：在淡色材料上（通常是纸）覆上一层透明膜，将膜加热一段时间后变成深色（一般是黑色，也有蓝色）。图象是通过加热，在膜中产生化学反应而生成的。这种化学反应是在一定的温度下进行的。高温会加速这种化学反应。当温度低于60℃时，膜需要经过相当长，甚至长达几年的时间才能变成深色；而当温度为200℃时，这种反映会在几微秒内完成。热敏打印机有选择地在热敏纸的确定位置上加热，由此就产生了相应的图形。加热是由与热敏材料相接触的打印头上的一个小电子加热器提供的。加热器排成方点或条的形式由打印机进行逻辑控制，当被驱动时，就在热敏纸上产生一个与加热元素相应的图形。控制加热元素的同一逻辑电路，同时也控制着进纸，因而能在整个标签或纸张上印出图形。


###硬件连接

<div align = "center">
    <img src="/media/dayinji2.png" width="100%">
    <img src="/media/dayinji3.png" width="100%">
    <h5>图2 3 打印机连线</h5>
</div>


###功能简介


![](/media/dyj1.png)

* 连接打印设备。调用该积木块前请确保打印机已连接。
* 注：打印前请先调用该积木块。
  
![](/media/dyj2.png)

* 打印图片。

![](/media/dyj3.png)

* 打印图片并自动缩小到合适打印的尺寸。

![](/media/dyj4.png)

* 打印图片的素描像并自动缩小到合适打印的尺寸。

![](/media/dyj5.png)

* 打印一行文字。注：该积木块无法正常打印中文。

![](/media/dyj6.png)

* 打印条形码。

![](/media/dyj99.png)

* 打印一行文字。支持中英文。

![](/media/dyj8.png)

* 打印一行中文文字，可调节字体大小，打印的水平、垂直起始位置。

![](/media/dyj9.png)

* 打印空白行。

![](/media/dyj10.png)

* 设置打印位置（左对齐/居中/右对齐），该设置对中文内容无效。

![](/media/dyj11.png)

* 设置打印字体大小，该设置对中文内容无效。

![](/media/dyj12.png)

* 设置打印机默认格式。

![](/media/dyj13.png)

* 使用打印机打印文件。要确保打印机联网，并且支持eprint功能。


###参数说明


![](/media/dyj1.png)

* 无参数。

![](/media/dyj2.png)

* 参数一：输入要打印图片的本地路径。

![](/media/dyj3.png)

* 参数一：输入要打印图片的本地路径。

![](/media/dyj4.png)

* 参数一：输入要打印图片的本地路径。

![](/media/dyj5.png)

* 参数一：输入要打印的文字。注意该积木块无法正常打印中文。

![](/media/dyj6.png)

* 参数一：输入要打印的字符串。
* 参数二：选择打印的类型。

![](/media/dyj99.png)

* 参数一：输入要打印的文字，支持中英文。

![](/media/dyj8.png)

* 参数一：输入要打印的文字。
* 参数二：输入打印文字的大小。
* 参数三：输入打印水平起始位置。
* 参数四：输入打印垂直起始位置。

![](/media/dyj9.png)

* 参数一：输入要打印几行空白。

![](/media/dyj10.png)

* 参数一：设置打印位置（左对齐/居中/右对齐）

![](/media/dyj11.png)

* 参数一：设置打印字体大小（小号/中号/大号）

![](/media/dyj12.png)

* 无参数

![](/media/dyj13.png)

* 参数一：打印机的邮箱
* 参数二：要打印的文件绝对路径，文件大小不能超过10M，支持打印的文件格式有Word、Excel、PPT、HTML、TXT，图片必须为JPG格式。并且水平和垂直分辨率大于300像素。



###积木块应用

<div align="center">
    <img src="/media/screenshot43.png" alt="图2" width="455">
    <h4>（图5）打印机打印多行文字</h4>
</div>  


##2.综合运用案例

1. 打印机相关脚本
<div align = "center">
    <img src="/media/dayinji4.png" width="100%">
    <h5>图4 打印机相关脚本</h5>
</div>
2. 通过按键打印文本
<div align = "center">
    <img src="/media/dayinji5.png" width="100%">
    <h5>图5 打印机测试</h5>
</div>
3. 打印文本并调整字体大小及位置
<div align = "center">
    <img src="/media/dayinji6.png" width="100%">
    <h5>图6 印文本并调整字体大小及位置</h5>
</div>

4. 拍摄图像自动打印
<div align = "center">
    <img src="/media/dyj98.png" width="100%">
    <h5>图7 拍立得</h5>
</div>


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/dyj.txt" download="" target="_blank">打印机测试</a>
* <a href="../download/积木块说明案例源代码/dyj1.txt" download="" target="_blank">打印机打印文字</a>


##4、相关课程链接
1. [语音自助打印出入证](https://mp.weixin.qq.com/s/2iPQK7nwpY5DGUlvaeeNNw)
