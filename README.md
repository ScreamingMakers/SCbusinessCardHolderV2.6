# SCbusinessCardHolderV2.6
V2.6 of the Screaming Circuits open source, hackable, electronic business card holder 

The Screaming Circuits business card holder is a multi-function device intended for your amusement and as a demonstration of our workmanship.

It has 19 LEDs along the bottom of the board, with 16 being broken out to optional headers - for your hacking pleasure. Along the top, it uses the two user buttons, and the I2C/SPI and ICSP headrs to hold the business cards.

V2.6 also has all eight bits of ports A and C brought out to .1" headers. Port bits D5/An25, D6/TX, D7/RX, B0/A12, and B3/CCP2 are brought out to a separate header.

Note that this kit uses a pair of CR1220 coin cell batteries. The silk screen erronously calls for CR2032 batteries. Oops. My bad.
Mechanical build instructions:

After soldering in the I2C and ICSP pin headers, attaching the rubber feet, and inserting the batteries, it’s ready to go. Place it on your desk and put about ten business cards in. When someone takes a card (or if you pound on your keyboard hard enough) some of the LEDs will flash.

If you tip it up, so that the LEDs run along the bottom, it will act as a spirit level, and as a short ruler. It’s not angle calibrated. Doing so is up to you.

The microcontroller fitted is of the Microchip PIC18F46K22 family. This run of V2.6 was produced with a PIC18F46K22. V2.5 had uses CR2032 batteries and came with the PIC18F43K22 – the same MCU, but with less FLASH and SRAM. The accelerometer is a Freescale MMA8452Q. The schematic and layout were created with EagleCAD. The code was written and compiled with Microchip XC8 in Mplab-X.

One of the pin headers is connected to the I2C and SPI bus pins on the MCU. The other is connected to the Microchip ICSP (in circuit serial programming) pins on the MCU. Button Usr 1 is connected to I/O pin RB4, and Usr 2 is connected to RB5.
