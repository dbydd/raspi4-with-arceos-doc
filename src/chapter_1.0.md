# 第一阶段：认识树莓派及ArceOS编译

***本阶段主要以认识树莓派为主，学会如何编译支持树莓派4b的 Qemu 模拟器、如何在树莓派4b上运行 ArceOS。***

## ArceOS：

[ArceOS实验环境配置](https://rcore-os.cn/arceos-tutorial-book/ch01-00.html)

克隆这个仓库：

```shell
https://github.com/chenlongos/arceos
```

生成ArceOS代码仓库。



## 前置了解：树莓派相关知识

[树莓派新手入门手册](https://github.com/chenlongos/raspi4-with-arceos-doc/blob/master/src/assert/%E6%A0%91%E8%8E%93%E6%B4%BE4B%E6%96%B0%E6%89%8B%E5%85%A5%E9%97%A8%E6%89%8B%E5%86%8C.pdf)

  树莓派4B（Raspberry Pi 4 Model B）是一款功能强大的单板计算机，由Raspberry Pi基金会推出。它提供了丰富的特性和扩展性，适用于各种项目和应用。以下是与树莓派4B相关的一些知识：
1.	规格和硬件：树莓派4B采用了Broadcom BCM2711 SoC处理器，具有四个ARM Cortex-A72 CPU核心、VideoCore VI GPU和1GB、2GB或4GB LPDDR4内存选项。它还配备了多个USB 3.0和USB 2.0接口、Gigabit以太网端口、HDMI输出、MicroSD卡槽等。
2.	操作系统支持：树莓派4B可以运行各种操作系统，包括Raspberry Pi官方的Raspberry Pi OS（以前称为Raspbian），以及其他基于Linux的发行版如Ubuntu、Fedora等。还可以安装其它的操作系统。
3.	GPIO引脚：树莓派4B具有40个GPIO（通用输入/输出）引脚，可以用于连接和控制各种外部设备，如传感器、LED、电机等。这些引脚还可以通过编程语言进行访问和控制。
4.	外设接口：除了GPIO引脚，树莓派4B还提供了丰富的外设接口。它具有多个USB端口（包括USB 3.0和USB 2.0）、以太网端口、HDMI接口（支持4K分辨率输出）、音频/视频接口、摄像头接口、显示器接口等。
5.	储存和扩展：树莓派4B使用MicroSD卡作为主要的存储介质，可以通过插入不同容量的MicroSD卡来扩展存储空间。此外，它还具有两个Micro HDMI端口和一个CSI摄像头接口，可用于连接外部显示器和摄像头模块。

   
树莓派主板如下图所示：

![](assert/主板.png)

小车如下图所示（最上方是一块树莓派主板）：

![](assert/小车.jpg)

树莓派跑ArceOS通过串口控制小车运动：

![](assert/yuan.gif)
