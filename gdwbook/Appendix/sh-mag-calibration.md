# 树莓派指南针校准说明

校准步骤：

1. 安装依赖包
2. 安装校准软件
3. 校准

注：

- ***上述步骤 1 仅需在全新树莓派上操作。古德微定制后的树莓派固件可跳过；***
- 若指南针工作正常，无需校准

## 安装依赖

为了正常工作，Sense HAT需要一个最新的内核，启用I2C，以及一些库来开始。

确保您的APT包裹清单是最新的：

```bash
sudo apt-get update
```

接下来，安装sense-hat软件包，确保内核是最新的，启用I2C，并安装必要的库和程序。
安装完成后重新启动树莓派。

```bash
sudo apt-get install sense-hat
sudo reboot
```

### 安装校准程序

安装校准程序：

```
sudo apt-get update
sudo apt-get install octave -y
cd
cp /usr/share/librtimulib-utils/RTEllipsoidFit ./ -a
```

执行

```
cd RTEllipsoidFit
RTIMULibCal
```

### 执行校准

按如下步骤校准：

- 运行上述程序后，您将看到此菜单：

```
Options are:

  m - calibrate magnetometer with min/max
  e - calibrate magnetometer with ellipsoid (do min/max first)
  a - calibrate accelerometers
  x - exit
Enter option:
```

- 按小写m。然后将显示以下消息; 按任意键开始。

```
    Magnetometer min/max calibration
    --------------------------------
    Waggle the IMU chip around, ensuring that all six axes
    (+x, -x, +y, -y and +z, -z) go through their extrema.
    When all extrema have been achieved, enter 's' to save, 'r' to reset
    or 'x' to abort and discard the data.

Press any key to start...
```

- 启动后，您将看到类似于滚动屏幕的内容：

```
Min x:  51.60  min y:  69.39  min z:  65.91
Max x:  53.15  max y:  70.97  max z:  67.97
```


- 关注屏幕最底部的两个数据，因为这些是最近发布的测量结果。然后必须以你能想到的每种可能的方式移动树莓派。此时可以将所有非必要的电缆拔下以边操作，切记勿将电源线断开。
- 尝试在每个俯仰，滚转和偏航轴上获得一个完整的圆。这样做时，请注意不要意外弹出SD卡。花几分钟移动树莓派，当你发现数据不再变化时停下来（此时才算数据校准结束）。
- 现在按小写s然后小写x退出程序。如果现在运行该ls命令，您将看到RTIMULib.ini已创建新文件。

*除了这些步骤之外，您还可以通过执行上述步骤来执行椭球拟合，但是按下e而不是m*

- 完成后，将结果 `RTIMULib.ini` 复制到 `/etc` /并删除本地副本 `~/.config/sense_hat/`：

```
rm ~/.config/sense_hat/RTIMULib.ini
sudo cp RTIMULib.ini /etc
```

- 然后校准数据库保存成功后，结束。建议重启树莓派。



