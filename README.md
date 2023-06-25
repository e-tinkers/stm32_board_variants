# TechStudio G070 Boards Arduino IDE configuration

This repo contains the board configuration for 
 * TechStudio G070 Boards
 * PalmTop board 

> For more details on the usage of these custom boards, please refer to [blog 
post](https://www.e-tinkers.com/2023/06/build-a-palmtop-handheld-with-stm32g070-part-1/) on 
e-tinkers.com.

on Arudino IDE based on ST Microelectronics' official [Arduino Core STM32](https://github.com/stm32duino/Arduino_Core_STM32).

The Generic variants for G070KBT/G070CBT has been part of the Arduino Core STM32 releasee version 2.3.0 based on TechStudio's [Pull Request](https://github.com/stm32duino/Arduino_Core_STM32/pull/1638).  For custom boards, this repository is required to be placed in hardware directory within Arduino IDE environment. This repository will no longer needed once those variants are added into STM32duino core.

## Installation

- In order to use the custom board setting, you must have the STM32duino Arduino Core installed, if you don't have it installed yet, please follow the "Getting Started" instructions at https://github.com/stm32duino/wiki/wiki/Getting-Started to install the Arduino Core.

- Quit the Arduino IDE.

- Clone this github into your Arduino hardware environment by creating a **hardware** directory.

```
    $ mkdir -p $HOME/Arduino/hardware
    $ cd $HOME/Arduino/hardware
    $ git clone https://github.com/e-tinkers/variants.git variants
```

## Configuration

Launch Arduino IDE, and select the board from **Tools -> Boards -> STM32G070xx Custom Boards**. Make sure that you choose the correct board part number, upload method, etc., and you are ready to go.

![Arduino IDE Board Configuration](board_configuration.png)
