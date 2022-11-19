# Marlin-Ender 3 Max

Note: these are just the configuration files. You need the rest of the code at https://marlinfw.org/

These configuration files have the following enabled for the Ender 3 Max.

- A filament sensor with advanced pause
- m600 change filament script
- Mesh Bed leveling with a 9 probe grid
- Bed Tramming
- Individually move axises
- TMC2208_Standalone Drivers for X and Y axises
- A4988 Stepper drivers for Extruder and Z axis
- Presets for PLA, PETG, and ABS

ABS: 240 hotend, 110 Bed
PETG: 220 Hotend, 85 Bed
PLA: 195 Hotend, 60 Bed

If you want to automatically turn your printer off after a print

- Bed size is increased on y axis by 10 mm

Insert the following lines into your slicer: 

G1 X0 Y210 F1000 ; Move Heat Bed to the front for easy print removal

M109 R40; Wait for the hotend to cool down to 40C

G1 X0 Y310 F1000; Move bed back to turn off printer

Full tutorial available here: https://www.thingiverse.com/thing:3744808
