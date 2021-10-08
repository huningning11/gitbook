#####一、4G模块使用设置方法
此方法适合SIM7600X 4G模块与树莓派的连接使用。  
1、	把4G模块与树莓派连接（40pin针脚对齐即可），配套的USB线一端连接到4G模块的USB接口（注意不是USB TO UART接口），另外一端连接到树莓派的USB接口，把天线连接到4G模块的MAIN主天线接口；  
<img src="/Appendix/four-G-picture/1.jpg" width="50%" height="50%">  
<img src="/Appendix/four-G-picture/12.jpg" width="50%" height="50%">  
2、	把控制方式选择到B树莓派控制，工作电压选择到5V，如果还需要使用到扩展板，可以把扩展板直接安装在4G模块上面（40pin针脚对应即可）  
<img src="/Appendix/four-G-picture/2.jpg" width="50%" height="50%">  
3、	连接树莓派相关配件，启动树莓派，看到4G模块的电源指示灯和网络状态灯常亮，表示电源供电正常，网络正在找网。  
4、	在树莓派的桌面，打开终端，出现如下界面。  
<img src="/Appendix/four-G-picture/4.jpg" width="50%" height="50%">  
<img src="/Appendix/four-G-picture/42.jpg" width="50%" height="50%">  
5、	在终端输入sudo raspi-config指令，按下Enter回车键，出现如下界面。 
<img src="/Appendix/four-G-picture/5.jpg" width="50%" height="50%">   
6、	使用键盘的上下键，选择到Interfacing Options选项，按下Enter回车键，出现如下界面。  
<img src="/Appendix/four-G-picture/6.jpg" width="50%" height="50%">    
<img src="/Appendix/four-G-picture/62.jpg" width="50%" height="50%">  
7、	通过键盘的上下键，选择到Serial选项，按下Enter回车键，出现如下界面。  
<img src="/Appendix/four-G-picture/7.jpg" width="50%" height="50%">  
8、	通过左右方向键，选择到否，按下Enter回车键，出现如下界面。  
<img src="/Appendix/four-G-picture/8.jpg" width="50%" height="50%">  
9、	选择到是，按下Enter回车键，出现初始的界面。  
<img src="/Appendix/four-G-picture/9.jpg" width="50%" height="50%">    
10、关闭终端，通过系统，重新启动树莓派。  
<img src="/Appendix/four-G-picture/10.jpg" width="50%" height="50%">  
<img src="/Appendix/four-G-picture/10 2.jpg" width="50%" height="50%">  
11、树莓派重新启动之后，登录古德微平台，在智能硬件选项里面找到4G通信模块的相关积木块，使用开机积木块测试4G模块是否启动，调试区有对应的信息输出，通知书4G模块上的网络状态灯一直闪烁，说明4G模块正常启动，可以使用了。  
<img src="/Appendix/four-G-picture/11.jpg" width="50%" height="50%">  
<img src="/Appendix/four-G-picture/112.jpg" width="50%" height="50%">  