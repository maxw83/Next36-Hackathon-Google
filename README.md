Next36 Hackathon @ Google
======================

A product to facilitate driver-to-driver communication via a Myo gesture control device and a MeU LED display panel. This project was made for the 2014 Next36 Wearable Tech Hackathon @ Google Canada. Our team (Axiom) finished 3rd place.

Team: @julytn, @maxw83, @bazhunga, Ken Liao, Wenyi Yin

Link to Hackathon: http://www.thenext36.ca/news/they-came-they-hacked-they-conquered-the-next-36-wearable-tech-hackathon-in-review
>"Axiom, finishing in 3rd place, kept up with the theme of safe, integrated environments. By leveraging the MeU LED displays and the Myo’s gesture control technology, their goal was to create a new method of light-hearted communication for drivers. For instance, a driver wearing the Myo may become frustrated when another driver cuts him off at an intersection and he’ll clench his fists, causing an angry face to appear on the MeU. Conversely, the same driver might be given space to change into the right hand lane at the following intersection and create another gesture to display a happy face."

High level description of each file:

* AC.lua: Lua script that takes input from the Myo armband and outputs the resulting gesture as a simulated keystroke. The                 'keystroke' serves as input to PC_keypress_Serial_COM.

* PC_keypress__Serial_COM.pde: Processing script that waits for a keystroke and relays the signal to the MeU LED panel via a USB 
                              cable.

* MeU Serial COM.ino: Arduino script that is loaded onto the MeU device. This script recognizes input from the processing script   and displays a preprogrammed image on the LED array. 
