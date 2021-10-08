#flick hat
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识

Flick hat是一种扩展板，插槽可以直接连接到树莓派主板，使得使用者可以添加3D和手势功能。Flick hat可以和树莓派项目进行结合，以提供一个新的控制方法，即通过手势和触摸控制，甚至可以将已经完成的flick项目隐藏到非导电材料的后面，使用近场手势技术，它可以在以10cm为半径的3D球形区域内检测到手势，这就意味着使用者是需要滑动手部，轻点手指或者画一个形状，flick hat就可以进行追踪。

Flick hat即插即用，因此可以在短时间内进行启用和运行。Pi电源提供软件库，向用户展示什么是可能的，并协助用户启动项目。使用flick hat，用户可以控制计算机、TV、音乐系统等。

下图为flick hat的示意图。
<div  align = "center">
    <img src="/media/flickhat1.png" width="80%">
    <h5>图1 Flick hat</h5>
</div>

##二、硬件连接
Flick hat和树莓派的组装方法如下图所示。
<div  align = "center">
    <img src="/media/flickhatyingjianlianjie.png" width="100%">
    <h5>图2 flickhat与树莓派连接</h5>
</div>

##三、基础应用（图形化）
1.测试点击手势：调用flick hat的积木块可以在智能硬件里找到，古德微平台在智能硬件中有独立的积木模块—手势控制。如下图所示。
<div  align = "center">
    <img src="/media/flickhatjimukuai.png" width="100%">
    <h5>图2 flick hat积木块</h5>
</div>

下图为flick hat的手势示意图，以中心为节点，分别是上北下南，左西右东，和传统的地图指针是一样的。
<div  align = "center">
    <img src="/media/flickhatshangbeixianan.png" width="100%">
</div>
<div  align = "center">
    <img src="/media/shangbeixiananflickhat.png" width="100%">
</div>

具体的测试代码如下图所示：
<div  align = "center">
    <img src="/media/ceshiflickhat.png" width="100%">
</div>

2.通过flickhat进行控制小灯的亮灭：通过判断手势是否为center，从而控制小灯的亮灭，如果手势为center，则小灯亮起，如果手势不是center，则小灯熄灭，具体程序如下图所示。
<div  align = "center">
    <img src="/media/flickhatkongzhixiaodengliangmie.png" width="100%">
</div>

3.此处为代码下载链接

4.flick hat相关程序效果演示视频

[flick hat效果演示视频](https://mc.dfrobot.com.cn/thread-302607-1-1.html)


##四、基础应用（Python）
1. 手势识别控制灯带

暂无，需要后续补充

##五、相关课程链接
1. [智能视力测试仪（上）](https://mp.weixin.qq.com/s/-3PwAOlAULrNESi4N4OCaQ)
2. [智能视力测试仪（下）](https://mp.weixin.qq.com/s/GP9lSImdNFz2zUetaMI2FA)
