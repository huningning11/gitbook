#人脸检索积木块区

![](/media/BD_facesearch0.png)

##1.功能描述

###功能简介

![](/media/BD_face_search_info.png)

* 通过百度AI人脸识别进行人脸检测功能，初始化人脸检索信息。运行其他人脸检索积木块时，须先运行该积木块。

![](/media/BD_face_search_facelocation.png)

* 获取指定人脸框在人脸照片中的坐标位置以及人脸的倾斜角度；坐标位置从左上角开始。

![](/media/BD_face_search_userinfo.png)

* 获取指定人脸用户的信息字典。

![](/media/BD_face_search_facegroup.png)

* 获取指定人脸用户所在的用户组，该用户组与百度AI上的对应一致。

![](/media/BD_face_search_faceuser.png)

* 获取指定人脸所对应的用户名，该用户名与百度AI上的对应一致。


###参数说明

![](/media/BD_face_search_info.png)

* 参数一：本地图片绝对路径，如：/home/pi/imageTemp/face.jpg；  
  数据类型为：字符串（文本）；
  
* 参数二：为百度AI上对应的人脸库用户组，不同用户组用“，”分隔，格式如：‘group1,group2’；  
  数据类型为：字符串（文本）；
  
* 参数三：为最多的处理人数，数据范围为：1-10；数据类型为：整型（数字）；  
  若一张照片中有20张人脸，该参数设置为：3；即处理最多人数为3人，最终返回的结果也只包含前三个人的信息；  
  **人脸识别顺序按方框大小排列，即：按人脸的像素大小顺序排列。**

![](/media/BD_face_search_facelocation.png)

* 参数一：欲获取人脸的序列号，数据最大值为第一个积木块的处理人数；  
  数据类型为：整型（数字）。

![](/media/BD_face_search_userinfo.png)

* 参数一：欲获取人脸的序列号，数据最大值为第一个积木块的处理人数；  
  数据类型为：整型（数字）。

![](/media/BD_face_search_facegroup.png)

* 参数一：欲获取人脸的序列号，数据最大值为第一个积木块的处理人数；  
  数据类型为：整型（数字）。

![](/media/BD_face_search_faceuser.png)

* 参数一：欲获取人脸的序列号，数据最大值为第一个积木块的处理人数；  
  数据类型为：整型（数字）。

###返回值

![](/media/BD_face_search_info.png)

* 返回值为人脸信息的字典；列表内容包含：每个人脸的信息字典：人脸位置信息、人脸所属的用户组、人脸所对应的用户名、相似度等；  
  **字典人脸的数量与参数三的取值有关**，若取值为三，则最多只返回包含三个人脸信息的字典。  
  若获取失败则返回：None；
  数据类型为：列表。

![](/media/BD_face_search_facelocation.png)

* 返回指定人脸在照片中的位置信息字典：  
  包含包括：[人脸框的x/y轴像素坐标,宽/高度,人脸框相对于竖直方向顺时针旋转角]；  
  X和Y、宽度和高度的取值范围与照片像素有关；人脸框旋转角度范围：-180°~180°；  
  积木返回值数据类型为：字典；列表中的数据类型都为：整型。

![](/media/BD_face_search_userinfo.png)

* 返回指定人脸的信息字典，包括：人脸所属的用户组、人脸所对应的用户名、相似度；  
  数据类型为：字典。

![](/media/BD_face_search_facegroup.png)

* 返回指定人脸所属的用户组名，如：“group1” ，数据类型为：字符串（文本）。

![](/media/BD_face_search_faceuser.png)

* 返回指定人脸所对应的用户名，如：“GDWrobot”，数据类型为：字符串（文本）。

###积木块应用

<div align="center">
    <img src="/media/BD_facesearch1.png" alt="图2" width="1145">
    <h4>（图1）输出人脸搜索结果</h4>
</div>

##2.综合运用案例

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/facesearch-1" download="" target="_blank">输出人脸搜索的结果</a>