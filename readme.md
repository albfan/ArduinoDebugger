Overview:
  * This project will allow you to set a breakpoint in your sketch and step through it
  * Proper wiring to each device is supported and expected in some cases
  * Actual Arduino libraries such as Keypad.cpp are used wherever possible.
  
Supported Projects/Component:

|Project File|Components|Description|
|------------|----------|-----------|
|LEDSwitch.txt|LED, Momentary Depress Switch|LED goes on when switch is pressed|
|Resistor5VSwitch.txt|LED, Resistor, Momentary Depress Switch|LED goes on when switch is pressed|
|Blinky.txt|LED|LED goes on/off automatically|
|Digit3.txt|3 Digit 7 segment display, Momentary Depress Switch|7 segment display updates when momentary depress switch presed|
|Keypad.txt|4x4 matrix keypad|Serial output updates upon key press|
|KeypadDisplay.txt|4x4 matrix keypad, LCD Display|LCD display updates upon key press|
|LCDDisplay.txt|LCDDisplay, Momentary Depress Switch|LCD display updates when switch is pressed|
|SevenSeg.txt|7 segment display of single digit|7 segment digit increments upon switch press|
|RotaryDip.txt|Rotary Dip switch|Serial output updates when one of 3 rotary dip switches are changed|
|ShiftRegister.txt|74HC595 Shift Register, LED, Momentary Depress Switch|LEDs connected to shift register update when switch is pressed|
|Multiplexer.txt|4051 Multiplexer|When switch is depressed multiplexer chooses other input|

Free CPP Compiler:  
  The free cpp compiler that was used to build this project can be downloaded from
  http://sourceforge.net/projects/orwelldevcpp/ 

Build/Run instructions:
  * clone ArduinoDebugger
  * Compile and Run, Open a project
  * Rebuild All if the sketch.ino changes
  * Set breakpoints, Debug
  
Online videos that demonstrate usage:
  * [video1](http://www.youtube.com/watch?v=AdZ5GbDC1h0&feature=youtu.be)
  * [video2](http://www.youtube.com/watch?v=laa9VnRzuT0&feature=youtu.be)
  * [video3](http://www.youtube.com/watch?v=AdZ5GbDC1h0&feature=youtu.be)  
  * [3 Digit 7 segment display](http://youtu.be/_W_GPd936jg)
  * [Rotary Dip](http://www.youtube.com/watch?v=vOSc0lCG9bM&feature=youtu.be)
  
Last Tested 6/7/2013 on Windows OS:
  Windows 8
  
Last Tested with Arduino libraries from version
  1.0.2   
  
Questions/Comments
  paulware@hotmail.com
  
Help with projects
  [I can help with projects](http://fiverr.com/paulware/help-with-your-arduino-project)

[![I sell on Tindie](https://s3.amazonaws.com/tindie-static/badges/tindie-large.png)](https://tindie.com/shops/Paulware/?ref=offsite_badges&utm_source=sellers_Paulware&utm_medium=badges&utm_campaign=badge_large)

I have recently discovered [TDD](http://en.wikipedia.org/wiki/Test-driven_development) which dictates that all code changes be preceded by a test case enhancement.  While I don't have that many test-cases, I do have a suite of projects which are loaded and tested before every release.

Design Notes
* SimUtilities Class
  * Contains utilities to list all connections and set a value on the connection
* Pull-up Resistor
  * pinMode (pinNumber,INPUT);
  * digitalWrite (pinNumber,1); // Set pull-up resistor
  * Will have constValue.value = 1, and constValue.resistance = 20000
  
