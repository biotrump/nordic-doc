[The segger IDE, Segger Embedded Studio, SES, is the only IDE tool to work for Nordic nrfxxx SDK since 2020.](
https://developer.nordicsemi.com/nRF_Connect_SDK/doc/1.3.0/nrf/gs_installing.html#installing-ses-nordic-edition)  
# [1. Download Segger Embeded Studio for Nordic](https://developer.nordicsemi.com/nRF_Connect_SDK/doc/1.3.0/nrf/gs_installing.html#gs-installing)  
This is a special segger embeded studio,SES, for nordic.

## [2. Upgrade firmware to j-Link is the first step for debug and download](https://www.segger.com/downloads/jlink/JLink_Linux_x86_64.deb)

### [j-Link is an old debug device, so it needs firmware update.](https://www.segger.com/downloads/jlink/#J-LinkSoftwareAndDocumentationPack)  

### New DevKit of nordic after Nov 2019 gets a free license to use segger IDE tool.  
### PCA10056 nRF52840-DK is old enough shipped before Nov 2019, so segger IDE does NOT support it any free license.  
* After segger j-link tool is installed in your PC, "nRF Connect for Desktop" tool can automatically update firmware to segger j-link, so this is the first step to work for Nordic nrf board.

# 3. The nordic nRF5 SDK and IDE Tool Installation
## [*1. The first step is to install "nRF Connect for Desktop"](https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/gs_assistant.html#gs-assistant)  

## [2. "Getting Started Assistant" from "nRF Connect for Desktop"](https://developer.nordicsemi.com/nRF_Connect_SDK/doc/latest/nrf/gs_assistant.html#getting-started-assistant)
It assists you to install and setup tools and environment.

## [3. Download nRF5 SDK](https://www.nordicsemi.com/Software-and-tools/Software/nRF5-SDK/Download#infotabs)  
* The nRF Connect SDK is where you begin building low power wireless applications with Nordic Semiconductor nRF52, nRF53, and nRF91 Series devices.
* The SDK contains optimized cellular IoT (LTE-M and NB-IoT), Bluetooth Low Energy, Thread, Zigbee, and Bluetooth Mesh stacks, a range of applications, samples, and reference implementations, as well as a full suite of drivers for Nordic Semiconductor’s devices. 
* The nRF Connect SDK includes the Zephyr™ real-time operating system (RTOS), which is built for connected low power products.

## 4. Open an example of nRF SDK in SES to build it for PCA10056, nrf52840.
   * SES: File->Open solution-> browse to /path/sdk/examples/peripheral/blinky/pca10056/blank/ses/blinky_pca10056.emProject
   * open blinky_pca10056.emProject
   * build the solution.
   * Target-> Download blinky_pca10056
