# 前言

```
所有的PCB设计都源于芯片选型与原理图设计。
项目中所用的芯片是设计的蓝图，是为了完成一定的功能，所需要采用的器件。
所以设计流程应该是：
1、功能设计，模块划分；
2、芯片选型，阅读器件手册；
3、选择参考设计，制作原理图；
4、原理图仿真与验证；
5、PCB布板，需要参照器件参考手册中的布局布线要求，制板。
```

划分步骤来看，一个典型的PCB设计流程包括以下几个关键的步骤

 - 制作元器件
 - 设计原理图
 - 进行仿真验证（可选）
 - 制作元器件的封装
 - 设计PCB
 - 输出制板

这个笔记的顺序按照这个方向展开。我们预计在**仿真验证**部分，利用`ngspice`或其Python版本`ngspuce`（中间只差了一个**y**）对原理图进行仿真验证（待定）。这个项目的主要初衷是设计评估AC恒流源，主要包括howland电路、改进型howland电路以及电流镜。

 - 目的：设计评估howland电流源
 - 设计原理图，利用spice进行仿真评估
 - 制作PCB，测试对比性能

最终的设计目的，是1、设计`microzed`的载板，用于实现阻抗测量的功能；2、利用最新的`esp32`模块和`ad5933`模块，设计便携、无线式、微型宽频阻抗测量设备。

