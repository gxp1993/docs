W60X 开发资源
=============

.. toctree::
   :hidden:

   兼容版AT开发 <at/index>
   soc二次开发 <soc/index>
   arduino开发<arduino/index>
   rt-thread/index
   alios-things/index
   vsf/index
   
   
.. image:: index.assets/1549913783533.png
   :width: 500px

**一、AT固件说明和区分方式**

W600 系列wifi 模组拥有两个版本的AT固件；

**兼容版AT固件**\ 和\ **WM_AT固件**\ 是两个不同版本的SDK，兼容版AT固件是兼容ESP系列AT指令的固件，WM_AT固件是由联盛德官方SDK编译而来，用户在不知道手里的AT固件是哪一个版本时，可以通过一条指令做判断。

**兼容版AT固件**\ ，发送指令 AT，返回OK，发送指令 AT+ ,报错；

**WM_AT 固件**\ ，发送指令AT+，返回OK；发送指令AT，无应答；

**1.AT固件的获取方式**

**1.1 兼容版AT固件**

兼容版AT固件兼容乐鑫ESP8266 AT 指令集；

该固件不开源，可通过 `兼容版AT指令开发入门指导 <at/start>`__  获取；


**1.2 WM_AT固件**

**该固件可通过修改联盛德官方SDK的宏定义，编译后获取**\ （宏定义默认打开）；

首先，参考 `SOC开发入门指导 <soc/start>`__ ，搭建联盛德SDK二次开发环境；

其次，找到 /include/wm_config.h 文件，通过修改宏定义 TLS_CONFIG_AT_CMD
来选择是否打开AT功能配置 ；

最后，编译烧录；

**二、联盛德 SDK 开发**

**1.WM_AT固件**

参考 `WM_AT开发入门指导 <wm_at/start>`__ ；


**2.SPI透传固件**

该固件可通过修改联盛德官方SDK的宏定义，编译后获取（宏定义默认打开）。

参考本篇1.2章节，通过修改宏定义 TLS_CONFIG_RI_CMD
来选择是否打开SPI透传固件的配置；

参考 `SPI透传固件开发入门指导 <spi_ri/start> __ ；

**3.SOC二次开发**

参考 `SOC开发入门指导 <soc/start>`__ ；


**三、Arduino 开发**

参考 `W600_Arduino 开发入门指导 <arduino/start>`__；

**四、RT-Thread 开发**

参考 `W600_RT-Thread 开发入门指导 <rt-thread/start>`__；

**五、Alios Things 开发**

参考 `W600_Alios Things 开发入门指导 <alios-things/start>`__；

**六、VSF开发（待更新）**

参考 W600_VSF 开发入门指导；



