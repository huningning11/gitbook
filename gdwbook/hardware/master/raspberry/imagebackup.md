#系统备份与恢复

为了大家更容易上手，古德微为大家准备好了系统镜像。以下介绍系统备份和恢复的方法。

##1. 备份前准备

   * 安装了系统的TF卡
   * 在Windows系统下载安装 Win32DiskImager 软件
   
##2. 使用 Win32DiskImager 备份

先新建一个空白的.img 后缀的文件(注意：路径名和文件名不能含有中文)。比如：我在 E 盘imageBack目录下新建了一个”raspberrypi.img”文件。

备份系统可以分为三步。第一步，选择含系统的TF 卡；第二步，选择下载好的镜像文件；第三步，点击“读取”（Read）。

<div align="center">
    <img src="/media/imageback.png" width="80%">
    <h4>镜像备份</h4>
</div>

注意：
   * 使用 Win32DiskImager 备份属于全盘备份(无压缩)，即 16G TF 卡备份完成后的镜像文件也是 16G 左右；
   * 备份时一定不要点击写入（Write），否则 TF 卡中的系统和文件将不复存在

##3. 使用 win32DiskImager 恢复

恢复系统也可以分为三步。第一步，选择新的TF 卡/已格式化的TF 卡；第二步，选择之前备份的镜像文件；第三步，点击“写入”（Write）。


# 格式化 TF 卡

这里主要说一下格式化 TF 卡的方法。(注意：重新烧录其他系统需要先格式化，只使用 Windows 本身的格式化方法是不能解决问题的，格式化会清空SD卡的所有数据)

##格式化 SD 卡

打开 SDFormatter 工具格式化 TF(MicroSD)卡，如下图所示：   

<div align="center">
    <img src="/media/imageformat.png" width="80%">
    <h4>格式化</h4>
</div>

格式化完成后，等待片刻，重新插上 SD 卡，即可在我的电脑看到 SD 卡原空间大小。

###注意：

   * 建议连续格式化两遍，第二遍格式化时请把 Volume Label里的文字清空，特别有时boot可能会变成乱码。这样可以确保格式化成功