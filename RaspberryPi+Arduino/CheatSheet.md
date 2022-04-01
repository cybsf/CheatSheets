# Cheatsheet for Python/C++ for Raspberry Pi/Arduino

## RaspberryPi

## Arduino

### blink.ino
```
int ledPin = 13

void setup() {
  // put your setup code here, to run once:
  pinMode(ledPin, OUTPUT); 	//set pin 13 as output
}

void loop() {
  // put your main code here, to run repeatedly:
  digitalWrite(ledPin, HIGH); 	// Turn the LED on
  delay(1000);			// Wait for 1 second
  digitalWrite(ledPin, LOW); 	// Turn the LED of
  delay(1000);			// Wait for 1 second
}
```
