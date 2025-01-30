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

CODE: 
// Define the LED pins
const int led1 = 2;  // First LED connected to pin 2
const int led2 = 3;  // Second LED connected to pin 3
const int led3 = 4;  // Third LED connected to pin 4
const int led4 = 5;  // Fourth LED connected to pin 5
const int led5 = 6;  // Fifth LED connected to pin 6

void setup() {
  // Set all LED pins as OUTPUT
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);
  pinMode(led3, OUTPUT);
  pinMode(led4, OUTPUT);
  pinMode(led5, OUTPUT);
}

void loop() {
  // Turn on LEDs sequentially
  digitalWrite(led1, HIGH);
  delay(500);  // Wait for 500ms
  digitalWrite(led2, HIGH);
  delay(500);
  digitalWrite(led3, HIGH);
  delay(500);
  digitalWrite(led4, HIGH);
  delay(500);
  digitalWrite(led5, HIGH);
  delay(500);

  // Turn off LEDs in reverse order
  digitalWrite(led5, LOW);
  delay(500);
  digitalWrite(led4, LOW);
  delay(500);
  digitalWrite(led3, LOW);
  delay(500);
  digitalWrite(led2, LOW);
  delay(500);
  digitalWrite(led1, LOW);
  delay(500);
}
