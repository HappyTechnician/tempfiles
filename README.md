The board layout and schematic rpresentation are for my 3D printer enclosure. I share this with no warrenty of and kind.
The Raspberry Pi Pinout is representative of the 40 pin layout for the Raspberry Pi family. The mount holes are representative of the Pi Zero and the full size pi boards.
 The power supply input should be connected to 24 VDC PSU able to carry the extra currend of 2 ampers required to drive full current throught the MOSfet drivers on this board.
 connection pinout:
 J2-1: 12VDC driven from GPIO23.  J2-2: Supply ground.  J2-3 direct connected to GPIO17 for Tachometer(Fan)
 J3-1: 12VDC driven from GPIO24.  J3-2: Supply ground.  J3-3 direct connected to GPIO27 for Programable RGB
 J4-1: 12VDC dirven from GPIO25.  J4-2: Supply ground.  J4-3 direct connected to GPIO22 for accesory needs.
 J5-1: 12VDC driven from GPIO8.   J5-2: Supply Ground.  J5-3 Direct connected to GPIO5 for accessory needs
***   WARNING   ****   CONNECTING PIN 3 OF ANY OUTPUT TO A 12 VOLT SORCE WILL KILL YOUR MCU ******

THIS BOARD WAS CREATED WITH THE IDEA OF CONSOLIDATING BUCK SUPPLIES AND MOSFET DRIVERES INTO ONE BOARD TO POWER AND PROVIDE PWM SOURCE FOR AN ENCLOSURE.  You may use it for any purpose you may need with a Raspberry Pi board, 40 pin header.
