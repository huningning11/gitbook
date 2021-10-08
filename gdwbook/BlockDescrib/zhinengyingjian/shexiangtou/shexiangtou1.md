#摄像头积木块区


![](/media/shexiangtou01.png)

##1.功能描述

###功能简介
* 摄像头（webcam）一般具有视频摄像/传播和静态图像捕捉等基本功能，它是借由镜头采集图像后，由摄像头内的感光组件电路及控制组件对图像进行处理并转换成电脑所能识别的数字信号，然后借由并行端口或USB连接输入到电脑后由软件再进行图像还原；
* 根据接口方式的不同可以分为USB摄像头和树莓派摄像头，根据能否调焦可分为普通摄像头和可调焦摄像头；
* 摄像头多用作实时照片的获取，物体的识别等功能；
***
![](/media/shexiangtou02.png)
* 功能简介：用树莓派摄像头拍一张照片；
* 返回值：返回照片的保存路径；
***
![](/media/shexiangtou03.png)
* 功能简介：输出视频到网页；该模块主要目的是提供摄像头预览功能；
* 参数一：输入要显示的帧数；
***
![](/media/shexiangtou04.png)
* 功能简介：通过树莓派摄像头拍一段视频；
* 参数一：输入拍摄的时间；
* 参数二：输入该视频保存的路径；
* 返回值：返回该视频保存的路径；
***
![](/media/shexiangtou05.png)
* 功能简介：关闭摄像头；
***
![](/media/shexiangtou06.png)
* 功能简介：输出视频到网页；该模块主要目的是提供USB摄像头预览功能；
* 参数一：输入要显示的帧数；
* 参数二：选择拍照使用的设备编号；可通过获取video设备列表查询；
***
![](/media/shexiangtou07.png)
* 功能简介：通过USB摄像头录制一段视频；
* 参数一：输入视频拍摄的时间；
* 参数二：选择拍摄视频保存的路径；
* 参数三：选择拍摄视频使用设备编号；
***
![](/media/shexiangtou08.png)
* 功能简介：用树莓派摄像头拍摄一张照片；
* 参数一：输入预览的时长；
* 返回值：返回照片的保存路径；
***
![](/media/shexiangtou09.png)
* 功能简介：获取树莓派video的设备列表，当USB摄像头插入时，用来获取其设备id；
* 参数一：返回设备id；
***
![](/media/shexiangtou10.png)
* 功能简介：用USB摄像头拍摄一张照片；
* 参数一：选择拍摄照片的分辨率；
* 参数二：输入拍摄的设备编号；
* 参数三：输入预览的时间；
* 返回值：返回照片的保存路径；
***
![](/media/shexiangtou11.png)
* 功能简介：用树莓派摄像头拍摄一张照片；
* 参数一：输入分辨率宽为多少像素；
* 参数二：输入分辨率高为多少像素；
* 参数三：输入预览的时间；
* 返回值：返回照片的保存路径；
###实物图

<div align="center">
    <img src="/media/shexiangtou1.png" alt="图1" width="828">
    <h4>（图1）树莓派摄像头</h4>
</div>  

<div align="center">
    <img src="/media/shexiangtou12.jpg" alt="图2" width="400">
    <h4>（图2）USB摄像头</h4>
</div>  

###接线图

<div align="center">
    <img src="/media/shexiangtou2.png" alt="图3" width="871">
    <h4>（图3）树莓派摄像头连线</h4>
</div>  

<div align="center">
    <img src="/media/connect-camera.gif" alt="图4" width="842">
    <h4>（图4）树莓派摄像头连接动画演示</h4>
</div>  

<div align="center">
    <img src="/media/shexiangtou13.jpg" alt="图5" width="540">
    <h4>（图5）USB摄像头连线</h4>
</div>  







###积木块应用
<div align="center">
    <img src="/media/shexiangtou14.png" alt="图6" width="634">
    <h4>（图6）摄像头测试案例</h4>
</div>  

##2.综合运用案例
<div align="center">
    <img src="/media/shexiangtou15.png" alt="图7" width="512">
    <h4>（图7）摄像头文字识别</h4>
</div>  


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/shexiangtouanli1.txt" download="" target="_blank">摄像头测试案例</a>
* <a href="../download/积木块说明案例源代码/shexiangtouanli2.txt" download="" target="_blank">摄像头文字识别</a>