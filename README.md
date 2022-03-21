# Py-Apple Controller 开源四足万能控制器

## 1 简介

  **菠萝万能控制器**，是一个由灯哥开源的，基于[GPL-3.0](https://github.com/ToanTech/Inverted_Pendulum_DengFOC/blob/main/LICENSE)开源协议和ESP32主控芯片的低成本四足机器人控制器，控制器集成了全部四足机器人的必须硬件，完美支持 **Py-Apple Dynamics** **系列开源四足控制软件**

  开源的版本主要有两个，一个是全集成主控板，一个是分立式元器件主控板。分别照顾不同的DIY需求，目前优先开源分离式元器件主控板。**喜欢项目的话，请B站一键三连并 Star 项目哦**

#### 具体参数表

| **功能项** | **参数**                                                     |
| ---------- | :----------------------------------------------------------- |
| 处理器     | Xtensa® LX6 32-bit 双核处理器；7 级流水线架构，支持高达 240 MHz 的时钟频率；448 KB 的 ROM,全集成主控板8MB RAM，分立512KB RAM |
| WIFI       | 802.11n MCS0-7 支持 20 MHz 和 40 MHz 带宽;802.11n MCS32 (RX);802.11n 0.4 µs 保护间隔;数据率高达 150 Mbps;接收 STBC 2×1; 发射功率高达 20.5 dBm;可调节的发射功率;天线分集 |
| 蓝牙       | Class-1、Class-2 和 Class-3 发射输出功率，动态控制范围高达 24 dB • π/4 DQPSK 和 8 DPSK 调制 |
| 陀螺仪     | MPU6050六轴陀螺仪，集成加速度和角度输出;角速度全格感测范围为±250、±500、±1000与±2000°/sec (dps);加速器全格感测范围为±2g、±4g±8g与±16g |
| 舵机支持   | 宽电压支持，支持5v-8v模拟/数字 舵机（基于PWM控制）           |



## 2 **菠萝开源四足机器人项目的组成**

  您现在浏览的是[**菠萝开源四足机器人项目**](https://github.com/ToanTech/py-apple-quadruped-robot)的其中一个分项目的 Github **菠萝动力开源四足万能控制器（Py-Apple Controller）**。**菠萝开源四足机器人项目**，是一个大型全套四足机器人开源项目。主要由三个分项目构成：

- [Py-Apple Dynamics 系列 开源四足控制软件](https://github.com/ToanTech/py-apple-dynamics)
- Py-Apple Controller 系列 开源四足万能控制器（即本项目）
- [Py-Apple Structure 系列 开源四足机械结构](https://github.com/ToanTech/py-apple-structure)

## 3 用户支持和讨论论坛

- 用户支持**QQ群**（桌面级四足机器狗交流群 PY PY DOG）：**1071643412**
- 讨论论坛（机器狗工坊）：http://www.leggedrobot.cn/forum.php?mod=forumdisplay&fid=44

## 4 Py-Apple Controller 项目搭建方法

- 第一步：根据用途和需求，下载本 Github 中你需要 Controller 版本
- 第二步：根据PCB文件，前往淘宝或者嘉力创打板
- 第三步：根据开源配件表，配齐所有电控元器件
- 第四步：根据[焊接教程](https://www.bilibili.com/video/BV1nv411B7d5)焊接万能控制器
- 第五步 : 到[Py-Apple Dynamics 系列 开源四足控制软件](https://github.com/ToanTech/py-apple-dynamics)处，根据提示下载最新软件，并且按照[此教程](https://www.bilibili.com/video/BV1mv411B7dR)烧录程序。
- 第六步：用电脑访问[这里](https://space.bilibili.com/493192058/channel/detail?cid=135699)（最好用电脑，否则有可能打不开频道），观看剩下的万能控使用教程以及调参数方法，上手使用万能控制器

## 5 开源开发信息

- Py-Apple Controller Github仓库：https://github.com/ToanTech/py-apple-controller
- 菠萝狗开源四足机器人项目开发者交流QQ群：<u>**960502665**</u>

## 6 Py-Apple Controller  贡献者

- [点击查看贡献者列表](contributors_m.md)

## 7 如何参与到 Py-Apple  Controller  开源项目开发团队中

-  Py-Apple Controller 项目是开源的，我们鼓励参与修改和贡献新的机械结构：[点击查看如何在Py-Apple Controller Github 仓库中贡献的指导](http://www.leggedrobot.cn/forum.php?mod=viewthread&tid=51)
-  需要的功能设想和bug可以发布到 Issue list [点击进入 ISSUE LIST](https://github.com/ToanTech/py-apple-controller/issues)
-  有其他参与问题需要联系项目管理及贡献者 ：[点击查看联系方式](contributors_m.md)

## 8 当前 Py-Apple  Controller  版本特点

  目前的最新的版本是 **Py-Apple Controller  V4.0** 。目前开源的版本是直插元器件的版本。实现的功能如下：

- 稳定的WIFI支持
- 稳定的蓝牙支持
- 稳定的陀螺仪MPU6050支持
- 稳定的舵机支持，支持无极舵机电压调节（5V-8V）和最多十六路PWM舵机
- 扩展I/O、CAN口、串口支持