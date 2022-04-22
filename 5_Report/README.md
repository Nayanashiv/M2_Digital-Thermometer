Digital Thermometer

    Thermometers are the device we use to measure the temperature in any desired scale and we all will be quite familiar with the analog thermometers. There are some disadvantages in analog thermometers and this can be overcome by using this digital thermometer using avr. The above embedded system shows the design and implementation of a simple Digital Thermometer using Atmega16 (AVR),  LM35 & 16×2 LCD.

    In this project we are going to design a circuit for measuring temperature. This circuit is developed using “LM35”, a linear voltage sensor. Temperature is usually measured in “Centigrade” or “Faraheite”. “LM35” sensor provides output based on scale of centigrade.

    LM35 is three pin transistor like device. It has VCC, GND and OUTPUT. This sensor provides variable voltage at the output based on temperature.For every +1 centigrade raise in temperature there will be +10mV higher output. So if the temperature is 0◦centigrade the output of sensor will be 0V, if the temperature is 10◦ centigrade the output of sensor will be +100mV, if the temperature is 25◦ centigrade the output of sensor will be +250mV.

    So for now with LM35 we get temperature in the form of variable voltage. This temperature dependent voltage is given as input to ADC (Analog to Digital Converter) of ATMEGA32A. The digital value after conversion obtained is shown in the 16x2 LCD as temperature.

Atmega connections are as follows:
Pin1 (Ground/Source Pin): This is a GND pin of display, used to connect the GND terminal of the microcontroller unit or power source.
Pin2 (VCC/Source Pin): This is the voltage supply pin of the display, used to connect the supply pin of the power source.
Pin3 (V0/VEE/Control Pin): This pin regulates the difference of the display, used to connect a changeable POT that can supply 0 to 5V.
Pin4 (Register Select/Control Pin): This pin toggles among command or data register, used to connect a microcontroller unit pin and obtains either 0 or 1(0 = data mode, and 1 = command mode).
Pin5 (Read/Write/Control Pin): This pin toggles the display among the read or writes operation, and it is connected to a microcontroller unit pin to get either 0 or 1 (0 = Write Operation, and 1 = Read Operation).
Pin 6 (Enable/Control Pin): This pin should be held high to execute Read/Write process, and it is connected to the microcontroller unit & constantly held high.
Pins 7-14 (Data Pins): These pins are used to send data to the display. These pins are connected in two-wire modes like 4-wire mode and 8-wire mode. In 4-wire mode, only four pins are connected to the microcontroller unit like 0 to 3, whereas in 8-wire mode, 8-pins are connected to microcontroller unit like 0 to 7.
Pin15 (+ve pin of the LED): This pin is connected to +5V
Pin 16 (-ve pin of the LED): This pin is connected to GND.

