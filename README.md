# HomeKitSwitch

在B站大佬创客尹白猿[视频地址](https://www.bilibili.com/video/BV1V3411376C/?spm_id_from=333.1007.top_right_bar_window_history.content.click&vd_source=80076cf940dd05a06499f77a50708aba)基础上修改;

up主源码[开源地址github](https://github.com/yinbaiyuan/HomeKitSwitch).  

## 问题

当我使用大佬源码编译发现报错error: 'base64' has not been declared

经查阅发现根本原因是 base64.h 和 base64.c 与核心库冲突。----2024/1/31

## 解决

将源文件中base64.h 和 base64.c重命名就好了 

# 参考文献

- [如果与 WifiManager 一起使用，则会出现有关 base64 的错误](https://github.com/Mixiaoxiao/Arduino-HomeKit-ESP8266/pull/183); 

- homkit大佬[Mixiaoxiao](https://github.com/Mixiaoxiao?tab=repositories)的源码贡献；本项目参考[[Arduino-HomeKit-ESP8266](https://github.com/Mixiaoxiao/Arduino-HomeKit-ESP8266)]；
  
  

# 更多homkit优秀项目

* RavenSystem[esp-homekit-devices](https://github.com/RavenSystem/esp-homekit-devices)
  
  高级固件可添加原生 Apple HomeKit 支持和通过 WiFi 的自定义配置，兼容任何基于 ESP32、ESP32-S、ESP32-C 和 ESP8266 系列的 SoC。
* 一位的大佬[教程](https://imwtx.com/archives/143/)


