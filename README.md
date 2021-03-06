# LTEBS_2021_II_Group_06_EAGLE
Authors: Artioli Francesca, Parrella Giovanni

This repository contains a complete Eagle project of a custom PCB, designed in order to ease the assessment of the performance of the PSoC-5LP microcontroller. 
In particular, the repository contains the schematic (.sch), the board (.brd) and the design-rule-check file (.dru) based on technical requirements by MDSrl. 

The PCB embeds the developement kit for PSoC-5LP (namely CY8CKIT-059_TARGET) together with sensors and additional components required to conduct the proper testing.

### Sensors (from SparkFun-Sensors.lbr) 
-	Light Sensor

	PHOTOCELLPTH - PHOTOCELL

- 	Analog Temperature Sensor

	TMP36GT9 - TO-92
  
### Libraries 

- SparkFun-Eagle-Libraries, downloaded from https://github.com/sparkfun/SparkFun-Eagle-Libraries

- CY8KIT-059.lbr, downloaded from https://github.com/dado93/Cypress-Eagle

- Group_06_Library.lbr, a custom library for TMUX1208 and TCA9546A from Texas Instruments.

### Notes on Group_06_Library.lbr
-	We have decided to design the pads for both components TMUX1208 (package QFN-16) and TCA9546A (package TSSOP-16) with a rectangular shape. 
-	Regarding package dimension of component TMUX1208 we have decided to keep the middle value between maximum and minimum dimension (1.80mmx2.60mm).
-	Regarding package dimension of component TCA9546A we have decided to keep the middle value between maximum and minimum dimension (4.4mmx5mm).
-	In both the components' footprint we have added the profile silkscreen in a way that it wouldn't provide a stop-mask error in the DRC (even if we have not considered stop mask error when running the DRC file, as suggested). 

### Notes on Group_06.sch 
-	Schematic is divided into two pages.

### Notes on Group_06.brd
-	The trace dimension was set to 10 mils for all traces of the PCB, except for those connecting to the mux which were set to 8 mils to avoid clearance errors.
-	Final board dimensions are : 60.83 mm x 72.39 mm

### Notes on Group_06.dru
-	We followed the requirements from the MDSrl.
-	The "check stop mask" option in the MISC section was not selected, as suggested. 
