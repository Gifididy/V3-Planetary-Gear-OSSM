# V3-Planetary-Gear-OSSM
My take on an OSSM variant using a planetary gear set to increase torque while still using the core hardware of the original OSSM. An easy fix for if the OSSM does not have enough torque/force for you. 

Note on some of the printer settings I use.

Nozzle: .6mm

Layer height: .3mm

Wall, top & bottom thickness: 1.2mm

Infill: 30%

Some support is needed for the planet carrier and the top motor mount that has the planet carrier bearing screw. Depending on your settings, you may be able to not use any support material at all. 

Should use less than a spool of filament. I've been using PLA for reference. 

## Hardware

Hex cap metric screws

3 x M3x12 - Endstops

7 x M3x8 - Rack

1 x M4x8 - Set screw for spindle gear 

10 x M4x16 - Used for connecting motor mount & 2 pin mount to the top bracket

6 x M4x12 - For mounting to a plywood base. May need to be longer depending on the mounting method. I used m4 threaded inserts for wood. 

10 x M4x8 - Linear rail & Rack

4 x M5x16 - Gear bearing screws

4 x M5x25 - Motor mount bolts

5x M4x5.5mm wide threaded inserts - Set into top bracket and spindle gear set screw. 

10 x M3 nuts

6 x M4 nuts

4 x M5 nuts

------

2 x 8mm dowels - Each 85mm or longer.

4x 685ZZ Bearings - Same ones OSSM uses.

1 x MGN12H Linear rail - Same style OSSM uses. I'm using a 400mm one currently.

180W servo - Recommended OSSM one.
.=
OSSM control board and remote - Will need to modify software. Just a couple values need to be changed.

Appropriate power supply.

## Changes to code

In utilities.cpp

Line 502 & 533 changed to 200. (Increased homing speed)

Line 503 & 534 changed to -2000 & 2000 respectively. (I have not figured out how to change the distance a mm is)

Line 481 value changed to 2.

In pattern.h I disabled line 850 and 851 because those sucked to accidently switch to. 




