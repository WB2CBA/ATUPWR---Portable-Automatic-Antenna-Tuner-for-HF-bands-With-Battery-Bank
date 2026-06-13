ATUPWR – ATU and Power Bank for Field Portable Operations
---------------------------------------------------------

<img width="1512" height="1204" alt="IMG_3319" src="https://github.com/user-attachments/assets/7e61053b-f030-4129-b74e-d435c4151126" />

ATUPWR is a Power bank and Automatic Antenna tuner combo for QRP Portable operations.

ATUPWR unit consists of 3 pcb boards,

-	Powerbank PCB,

-	Automatic Antenna Tuner PCB,


-	 Control Interface and Display PCB,

POWER BANK PCB:
---------------

Power bank max output voltage is 12.6V fully charged. Power bank utilizes 3 x 18650 Li-ion 

batteries and a 3S 20A BMS(Battery Management System) module. This module can monitor 

battery Overvoltage/Undervoltage, also charging balancing. 

Here is Power bank board layout:

<img width="1511" height="1549" alt="IMG_3324" src="https://github.com/user-attachments/assets/ae343489-8a49-4a52-b02e-91864f456ae2" />
<img width="1392" height="1465" alt="IMG_3323" src="https://github.com/user-attachments/assets/8e3114cb-290d-4b0b-a69a-fdb421a72a84" />
Power Bank PCB has a 5.5x2.1 DC Barrel Plug female adapter. This plug can be utilized to power 
any 12V QRP transceiver. 

Also this Barrel connector plug can be used for charging using a 12.6 Charging adapter.

This wall charging adapter is used for charging which puts out constant current 12.6V:

https://a.co/d/0at9GylA

These chargers are common and cheap so no charger facilitated in the pcb design.

Automatic Antenna Tuner PCB:
----------------------------

Automatic Antenna Tuner PCB is N7DDC David Finitsky’s ATU 100 7x7 Automatic Antenna Tuner 

adapted and modified to work as a 20W max QRP ATU.  Operation of ATU is identical to ATU 100.

For more details on ATU100 and its operation please refer to this link:

https://github.com/Dfinitski/N7DDC-ATU-100-mini-and-extended-boards

<img width="1512" height="2016" alt="IMG_3321" src="https://github.com/user-attachments/assets/32cb2a03-78c9-42ad-9502-9c065a1b9f20" />

ATU BOARD JUMPER SETTINGS:
--------------------------

<img width="1076" height="766" alt="607506815-ad0cdc8a-0003-4ff4-b53a-17f0f3dfb46a" src="https://github.com/user-attachments/assets/5000f64d-2e76-4760-a10c-8448bcb0458b" />

ATU BN43-202 Binocular Coil:
----------------------------

(Note that BN43-1502 used in examples below though same applies to BN43-202 binocular)

All Toroids and Binocular coil can be wound using AWG24/0.35mm magnet wire.

Winding and installing the binocular toroid:

To wind the BN43-202 inductor core start at one side of the core and feed the enamel 

copper wire 5 times through the hole. Every time the enamel copper wire goes through the 

hole counts as one turn.

After completing 5 turns in the first hole now start from the second hole on the opposite 

side of binocular core at the second hole. When winding the toroid, try and keep the wire as 

close as practical to the toroid. When you finish it should look like the example in the photo below:

<img width="476" height="182" alt="binocular1" src="https://github.com/user-attachments/assets/3544b3e3-0624-49e5-a180-79efe6627911" />

NOTE: the entry and exit points of the wires (below and above) on each side of the binocular toroid.

Wind your binocular toroid in the same manner. Ensure that the windings do not overlap and are evenly spaced.

Remove the enamel coating from the wires by either sanding or scraping with a sharp 

modeling knife and tin the wires with solder as shown below:

<img width="447" height="200" alt="binocular2" src="https://github.com/user-attachments/assets/3cbef20c-0ad1-485a-85c4-5caa5ad30974" />

Next cut two 1.5” (~35mm) insulated electrical wire. These two wires will be fed through the 

holes of  binocular core (white wires in the photo), and soldered to the PCB as shown in the 

photographs below:
<img width="776" height="200" alt="binocular3" src="https://github.com/user-attachments/assets/fa3da4e6-7719-49ef-8e8e-4b855a517a38" />

Adjust the length of these insulated through wires as needed before soldering – take your 

time to ensure a neat and uniform installation.

Winding ATU Toroids:
--------------------
For ATU Toroids AWG24/0.35mm Magnet wire can be used.

There are altogether 7 toroids to wind.

These are:

- 3 x T37-6 type

- 2 x T37-2 Type

- 2 x T50-2 type

Winding Turns for these Toroids are listed below:

L1 - T37-6  4 Turns

