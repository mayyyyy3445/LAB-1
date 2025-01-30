# LAB-1

Each LED is connected to the Arduino through a resistor, and the circuit is powered via a USB connection to the Arduino.

Explanation of the Setup:
	1.	Arduino Uno: The microcontroller board used to control the LEDs.
	2.	Breadboard: Used for prototyping and easy circuit connections.
	3.	LEDs: Five LEDs (blue, yellow, red, brown, and green) are connected in parallel.
	4.	Resistors: Each LED has a resistor in series to limit the current and prevent damage.
	5.	Wiring:
	•	The long leg (anode, +) of each LED is connected to an Arduino digital output pin.
	•	The short leg (cathode, -) is connected to the ground (GND) of the Arduino.

Functionality:
	•	The Arduino can control the LEDs by setting the respective pins HIGH (ON) or LOW (OFF) through code.
	•	A program (sketch) in the Arduino IDE would allow the LEDs to blink, turn on in sequence, or respond to input.

