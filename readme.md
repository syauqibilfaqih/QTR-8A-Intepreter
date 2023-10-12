This is the repository of QTR-8A Interpreter circuit that supports both digital data transmission through gpio pins and UART communication between master microcontroller and slave microcontroller, which is Arduino Nano, to read the QTR-8A sensor data. Use KiCad to open the schematic and board file, whereas use PlatformIO VS Code to open the code and build it.

![image](https://github.com/syauqibilfaqih/QTR-8A-Intepreter/assets/70939903/1892c29d-29e9-45bf-a563-005ce13b04ad)

To calibrate the line sensor, there are three ways to trigger the calibration mode:

1. By pressing button
2. By sending command "clib" via UART
3. By giving active signal to pin 12

Once the calibration mode is activated, move the sensors to get the black and white surface of the track. When it's done, the led indicators will show the correct reading state, where if the sensor read the black surface, the led will be turned on, otherwise it will be turned off.

