#树莓派百科
树莓派(Raspberry Pi，简写为 RPi 或 RasPi )是一款基于 ARM 的微型电脑主板，旨为学生计算机编程教育而设计，其系统基于 Linux，由注册于英国的慈善组织“Raspberry Pi 基金会”开发，Eben•Upton 为项目带头人。别看其外表“娇小”，内“心” 却很强大，上网、看视频、听音乐等功能都有，可谓是“麻雀虽小，五脏俱全”。自问世以来，受众多计算机发烧友和创客的追捧，在小学、中学和大学的编程教育中得到广泛的应用。

#树莓派的家族

<table style="width:100%;table-layout:fixed;">
    <tr>
        <td><b>特征</b></td>
        <td><b>Zero</b></td>
        <td><b>3代A+型</b></td>        
        <td><b>3代B型</b></td>
        <td><b>3代B+型</b></td>
        <td><b>4代B型</b></td>
    </tr>
    <tr>
        <td rowspan="2"><b>SOC</b></td>
        <td>BCM2835</td>
        <td>BCM2837B0</td>
        <td>BCM2837</td>
        <td>BCM2837B0</td>
        <td>BCM2711</td>       
    </tr>
      <tr>
          <td colspan="5" ><center>(CPU、GPU DSP 和 SDRAM)</center></td>
      </tr>  
    <tr>
        <td ><b>CPU</b></td>
        <td>ARM1176JZF-S </td>
        <td>ARM Cortex-A53 </td>
        <td>ARM Cortex-A53 </td>
        <td>ARM Cortex-A53 </td>
        <td>ARM Cortex-A72 </td> 
    </tr>      
    <tr>
        <td ><b>速率&核心</b></td>
        <td>1GHz 单核</td>
        <td>1.4GHz 四核</td>
        <td>1.2GHz 四核</td>
        <td>1.4GHz 四核</td>
        <td>1.5GHz 四核</td> 
    </tr>            
    <tr>
        <td ><b>GPU</b></td>   
        <td colspan="4" ><center>400 MHz Broadcom videoCore IV</center></td>
        <td ><center> 500 MHz Broadcom VI</center></td>
    </tr>
    <tr>
        <td ><b>RAM</b></td>
        <td>512MB</td>
        <td>512MB</td>
        <td>1GB</td>
        <td>1GB</td>
        <td>2GB、4GB、8GB</td> 
    </tr>           
    <tr>
        <td rowspan="2"><b>USB</b></td>
        <td>MicroUSB 1个</td>
        <td>USB2 1个</td>
        <td>USB2 4个</td>
        <td>USB2 4个</td>
        <td>USB2 2个，USB3 2个</td>       
    </tr>
    <tr>
          <td colspan="5" ><center>支持 USB Hub 扩展</center></td>
    </tr>      
    <tr>
        <td ><b>视频输出</b></td>    
        <td colspan="4" >支持HDMI(1.3 和1.4)， 分辨率为 640*350 至 1920*1200</td>
        <td colspan="1" >支持两个Micro HDMI， 分辨率为 4K 60Hz + 1080p</td>
    </tr>       
    <tr>
        <td ><b>音频输出</b></td>    
        <td colspan="5" >3.5mm 插孔(Zero 无此项)，HDMI(高清晰度多音频/视频接口)，usb声卡</td>
    </tr>           
    <tr>
        <td ><b>音频输入</b></td>    
        <td colspan="5" ><center>USB全向麦，USB声卡</center></td>
    </tr>           
    <tr>
        <td ><b>数字接口</b></td>    
        <td colspan="5" ><center>CSI(摄像头)和 DSI(显示屏)排线接口</center></td>
    </tr> 
     <tr>
         <td ><b>SD卡接口</b></td>    
         <td colspan="5" ><center>Micro SD 接口</center></td>
     </tr>        
     <tr>
         <td ><b>网络</b></td>   
         <td>板载蓝牙和wifi</td>
         <td>板载蓝牙和wifi（2.4GHz and 5GHz）</td>         
         <td ><center>10/100 以太网 (RJ45)接口，载蓝牙和wifi</center></td>
         <td colspan="1" ><center>10/300 以太网 (RJ45)接口，载蓝牙和wifi（2.4GHz and 5GHz）</center></td>
         <td ><center>10/1000 以太网 (RJ45)接口，载蓝牙5.0和wifi（2.4GHz and 5GHz）</center></td>
     </tr>    
      <tr>
          <td ><b>引脚插槽</b></td>    
          <td colspan="5" ><center>40 针</center></td>
      </tr>                
      <tr>
          <td ><b>电源输入</b></td>    
          <td colspan="4" ><center>5V，通过 MicroUSB 或 GPIO 引脚</center></td>
          <td><center>5V，通过 Type C 或 GPIO 引脚</center></td>         
      </tr>             
      <tr>
          <td ><b>电流</b></td>   
          <td>约 1A</td>
          <td colspan="3" ><center>约 2—3A</center></td>
           <td colspan="1" ><center>3A</center></td>         
      </tr>         
      <tr>
          <td ><b>尺寸(mm)</b></td>   
          <td>65*30</td>
          <td>65*56</td>          
          <td colspan="3" ><center>85*56*17</center></td>
      </tr>       
</table>

由于篇幅有限，早期的一代、二代和一些细微的差别未作说明，敬请谅解！

树莓派就相当于(不是等同于)集成了 CPU、显卡、内存的微型 PC 主板，只不过这块主板是 Arm 架构的。树莓派自 2012 发售以来，现在已经是第四代了。上表中可以看出，升级后的树莓派性能增强了很多。按照这样的增长速度，有理由相信在不久的将来，树莓派性能能够追平一般家用 PC。


