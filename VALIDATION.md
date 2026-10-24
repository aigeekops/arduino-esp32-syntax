# 验证记录

更新日期：2026-10-24。

## 编译验证

使用 Arduino-ESP32 3.3.12、FQBN `esp32:esp32:esp32` 编译，退出码 0：

| 程序 | 结果 | 日志 |
|---|---|---|
| `examples/syntax_lab` | 编译通过 | [日志](validation/syntax-lab-compile.txt) |
| `examples/cooperative_timing` | 编译通过 | [日志](validation/cooperative-timing-compile.txt) |
| `examples/serial_control` | 编译通过 | [日志](validation/serial-control-compile.txt) |
| `sketches/project`（第 16 课综合项目） | 编译通过 | [日志](validation/project-compile.txt) |

正文中的浏览器脚本片段另用 Node.js `--check` 做过语法检查，通过。

## 这份记录没有覆盖什么

- **没有烧录到实体开发板，没有接线，也没有测量。** 编译通过与实际硬件行为是两件不同的事。
- 文中的输入输出表、计时推演表是按给定代码推导的预期值，不是从板子回读的记录。
- 16 份课程示例是与制作教程时的本地模板逐个比对一致的快照；网站课程仍在更新，同名源文件可能已有差异，差异记录在 `VERSION.json` 中，不能据此声称示例与网站最新代码逐行一致。
- 正文里的局部片段只说明某种写法，不一定具备独立 sketch 的完整结构；只有标注「完整程序」的文件才可单独使用。

## 版本与快照

示例基线：ESP32-WROOM-32E、Arduino-ESP32 3.3.12、串口 115200。屏幕课程使用 Adafruit SSD1306 2.5.17、Adafruit GFX Library 1.13.0、Adafruit BusIO 1.17.4。源码快照的哈希与来源见 [VERSION.json](VERSION.json)。
