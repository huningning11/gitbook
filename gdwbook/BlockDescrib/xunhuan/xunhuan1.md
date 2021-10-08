#循环积木块

![](/media/xunhuan1.png)

![](/media/xunhuan3.png)

![](/media/xunhan2.png)

##1.功能描述

###功能简介

![](/media/xunhuan1.png)

* 执行框中的程序直到达到一定次数后跳出循环。

![](/media/xunhuan3.png)

* 执行框中的程序直到达到不满足条件后跳出循环。

![](/media/xunhan2.png)

* 设置循环的区间和参数，执行框中的程序直到达到区间最大值后跳出循环。

###参数说明

![](/media/xunhuan1.png)

* 参数一：填输入循环所需要执行的次数，数据类型为：整型（数字）。

![](/media/xunhan2.png)

* 参数一：默认为i，可改为自己设置的变量；
* 参数二：变量参数的初始值，数据类型：整型（数字）；
* 参数三：变量参数的停止值，数据类型：整型（数字）；
* 参数四：变量参数的间隔值，数据类型：整型（数字）；




###积木块应用

<div align="center">
    <img src="/media/xunhuantupian1.png" alt="图1" width="755">
    <h4>（图1）循环使用案例1</h4>
</div>

* 设置参数为10，则循环框内程序10次，在输出10个调试信息后程序停止。
<div align="center">
    <img src="/media/xunhuantupian2.png" alt="图2" width="651">
    <h4>（图2）循环使用案例2</h4>
</div>

* 在循环条件处设置条件为真是常用的无限循环使用方法，循环的条件一直满足则循环一直继续，该程序将会一直输出调试信息。
<div align="center">
    <img src="/media/xunhuantupian3.png" alt="图3" width="844">
    <h4>（图3）循环使用案例3</h4>
</div>

* 设置变量为默认i，起始为1，终止为10，间隔为1，则程序开始时赋值i=1，进行1次循环，后对i增加间隔值，即i=1+1=2，再进行一次循环，直到i=10，进行循环后跳出程序。该程序中每进行一次循坏输出一次i值，最终输出数字1到10后程序停止。




##3.案例代码下载
* <a href="../download/积木块说明案例源代码/xunhuananli1.txt" download="" target="_blank">循环案例1代码</a>
* <a href="../download/积木块说明案例源代码/xunhuananli2.txt" download="" target="_blank">循环案例2代码</a>
* <a href="../download/积木块说明案例源代码/xunhuananli3.txt" download="" target="_blank">循环案例3代码</a>