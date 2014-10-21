Next36-Hackathon-Google
======================

A product to facilitate driver-to-driver communication via a Myo gesture control device and a MeU LED display panel. This project was made for the 2014 Next36 Wearable Tech Hackathon @ Google Canada. Our team (Axiom) finished 3rd place.

Team: @julytn, @maxw83, @bazhunga, Ken Liao, Wenyi Yin

Link to Hackathon: http://www.thenext36.ca/news/they-came-they-hacked-they-conquered-the-next-36-wearable-tech-hackathon-in-review

High level description of each file:

*AC.lua: Lua script that takes input from the Myo armband and outputs the resulting gesture as a simulated keystroke. The                 'keystroke' serves as input to PC_keypress_Serial_COM.

*PC_keypress__Serial_COM.pde: Processing script that waits for a keystroke and relays the signal to the MeU LED panel via a USB 
                              cable.

*MeU Serial COM.ino: Arduino script that is loaded onto the MeU device. This script recognizes input from the processing script   and displays a preprogrammed image on the LED array. 
