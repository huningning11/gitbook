#异常积木块区

![](/media/gxd/exception/exception001.jpg)
![](/media/gxd/exception/exception002.jpg)
![](/media/gxd/exception/exception003.jpg)
![](/media/gxd/exception/exception004.jpg)

##1.功能描述

###使用场景
异常即是一个事件，该事件会在程序执行过程中发生，影响了程序的正常执行。
<br>一般情况下，在无法正常处理程序时就会发生一个异常。
<br>异常表示一个错误。
<br>当程序发生异常时我们需要捕获处理它，否则程序会终止执行。

###功能介绍
![](/media/gxd/exception/exception005.jpg)
* 功能简介：首先运行”try“对应的积木块，如果程序运行出错，运行”exception“对应的积木块
* 参数说明：无
* 返回值：无

![](/media/gxd/exception/exception006.jpg)
* 功能简介：首先运行”try“对应的积木块，如果程序运行出错，运行”exception“对应的积木块，无论程序是否出现异常最终运行”finally“对应的积木块
* 参数说明：无
* 返回值：无

![](/media/gxd/exception/exception007.jpg)
* 功能简介：返回程序异常的错误信息
* 参数说明：无
* 返回值：程序异常的错误信息，数据类型：字符数据类型。

![](/media/gxd/exception/exception008.jpg)
* 功能简介：返回发生程序异常的程序行数
* 参数说明：无
* 返回值：发生程序异常的程序行数，数据类型：整形（数字）。



###积木块应用
* 首先运行”try“对应的积木块，如果程序运行出错，运行”exception“对应的积木块，输出”FALSE“
![](/media/gxd/exception/exception001.jpg)

* 功能简介：首先运行”try“对应的积木块，如果程序运行出错，运行”exception“对应的积木块，输出”FALSE“，无论程序是否出现异常最终运行”finally“对应的积木块，输出”程序正常运行“
![](/media/gxd/exception/exception002.jpg)

* 首先运行”try“对应的积木块，如果程序运行出错，运行”exception“对应的积木块，输出”程序异常的错误信息“
![](/media/gxd/exception/exception003.jpg)

* 首先运行”try“对应的积木块，如果程序运行出错，运行”exception“对应的积木块，输出”发生程序异常的程序行数“
![](/media/gxd/exception/exception004.jpg)
##2.综合运用案例
无

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/gxd/exception/exception001.txt" download="" target="_blank">异常处理1</a>
* <a href="../download/积木块说明案例源代码/gxd/exception/exception002.txt" download="" target="_blank">异常处理2</a>
* <a href="../download/积木块说明案例源代码/gxd/exception/exception003.txt" download="" target="_blank">输出”程序异常的错误信息“</a>
* <a href="../download/积木块说明案例源代码/gxd/exception/exception004.txt" download="" target="_blank">输出”发生程序异常的程序行数“</a>