#Cheatsheet for Python/C++ for Raspberry Pi/Arduino

##RaspberryPi

##Arduino


###blink.ino
```
void setup() {
  // put your setup code here, to run once:
pinMode(13, OUTPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
  digitalWrite(13, HIGH); // Turn the LED on
  delay(1000);
  digitalWrite(13, LOW); // Turn the LED on
  delay(1000);
}
```
