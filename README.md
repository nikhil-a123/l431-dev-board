# STM32L431RCT6 Development Board

This project is a template for the VCC-GND STM32L431RCT6 development board, which was purchased from [Aliexpress](https://www.aliexpress.com/item/1005006974372877.html). There seems to be little to no English documentation for this development board, so this document will try to collate all the information that I have been able to find.

## Overview

The board is designed by VCC-GND Studio, and features:

* STM32L431RCT6 Microcontroller
  * 256KB FLASH
  * 64KB RAM
  * QuadSPI peripheral
  * SDMMC peripheral
* 2 headers to break out connections to the MCU
* RTC battery connection routed to the header
* 8MHz and 32.768KHz external oscillators for HSE and LSE clock sources
* USB-C socket for power supply only (L431 doesn't support USB)
* Unpopulated header for USART ()
* Header for external battery
* Switch to select the power source (USB, external battery, external 3V3 source)
* MicroSD Card slot connected to MCU SDMMC interface
* Pad for Winbond W25QXX QuadSPI Flash, connected to QuadSPI peripheral (Don't think it is fitted by default)
* BOOT0 and RESET switches
* User switch connected to PB3 GPIO
* Power LED and User LED
* SWD header for debugging

## Notes

* SD Card slot has "SDIO_SW" connected to PA8, possibly some kind of SD card detection signal?
