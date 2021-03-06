[![返回目录](https://parg.co/UCb)](https://github.com/wx-chevalier/Awesome-CheatSheets)

# ESP CheatSheet

ESP8266,及其升级版 ESP32 系列,其本质是一个带有 Wlan 收发器的单片机,由于其内核较为冷门(Tensilica 架构 ),所以主流的开发工具几乎都不支持,目前可用的开发手段有:

1.Arduino IDE,使用一种类似 C++的语言编程,多数功能已经封装好;

2.刷 Node MCU 固件,使用 Lua 脚本编程,有第三方的类 IDE 工具,多数功能已经封装好;

3.刷 AT 固件,将其作为从属芯片,使用额外的控制器通过串口 AT 指令来控制;

4.使用官方 SDK 从底层进行开发;

ESP8266 是单核 Tensilica L106 （32 位 MCU）的 Wi-Fi 芯片，主频最高可达 160MHz。

ESP32 是双核 Tensilica L108 (32 位 MCU）的 Wi-Fi 芯片，主频更高可达 250MHz，性能更强，内存更大有 400KB SRAM。另外还集成了蓝牙 BLE。

由于 ESP32 的 MCU 性能更强，内存更大，可以处理包括音频、视频在内的更复杂 Wi-Fi 应用。还可以应用在需要蓝牙和 Wi-Fi 共存的 IOT 场景中。
