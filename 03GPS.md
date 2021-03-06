
## 提案名称： 基于HackRF开发GPS信号仿真模拟器

## 提案内容

**提案描述：**
研究并实现基于HackRF的GPS信号仿真模拟器，使得用户在电脑上给定地理坐标之后，通过HackRF发射出各卫星对应GPS模拟信号，并能通过一般的GPS接收机得到物理验证。

GNSS-SDR是德国同学发起的使用软件无线电来对接收到的卫星定位系统信号进行处理的项目，在开发信号生成部分时可以参考。

HackRF是一款历史上首次从软件、固件、电路原理图和PCB板图完全开源而毫无保留的软件无线电平台，可以覆盖10MHz - 6GHz，已经在kickstarter上成功融资。将会使得更多的软件工程师、Linux黑客们获得直
接操作无线电波的可能。同时，对无线信号的安全分析也将会成为人们关注的新领域。

GNURadio开源软件无线电框架提供了全面的对各种通信系统常用的信号处理模块，并提供了完整的信号开发模块，并已经形成完善良好的开源生态环境。但由于长久以来没有价格平易近人的硬件外设方案，使得GNURadio的学习门槛较高。HackRF的出现将使得开源软件无线电被大众普遍认识提供了可能。


具体要求:

1. 分析GPS的信号原理
2. 使用Matlab完成信号的仿真
3. 调试基带信号，使其能够通过HackRF发射出来，并可以在手机上得到验证
4. 不依赖于Matlab完成信号的生成
5. 发布代码及教程

**项目代码地址：**
 - <https://github.com/mossmann/hackrf>
 - <http://gnss-sdr.org>

**计划：**

* 中期检查前完成Matlab生成的IQ信号仿真，通过HackRF发射后可以被一般GPS接收机解析
* 结题之前完成不依赖于Matlab的信号生成及HackRF发射

**联系方式：**

* email: <putaoshu@gmail.com>

## 对学生的要求

* 熟悉信号处理知识
* 了解GPS定位的原理
* 对射频调试有一定的概念

## 完成标准

* Matlab生成的信号可以通过软件解调
* 可以指定输入经度/纬度
* 提供一个简单的命令行参数实用程序，直接对接hackrf_transfer程序
