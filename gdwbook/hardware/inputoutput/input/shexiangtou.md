#摄像头
##目录
一、基础知识

二、硬件连接

三、基础应用（图形化）

四、基础应用（Python）

五、相关课程链接

##一、基础知识

摄像头（webcam）一般具有视频摄像/传播和静态图像捕捉等基本功能，它是借由镜头采集图像后，由摄像头内的感光组件电路及控制组件对图像进行处理并转换成电脑所能识别的数字信号，然后借由并行端口或USB连接输入到电脑后由软件再进行图像还原。如图1所示。
<div align = "center">
    <img src="/media/shexiangtou1.png" width="100%">
    <h5>图1 摄像头</h5>
</div>

##二、硬件连接
<div align = "center">
    <img src="/media/shexiangtou2.png" width="100%">
    <h5>图2 摄像头连线</h5>
    <img src="/media/connect-camera.gif" width="100%">
    <h5>图3 摄像头连接动画演示</h5>
</div>

##三、基础应用（图形化）

1. 摄像头脚本
<div align = "center">
    <img src="/media/shexiangtou3.png" width="100%">
    <img src="/media/shexiangtou4.png" width="100%">
    <h5>图4 摄像头脚本</h5>
</div>

2. 拍照并储存
<div align = "center">
    <img src="/media/shexiangtou5.png" width="100%">
    <h5>图5 拍照并储存</h5>
</div>

##四、基础应用（Python）
1. 拍照并储存
```python
from picamera import PiCamera
from time import sleep
camera = PiCamera()
camera.start_preview() # 开始预览 
sleep(3) # 预览3秒钟
camera.stop_preview() # 停止预览
camera.capture('/home/pi/Desktop/image.jpg') # 拍照并保存至桌面
```

##五、相关课程链接
1. [文字识别](https://mp.weixin.qq.com/s/8oVdUxfMslluUfM1St2UHw)
2. [语音自助打印出入证](https://mp.weixin.qq.com/s/2iPQK7nwpY5DGUlvaeeNNw)
3. [智能停车场](https://mp.weixin.qq.com/s/y8r2pbIMUL1xHIxC4kkoZQ)