# Deafblind Communication Device

## Setting Up

You need a Raspberry Pi, 6 motors, 8 buttons, breadboards (depending on the setup and their sizes), a LED matrix, and an appropriate number of transistors and wires. As far as the wiring goes, we used the  WiringPi library (together with [this diagram](https://raw.githubusercontent.com/ppelleti/hs-wiringPi/master/pin-diagram.png)). Wire it up as you see fit and according to your setup.

For the physical design of the device, we encourage everyone to be as creative as possible. Our own contraption is eco-friendly, built with a recycled box, an egg carton for the motors, strepsils caps to cover the motors, blue tack, hot glue, tape etc. because it was just a prototype.

<img src = "/images/1.jpg">
<img src = "/images/2.jpg">
Also, do not forget to connect the Raspberry Pi to a screen with the appropriate wires. ;)

## Prerequisites

Generally, the Raspberry Pi comes with WiringPi. If not, make sure to get it. You can check that by typing in a terminal

```
$ gpio - v
```

If something shows up it means it is installed.

## Project Specification

In order to run it, you need to run [translate](translate) from the terminal.

The user will be prompted to a menu, where they can choose whice mode of translation they want to use.
- Text to Braille:
  - They can choose the time each character will be displayed for (eg. 1.5s)
  - They can choose to read from a text file or directly from the terminal

- Braille to Text:
  - Use the BrailleBoard to type what character the user  wants, no matter which order the buttons are pressed
  - After each character the user has to press ENTER
  - In order to type numbers the DIGIT  character has to be typed in first (see below)
  - To finish a message, type in the EXIT character

<img src = "/images/3.jpg">

### Goals

- providing the deafblind community with a cheaper alternative to the current communication devices.
- addressing a real-life need which tests out the practicality of a Raspberry Pi

### Features

- 6 motors used to provide a tactile translation into Braille
- an LED matrix to also show the output in Braille (for testing purposes and in order to be able to build up on it in the future)
- a "BrailleBoard" which allows the user to type directly in Braille, also coming with a button for SHIFT and another button for ENTER

## Authors

- [Bianca Teodora Catea](https://github.com/BiancaTC/)
- [Ioana-Adelina Filip](https://github.com/AdelinaFilip/)
- [Lazar Lukic](https://github.com/ll8618/)
- [Roko Parac](https://github.com/rparac/)
