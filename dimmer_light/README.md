# 调光灯 (Dimmer Light)

>> Apply to ESPhome 1.14.3

## 需求

**设备**
- 三组 MOS 调光灯，分别通过三个按钮单独控制。
- 面板带 2812mini 状态灯。

**功能需求**
1. 当调光灯开启时，面板状态灯从 **off_color** 渐变到 **on_color**。
2. **on_color** 和  **off_color** 支持通过 HA 前端修改或者自动化批量修改颜色与亮度。
3. 状态灯支持通过自动化临时修改颜色。

## Pin 使用表

| Pin       | 功能               |  接入实体  | 
| --------- | -----------------  | --------- |
| GPIO0     | 实体开关2           | 开关2     |
| GPIO2     | 实体开关3           | 开关3     |
| GPIO4     | 实体开关1           | 开关1     |
| GPIO5     | 面板状态灯3         |  2812mini |
| GPIO12    | 虚拟，状态灯 ON 颜色 | 悬空      |
| GPIO13    | 虚拟，状态灯 OFF 颜色| 悬空      |
| GPIO18    | 面板状态灯2         | 2812mini  |
| GPIO19    | 面板状态灯2         | 2812mini  |
| GPIO21    | 调光灯输出3         | MOS_3     |
| GPIO23    | 调光灯输出1         | MOS_1     |
| GPIO25    | 调光灯输出2         | MOS_2     |
