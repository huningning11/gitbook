#常见警示信息含义及解决方式

##1、黄色闪电符号

<img src="/media/yellowsymbol.png"  align = "center" width="30%">
<h5 align = "center">闪电符号示意图</h5>

树莓派显示器右上角可能会出现“闪电”符号，即欠压警告。之所以为出现这个提示，可能是因为树莓派供电电压的问题，如果如果Raspberry Pi的电源电压低于4.63V（+/- 5％），则会显示以下图标。遇到这种情况，最好排查硬件设备，观察是否耗电太多，例如灯带过长；或者还可以更换更好的电源。

##2、红色温度计符号

###温度过高警告（80-85℃）

<img src="/media/85sheshidu.png"  align = "center" width="30%">
<h5 align = "center">温度计1</h5>

如果芯片（soc）的温度在80℃和85℃之间，则显示以下图标。CPU核心将被限制回来以试图降低核心温度。

###温度过高警告（超过85℃）

<img src="/media/85yishang.png"  align = "center" width="30%">
<h5 align = "center">温度计2</h5>

如果芯片的温度超过85℃，则会显示以下图表。CPU核心和GPU将会被限制回来以试图降低核心温度。

解决方法：可以直接使用散热器进行冷却散热直到警告符号消失，或者中断所有的程序，让CPU降温，甚至可以直接断电进行休息。

##3、CPU占有率

如果树莓派连接到显示器，则可以直接在显示器的右上角看到CPU占用率，如果是采用远程桌面的形式，则需要借助远程的操作软件，例如VNC才可以看到CPU占有率，以百分比的形式显示，如果CPU占有率过高，则可以采取关闭不必要的端口的方式来减少CPU的占有率。