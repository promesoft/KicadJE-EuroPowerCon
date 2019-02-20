# KicadEuroPowerCon
Powerplane for Eurorack Doepfer connectors

## Status - Rev B board in prototest - no issues
| Stage/Test  | Status |
| ------------- | ------------- |
| create material  | sch/pcb/gerber produced and uploaded  |
| production  | ordered/produced/delivered  |
| Initial Inspection | Visual-OK Mounting-OK |
| Initial Technical Test | +-20V in +9V in  
| | +/-12v out +5V out 
| | LED's working|
| Initial Product Test | Powercon burn in ok with 10pin VCF |
|  | Powercon 16pin - Not tested|
| Long Term Product Test | ongoing |

### Errata

### Issues and Notes
 * fuse holder for +5V should be changed
 * virtual GND should be powered behind fuse
 
## Physical Construction
100x100mm
Optional cut in 2 where the top part can be used as a normal regulator board.

## Features
+/- 12V Supply
 - Requires +-14,5v to +-27v. Input can be either linear transformer with/without bridge rectifier, or switched mode. 
 - Max 1,5A will require additional cooling of the regulators and larger diodes.
 - Optional disable regulation
 - Optional synthetic GND if only single ended supply is available.
 
+5V Supply
 - Requires 7-25V input either as linear transformer with/without bridge rectifier, or switched mode PSU.
 - Optional input from +15V thru supply 
 - Max 1,5A will require additional cooling of the regulators and larger diodes.
 - Optional disable regulation

Thru
 - Both 7V and +-15 input sections can be sent thru to a second module for daisy chaining of modules.

Reg out
 - Regulated outputs can be send out to other power distribution modules or directly to Synth modules that does not require the Doepfer 10pin or 16pin power input.
 
## Board Layout
- Top - Power in
- Top Right - Regulated power out
- Bottom - Doepfer Powercon

# Electrical Construction
Intended function

## Schematic
![](KicadEuropowerSchematic_RevB.png)
## 3D
![](KicadEuropower3D-RevB-Top1.png)
![](KicadEuropower3D-RevB-Bottom1.png)
