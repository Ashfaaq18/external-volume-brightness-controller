# external-volume-brightness-controller
An external volume and brightness controller circuit for Windows PC


## Top level Design idea

![ExtWinVol BriController drawio(3)](https://github.com/Ashfaaq18/external-volume-brightness-controller/assets/27722888/a471bb13-e5df-40b7-b6b5-099ef11513b0)

The rough idea to build a prototype of the above design,
1.	Create a barebones windows app to,
    - Retrieve the brightness and volume of the system and show in GUI
    - Set the brightness and volume of the system
    - Send the retrieved data through COM port
2.	Use an Arduino to,
    - Display the data coming from the app in the IDE console
    - Send test data from Arduino to the app and change the brightness and volume accordingly
3.	Simulate a barebone circuit in LTSpice to,
    - generate signals which can be read by the Arduino GPIO ports.
    - The circuit should have a controller for the input and LEDs to display the output

By implementing the hardware of LTSpice circuit and connecting it to the Arduino which, inturn, is connected to the PC. The system should be able to control the PC's volume and brightness.

## Files in this repository

The Controller App development, Arduino code and LTSpice circuit designs will be added to this repository as development proceeds.

## Why make this overcomplicated system? 
Just to challenge myself to work with low level code and hardware.
This system can also be extended further in the future to control various other Windows OS parameters with an external circuit.
