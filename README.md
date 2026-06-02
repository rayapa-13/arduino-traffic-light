# Arduino Traffic Light Simulation

My first Arduino project built using Tinkercad.

<img width="462" height="267" alt="Screenshot 2026-06-02 165347" src="https://github.com/user-attachments/assets/f445ea37-bc5e-4f92-9c03-ac2855b0f987" />

## Project Overview

This project simulates a traffic light system using an Arduino Uno, three LEDs (red, yellow, and green), and resistors.

## Components Used

* Arduino Uno
* Red LED
* Yellow LED
* Green LED
* 3 Resistors
* 
## How It Works

The Arduino controls the LEDs in sequence:

1. Green LED turns ON for 5 seconds.
2. Yellow LED turns ON for 2 seconds.
3. Red LED turns ON for 5 seconds.
4. The cycle repeats continuously.

## Skills Learned

* Basic Arduino programming
* LED polarity
* Circuit connections
* Use of resistors
* Digital output pins

## Tools Used

* Tinkercad
* Arduino
* GitHub

## Circuit Code

```cpp
int red = 13;
int yellow = 12;
int green = 11;

void setup() {
  pinMode(red, OUTPUT);
  pinMode(yellow, OUTPUT);
  pinMode(green, OUTPUT);
}

void loop() {
  digitalWrite(green, HIGH);
  delay(5000);
  digitalWrite(green, LOW);
  
  digitalWrite(yellow, HIGH);
  delay(2000);
  digitalWrite(yellow, LOW);
  
  digitalWrite(red, HIGH);
  delay(5000);
  digitalWrite(red, LOW);
}

