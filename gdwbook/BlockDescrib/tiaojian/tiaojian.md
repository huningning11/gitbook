#条件语句积木块区
![](/media/gxd/tiaojian/0010.jpg)
![](/media/gxd/tiaojian/004.jpg)
![](/media/gxd/tiaojian/005.jpg)
![](/media/gxd/tiaojian/006.jpg)
![](/media/gxd/tiaojian/007.jpg)
![](/media/gxd/tiaojian/008.jpg)
![](/media/gxd/tiaojian/009.jpg)
###使用场景
* 条件语句是通过一条或多条语句的执行结果（True或者False）来决定执行的代码块，条件语句中任何非0和非空（null）值为true，0 或者 null为false。
条件语句用于控制程序的执行，基本形式为："判断条件"成立时（非零），则执行后面的语句。


##1.功能描述

![](/media/gxd/tiaojian/0010.jpg)
![](/media/gxd/tiaojian/011.jpg)
* 功能简介：通过一条或多条语句的执行结果（True或者False）来决定执行的代码块，判断条件成立时（非零），则执行。
  <br>点击齿轮，可以增加”否则如果“，”否则“语句。
* 参数说明：整型（数字）
* 返回值：true/false，数据类型为：常量型。

![](/media/gxd/tiaojian/004.jpg)
![](/media/gxd/tiaojian/012.jpg)
* 功能简介：根据积木块参数（<;>;=;≠;≥;≤）对参数一，二进行判断，如果参数一，二符合积木块参数（<;>;=;≠;≥;≤）判断，返回真，否则返回假。
  <br>点击积木块参数即可更改积木块参数。
* 参数说明：参数一：整型（数字）。
  <br>参数二：积木块参数（<;>;=;≠;≥;≤）
  <br>参数三：整型（数字）。
* 返回值：true/false，数据类型为：常量型。

![](/media/gxd/tiaojian/005.jpg)
![](/media/gxd/tiaojian/013.jpg)
* 功能简介：根据积木块参数（和;或）对参数一，二进行判断，如果参数一，二符合积木块参数（和;或）判断，返回真，否则返回假。
  <br>点击积木块参数即可更改积木块参数。
* 参数说明：参数一：参数一：整型（数字）。
  <br>参数二：积木块参数（和;或）
  <br>参数三：整型（数字）。
* 返回值：true/false，数据类型为：常量型。
  
![](/media/gxd/tiaojian/006.jpg)
* 功能简介：积木块参数（非）会调转参数一的类型，如果参数一为真，输出假；如果参数一为假，输出真。
* 参数说明：参数一：整型（数字）。
  <br>参数二：积木块参数（非）
* 返回值：true/false，数据类型为：常量型。

![](/media/gxd/tiaojian/007.jpg)
![](/media/gxd/tiaojian/014.jpg)
* 功能简介：根据积木块参数（真;假）返回真和假，当积木块参数为真，返回真;积木块参数为假，返回假。
  <br>点击积木块参数即可更改积木块参数。
* 参数说明：积木块参数（真;假）
* 返回值：true/false，数据类型为：常量型。

  
![](/media/gxd/tiaojian/008.jpg)
* 功能简介：返回一个空值。
* 参数说明：无
* 返回值：none，数据类型为：常量型。
  
![](/media/gxd/tiaojian/009.jpg)
* 功能简介： 首先判断“测试”对应的参数一，如果为真，输出“如果为真“对应的参数二；
  如果为假，输出“如果为假“对应的参数三。
* 参数说明:参数一：true/false，数据类型为：常量型。
  <br>参数二：整型（数字），字符数据类型。
  <br>参数三：整型（数字），字符数据类型。
* 返回值：true/false，，数据类型为：常量型。

###积木块应用

![](/media/gxd/tiaojian/0003.jpg)
* 条件语句多次判断，决定执行语句

![](/media/gxd/tiaojian/0004.jpg)
* 条件语句（<;>;=;≠;≥;≤）判断

![](/media/gxd/tiaojian/0005.jpg)
* 条件语句（和;否）判断

![](/media/gxd/tiaojian/0006.jpg)
* 条件语句参数（非）调转输入参数类型。

![](/media/gxd/tiaojian/0007.jpg)
* 条件语句参数（空），输出为空。

![](/media/gxd/tiaojian/0008.jpg)
* 条件语句首先判断积木块语句输入，并决定输出结果。

##2.综合运用案例
无


##3.案例代码下载
* <a href="../download/积木块说明案例源代码/gxd/条件语句综合实验案例.txt" download="" target="_blank">条件语句综合实验案例</a>
