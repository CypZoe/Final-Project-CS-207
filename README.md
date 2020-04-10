# Final-Project-CS-207-LED-Pixel-Star
This is project involves using sewable hardware to sew LEDs onto a piece of woven fabric in the shape of a star. These LEDs are daisy chained together and sewn to a Gemma V2 microcomputer. The colour of the LED string changes depending on the amount of light detected in the environment by a photoresistor. A pushbutton can be used to cycle through colours independent of the presence of light in the environment.

<img src="img/IMG_20200409_170133.jpg" width = "500">
<img src="img/IMG_20200409_170221.jpg" width = "500">

# Repository Content
/src - location of software
/hardware - location of the fritzing files for the breadboard and schematic of this circuit
/build - locations of files that are compiled and ready to run
/libraries - the location of the link to the required library
/examples - Example files from Arduino IDE that will run on the harware
/img - location of files used
/README.md - the file you are currently reading

# Requirements and Materials

Libraries needed
- Adafruit_NeoPixel.h (https://learn.adafruit.com/adafruit-neopixel-uberguide/arduino-library-installation)

Materials Used
- 10 x Adafruit FLORA Neopixel
- 1 x photoresistor
- 1 x pushbutton
- 1 x Gemma V2 microcomputer
- 1 x 3 ply conductive thread spool (18 meters)
- 1 x embroider hoop
- 1 x USB cable - A/MicroB - 3ft
- 1 x pack of sewing needles
- 1 x alligator clips

# Build Instructions

The Adafruit FLORA Neopixel should be positioned roughly one inch apart on a piece of woven fabric which has been placed in an embroidery hoop. They should then be sewn together in a daisy chained with the data line out of one neopixel being sewn to the data line in of the next neopixel in the circuit. The first neopixel in the circuit is sewn to the Gemma V2 microcomputer with the data line in being sewn to pin D1. The ground on the microcomputer is then sewn in a continuos manner through each neopixels ground which is indicated by a subtraction sign. The same process is repeated with the voltage out of the microcomputer being sewn through each of teh voltage in holes of the neopixels which is denoted by a plus sign. The photoresistor is then sewn to the A1 pin and ground of the microcontroller. Finally the pushbutton is attached, via a wire that has been striped at both ends, to the D0 pin of the microcontroller and the parrallel leg is hooked under the conductive thread that was previously sewn to ground.

<img src="Hardware/Light-Activated Pixel Star Schematic.jpg" width = "500">

<img src="Hardware/Light-Activated Pixel Star breadboard.jpg" width = "500">

# Usage

To use this circuit you first need to upload the code. After this you can manipulate the amount of light hitting the photoresistor, this will change the colour of the neopixel string. To cycle through different colours independent of the amount of light present in the environment, hold down the pushbutton.

# Team
This project was done individually and as such I, Cypriana, was the only contributor.

# Credits
- Becky Stern - The creator of the circuit used as a template for this project
- Phillip Burgess - The writter of the code used in the project used as a template for this project
