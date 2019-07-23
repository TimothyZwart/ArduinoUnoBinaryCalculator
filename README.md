# ArduinoUnoBinaryCalculator
Arduino Binary Calculator with LCD screen

Makes Use of debounce method to allow for control with only two buttons.


## Requirements for Project
### Welcome / Splash Screen
■ You should have text greeting the user
■ Pressing button 1 or 2 individually has no effect on this screen.
■ You must press both buttons at the same time to go to the next screen.
### Byte 1 input
■ Should allow you to change 1 bit at a time with button 1 and use button 2
to move from bit to bit.
■ When you finish changing the lowest order bit (rightmost bit) and press
button 2 you will be brought to the Byte 2 input screen.
### Byte 2 input
■ Should allow you to change 1 bit at a time with button 1 and use button 2
to move from bit to bit.
■ Just as with with the Byte 1 screen moving from the last digit using button
2 should bring you to the solution screen.
### Solution Screen
■ Should have text at the top describing the screen function (solution)
■ Solution should be in Binary form!
■ Math should be correct
■ Output should allow for more than 1 byte so overflow is not lost
● Ex. 11111111 + 11111111 should = 1 1111 1110 (note extra bit)
■ Pressing button 1 or 2 individually has no effect on this screen.
■ You must press both buttons at the same time to go to the next screen.
### Contrast Screen
■ Screen should explain to the user how to adjust the contrast.
■ User should be able to adjust the contrast up and down (not just one
direction that loops around)
■ Pressing both buttons will leave the screen.
