# Bolt-Industries
![image](https://user-images.githubusercontent.com/58665565/154830776-ed1128a7-f4ef-473b-8738-91d0eeef3ae1.png)

Welcome to the Bolt Industries Github Repo.

Here you will find firmware for the Pico 87 Mechanical Keyboard, as well as the open source hardware. 

If you would like to get your hands on a Pico 87 Mechanical keyboard, you can find the kit in the Bolt Industries store: 
www.boltind.com


Hardware:

In the hardware folders, you will find the schematic and PCB's in .PDF form as well as .JSON that can be imported into Easy EDA so that you can modify them to your liking.

BMK firmware
Bolt (Industries) Mechanical Keyboard

The Pico 87 Mechanical keyboard is compatable with two flavors of firmware. The first is BMK. BMK stands for Bolt Industries Mechanical Keyboard. It is a custom built firmware written in the Arduino IDE. If you are comfortable using the Arduino IDE, then You will probably like BMK. Changing the function of a key is as easy as changing a line of code in the sketch. BMK uses the keyboard.h library to doall the keyboard functions. For more information about what you can do with the Keyboard.h library, visit the arduino referande page here: https://www.arduino.cc/reference/en/language/functions/usb/keyboard/ To install it, simply download the sketch called BMK.ino and follow the directions in the sketch.


KMK firmware

KMK is a mechanical keyboard firmware that runs on circuit python. 
Installing KMK is a little more involved.
1. Download and flash circuit python to your Pico. https://circuitpython.org/board/raspberry_pi_pico/
2. Download and unzip the KMK firmware from the KMK repo. https://github.com/KMKfw/kmk_firmware
3. Plug in your keyboard without holding down the bootsel button, and a drive called circuit python should appear. 
4. Copy boot.py from the KMK firmware, and code.py from this repository onto your circuit python drive (your pico.) 
5. Your keyboard should immidatly start working!

Note that this is the first time Ive ever done anything with Python. The main.py file works like a perfectly functioning keyboard, but I'm sure it can be done better. If you feel inclined to make any improvements, please don't hesitate to submit a pull request or email me your code and I'll commit it to the main repo. 

Matrix tester: 
This is a neat Python program to test the key matrix after you get everything soldered, as well as a nice set of assembly instructions. It was written by 
Pierre Constantineau, one of the project's backers. The tester program just lights up the LED between F1 and F2 when a key is pressed. It's a really simple way to test your soldering. You can find it on Pierre's Repo here: https://github.com/jpconstantineau/pico-87-keyboard


![image](https://user-images.githubusercontent.com/58665565/154625246-d543506a-e4ff-4449-9799-5506421c1dbc.png)
