#中断循环积木块

![](/media/zhongduanxunhuan.png)

![](/media/xiayixunhuan.png)


##1.功能描述

###功能简介

![](/media/zhongduanxunhuan.png)

* 中断当前循环，跳出到循环的下一个程序；

![](/media/xiayixunhuan.png)

* 中断本次循环，跳过循环的剩余部分进行下一次循环。




###积木块应用

<div align="center">
    <img src="/media/zhongduananli.png" alt="图1" width="699">
    <h4>（图1）中断循环使用案例</h4>
</div>

* 循环参数值为10，该循环本应执行10次，当第一次循环运行到中断循环代码时，跳出循环，所以该程序输出一次调试信息后停止。

<div align="center">
    <img src="/media/xiayixunhuananli.png" alt="图2" width="664">
    <h4>（图2）下一循环使用案例</h4>
</div>

* 循环参数i，从1到10，间隔为1，该程序本应该执行输出10次调试信息，但当满足条件i>1时，执行积木继续下一次循环，跳过剩余的输出调试信息程序，所以最终只输出一次调试信息。



##3.案例代码下载
* <a href="../download/积木块说明案例源代码/zhongduanxunhuandaima.txt" download="" target="_blank">中断循环案例代码</a>
* <a href="../download/积木块说明案例源代码/xiayixunhuandaima.txt" download="" target="_blank">下一循环案例代码</a>