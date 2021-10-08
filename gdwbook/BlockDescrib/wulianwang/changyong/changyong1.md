#物联网常用积木块区

![](/media/wulianwang01.png)

##1.功能描述

###功能简介
![](/media/wulianwang02.png)
* 功能简介：向目标设备发送数据；
* 参数一：输入需要发送的设备号；
* 参数二：发送数据的主题；
* 参数三：发送数据的具体内容；
***
![](/media/wulianwang03.png)
* 功能简介：监听目标主题并设置初始值；
* 参数一：输入需要监听的主题；
* 参数二：输入初始值；
***
![](/media/wulianwang04.png)
* 功能简介：获取监听主题的数据；需要先调用上一个监听主题的积木块；
* 参数一：输入监听的主题；
* 返回值：返回监听主题的数据；
***
![](/media/wulianwang05.png)
* 功能简介：判断物联网是否收到新数据；
* 参数一：收到新数据返回True，没有则返回False；
***
![](/media/wulianwang06.png)
* 功能简介：判断是否收到目标主题的新数据；
* 参数一：收到新数据返回True，没有则返回False；
***
![](/media/wulianwang07.png)
* 功能简介：自定义物联网服务器和端口号；如不执行本命令，则物联网服务器为古德微的mqtt服务器；如果需要本命令设置自定义物联网服务器，请先复位树莓派，再执行本命令；如mqtt服务器无需校验用户名和密码，则用户名和密码字段无需理会；
* 参数一：输入物联网的服务器；
* 参数二：输入物联网端口；
* 参数三：输入用户名；
* 参数四：输入用户名对应密码；
***
![](/media/wulianwang08.png)
* 功能简介：开启SloT服务器；
***
![](/media/wulianwang09.png)
* 功能简介：停止SloT服务器；
***
![](/media/wulianwang10.png)
* 功能简介：获取当前设备号；
* 返回值：返回当前设备的序号；


###积木块应用
<div align="center">
    <img src="/media/wulianwang11.png" alt="图1" width="937">
    <h4>（图1）物联网拍照</h4>
</div>  

##2.综合运用案例

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/wulianwanganli1.txt" download="" target="_blank">物联网拍照</a>
