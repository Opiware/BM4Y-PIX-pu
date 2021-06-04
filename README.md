
# BM4Y-PIX OpiBerry Embedded ARM

### BM4Y-PIX
* OpiBerry Embedded ARM Cortex-A72
* Hardware Guide

[image1]


#### BM4Y-PIX OpiBerry Embedded ARM
* Compact. Low Power. Affordable
* High-performance expandable
* Embedded Linux, FreeRTOS.

*Copyright © Opiware Solutions. All Rights Reserved. | Version: 0.1  2020 Nov.*

-------------------------------------------------------------------------------

#### Trademarks
The Opiware logo is a registered trademark of Opiware Solutions. All other trademarks or registered marks in this manual belong to their respective manufacturers.

#### Disclaimer
Information in this document is subject to change without notice and does not represent a commitment on the part of Opiware.

Opiware provides this document as is, without warranty of any kind, either expressed or implied, including, but not limited to, its particular purpose. Opiware reserves the right to make improvements and/or changes to this manual, or to the products and/or the programs described in this manual, at any time.

Information provided in this manual is intended to be accurate and reliable. However, Opiware assumes no responsibility for its use, or for any infringements on the rights of third parties that may result from its use.

This product might include unintentional technical or typographical errors. Changes are periodically made to the information herein to correct such errors, and these changes are incorporated into new editions of the publication

Operation is subject to the following two conditions:
1. This device may not cause interference and
2. This device must accept any interference. Including interference that may cause undesired operation of the device.

#### Safety information

ATTENTION: Before Connecting the device to DC power input, make sure the DC power source voltage is stable.

ATTENTION: This product is intended to be mounted to a well-grounded mounting surface, such as a metal panel.

This Metal surface can be very hot when operating in high temperature. To avoid  injure, please do not touch the metal surface.

-------------------------------------------------------------------------------

## 1. Introduction
  BM4Y-PIX based on ARM Cortex-A72, is a computer board with highly integrated and low power consumption. BM4Y-PIX provides an ideal building block that easily integrates with a wide range of target markets, such as industrial control, automation, IoT mobile gateway, kiosk, digital signage and many other dedicated applications.

#### 1.1 Features
* Broadcom BCM2711, Quad core Cortex-A72 (ARM v8) 64-bit SoC @ 1.5GHz
* 2GB, 4GB or 8GB LPDDR4-3200 SDRAM (depending on model)
* 2.4 GHz and 5.0 GHz IEEE 802.11ac wireless, Bluetooth 5.0, BLE
* 1x Gigabit Ethernet
* 2x USB 3.0 ports; 2x USB 2.0 ports.
* Raspberry Pi standard 40 pin GPIO header (fully backwards compatible with previous boards)
* 2× Micro-HDMI ports (up to 4kp60 supported)
* 2-lane MIPI DSI display port
* 2-lane MIPI CSI camera port
* 4-pole stereo audio and composite video port
* H.265 (4kp60 decode), H264 (1080p60 decode, 1080p30 encode)
* OpenGL ES 3.0 graphics
* Micro-SD card slot for loading operating system and data storage
* 5V DC via USB-C connector (minimum 3A*)
* 5V DC via GPIO header (minimum 3A*)
* Power over Ethernet (PoE) enabled (requires separate PoE HAT)
* Operating temperature: 0 – 50 degrees C ambient
* OS Supported: Windows IoT / Linux / OpenWRT / FreeRTOS / RT-Thread

#### 1.2 Specifications (Hardware)

***CPU / Memory***
* CPU: Broadcom BCM2711 ARM SoC @ 1.5GHz
* SDRAM: 2GB, 4GB or 8GB LPDDR4-3200
* Flash: 32GB / 16GB SSD
* DataFlash: Micro-SD for data storage & backup

***Network Interface***
* Type: 1x Gigabit Ethernet
* Connector Type: RJ45
* Wireless, Bluetooth BLE

***USB 3.0 / USB 2.0 Host Interface***
* 2× USB 2.0 supports 480Mb/s max
* 2× USB 3.0 supports 5 Gbit/s max;
* 1 port being used

***SD Slot***
* 1x Micro-SD socket, support up 128G
* SD 2.0 compliant, supports SDHC

***Optional TTY Serial Ports***
* RS-232 or RS-485, software select
* RS-232 Signals: TX, RX, RTC, CTS
* RS-485 Signals: Data+, Data-
* RS-485 Automatic Flow Control: Yes
                                        
***Optional TTY Serial Port Parameters***
* Baud Rate: up to 921.6Kbps
* Parity: None, Even, Odd, Mark, Space
* Data Bits: 5, 6, 7, 8
* Stop Bits: 1, 1.5, 2
* Flow Control: RTS/CTS, XON/XOFF, None

***Optional Console / Debug Ports***
* Support USB console port
* Serial console port

***Power Requirement***
* Input Voltage: 110~240VAC to 5VDC adapter
* Typical Consumption: 2.5 Amp @ 5VDC

