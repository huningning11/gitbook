#数码管积木块区

![](/media/shumaguan01.png)

##1.功能描述

###功能简介

* led数码管（LED Segment Displays）由多个发光二极管封装在一起组成“8”字型的器件，引线已在内部连接完成，只需引出它们的各个笔划，公共电极。数码管实际上是由七个发光管组成8字形构成的，加上小数点就是8个。这些段分别由字母a,b,c,d,e,f,g,dp来表示。

![](/media/shumaguan02.png)

![](/media/shumaguan05.png)

* 功能说明：设置数码管亮度；在调用数码管前需要先调用此模块设置亮度；
* 参数说明：参数一输入0-3表示几号数码管，参数二输入0-7表示亮度；

![](/media/shumaguan03.png)

* 功能说明：设置数码管需要显示的内容和显示的位置，以及是否需要显示点；
* 参数说明：参数一输入0-3表示控制数码管的位置，参数二输入0-9表示数码管需要显示的数字，参数三输入0-1，表示是否需要显示当前位置的点；

![](/media/shumaguan04.png)

* 功能说明：关闭相应位置的数码管；
* 参数说明：输入0-3表示需要关闭几号数码管；




###实物图

<div align="center">
    <img src="/media/shumaguan1.jpg" alt="图1" width="310">
    <h4>（图1）四位数码管实物图</h4>
</div>  

<div align="center">
    <img src="/media/shumaguan2.png" alt="图2" width="622">
    <h4>（图2）数码管控制原理图</h4>
</div>  

###连接图


<div align="center">
    <img src="/media/shumaguan3.png" alt="图3" width="1166">
    <h4>（图3）数码管接线图及引脚示意图</h4>
</div> 



###积木块应用
1. 数码管基本结构如图所示
<div align = "center">
    <img src="/media/shumaguan4.png" width="870">
    <h5>图4 数码管基本设置</h5>
</div>
2. 测试数码管：显示一个字符。程序如下
<div align = "center">
    <img src="/media/shumaguan5.png" width="955">
    <h5>图5 显示一个字符</h5>
</div>
3. 在数码管上显示多个字符
<div align = "center">
    <img src="/media/shumaguan6.png" width="947">
    <h5>图6 显示多个字符</h5>
</div>
4. 在数码管上显示小数
<div align = "center">
    <img src="/media/shumaguan7.png" width="1125">
    <h5>图7 显示小数</h5>
</div>
5. 显示冒号
<div align = "center">
    <img src="/media/shumaguan8.png" width="991">
    <h5>图8 显示冒号</h5>
</div>


##2.综合运用案例
<div align="center">
    <img src="/media/shumaguan06.png" alt="图9" width="604">
    <h4>（图9）数码管倒计时</h4>
</div>  



##3.案例代码下载
* <a href="../download/积木块说明案例源代码/shumaguananli1.txt" download="" target="_blank">数码管倒计时</a>
