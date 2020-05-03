SNES 1Chip Audio DAC replacement
--------------------------------

### Purpose

This board design is suited to replace the 1Chip-SNES audio DAC, which is labeled by U6.  
This board **does not** fixes dead S-MIX, which is U10.

At the moment I don't know whether the boards fits (mechanically) into a SNES model 2 (small form factor SNES)

### Installation

- assemble the board (BOM on bottom silk screen and listed below)
- remove U6
- if you are going to recap your system, you can remove C15 and leave the footprint of C15 unpopulated  
  (it does not hurt to left C15 in place)
- connect the board to the footprint of U6. Check up for adjacent shorts afterwards.  
  (the board do not have to be isolated from bottom as it's a single layer design)
- check for connections at U6:
  - p1: R48 (bottom side mainboard) (audio out right)
  - p2: C15 + (and Vcc through board design)
  - p3: GND
  - p4: R51 (bottom side of mainboard) (audio out left)
  - p5: U2 pin 94 (LRCK)
  - p6: U2 pin 93 (DATA)
  - p7: U2 pin 92 (SCLK)
  - p8: Vcc (+5V)
- connect pad labeld by _U2:52_ with U2 pin 52 (also extension port pin 21)


### BOM

- U1: CS4338-KSZ (SOIC-8 package)
- C1: 0.1uF / 25V+ (SMD 0603 package)
- C2: 1uF /25V+ (SMD 0603 package)

### PCB

Get your PCB from OSHPark or anywhere you like.  
To smoothen the installation, choose a substrate thickness as thin as possible.

## ENJOY!!!