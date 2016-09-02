# Pulse
心率检测IoT

2016暑期实训

## Requirements

* STM32f10x开发板
* J-Link
* 串口转USB模块
* 心率传感器模块

## Basic Principle

利用心率传感器采集心率模拟量数据，对应的 STM32 的 GPIO 管脚设为模拟量输入 AIN，利用 ADC 转换为数字量，再利用 DMA 直接从 ADC 寄存器读取数据到内存，经过 CPU 相关运算之后，再把心率相关数据利用 USART1 发送到 PC 进行心率波形的展示。

## Acknowledgement

感谢**邴哲松**老师的指导。

## Copyright

Copyright © 2016 [gaoyve](https://github.com/gaoyve). All rights reversed.