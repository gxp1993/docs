W600 Arduino 入门教程
=====================

1.简介
------

`Arduino <https://baike.baidu.com/item/Arduino>`__\ 是一款便捷灵活、方便上手的开源电子原型平台。

W600 与 Arduino
的结合，使得W600继承了Arduino的开放性、易用性、交流性、丰富的第三方资源，更便捷的支持开发者进行自己的产品设计。

2.准备工作
----------

-  arduino开发包: :download:`RT-Thread_W60X_SDK_0.1.0 <soc/RT-Thread_W60X_SDK_0.1.0.zip>` 
-  硬件准备：TB-01开发板（\ `购买链接 <http://shop.thingsturn.com/>`__\ ）
-  串口下载工具：`串口调试助手 </download/tools>`__ 

3. 环境搭建
-----------

3.1 下载arduino ide
~~~~~~~~~~~~~~~~~~~

开发者可以通过 https://www.arduino.cc/官网下载最新版本 Windows 系统的
Arduino IDE 开发环境， 建 议 Arduino IDE 版 本 不 低 于 1.8.7 的 免 安
装 版 （ 一 个 下 载 链 接 为 ：
https://downloads.arduino.cc/arduino-nightly-windows.zip），解压路径中不要出现空格。

3.2 后续步骤
~~~~~~~~~~~~

参考Arduino开发包w600-arduino-InnerIDE-0.2.1:raw-latex:`\w`600-arduino-InnerIDE-0.2.1目录下的《WM_w600-arduino-InnerIDE-instruction_v1.1_190218.pdf》

另附上一份调试文档，该文档包含了当前版本提供的Demo的详细使用说明，文档路径为Arduino开发包的sdk:raw-latex:`\w`600-arduino-InnerIDE-0.2.1:raw-latex:`\w`600-arduino-InnerIDE-0.2.1:raw-latex:`\hardware`:raw-latex:`\hardware`:raw-latex:`\w`600:raw-latex:`\w`600-arduino-0.2.1:raw-latex:`\doc  `《WM_Arduino-Examples-instruction_v1.2_190125.pdf》

4.注意事项
~~~~~~~~~~

4.1 首次使用
^^^^^^^^^^^^

首次使用当前版本Arduino SDK的用户无法使用Arduino
IDE进行下载，请先使用星通智联串口调试助手下载开发包根目录下的测试文件
test.fls。

.. image:: start.assets/1551061923474.png


4.2 下载速率
^^^^^^^^^^^^

Arduino
IDE默认的下载速率为2Mbps，该速率当前版本无法修改，用户的串口工具的串口芯片如果不支持2Mbps的话，无法直接使用Arduino下载，参考4.1进行下载.

| Arduino IDE编译默认生成的固件路径为
  C:\Users\17118\AppData\Local\Temp\arduino_build_xxxxx

.. image:: start.assets/1551062211023.png


4.3 其他
~~~~~~~~

有问题和提供建议的用户，请加QQ群860320067 联系群管理在线解决问题。
