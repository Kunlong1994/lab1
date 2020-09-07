# Part I
# Light It Up
 
## Overview
For this assignment, you are going to 

A) [Set up a breadboard](#part-a-set-up-a-breadboard) 

B) [Manually blink a LED](#part-b-manually-blink-a-led) 

C) [Blink a LED using the Arduino](#part-c-blink-a-led-using-arduino)

D) [Manually fade a LED](#part-d-manually-fade-a-led) 

E) [Fade a LED using Arduino](#part-e-fade-a-led-using-arduino)

F) [Frankenlight](#part-f-frankenlight)

## In The Report
For the report, make a copy of this wiki page for your own repository, and then delete everything but the headers and the sections between the **stars**. Write the answers to the questions under the starred sentences. Include snippets of code that explain what you did.

Deliverables are due next Tuesday. Post a link to the wiki page on your main class hub page.

## Part A. Set Up a Breadboard



**Include a picture of your own breadboard in the report. (We trust you to plug the Metro Mini and wires in properly. This is really practice for including images in your reports.)**

## Part B. Manually Blink a LED

**a. What color stripes are on a 220 Ohm resistor?**
red red brown gold
 
**b. What do you have to do to light your LED?**
first install the driver, or try to fing the COM port in device manager
## Part C. Blink a LED using Arduino



### 1. Blink the on-board LED


**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**
int led = 10
void setup() {
  pinMode(led, OUTPUT); \\Change the pin port number to 10
}

void loop() {
  digitalWrite(led, HIGH);   
  delay(1000);                      
  digitalWrite(led, LOW);   
  delay(1000);       
**b. What line(s) of code do you need to change to change the rate of blinking?**
change delay(1000) to delay(2000)
**c. What circuit element would you want to add to protect the board and external LED?**
the resistor, to reduce the voltage to 2 volts.
**d.  At what delay can you no longer *perceive* the LED blinking? (And how can you prove to yourself that it is, in fact, still blinking?**
50, current is still flowing and when change delay to 500, it starts to blink again

**e. Save your new blink code to your lab 1 repository, with a link on the Lab report wiki page.**

### 2. Blink your LED


**Make a video of your LED blinking, and add it to your lab submission.**

## Part D. Manually fade a LED
**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**
No, potrntiometer provides different resistance, when the resistance is too high, there is not enough current for led
## Part E. Fade a LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**
use int to input brightness and fade amount, use analogWrite() to set the brightness
**b. What is analogWrite()? How is that different than digitalWrite()?**
 analogWrite() sets the value of a PWM output pin on a scale of 0 - 255.
 digital sets the value only to HIGH and LOW


## Part F. FRANKENLIGHT!!!



### 1. Take apart your electronic device, and, as well as you can, draw a system diagram of what is inside. 

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

**d. Is information stored in your device? Where? How?**

### 2. Using your diagram, figure out where a good point would be to hijack your device and implant an LED.

### 3. Build your light!


**Make a video showing off your Frankenlight.**

**Include any diagrams or photos in your lab write-up.**

