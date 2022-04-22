Digital Thermometer

Thermometers are the device we use to measure the temperature in any desired scale and we all will be quite familiar with the analog thermometers. There are some disadvantages in analog thermometers and this can be overcome by using this digital thermometer using avr. The above embedded system shows the design and implementation of a simple Digital Thermometer using Atmega16 (AVR),  LM35 & 16×2 LCD.

In this project we are going to design a circuit for measuring temperature. This circuit is developed using “LM35”, a linear voltage sensor. Temperature is usually measured in “Centigrade” or “Faraheite”. “LM35” sensor provides output based on scale of centigrade.

LM35 is three pin transistor like device. It has VCC, GND and OUTPUT. This sensor provides variable voltage at the output based on temperature.
For every +1 centigrade raise in temperature there will be +10mV higher output. So if the temperature is 0◦centigrade the output of sensor will be 0V, if the temperature is 10◦ centigrade the output of sensor will be +100mV, if the temperature is 25◦ centigrade the output of sensor will be +250mV.

So for now with LM35 we get temperature in the form of variable voltage. This temperature dependent voltage is given as input to ADC (Analog to Digital Converter) of ATMEGA32A. The digital value after conversion obtained is shown in the 16x2 LCD as temperature.
