# M2_Embedded_HCS
## Heat Control System

### THEORY:>

The heat control system is basically used to control the temperature of a car seat. When a user or driver of the car gets seated on a car, the button sensor gets activated.
After that, the user gets access to turn on the heater. The temperature sensor keeps monitoring the temperature and sends the analog value to the microcontroller.
The microcontroller processes the analog input of the temperature sensor and outputs a temperature value through serial communication.
All the activities of the control system are done on a microcontroller called Atmega328.

### SIMULATION:>

The functionality of the heat control system is coded in embedded c and the working is demonstrated using simuation in a software called SimulIDE.
Below shows two images where in the 1st image shows the status of the simulation when the system is OFF and the second image shows the status of the system when it is ON. 

#### ON

![ON](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Simulation.gif)

#### OFF

![OFF](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Simulation_OFF.PNG)

#### Outputs

|Circuit|RAM Table|
|:--:|:--:|
|![CIRCUIT](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Circuit.gif)|![RAM_TABLE](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/RAM_table.gif)|
|CRO|Serial Monitor|
|![CRO](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Oscilloscope.gif)|![ON](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Serial_Monitor.gif)|

### Functionality 

* When the two switches are closed, the first LED glows indicating the actuation of the system and the heater.
* Next the analog input from the temperature sensor is received and digitized.
* The digitized temperature input is visualized using Pulse Width Modulation.
* The corresponding temperature values based on the digitized temperature input is transmitted by the UART protocol. Here the data is displayed on the serial monitor.

### CI  And  Code Quality 

|Code Quality Score|Code Grade|Codacy|CI|Compile Linux|Git Inspector|Linux c/c++ CI|Cpp Check|
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|![Code Quality Score](https://api.codiga.io/project/30017/score/svg)|![Code Grade](https://api.codiga.io/project/30017/status/svg)|[![Codacy Badge](https://app.codacy.com/project/badge/Grade/62503ea0dee44bc3ab92614946c3cdb3)](https://www.codacy.com/gh/satyendra11111/M2_Embedded_Heat-Control-System/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=satyendra11111/M2_Embedded_Heat-Control-System&amp;utm_campaign=Badge_Grade)|[![CI](https://github.com/satyendra11111/M2_Embedded_Heat-Control-System/actions/workflows/main.yml/badge.svg)](https://github.com/satyendra11111/M2_Embedded_Heat-Control-System/actions/workflows/main.yml)|[![Compile-Linux](https://github.com/VatsalKr/M2_Embedded_Temperature_Controlled_Car_Seats/actions/workflows/compile.yml/badge.svg)](https://github.com/satyendra11111/M2_Embedded_Heat-Control-System/actions/workflows/compile.yml)|[![GitInspector](https://github.com/VatsalKr/M2_Embedded_Temperature_Controlled_Car_Seats/actions/workflows/Gitinspector.yml/badge.svg)](https://github.com/VatsalKr/M2_Embedded_Temperature_Controlled_Car_Seats/actions/workflows/Gitinspector.yml)|[![Linux C/C++ CI](https://github.com/VatsalKr/M2_Embedded_Temperature_Controlled_Car_Seats/actions/workflows/Linux-c-cpp.yml/badge.svg)](https://github.com/VatsalKr/M2_Embedded_Temperature_Controlled_Car_Seats/actions/workflows/Linux-c-cpp.yml)|[![cppcheck](https://github.com/satyendra11111/M2_Embedded_Heat-Control-System/actions/workflows/CodeQuality.yml/badge.svg)](https://github.com/satyendra11111/M2_Embedded_Heat-Control-System/actions/workflows/CodeQuality.yml)|


