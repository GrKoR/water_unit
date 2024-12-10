# ESPHome Water Control Unit

**Current status:** not finished, work in progress.


## Features
* Hot and cold water consumption monitoring (reed switch output of the meters).
* Measurement of the water pressure before filters and after pressure reducer for both hot and cold water.
* Measurement of the water temperature for: water heater, hot water inlet, cold water inlet.
* Control of the air temperature in the device's case.
* Automatic and manual mode for opening / closing of hot and cold water.
* Water leakage control in several points of the system. 
* It is possible to manually ignore leakage for 10 minutes. 
* Values of total water consumption counters are stored in the flash during reboot.
* Initial values of total water consumption counters can be set by Home Assistant service calls.
* Implemented once per month call of valve's service action (close & open of water inlets).
* Stores date of last service action.
* Helpers: 1-wire online device searching, average ADC voltage measurement, disable pressure value publishing to the Home Assistant.


## Hardware

CPU board of this project is [WT32-ETH01](https://files.seeedstudio.com/products/102991455/WT32-ETH01_datasheet_V1.1-%20en.pdf) with the following pin usage:  
![esp-pinout](https://github.com/GrKoR/)


Schematic diagram of the board:  
![board-schematic](https://github.com/GrKoR/)

PCB of the water unit (made only as a test of trace routing for handmade prototyping):  
![pcb-prototype](https://github.com/GrKoR/)