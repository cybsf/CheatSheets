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

### button.ino
// LOW = circuit closed = button pushed in
// HIGH = circuit open = button not pushed in

const int ledPin = 13;
const int buttonPin = 9;

int buttonState = HIGH;

void setup() {
  // put your setup code here, to run once:
  pinMode(ledPin, OUTPUT);
  pinMode(buttonPin, INPUT_PULLUP);
}

void loop() {
  // put your main code here, to run repeatedly:

  buttonState = digitalRead(buttonPin);

  // check if the pushbutton is pressed. If it is, the buttonState is HIGH:
  if (buttonState == LOW) {
    // turn LED on:
    digitalWrite(ledPin, HIGH);
  } else {
    // turn LED off:
    digitalWrite(ledPin, LOW);
  }
}



