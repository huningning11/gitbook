#180°舵机
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识
LCD液晶屏是Liquid Crystal Display 的简称，LCD 的构造是在两片平行的玻璃当中放置液态的晶体，两片玻璃中间有许多垂直和水平的细小电线，透过通电与否来控制杆状水晶分子改变方向，将光线折射出来产生画面。LCD比CRT的使用寿命更长，能源消耗更低，成本更低。

屏幕能显示的基本原理就是在两块平行板之间填充液晶材料，通过电压来改变液晶材料内部分子的排列状况，以达到遮光和透光的目的来显示深浅不一，错落有致的图象，而且只要在两块平板间再加上三元色的滤光层，就可实现显示彩色图象。

此处我们使用的是2*16的LCD屏，如下图所示。
<img src="/media/LCDshiyitu.png"  align = "center" width="80%">
<h5 align = "center">LCD显示屏</h5>

##二、硬件连接

LCD显示屏有四个引脚，分别为GND、VCC、SDA、SCL，在LCD屏接入扩展板时，需注意扩展板的接口顺序与该模块接口不一致，需要借助杜邦线进行连接，当该模块正确接入扩展板后，LCD屏幕会亮起，显示蓝色，效果如下图所示。

连接端口对应为：GND—GND、VCC—VCC、SDA—CLK、SCL—DATA

<img src="/media/LCDlianxian.png"  align = "center" width="100%">
<h5 align = "center">图2 LCD屏正确连接示意图</h5>

##三、基础应用（图形化）
1、	测试LCD屏程序，在LCD屏的第二行第一列显示字符串hello world。具体代码以及显示效果如下图所示。

<img src="/media/LCDdaima.png"  align = "center" width="100%">
<h5 align = "center">图2 测试代码</h5>

<img src="/media/LCDshixianxiaog.png"  align = "center" width="100%">
<h5 align = "center">图3 实现效果 </h5>

2.此处为程序代码下载链接


##四、基础应用（Python）
暂无，需要后期补充


##五、相关课程链接
暂无，需要后期补充