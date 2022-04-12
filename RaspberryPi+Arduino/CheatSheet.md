# Cheatsheet for Python/C++ for Raspberry Pi/Arduino

## RaspberryPi

### blink_serialCommands_pi2arduino_sender.pi
```
# THIS PROGRAM SENDS ON & OFF COMMANDS TO THE SERIAL CONNECTED ARDUINO
import serial
import time
  
if __name__ == '__main__':
    ser = serial.Serial('/dev/ttyUSB0',9600, timeout=1)
    ser.flush()
  
    while True:
        ser.write(b"ON\n")
        time.sleep(3)
        ser.write(b"OFF\n")
        time.sleep(3)
```
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
### blink_serialCommands_pi2arduino_receiver.ino
```
// THIS PROGRAM LISTENS TO THE SERIAL CONNECTION AND TURNS ON THE LED DEPENDING ON THE INPUT
// LOW = button pushed in
// HIGH = button not pushed in

// const variables
const int ledPin = 13;

// other variables
int buttonState = HIGH;
String command = "";

void setup() {
  Serial.begin(9600);               // set serial connection
  pinMode(ledPin, OUTPUT);          //set LED pin 13 as output
  delay(2000);
}

void loop() {
  if (Serial.available()){
  command = Serial.readStringUntil('\n');
  command.trim();
  
  if(command.equals("ON")){
      // turn LED on:
    digitalWrite(ledPin, HIGH);
  } else{
    // turn LED off:
    digitalWrite(ledPin, LOW);
  }
 }
}
```
