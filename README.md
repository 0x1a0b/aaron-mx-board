Forked from https://git.okoyono.de/aaron/mx-board



mxboard
=======

Cherry MX breakout board for Arduino, RaspberryPi and other boards.

![front](/images/v01_front.png)
![back](/images/v01_back.png)

Order here: https://oshpark.com/shared_projects/PogDjaIS


Arduino Sample
==============

```arduino
const int buttonPin = 10;
const int ledPin = 11;

void setup() {
  pinMode(buttonPin, INPUT);
  pinMode(ledPin, OUTPUT);
}

void loop() {
  // The switches are equiped with pull-down resistors. So if the
  // button is pressed, you read a HIGH, if the button is released
  // you read a LOW.
  digitalWrite(ledPin, digitalRead(buttonPin));
}
```
