# Cheatsheet for Python/C++ for Raspberry Pi/Arduino

## RaspberryPi

## Arduino

### blink.ino
```
// THIS PROGRAM BLINKS THE LED ON DP13

// const variables
const int ledPin = 13

// other variables

void setup() {
  pinMode(ledPin, OUTPUT); 	//set pin 13 as output
}

void loop() {
  digitalWrite(ledPin, HIGH); 	// Turn the LED on
  delay(1000);			// Wait for 1 second
  digitalWrite(ledPin, LOW); 	// Turn the LED of
  delay(1000);			// Wait for 1 second
}
```

### button.ino
```
// THIS PROGRAM TURNS ON THE LED ON DP13 WHEN PRESSING THE BUTTON 
// LOW = button pushed in
// HIGH = button not pushed in

// const variables
const int ledPin = 13;
const int buttonPin = 9;

// other variables
int buttonState = HIGH;

void setup() {
  pinMode(ledPin, OUTPUT);		//set LED pin 13 as output
  pinMode(buttonPin, INPUT_PULLUP);	//set button pin 9 as input 
}

void loop() {

  buttonState = digitalRead(buttonPin);	//read button status

  // checks status of button and turn on/off LED
  if (buttonState == LOW) {
    // turn LED on:
    digitalWrite(ledPin, HIGH);
  } else {
    // turn LED off:
    digitalWrite(ledPin, LOW);
  }
}
```

