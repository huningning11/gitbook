#文本寻找积木区

![](/media/wenbenzhuanhua1.png)

##1.功能描述


![](/media/wenbenzhuanhua2.png)

* 功能介绍：将字符串按UTF-8格式进行解码；
* 参数说明：输入UTF-8格式需要解码的字符文本；
* 返回值：返回解码后的字符文本。

![](/media/wenbenzhuanhua3.png)

* 功能介绍：对字符串进行MD5加密；
* 参数说明：输入需要加密的字符文本；
* 返回值：返回加密后的字符文本。

![](/media/wenbenzhuanhua4.png)

* 功能介绍：将字符串按UTF-8格式进行编码；
* 参数说明：输入需要编码为UTF-8格式的字符文本；
* 返回值：返回编码后的字符文本。

![](/media/wenbenzhuanhua5.png)

* 功能介绍：将字符串中的所有指定字符转化为另一字符；
* 参数说明：
  * 参数一：输入需要转化的文本；
  * 参数二：输入需要转化的字符；
  * 参数三：输入转化后的字符；
* 返回值：返回指定字符转化为目标字符后的整段文本。



###积木块应用

<div align="center">
    <img src="/media/wenbenzhuanhua6.png" alt="图1" width="1108">
    <h4>（图1）文本转化案例1</h4>
</div>  

* 当输入的字符串中有中文时，文本字节的长度会与字数不符，一般一个中文字符有三个字节长度。由案例可知这时我们无法直接从文本中提取出中文字符，这时我们需要先通过UTF-8解码方法将目标文本转化为unicode格式，这时每个字符都表示为一个unicode码，我们再选取相应位置的文本字符，再将格式通过UTF-8编码方法转回str字符格式，即可提取出字符串中相应的中文字符。

<div align="center">
    <img src="/media/wenbenzhuanhua7.png" alt="图2" width="952">
    <h4>（图2）文本转化案例2</h4>
</div>  

* 将文本中的目标字符全部替换为另一种字符。

##3.案例代码下载
* <a href="../download/积木块说明案例源代码/wenbenzhuanhuaanli1.txt" download="" target="_blank">文本转化案例1</a>
* <a href="../download/积木块说明案例源代码/wenbenzhuanhuaanli2.txt" download="" target="_blank">文本转化案例2</a>