L2 - T37-6  6 Turns

L3 - T37-6  9 Turns

L4 - T37-2  11 Turns

L5 - T37-2  16 Turns

L6 - T50-2  21 Turns

L7 - T50-2  30 Turns


Interface and Display PCB:
--------------------------

<img width="2016" height="998" alt="IMG_3327" src="https://github.com/user-attachments/assets/14867a08-75a2-4c6b-bfcc-8a01b475021a" />

Interface and display pcb has couple of functions. It has control switches to control ATU

functions, has also an 0.92” OLED Display for displaying TX power, antenna power, SWR and 

Power/SWR efficiency. Also displays L and C values of tune.

Interface and display pcb has also a four LED battery level indicator. Battery levels are indicated 

as 100% with a green LED, 75% with a green LED, 50% with a yellow LED and 25% with a red 

LED. When battery discharge is below 25% red LED flashes warning that a battery charge is imminent.

There is also a slide switch which turn on and off ATU+ interface display board. Power bank is 

always on and does not consume any battery if not used.  

-	ATU main board and interface display board has two PIC micro controllers.

-	ATU utilizes a PIC16F1938 micro controller and Battery Level display utilizes a PIC12F675 micro controller. 

These microcontrollers can be programmed using PICKIT3,PICKIT4 or PICKIT5 microchip 

programming adapters using posted .hex files in this github files section.

These programmers are common in online shopping sites like amazon.com

OLED DISPLAY BOARD JUMPER SETTING:
----------------------------------
<img width="2016" height="888" alt="OLED JUMPERS" src="https://github.com/user-attachments/assets/95e6238c-4770-4047-b0cb-17d5bfea8198"> 
  


Here are some photos that will help for your build:

<img width="2558" height="1080" alt="IMG_3325" src="https://github.com/user-attachments/assets/e70defb4-4260-4da2-b101-8cb9a742a318" />
Sideview of stacked boards.

<img width="1511" height="1490" alt="IMG_3322" src="https://github.com/user-attachments/assets/3d6c230f-dfb8-481a-990b-fa46fa7515d5" />
90-degree 2.54 pitch male header is used to connect display interface to ATU as shown.

<img width="1403" height="1008" alt="IMG_3328" src="https://github.com/user-attachments/assets/b24811b4-c39b-4e8e-89af-b81516ee6fba" />
<img width="1411" height="1207" alt="IMG_3329" src="https://github.com/user-attachments/assets/db4ab3d4-f240-44b6-aa7c-e41d956d2bc2" />

For SMD part soldering I designed boards to be manufactured by JLCPCB of China. This makes 

life easy as these boards arrive pre-soldered of all smd parts. 

Here is the link for JLCPCB:

https://jlcpcb.com/

Through Hole Part BOM List:
---------------------------

-	1 x OLED Display:  https://a.co/d/00k2FKqb

-	2 x BNC PCB Type connector: https://a.co/d/00Qw3aV2

-	1 x BMS Module: https://a.co/d/09KkfIuF

-	1 x 3-18650 Battery Holder: https://a.co/d/0ct3JXyp

-	2 x Green 3mm LED

-	1 x Yellow 3mm LED

-	1 x Red 3mm LED

-	3 x T37-6 Toroid,  2 x T37-2 Toroid, 2 x T50-2 toroid, 1 x BN43-202 binocular core from: 

https://kitsandparts.com/

-	1 x 28 pin skinny DIP IC socket: https://a.co/d/0bKs36lj

-	1 x 8 pin DIP IC socket: https://a.co/d/08990Qoa

-	PIC16F1938 Microcontroller : 

https://www.digikey.com/en/products/detail/microchip-technology/PIC16F1938-I-SP/2258599

-	PIC12F675 Microcontroller: 

https://www.digikey.com/en/products/detail/microchip-technology/PIC12F675-I-P/459171

-	17 mm male 2.54 mm pitch pin header : https://a.co/d/0cHgaR7P

This pin header is used on battery board for stacking ATU board to Power bank board.

-	2.54 mm pitch female header: https://a.co/d/06al5QaQ

             This female header is used on ATU board for stacking ATU board to Power bank Board.

-	3 x 6mm x 6mm x 12mm Tactile switch : https://a.co/d/00haVKzx

-	Slide Switch: https://a.co/d/0hbDwx5R

-	DC Barrel Connector PCB type : https://a.co/d/0g5969O2

-	90-degree 2.54 mm pitch male header: https://a.co/d/0j8ei4eA

  This header is used for attaching ATU to Display Board
  

ACKNOWLEDGEMENT:
----------------

I would like to thank David Finitsky, N7DDC for his brilliant ATU100 Automatic Antenna Tuner.


Barb WB2CBA - 06/2026















