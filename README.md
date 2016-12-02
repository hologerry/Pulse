# Pulse
An IoT system, sensing the heart pulse. It's the final project of the Summer Internship 2016.

[中文介绍](README_CN.md)

## Requirements

* STM32f10x board
* J-Link suite
* UART to USB Peripheral
* [Pulse Sensor](http://pulsesensor.com) Peripheral

## Implementation

Get the heart pulse analog data by using pulse sensor, set the STM32 corresponding GPIO pin as AIN mode, convert the analog to digital data by using ADC, then read the data from ADC's register to memory by using DMA, analysis the data to get heart pulse info, finally send the heart pulse info to PC through USART1 and PC application shows the heart pulse.

## Acknowledgement

Thanks to [邴哲松](http://www.cyembedded.com/se.asp?nowmenuid=500066)'s instructions.

## Copyright

[LICENSE](LICENSE)