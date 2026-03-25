## Introduction
WisBlock is an amazing product built by the RAK company for IoT industry. It can build circuits like clicking blocks together to quickly realize your idea.

WisBlock consists of WisBlock Base, WisBlock Core, WisBlock Sensor and WisBlock IO.
- WisBlock Base → the block that the whole system is build on.    
- WisBlock Core → the processing unit with the micro-controller.    
- WisBlock Sensor → the blocks with variety of sensors.    
- WisBlock IO → the blocks that extend the communication options and interfacing capabilities of the WisBlock.

![WisBlock-Assembly](assets/repo/WisBlock-Assembly.png)


----
## Where to find what

----

### Documentation

- Documentation  
    - [Quick Start Guide RAK4630](https://docs.rakwireless.com/Product-Categories/WisBlock/RAK4631/Quickstart/)
    - [Quick Start Guide WisBlock Base](quickstart/Base)
    - [Quick Start Guide WisBlock IO Modules](quickstart/IOModules)
    - [Quick Start Guide WisBlock Sensor Modules](quickstart/SensorModules)
----

### Examples

- [Examples](/examples/)    
    - [Common for all WisBlock Cores](/examples/common/)
        - [Slot A - D Modules](/examples/common/sensors/)
            - [RAK1901_Temperature&Humidity_SHTC3](/examples/common/sensors/RAK1901_Temperature_Humidity_SHTC3/)
            - [RAK1906_Environment_BME680](/examples/common/sensors/RAK1906_Environment_BME680/)
            - [RAK1920_MikroBUS_Temperature_TMP102](/examples/common/sensors/RAK1920_MikroBUS_Temperature_TMP102/)
            - [RAK1920_QWIIC_AirQuality_SGP30](/examples/common/sensors/RAK1920_QWIIC_AirQuality_SGP30/)
            - [RAK1920_Grove_PIR_AS312](/examples/common/sensors/RAK1920_Grove_PIR_AS312/)
            - [RAK12020_Light_TSL_INT_TSL2591](/examples/common/sensors/RAK12020_Light_TSL_INT_TSL2591/)
            - [RAK12020_Light_TSL_Read_TSL2591](/examples/common/sensors/RAK12020_Light_TSL_Read_TSL2591/)
        - [IO Slot Modules](/examples/IO/)
			- [RAK12005_WaterDetector](/examples/common/IO/RAK12005_WaterDetector)
			- [RAK12035_SoilMoisture](/examples/common/IO/RAK12035_SoilMoisture)
			- [RAK12035_SoilMoisture](/examples/common/IO/RAK12035_SoilMoisture)
    
----
    
-    
    - [RAK4630 Examples](/examples/RAK4630/) 
        - [RAK4630 Communications](/examples/RAK4630/communications/)
            - [LoRa](/examples/RAK4630/communications/LoRa/)
                - [LoRaWAN](/examples/RAK4630/communications/LoRa/LoRaWAN/)
                - [LoRa P2P](/examples/RAK4630/communications/LoRa/LoRaP2P/)
            - [BLE](/examples/RAK4630/communications/BLE/)
                - [BLE Proximity Sensing](/examples/RAK4630/communications/BLE/ble_proximity_sensing/)
                - [BLE_OTA_DFU](/examples/RAK4630/communications/BLE/ble_ota_dfu/)
                - [BLE_UART](/examples/RAK4630/communications/BLE/ble_uart/)
                - [BLE_Health](/examples/RAK4630/communications/BLE/BLE_Health/)
                - [RAK12010 BLE](/examples/RAK4630/communications/BLE/RAK12010_Ble/)
                - [RAK12019 BLE](/examples/RAK4630/communications/BLE/RAK12019_UVlight_LTR390_Ble/)
            - [WiFi](/examples/RAK4630/communications/WiFi/)
                - [AT_Command_Test](/examples/RAK4630/communications/WiFi/AT_Command_Test/)
                - [connect_ap](/examples/RAK4630/communications/WiFi/connect_ap/)
        - [RAK4630 Power](/examples/RAK4630/power/)
            - [RAK4630_Battery_Level](/examples/RAK4630/power/RAK4630_Battery_Level_Detect/)
        - [RAK4630 Solutions](/examples/RAK4630/solutions/)
            - [BLE_Gateway](/examples/solutions/BLE_Gateway/)
            - [Hydraulic_Pressure_Monitoring](/examples/RAK4630/solutions/Hydraulic_Pressure_Monitoring/)
            - [Environment_Monitoring](/examples/RAK4630/solutions/Environment_Monitoring/)
            - [Water_Level_Monitoring](/examples/RAK4630/solutions/Water_Level_Monitoring/)
            - [Weather_Monitoring](/examples/RAK4630/solutions/Weather_Monitoring/)
            - [GPS_Tracker](/examples/RAK4630/solutions/GPS_Tracker/)
            - [PAR_Monitoring](/examples/RAK4630/solutions/PAR_Monitoring/)
            - [Soil_Conductivity_Monitoring](/examples/RAK4630/solutions/Soil_Conductivity_Monitoring/)
            - [Soil_pH_Monitoring](/examples/RAK4630/solutions/Soil_pH_Monitoring/)
            - [Wind_Speed_Monitoring](/examples/RAK4630/solutions/Wind_Speed_Monitoring/)
            - [Intelligent_Agriculture](/examples/RAK4630/solutions/Intelligent_Agriculture/)
            - [LoRaWAN_Health](/examples/RAK4630/solutions/LoRaWAN_Health/)
            - [RAK12010 LoRaWan](/examples/RAK4630/solutions/RAK12010_LoRaWan/)
            - [RAK12019 LoRaWan](/examples/RAK4630/solutions/RAK12019_UVlight_LTR390_LoRaWan/)
            - [RAK12035 LoRaWan](/examples/RAK4630/solutions/RAK12035_RAK4631_LPWAN/)


----

- Bootloader/Firmware
    - [RAK4630](bootloader/RAK4630)
        - [Flashable Bootloader](bootloader/RAK4630/Latest)
        - [Bootloader Source Code](bootloader/RAK4630/Latest/WisCore_RAK4631_Bootloader)
----

- PlatformIO installation
   - [Patch for PIO installation](PlatformIO)
   - [RAK4630 PlatformIO files](PlatformIO/RAK4630/)
----


## Overview
WisBlock is a modular Plug&Play system. Compared with other systems (Arduino, Raspberry Pi, M5Stack), it has several advantages:

1. Using a compact connector makes its size very small. A WisBlock Base board, which is the base carrier, is only 30mm by 60mm in size. One WisBlock Base can hold one micro-controller module (WisBlock Core), one IO module (WisBlock IO) and up to 4 sensor modules (WisBlock Sensor).

2. Using an industrial rated connector enables you to use the same modules from rapid prototyping to testing to final product.  

3. WisBlock is not only modular on hardware base. With ready to use software blocks, it is simple to create an application to match your implementation requirements.

----
## Modularity
### Base board
WisBlock Base is the base board that makes flexibility and modularity possible.

### Plug&Play hardware modules 
WisBlock Core → processing block with LoRa/LoRaWan, WiFi or BLE connectivity.    
WisBlock Sensor → wide range of sensor blocks.    
WisBlock IO → blocks for user interfaces, custom sensor connections and actuators.

### Plug&Play software modules
Using Arduino framework, WisBlock provides a free and widely available programming environment:
- Open Source libraries for communication protocols
- Open Source libraries for data processing
- Open Source libraries for sensors input
- Open Source libraries for actuators
- Open Source libraries for user interfaces

----
### WisBlock Base
WisBlock is build up on a WisBlock Base board. It is a platform carrier that allows easy plug-in of one WisBlock Core processing board, one WisBlock IO interface board and up to four WisBlock Sensor boards.

WisBlock Base is providing the power supply, battery and solar panel connections and charging block. In addition it has connectors for programming and debugging. 

During development phase, WisBlock Base allows you to quickly switch between microcontrollers, IO functionality and sensors by simply changing the modules.

Repairs and upgrades are easy with WisBlock Base on your final product, because modules can be changed with just Plug'n'Play.

For controlling and limiting power consumption of your IoT solution, WisBlock Base enables to control the power supply for the WisBlock Sensor and WisBlock IO modules, limiting the power consumption by switching off these modules if they are not needed.

----
### WisBlock Core
WisBlock Core is the processing unit of your IoT solution.

Select the processing power based on the requirements of your application from a range of processing boards which starts with low single core to high dual core processing power units are available. 

All of them communication capability, some of them offer in addition LoRa/LoRaWAN, WiFi, Bluetooth or Bluetooth Low Energy. All are designed for battery optimized low power consumption.

----
### WisBlock Sensor
A range of sensors for sensing environmental conditions (temperature, humidity, …), location and movement conditions (GNSS/GPS, accelerometer, …) that you just plug into WisBlock Base makes it easy to complete your application with the required sensors.

----
### WisBlock IO
WisBlock IO extensions provide your application with interfaces that are not covered by WisBlock Core or WisBlock Sensor blocks.     
This includes 
- user interfaces like 
  - keyboards
  - buttons
  - displays
- communication interfaces like    
  - 0~5V
  - 4-20mA
  - I2C
  - RS232
  - RS485
  - many more
- alternative power supplies like
  - 24V
  - POE
