# WiFi 状态 LED 指示灯

## 测试开发板


| **Microcontroller** | ESP8266EX |
| -- | -- |
| **Frequency** | 80MHz |
| **Flash** | 2MB |
| **RAM** | 36KB（不确定） |
| **Vendor** | [Espressif](http://www.esp8266.com/wiki/doku.php?id=esp8266-module-family&utm_source=platformio&utm_medium=docs) |

## 需求

通过指示灯显示当前 WiFi 状态.

- 当 WiFi 断开时，红灯闪烁（闪烁间隔1秒）。
- 当 WiFi 连时，蓝灯常亮。
- 当 WiFi 再次断开时候，蓝灯灭，红灯闪烁。

## Pin 使用表

| Pin       | 功能               |  接入实体  | 
| --------- | ----------------  | --------- |
| GPIO12    | 板载红灯           | 板载红灯  |
| GPIO13    | 板载绿灯           | 板载红灯  |
| GPIO14    | 板载蓝灯           | 板载红灯  |

