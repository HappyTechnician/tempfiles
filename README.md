The board layout and schematic rpresentation are for my 3D printer enclosure. I share this with no warrenty of and kind.

The Raspberry Pi Pinout is representative of the 40 pin layout for the Raspberry Pi family. 

The mount holes are representative of the Pi Zero and the full size pi 4 boards.

	
	The power supply input should be connected to 24 VDC PSU able to carry the extra current of 2 ampers required to drive full current throught the MOSfet drivers on this board.
 
	
	CONNECTION PINOUT:
The Pi Hat Driver Modual_54302 has been designed primarily as a 3D printer Enclosure controller using the 24VDC power supply as the input voltage at the 2 wire terminal block. With a Raspberry Pi as a host Micro-Computer/System Controller operaKng Klipper as the ApplicaKon Package Interfaced with the 3D printer control board.
The Klipper API allows the ability, through the ‘printer.cfg’ file, to use the GPIO pins from the Raspberry Pi to communicate with the MCU through UART, and to collect data from sensors through I2C. Also the use of output PWM signal to operate fans, lights, heaters, and relays. This modual uses the Texas Instruments TPS54302 DC-DC switching step down converter. To supply 12 VDC @3 Amps of current capacity to drive the peripheral devices. A TLP290-4 quad opto-isolator is used to isolate the GPIO pins from the output drive circuitry. AD4184 MosFets are used to ‘push’ the GPIO signal into a 12VDC connector.
2 connectors have PWM output only and 2 have a third pin for fan tachometer or a feedback sensor input direct to the GPIO header
The pinout order is as follows:
Header connecKon:
Pins 1,3,5,7,9,11,13,15,17,19 are to the inside of the header connector, and pins 2,4,6,8,10,12,1,4,16,18,20 are to the outside of the header connector. Pin designaKons are as follows: header pi / GPIO pin
1 = 3.3VDC (I2c power) connected directly to I2C connector
2 = 5VDC connected directly to pin 1 of UART connector
3 = GPIO 2 (SDA-I2C) connected directly to pin 2 of I2C connector
4 = 5VDC connected directly to header pin 2
5 = GPIO 3 (SCL-I2C) connected directly to pin 3 of I2C connector
6 = GPIO-GROUND connected directly to pin 2 of UART connector
7 = GPIO 4 NOT CONNECTED = may be used for extra connecKons out of board.
8 = GPIO 14 (TX-UART) connected directly to pin 3 of UART connector
9 = GPIO-GROUND connected directly to pin 4 of I2C connector
10 = GPIO 15 (RX-UART) connected directly to pin 4 of UART connector
11 = GPIO 17 (PWM-J9) connected through isolator to J9-2
12 = GPIO 18 NOT CONNECTED = may be used for extra connecKons out of board.
13 = GPIO 27 (PWM-J8) connected through isolator to J8-2
14 = GPIO GROUND connected to ground for I2C UART Isolator
15= GPIO 22 (PWM-J7) connected through Isolator to J7-2
16 = GPIO 23 (TACH/SENS-J6) connected directly to J6-3 (CAUTION)
17=3.3VDC NOTCONNECTED=maybeusedforextraconnecKonsoutofboard.
18 = GPIO 24 (TACH/SENS-J7) connected directly to J7-3 (CAUTION)
19 = GPIO 10 (PWM-J6) connected through Isolator to J6-2
20 = GPIO GROUND connected to ground for I2C UART Isolator
***   WARNING   ****   CONNECTING PIN 3 OF ANY J6 OR J7  TO A 12 VOLT SORCE WILL KILL YOUR MCU ****** ABSOLUTLY

THIS BOARD WAS CREATED WITH THE IDEA OF CONSOLIDATING BUCK SUPPLIES AND MOSFET DRIVERES INTO ONE BOARD TO POWER AND PROVIDE PWM SOURCE FOR AN ENCLOSURE.  

You may use it for any purpose you may need with a Raspberry Pi board, 40 pin header.
