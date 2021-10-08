#HUSKYLENS摄像头积木块区

<div align="left">
    <img src="/media/BD_huskylens0-2.png" alt="图1" width="330">
    <img src="/media/BD_huskylens0-1.png" alt="图1" width="409">
</div>  

##1.功能描述

###功能简介

![](/media/BD_huskylens_algorthim.png)

* 切换Huskylens摄像头算法，内置7种功能：人脸识别、物体追踪、物体识别、巡线追踪、颜色识别、标签识别、物体分类。
* 若不切换算法，可不调用该积木块，可通过摄像头上的滚轮按钮手动切换算法。
* 若需自动切换算法，可调用该积木，需在使用其他huskylens积木块之前使用该积木块。

![](/media/BD_huskylens_2_saveScreenshotToSDCard.png)

* 将Huskylens摄像头屏幕上的截图（带界面文字）保存到SD卡中，SD卡为摄像头上的SD卡，而非树莓派本地中。

![](/media/BD_huskylens_2_savePictureToSDCard.png)

* 将Huskylens摄像头所拍到的图片（无其他参数文字）保存到SD卡中，SD卡为摄像头上的SD卡，而非树莓派本地中。

![](/media/BD_huskylens_2_learn.png)

* Huskylens摄像头学习训练模型操作，运行该积木块后，摄像头对当前画面中的物体进行学习。

![](/media/BD_huskylens_2_forget.png)

* 将当前算法下的模型遗忘，其他算法的模型仍保留存在。

![](/media/BD_huskylens_2_setCustomName.png)

* 在当前算法下，重命名指定已学习的ID对象名称，不改变其他算法的对象ID名称。

![](/media/BD_huskylens_2_saveModelToSDCard.png)

* 在当前算法下，保存当前已学习过的训练模型，至摄像头上的SD卡中。

![](/media/BD_huskylens_2_loadModelFromSDCard.png)

* 在当前算法下，导入指定序号的模型，使用该积木块前，需先切换至需要使用的算法。

![](/media/BD_huskylens_judge_id.png)

* 用来判断摄像头画面中是否存在已学过的目标对象。

![](/media/BD_huskylens_request_id.png)

* 用来获取摄像头画面中已学习过的目标对象在摄像头画面的目标位置。

![](/media/BD_huskylens_id_blocks_data.png)

* 摄像头识别画面中已学习的目标对象时框出方框，该积木块可获取方框在画面的具体位置信息。
* **注：只针对有方框的算法目标对象，对箭头无效**

![](/media/BD_huskylens_id_arrows_data.png)

* 摄像头识别画面中已学习的目标对象时标出箭头，该积木块可获取箭头在画面的具体位置信息。
* **注：只针对有箭头的算法目标对象，对方框无效**

![](/media/BD_huskylens_sumnum.png)

* 用来获取画面中不同目标对象的种类数量。

![](/media/BD_huskylens_request_all.png)

* 用来获取画面中指定范围的所有目标对象位置信息。

![](/media/BD_huskylens_request_all_ID.png)

* 用来获取画面中已学习过的所有方框或箭头的ID。

###接口与按键说明

<div align="center">
    <img src="/media/BD_huskylens1.png" alt="图1" width="912">
    <h4>（图1）HUSKYLENS摄像头接口与按键</h4>
</div>  

####1-接口

* USB接口：连接到电源，给HuskyLens供电；也可以连接到电脑的USB接口，给HuskyLens升级固件。
* 4pin接口（I2C模式）

|  序号   | 标注  | 管脚功能 |用途|
| :----:|:----:|:----:|:----:|
| 1  | T |SDA|串行数据线|
| 2  | R |SCL|串行时钟线|
| 3  | - |GND|电源负极|
| 4  | + |VCC|电源正极|

* **USB接口与4pin接口，任接一个，即可对HuskyLens供电。**
* **由于板载了电源自动切换电路，USB接口与4pin接口可以同时接电源，且优先使用USB接口上的电源。**
* **请确保电源电压与功率足够，防止HuskyLens工作异常。**

####2-功能按键与学习按键

* 向左或向右拨动“功能按键”，切换到不同的功能；
* 短按“学习按键”，学习指定的物体；长按“学习按键”，从不同的角度和距离持续学习指定的物体；如果HuskyLens之前学习过，则短按“学习按键”，可让HuskyLens忘记当前功能下所学的；
* 长按“功能按键”，进入当前功能的二级菜单参数设置界面，向左、向右拨动或向下短按“功能按键”即可设置相关参数。

![](/media/BD_huskylens2.png)

###参数说明

![](/media/BD_huskylens_algorthim.png)

* 参数一：内置7种功能算法：人脸识别、物体追踪、物体识别、巡线追踪、颜色识别、标签识别、物体分类。  
  其他两种：二维码识别以及条形码识别需要更新最新版本固件（积木块未更新操作二维码与条形码积木块）。

![](/media/BD_huskylens_2_learn.png)

* 参数一：为学习对象的ID，数据类型为：整型（数字）。

![](/media/BD_huskylens_2_setCustomName.png)

* 参数一：为已学习对象ID，数据类型为：整型（数字）；
* 参数二：为指定对象名称，数据类型为：字符串（文本）；  
  **注：参数二最好命名为全英文格式，内置固件暂未支持所有的中文字。**

![](/media/BD_huskylens_2_saveModelToSDCard.png)

* 参数一：为模型保存的序列号，模型文件命名格式为：算法+ID(参数一)。  
  数据类型为：整型（数字）。

![](/media/BD_huskylens_2_loadModelFromSDCard.png)

