# NotSoBasicArduino
 The follwing files are my second foray into Arduino
 
 
## Table of Contents
* [Table of Contents](#TableOfContents)
* [LED_Fade](#LED_Fade)
* [Hello_LCD](#Hello_LCD)
* [Button Blink](#Button_Blink)

---

## LED_Fade

### Description & Code
Description goes here

Here's how you make code look like code:

```C++
// set the brightness of pin 9:
  analogWrite(led, brightness);

  // change the brightness for next time through the loop:
  brightness = brightness + fadeAmount;

  // reverse the direction of the fading at the ends of the fade:
  if (brightness <= 0 || brightness >= 255) {
    fadeAmount = -fadeAmount;
  }
```
The fade works by initiating a pin and then writing the code to make the fade happen including delay and fade brightness at the beginning and end of the fade itslef

### Evidence
https://create.arduino.cc/editor/apleasa54/7a0bae17-54c3-4c51-80d4-5a42eccba073

### Images
<img src="https://github.com/apleasa54/NotSoBasicArduino-1/blob/main/IMG_20201123_203808.jpg" width="400">

### Reflection
This assignment was fairly easy once I understood what I needed to do and was pretty fun to change the variables when I got the fade working.

## Hello_LCD

### Description & Code
Description goes here

Here's how you make code look like code:

```C++
Code goes here
```
Talk about how the code works, here....

### Evidence
link goes here

### Images
draw it yourself, take a picture, make a fritzing, whatever you want to EFFECTIVELY communicate how its put together.

### Reflection
## Button Blink

### Description & Code
```C++
int LED = 13;
int buttonState = 0;
int buttonPin = 7;
int delayVar = 1000;

// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin 13 as an output.
  pinMode(LED, OUTPUT);
  pinMode(buttonPin, INPUT);
  Serial.begin(9600); // This turns on my Serial Monitor
}





void loop() {
  buttonState = digitalRead(buttonPin);
  Serial.print("button State: ");
  Serial.print(buttonState);

  if (buttonState == HIGH) {
    blink(delayVar);
    Serial.print("\t delayVar:");
    Serial.println(delayVar);
    if (delayVar > 100)
      delayVar = delayVar - 100;
  }
  else
  {
    digitalWrite(LED, LOW);            // turn the LED off by making the voltage LOW
    delayVar = 1000;
    Serial.println("\t no blink!");

  }
}





void blink(int x) {
  digitalWrite(LED, HIGH);           // turn the LED on (HIGH is the voltage level)
  delay(x);                       // wait for a second
  digitalWrite(LED, LOW);            // turn the LED off by making the voltage LOW
  delay(x);                       // wait for a second
}

```


### Evidence
https://create.arduino.cc/editor/apleasa54/47fc136c-a371-4761-ba64-bd9baa5f4e1f/preview
### Images
<img src="https://github.com/apleasa54/NotSoBasicArduino-1/blob/main/Screenshot%202020-12-08%20at%2017.14.35.png?raw=true" width="400">

### Reflection
This Assignment was pretty hard for me, But I definitely learned a lot and got a better understanding of if/than statements.
