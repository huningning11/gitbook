#物联网课程
> 制作：杭州古德微机器人有限公司
> 最后更新：2020.4.16
>
>
## 目的
为响应国务院和教育部提出在中小学逐步设置人工智能和编程课程的号召，特开设基于树莓派的物联网主题课程。帮助学生通过编程和实践，感知、体验和应用物联网与人工智能，提升采集数据分析数据的能力，掌握具体实验现象、数据和实验原理通过图像和动画展示的方法。

物联网课程是本课程体系的进阶主题课程，在物联网课程中，首先简单的介绍物联网的概念和应用范围，然后用顺风耳、千里眼-数据采集，如来手-远程控制等直观的物联网体验感受知识的力量。
实验中通过智能数据采集、呈现、分析等实际案例的学习，有利于开启在科学实验和现实生活中融入人工智能，使人工智能的应用有迹可循。

##课程内容

树莓派人工智能课程如下：
<div align="center">
    <img src="/media/iot.png" width="80%">
</div>

具体课程内容请查看课程章节介绍，以下是部分课程案例。

##古德微机器人物联网应用案例
  杭州古德微机器人有限公司是一家致力于青少年编程教育的公司。公司通过自研的图形化在线编程平台，依托树莓派硬件，将编程结果实物化。在线编程平台集成了完备的MQTT物联网功能（如数据交换、远程控制，数据采集，数据呈现，自定义物联网服务器，语音和图片物联，万物互联等），使物联网教学演示便捷和直观，应用到创客作品的制作中，可以使得创客作品更智能，更有趣。
##公司Logo
<div align="center">
    <img src="/media/logo.jpg" width="20%">
</div>

##案例故事
 ***核心诉求：***
  我们希望在进行物联网教学时，可以很方便的将原理通过简单形象的展示出来，同时还可以和学生互动以增加学习的兴趣和对知识的理解。
  使用物联网技术制作创客作品时，可以很方便的通过编程添加各种物联网技术，如远程控制、数据采集、数据呈现、数据分析等，从而使得创客作品更智能，更神奇。
 
  ***解决方案：***
  古德微机器人开发的图形化在线编程平台，集成了MQTT客户端、本地服务器、远程服务器。用户只要简单的拖动下积木，进行简单编程，即可实现万物互联的各种神奇功能。
下面通过案例来说明如何使用本编程平台。
   - 案例1：无线按键控制灯
   - 案例2：爱心传递
   - 案例3：超声波数据实时采集和展示
   - 案例4：智能控制风扇
   
###第一步
登陆编程平台：gdwrobot.cn/robot_system/  （如图一）
<div align="center">
    <img src="/media/login.png" alt="图1" width="80%">
    <h4>图 1  编程平台登陆</h4>
</div>

###第二步
连接设备，将树莓派连接到编程平台
<div align="center">
    <img src="/media/mainui.png" alt="图2" width="80%">
    <h4>图 2  编程平台界面</h4>
</div>

###第三步
***案例 1 无线按键控制灯：*** 拖动积木编程，实现树莓派A按钮控制发送IOT信号、树莓派B接收IOT信号并控制小灯亮灭。如图3所示，通过积木编程可以通过树莓派A的按钮控制树莓派B的小灯。
详细内容可点击[观看微课](https://mp.weixin.qq.com/s?__biz=MzU4MTUyNzQ3Mw==&mid=2247484574&idx=5&sn=f70d97041b0503528dd85f9bd1099496&chksm=fd477640ca30ff563e78eff67fcfbf0042b10912891ae2415381bab501ec41634289b2f87fc6&token=234287060&lang=zh_CN&scene=21#wechat_redirect)
<div align="center">
    <img src="/media/itosend.png" alt="图3a" width="80%">
    <h4>图 3（a）树莓派A 按钮控制发送IOT信号</h4>
    <img src="/media/iotreceive.png" alt="图3b" width="80%">
    <h4>图 3（b）树莓派B 接收IOT信号并控制小灯亮灭</h4>
</div>

***案例 2 爱心传递：*** 拖动积木编程，实现树莓派A显示爱心，倾斜时消除爱心并发消息给树莓派B、树莓派B接收信号显示爱心，倾斜时消除爱心并发消息给树莓派C。如图4所示，通过积木编程可以倾斜。
详细内容可点击[观看微课](https://mp.weixin.qq.com/s/SPdllOlaYcwLu41sDYRL7A)
<div align="center">
    <img src="/media/loveA.png" alt="图4a" width="80%">
    <h4>图 4（a）树莓派A显示爱心，倾斜时消除爱心并发消息给树莓派B</h4>
    <img src="/media/loveB.png" alt="图4b" width="80%">
    <h4>图 4（b）树莓派B接收信号显示爱心，倾斜时消除爱心并发消息给树莓派C</h4>
    <img src="/media/loveC.png" alt="图4c" width="80%">
    <h4>图 4（c）树莓派C接收B的信号显示爱心</h4>
</div>

***案例 3 超声波数据实时采集和展示：*** 拖动积木编程， 实现图5a树莓派数据采集和发送代码，如图5b所示通过简单配置可生成图5c所示的自定义数据接收和展示页面，通过二维码还可以分享查看实时数据动态展示页面。
<div align="center">
    <img src="/media/datacapturecode.png" alt="图5a" width="80%">
    <h4>图 5（a）树莓派数据采集发送</h4>
    <img src="/media/datacaptureconfig.png" alt="图5b" width="80%">
    <h4>图 5（b）自定义网页配置</h4>
    <img src="/media/datacapturedisplay.png" alt="图5a" width="80%">
    <h4>图 5（C）数据实时动态展示</h4>
    <h4><img src="/media/datacaptureshare.png" alt="图5a" width="20%"></h4>
    <h4>图 5（d）二维码分享数据展示</h4>
</div>

***案例 4 智能控制风扇：*** 拖动积木编程，实现树莓派接收信号并控制风扇代码，如图6b所示通过简单配置可生成图6c所示的自定义远程控制界面、通过二维码还可以分享远程控制界面邀请好友一起远程控制风扇。
<div align="center">
    <img src="/media/romotcontrolcode.png" alt="图6a" width="80%">
    <h4>图 6（a）树莓派接收信号并控制风扇代码</h4>
    <img src="/media/romotcontrolconfig.png" alt="图6b" width="80%">
    <h4>图 6（b）自定义网页配置</h4>
    <img src="/media/romotcontrolpage.png" alt="图6a" width="80%">
    <h4>图 6（C）远程控制界面</h4>
    <h4><img src="/media/romotcontrolshare.png" alt="图6a" width="20%"></h4>
    <h4>图 6（d）二维码分享数据展示</h4>
</div>


##相关视频课程
1. [视频课程链接](https://www.bilibili.com/video/BV1Uh411X72S/)