# Pulse

一个检测心率的 IoT 应用，2016 年暑期实训课程设计。

[For English](README.md)

## Requirements

* STM32f10x 开发板
* J-Link 套件
* UART 至 USB 外设模块
* [Pulse Sensor](http://pulsesensor.com) 传感器外设

## Implementation

利用心率传感器采集心率模拟量数据，对应的 STM32 的 GPIO 管脚设为模拟量输入 AIN，利用 ADC 转换为数字量，再利用 DMA 直接从 ADC 寄存器读取数据到内存，经过 CPU 相关运算之后，再把心率相关数据利用 USART1 发送到 PC 进行心率波形的展示。

## Acknowledgement

感谢[**邴哲松**](http://www.cyembedded.com/se.asp?nowmenuid=500066)老师的指导。

## Copyright

[LICENSE](LICENSE)