# Final-Project-CS-207-LED-Pixel-Star
This project involves using sewable hardware to build a light activated pixel star. In this project LEDs are sewn onto the front side of a square of woven fabric in the shape of a star. These LEDs are daisy chained together and sewn then to a digital pin on the Gemma V2 microntroller. The colour of the LED string changes depending on the amount of light detected in the environment by a photoresistor. A pushbutton can, also, be used to cycle through colours independent of the presence of light in the environment.

<img src="img/IMG_20200409_170133.jpg" width = "500">
<img src="img/IMG_20200409_170221.jpg" width = "500">

# Repository Content
/src - location of software
/hardware - location of the fritzing files for the breadboard and schematic of this circuit
/build - locations of files that are compiled and ready to run
/libraries - the location of the link to the required library
/examples - Example files from Arduino IDE that will run on the harware of this project
/img - location of pictures of the circuit
/README.md - the file you are currently reading

# Requirements and Materials

Libraries needed
- Adafruit_NeoPixel.h (https://learn.adafruit.com/adafruit-neopixel-uberguide/arduino-library-installation)

Materials Needed
- 10 x Adafruit FLORA Neopixel LED's
- 1 x photoresistor
- 1 x pushbutton
- 1 x Gemma V2 microcontroller
- 1 x 3 ply conductive thread spool (18 meters)
- 1 x embroider hoop
- 1 x USB cable - A/MicroB - 3ft
- 1 x pack of sewing needles
- 1 x pack of alligator clips
- 1 x wire
- 1 x fabric chalk

# Build Instructions

The first step of this project is to position the LED's in the shape of a star, while the fabric is held tight in an embroidery hoop. Following this, mark the location of each LED with fabric chalk. These LED's should be positioned roughly one inch, or more, apart. They should then be sewn onto the fabric linking each data line out of one LED to the data line in of the next LED. After the data in and out of two LED's has been sewn together a knot should be tied, at each loose end, and clear nail polish should be painted over each knot. This process should be repeated until all the LED's have been daisy chained together in the shape of a star. The digital pin D1 on the Gemma V2 microcontroller should then be sewn to the data line in of the first LED. Following this the ground pin of the Gemma should be sewn in a continuos manner to ground pin of each LED. The ground pins of the Adafruit FLORA neopixel LED's are donated by a plus sign. This process should then be repeated with the voltage out pin being sewn to in a continuos manner to each voltage pin, denoted by a subtraction sign, of the LEDs.

The next step of building this circuit is to attach the photoresistor to the front of the fabric. To do this twist the both legs of the photoresistor into a spiral, leaving roughlt one and half centimeters of the photoresistor legs strait. The straight portion of the photoresistor legs should then be painted over with clear nailpolish. Following this sew one leg to the A1 pin of the Gemma V2 microcontroller and the other to the ground pin of the Gemma.

The last step of the build is to attach the pushbutton. This requires a wire which has haad its tubing stripped at both ends. One end of the stripped wire is then wrapped arround pin D0 of the Gemma V2 microcontroller and the other end is wrapped around on of the pushbutton legs.

<img src="Hardware/Light-Activated Pixel Star Schematic.jpg" width = "500">

<img src="Hardware/Light-Activate Pixel Star breadboard.jpg" width = "500">

# Usage

To use this circuit the first step is to upload the code. After this you can manipulate the amount of light hitting the photoresistor by covering the photoresitor with an object or by using a dimmer light switch, this will change the colour of the neopixel string. To cycle through six different colours independent of the amount of light present in the environment, hold down the pushbutton.

# Team
This project was done individually and as such I, Cypriana, was the only contributor.

# Credits
- Becky Stern - The creator of the circuit used as a template for this project
- Phillip Burgess - The writter of the code used in the project used as a template for this project
