#字典积木块区


##1.功能描述

###使用场景
字典是另一种可变容器模型，且可存储任意类型对象。
<br>字典的每个键值 key=>value 对用冒号 : 分割，每个键值对之间用逗号 , 分割，整个字典包括在花括号 {} 中。
<br>键一般是唯一的，如果重复最后的一个键值对会替换前面的，值不需要唯一。
###功能介绍
![](/media/gxd/list/017.jpg)
* 功能简介：创建一个空字典。
* 参数说明：字典
* 返回值：无

![](/media/gxd/list/016.jpg)
* 功能简介：为字典添加或者更新键值对，更新键值对会将输入的参数二替换原有的键值对的值。
* 参数说明：
  <br>参数一，字典
  <br>  参数二：键，数据类型：字符数据类型。
  <br> 参数三：值，数据类型：字符数据类型。
* 返回值：无

![](/media/gxd/list/018.jpg)
* 功能简介：清空字典内的所有字符串
* 参数说明：字典
* 返回值：无


![](/media/gxd/list/019.jpg)
* 功能简介：删除字典内的键为参数二的键值对
* 参数说明：
  <br>  参数一：字典
  <br>   参数二：键，数据类型：字符数据类型。
* 返回值：无

![](/media/gxd/list/010.jpg)
* 功能简介：输出指定字典的指定键对应的值
* 参数说明：
  <br>  参数一：字典
  <br>   参数二：键，数据类型：字符数据类型。
* 返回值：键对应的值，数据类型：字符数据类型。

![](/media/gxd/list/020.jpg)
* 功能简介：输出指定字典的所有键
* 参数说明： 字典
* 返回值：字典内的所有键，数据类型：字符数据类型。

![](/media/gxd/list/021.jpg)
* 功能简介：输出指定字典中所有值
* 参数说明：字典
* 返回值：字典内的所有值，数据类型：字符数据类型。

![](/media/gxd/list/022.jpg)
* 功能简介：以json字符串的格式输出指定字典的所有键值对
* 参数说明：字典
* 返回值：json格式下字典内的所有键值对，数据类型：json字符数据类型。


###积木块应用
* 创建一个名为变量的空字典
  ![](/media/gxd/list/037.jpg)

* 为字典变量添加或更新一个键为key，值为abc123的键值对
  ![](/media/gxd/list/038.jpg)

* 清空名为变量的字典
  ![](/media/gxd/list/039.jpg)

* 将字典变量中键为key的键值对删除
  ![](/media/gxd/list/040.jpg)

* 输出字典test1中的键为key对应的值
  ![](/media/gxd/list/044.jpg)

* 输出字典变量中的所有键
  ![](/media/gxd/list/041.jpg)

* 输出字典变量中的所有值
  ![](/media/gxd/list/042.jpg)

* 以json字符串的格式输出字典变量的所有键值对
  ![](/media/gxd/list/043.jpg)


##2.综合运用案例
无


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/gxd/list/list008.txt" download="" target="_blank">创建空字典</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list009.txt" download="" target="_blank">添加/更新字典键值对</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list010.txt" download="" target="_blank">清空字典</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list011.txt" download="" target="_blank">删除字典键相对应的值</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list012.txt" download="" target="_blank">查询字典所有键</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list013.txt" download="" target="_blank">查询字典所有值</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list015.txt" download="" target="_blank">json输出字典键值对</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list015.txt" download="" target="_blank">输出字典指定键对应的值</a>
