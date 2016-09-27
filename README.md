# About
This is a modified library for the Seeed Studio's [Rainbowduino v3.0] (http://wiki.seeedstudio.com/wiki/Rainbowduino_v3.0) board.

The change is to allow for nested interrupts during the horrendously long Timer Interrupt routine, which updates display lines. This will allow for UART interrupts to run, so no serial data should be lost anymore.