#列表修改积木块区


##1.功能描述
###使用场景
对列表进行删除，查询，插入等操作

###功能介绍

![](/media/gxd/list/007.jpg)
* 功能简介：查询列表长度
* 参数说明：列表
* 返回值：列表长度，数据类型：整型（数字）。

![](/media/gxd/list/006.jpg)
* 功能简介：查询列表是否为空
* 参数说明：列表
* 返回值：true/false，数据类型为：常量型。
  
![](/media/gxd/list/005.jpg)
![](/media/gxd/list/045.jpg)
* 功能简介：查询列表第一个/最后一个参数二的索引值。<br>点击积木块可以调整指定位置
* 参数说明：<br>参数一:列表
  <br>参数二:值，数据类型：整型（数字），字符数据类型。
* 返回值：匹配项的索引值，数据类型：整型（数字）。


![](/media/gxd/list/003.jpg)
![](/media/gxd/list/046.jpg)
![](/media/gxd/list/051.jpg)
* 功能简介：返回/返回并移除/移除 列表中指定位置的项。<br>指定位置包括第(参数二)个/倒数第(参数二)个/最后/随机/第一个。
  <br>点击积木块可以调整指定位置
* 参数说明：<br>参数一:列表
  <br>参数二:指定位置数字，数据类型：整型（数字）。
* 返回值：指定位置的项/无，数据类型：整型（数字）,字符数据类型。

![](/media/gxd/list/004.jpg)
![](/media/gxd/list/047.jpg)
![](/media/gxd/list/048.jpg)
* 功能简介：返回指定列表索引值为从（参数二/倒数参数二/从列表头部）到（参数三/倒数参数三/列表最后）的值
* 参数说明：<br>参数一:列表
  <br>参数二:指定位置数字，数据类型：整型（数字）。
  <br>参数二:指定位置数字，数据类型：整型（数字）。
* 返回值：列表中指定范围的项，数据类型：整型（数字）,字符数据类型。

![](/media/gxd/list/009.jpg)
![](/media/gxd/list/049.jpg)
![](/media/gxd/list/050.jpg)
* 功能简介：设置/插入 列表中（参数二/倒数参数二/列表头部/列表尾部/随机）项的值。
* 参数说明：<br>参数一:列表
  <br>参数二:值，数据类型：整型（数字）。
  <br>参数三:设置/插入到列表的内容，据类型：整型（数字），字符数据类型。
* 返回值：无


###积木块应用
* 查询列表test1长度
![](/media/gxd/list/028.jpg)

* 查询列表test1是否为空
![](/media/gxd/list/029.jpg)

* 查询列表test1中第一个值为1的项的索引值
![](/media/gxd/list/030.jpg)

* 获取列表test1倒数第二个项的值
![](/media/gxd/list/031.jpg)

* 获取一个子列表，内容为列表test1索引值从2到4的项
![](/media/gxd/list/032.jpg)

* 设置列表test1索引值为3的项值为3
![](/media/gxd/list/033.jpg)


##2.综合运用案例
无


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/gxd/list/list014.txt" download="" target="_blank">查询列表长度</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list001.txt" download="" target="_blank">查询列表是否为空</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list002.txt" download="" target="_blank">查询列表test1中第一个值为1的项的索引值</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list003.txt" download="" target="_blank">获取列表test1倒数第二个项的值</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list004.txt" download="" target="_blank">获取一个子列表，内容为列表test1索引值从2到4的项</a>
* <a href="../download/积木块说明案例源代码/gxd/list/list005.txt" download="" target="_blank">设置列表test1索引值为3的项值为3</a>

