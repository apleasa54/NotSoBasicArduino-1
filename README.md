# NotSoBasicArduino
 The follwing files are my second foray into Arduino
 
 
## Table of Contents
* [Table of Contents](#TableOfContents)
* [LED_Fade](#LED_Fade)
* [Hello_LCD](#Hello_LCD)
* [FillMeInLAter](#FillMeInLAter)
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