* 参数一：为保存的模型文件的序号，若模型保存时ID为1，则导入时，需要线切换至需要的算法后，再导入序号为1的模型文件。

![](/media/BD_huskylens_judge_id.png)

* 参数一：为学习对象的ID，数据类型为：整型（数字）。
* 参数二：方框或箭头，由算法类型确定是方框或者是箭头，否则无效。

![](/media/BD_huskylens_request_id.png)

* 参数一：为学习对象的ID，数据类型为：整型（数字）。
* 参数二：方框或箭头，由算法类型确定是方框或者是箭头，否则无效。

![](/media/BD_huskylens_id_blocks_data.png)

* 参数一：为学习对象的ID，数据类型为：整型（数字）。
* 参数二：  
  X轴的中心坐标-方框中心点的X轴坐标；   
  Y轴的中心坐标-方框中心的的Y中坐标；  
  宽度：方框宽度的像素大小；  
  高度：方框高度的像素大小。  

![](/media/BD_huskylens_id_arrows_data.png)

* 参数一：为学习对象的ID，数据类型为：整型（数字）。
* 参数二：  
  X轴的起点坐标，箭头起点的X轴坐标值；  
  Y轴的起点坐标，箭头起点的Y轴坐标值；  
  X轴的终点坐标，箭头终点的X轴坐标值；  
  Y轴的终点坐标，箭头终点的Y轴坐标值。  

![](/media/BD_huskylens_sumnum.png)

* 参数一：参数作用范围：所有=已学习+未学习；
* 参数二：方框或箭头，通过算法类型来确定。

![](/media/BD_huskylens_request_all.png)

* 参数一：参数作用范围：所有=已学习+未学习；
* 参数二：方框或箭头，通过算法类型来确定。

![](/media/BD_huskylens_request_all_ID.png)

* 参数一：方框或箭头，通过算法类型来确定。

###返回值

![](/media/BD_huskylens_judge_id.png)

* 返回True或False；画面中有指定ID对象返回True，否则为：False；  
  数据类型为：布尔型（bool）。

![](/media/BD_huskylens_request_id.png)

* 返回位置信息列表；  
  列表第一个元素为：方框中心（箭头起点）X轴坐标值，数据类型为数字；  
  列表第二个元素为：方框中心（箭头起点）Y轴坐标值，数据类型为数字；  
  列表第三个元素为：方框**宽度**像素值大小/箭头**终点X轴**坐标值，数据类型为数字；  
  列表第三个元素为：方框**高度**像素值大小/箭头**终点Y轴**坐标值，数据类型为数字。  

![](/media/BD_huskylens_id_blocks_data.png)

* 返回参数二指定**方框**对象值，数据类型为数字。

![](/media/BD_huskylens_id_arrows_data.png)

* 返回参数二指定**箭头**对象值，数据类型为数字。

![](/media/BD_huskylens_sumnum.png)

* 返回摄像头画面内，当前的方框/箭头的数量，数据类型为：数字。

![](/media/BD_huskylens_request_all.png)

* 返回值为指定范围内的所有方框/箭头的位置信息列表，数据类型为列表；
  若未识别到任何对象，则返回值为空列表；
* **列表中的元素为每个方框/箭头的位置信息列表，即返回值为：嵌套列表**

![](/media/BD_huskylens_request_all_ID.png)

* 返回值为画面中所有已学习的ID组成的列表，
  数据类型为：列表；列表元素数据类型为：数字；
  若没有识别到任何ID，则返回值为空列表


###使用场景
* HuskyLens二哈识图是一款简单易用的AI视觉传感器，直接输出识别结果给控制器，你无需折腾复杂的算法，就能制作非常有创意的项目。  
  在使用时需要将Huskylens设置中将协议种类切换为**I2C模式**。

###积木块应用
* 1、运行![](/media/BD_huskylens_algorthim-2.png)将算法切换至颜色识别。  

<div align="center">
    <img src="/media/BD_huskylens1.gif" alt="图2" width="300">
    <h4>（图2）算法切换过程图</h4>
</div>  

* **2、拍照、截屏保存到SD卡**

<div align="center">
    <img src="/media/BD_huskylens_savecompare.png" alt="图2" width="200">
</div>  

  * HuskyLens可以像一个卡片相机一样，拍照或者截屏摄像头画面，保存到SD卡中，HuskyLens板载一个SD卡插槽，将SD卡插入即可使用。截屏保存的图片包含屏幕上显示的文字、方框等内容，而拍照出来的图片只包含摄像头画面，没有方框、文字信息。  
HuskyLens的7大算法功能均支持该功能。使用此功能时，需要先插入一张SD卡。  
  * <font color=#FF0000> 小提示：</font>
  
    * HUSKYLENS保存的图片，分辨率为320*240，无法更改。
    * 请将SD卡格式化为**FAT32**。因拍照/截图并保存需要一定的时间，因此建议调用该功能的间隔至少**0.5秒**以上。   
    * SD卡插槽向内，需要从里向外插入，插入SD卡的过程如下图所示：

![](/media/BD_huskylens_SDcard.png)

##2.综合运用案例
<div align="center">
    <img src="/media/BD_huskylens3.png" alt="图3" width="663">
    <h4>（图3）基于Huskylens摄像头的人脸识别签到系统</h4>
</div>  

###案例功能简介

* 功能：通过huskylens的人脸识别功能，实现简单的人脸识别签到系统。

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/finger_printer1.txt" download="" target="_blank">基于Huskylens摄像头的人脸识别签到系统</a>
