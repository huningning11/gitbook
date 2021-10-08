#数码管
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识

led数码管（LED Segment Displays）由多个发光二极管封装在一起组成“8”字型的器件，引线已在内部连接完成，只需引出它们的各个笔划，公共电极。数码管实际上是由七个发光管组成8字形构成的，加上小数点就是8个。这些段分别由字母a,b,c,d,e,f,g,dp来表示。如图1所示。

<div align = "center">
<img src="/media/shumaguan1.jpg" width="100%">
<h5>图1 四位数码管</h5>
</div>
led数码管常用段数一般为7段有的另加一个小数点。位数有半位，1，2，3，4，5，6，8，10位等等，led数码管根据LED的接法不同分为共阴和共阳两类，了解LED的这些特性，对编程是很重要的，因为不同类型的数码管，除了它们的硬件电路有差异外，编程方法也是不同的。led数码管广泛用于仪表，时钟，车站，家电等场合。

<div align = "center">
    <img src="/media/shumaguan2.png" width="100%">
    <h5>图2 8段数码管</h5>
</div>

##二、硬件连接

数码管在与扩展板进行连接时，应遵循引脚顺序一一对应的原则正确插入，如遇到扩展板的接口顺序与扩展板引脚顺序不一致时，则应使用杜邦线进行连接。接口队形如下图所示。

<div align = "center">
    <img src="/media/shumaguan3.png" width="100%">
    <h5>图3 数码管连线</h5>
</div>

##三、基础应用（图形化）

1. 数码管基本结构如图所示
<div align = "center">
    <img src="/media/shumaguan4.png" width="100%">
    <h5>图4 数码管基本设置</h5>
</div>
2. 测试数码管：显示一个字符。程序如下
<div align = "center">
    <img src="/media/shumaguan5.png" width="100%">
    <h5>图5 显示一个字符</h5>
</div>
3. 在数码管上显示多个字符
<div align = "center">
    <img src="/media/shumaguan6.png" width="100%">
    <h5>图6 显示多个字符</h5>
</div>
4. 在数码管上显示小数
<div align = "center">
    <img src="/media/shumaguan7.png" width="100%">
    <h5>图7 显示小数</h5>
</div>
5. 显示冒号
<div align = "center">
    <img src="/media/shumaguan8.png" width="100%">
    <h5>图8 显示冒号</h5>
</div>

6、此处为下载链接

7、数码管效果演示视频

[数码管效果演示视频](https://weibo.com/3264309324/JE36iASi2)

##四、基础应用（Python）

准备工作：

步骤1：安装smbus模块
使用pip3 install smbus命令或者直接在Thonny内搜索安装。

步骤2：编写TM1650模块
打开网页链接：https://raw.githubusercontent.com/GDWrobot/modules/master/TM1650.py
新建一个TM1650.py文件，将网页上的所有代码复制粘贴并保存。

1. 点亮测试
<div align = "center">
    <img src="/media/shumaguan9.png" width="100%">
    <h5>图9 点亮测试</h5>
</div>
2. 功能介绍
<div align = "center">
    <img src="/media/shumaguan10.png" width="100%">
    <img src="/media/shumaguan11.png" width="100%">
    <h5>图10 11  功能介绍</h5>
</div>
3. 在数码管上显示四位数
<div align = "center">
    <img src="/media/shumaguan12.png" width="100%">
    <h5>图12 显示四位数</h5>
</div>

##五、相关课程链接
1. [电子时钟](https://mp.weixin.qq.com/s/7qiR2_X1MvG0sNlQNYTM9w)