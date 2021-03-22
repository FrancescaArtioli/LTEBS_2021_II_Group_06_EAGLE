# LTEBS_2021_II_Group_06_EAGLE
This repository contains a complete Eagle project of a custom PCB, designed in order to ease the assessment of the performance of the PSoC-5LP microcontroller. 
In particular, the repository contains the schematic (.sch), the board (.brd) and the design-rule-check file (.dru) based on technical requirements by MDSrl. 

The PCB embeds the developement kit for PSoC-5LP (namely CY8CKIT-059_TARGET) together with sensors and additional components required to conduct the proper testing.

### Sensors (from SparkFun-Sensors.lbr) 
-	Light Sensor

	PHOTOCELLPTH - PHOTOCELL

- Analog Temperature Sensor

	TMP36GT9 - TO-92
  
### Setup
The setup for testing purposes is based on a custom PCB. The PCB is powered through a 12V power jack, and a voltage regulator stabilizes the supply to 5V. I2C connectors and a quad bidirectional translating switch controlled via the I2C bus are embedded on the PCB.

### Libraries 

- SparkFun-Eagle-Libraries, downloaded from https://github.com/sparkfun/SparkFun-Eagle-Libraries

- CY8KIT-059.lbr, downloaded from https://github.com/dado93/Cypress-Eagle

- Group_06_Library.lbr, a custom library for TMUX1208 and TCA9546A.

### Notes on Group_06_Library.lbr
-	We have decided to design the pads for both components TMUX1208 (package QFN-16) and TCA9546A (package TSSOP-16) with a rectangular shape. 
-	Regarding package dimension of component TMUX1208 we have decided to keep the middle value between maximum and minimum dimension (1.80mmx2.60mm).
-	Regarding package dimension of component TCA9546A we have decided to keep the middle value between maximum and minimum dimension (4.4mmx5mm).

### Notes on Group_06.sch 
-	Schematic is divided into two pages.

### Notes on Group_06.brd

### Notes on Group_06.dru