***General***
* Real-time clock(RTC): Yes
* Buzzer: Yes
* Watchdog: Yes
* Dimensions (W x H x D): 78 x 108 x 24mm (3.0x4.25x0.94in)
* Weight: 324g (0.71lb)
* Operating Temperature: 0~70°C (32~158°F)
* Regulation: CE Class A, FCC Class A
* Installation: Optional Wall mounting, DIN-rail mounting

#### 1.3 Specifications (Linux Software)

***Operation Systems***
* Linux OS
* Supports bootup from SSD or SD card
* Support Backup/Restore from SD card/USB
* Boot Loader : Pi Bootloader
* File System : ETX4

***Software Development***
* Toolchain: gcc + glibc/uclibc/musl
* Supports remote C/C++ compilation

***Package Management***
* Package repository: Opiware self-
maintained repository
* Command: Standard apt, apt-get

***Popular Packages***
* Web server: Apache/Lighttpd
* Database: MySQL/SQLite3
* Scripting: PHP/Node.JS/Node-RED
* Text editor: vim/nano/sed
* Administration: WebRDS

***Software Documentation and Utility***
Please refer to “BM4Y-PIX” repository for software documentation and utility at following: http://www.github.com/Opiware/

#### 1.4 Packing List
* BM4Y-PIX: OpiBerry Embedded ARM Cortex-A72 with 2GB, 4GB or 8GB LPDDR4-3200 SDRAM, and 32GB / 16GB SSD Flash

#### 1.5 Optional Accessory
* PART-NUM3: DIN RAIL Mounting Kit
* PART-NUM4: 110~240VAC to 12VDC 1A Power Adaptor

## 2. Layout

#### 2.1 Connector & LED Indicator

* System Ready LED
* Giga LAN LED
* LAN LED
* Serial Port LED
* 9-48 VDC Power
* USB Console
* 10/100Mbps Ethernet
* Port
USB2.0
Gigabit Ethernet Port
RS-485 / RS-232
Ports

#### 2.2 Dimension
Unit: mm

## 3. Pin Assignment and Definitions

#### 3.1 LED Indicators

The LED provides the BM4Y-PIX operation information. The LED status is described
as follow:

* “Ready” (Ready LED indicator): Ready LED will turn on in green color while
power is properly supplied. After system is ready for operation, Ready LED will
keep in solid orange color and a beep will be heard

* “GLAN” & “LAN” (Network LED indicator): Link and Activity LED will turn ON
when the Ethernet cable is connected. When there is network data traffic, this LED
will flash.

* “P1 ~ P4” (Serial Port LED indicator): These eight dual color LEDs indicate the
data traffic at the serial ports. When RXD line is high then Green light is ON and
when TXD line is high, Yellow light is ON.

System Ready LED

Giga LAN LED

LAN LED

P1 ~ P4

(Serial Port LED)

#### 3.2 Serial Port

The BM4Y-PIX provide total four RS-485 / RS-232 ports that each port can be
configured by software.

RS-485 supports automatic direction control (by hardware).

The pin assignment is shown as following table.

Pin No. RS-232 RS-485

*1 DSR -*

*2 RTS DATA+*

*3 GND GND*

*4 TXD DATA-*

*5 RXD --*

*6 DCD -*

*7 CTS -*

*8 DTR -*

Enable/Disable Termination resistor for RS-485

The BM4Y-PIX equips on-board 120Ohm termination resistor for each RS-485 port.

Default setting is disable termination resistor. In order to enable termination resistor,
please remove the top cover of the BM4Y-PIX, and the adjust the associated jumper
to short position1 - 2, shown below:

RS-485 Port P1 P2 P3 P4

Jumper No. J2 J3 J4 J5

Termination Resistor Disabled (default)

Termination Resistor Enabled

1 2 3

1 2 3

RS-485 / RS-232

Ports

#### 3.3 Power Connector

Connecting +9 ~ +48VDC power line to the Power in terminal block. In the meantime,
Ready LED will turn on in green color while power is properly supplied.
After system is ready for operation, Ready LED will keep in solid orange color and a
beep will be heard

#### 3.4 Ethernet LAN Port

The Ethernet Port use RJ45 connector for both 10/100LAN port and GigaLAN port.

Pin definition of 10/100LAN connector.

PIN Signal

1 ETx +

2 ETx -

3 ERx +

6 ERx -

Pin definition of GigaLAN port

PIN Signal

1 TP0 +

2 TP0 -

3 TP1 +

4 TP2 +

5 TP2 -

6 TP1 -

7 TP3 +

8 TP3 -

#### 3.5 Console Port

There are two serial console ports for use:

• Micro-USB connector which is USB client acts as serial console port.

• Debug Console: There is a 4-pin wafer box header (JP3) inside the box.

Pin assignment is: RX, TX, +3.3V, GND.

Therefore, you need to open the upper metal case and prepare or purchase a
serial console cable to use the serial console port.

Or, it can be purchased “Console Cable” from Opiware, P/N is CB-PHDF9-050.

#### 3.6 USB Port

Two type-A USB 2.0 ports are built for operation.

1 2 3 4

RX

TX

+3.3V

GND

#### 3.7 SD card socket

There is a SD card socket inside as data storage. It can be accessed by opening top
cover.

SD Card

Socket
