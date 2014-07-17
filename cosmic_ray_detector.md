# Cosmic Ray Detector
## Overview
This project seeks to create an inexpensive cosmic ray detector capable of sensing rays greater than 1 GeV in energy. These can be used either as part of a timing synchronization solution, or as part of a large, distributed cosmic ray telescope.

![image](http://auger.physics.wisc.edu/images/crspectrum.gif "Cosmic Ray Spectrum")

***WARNING!***

***This project deals with high voltage. Make certain to use appropriate precautions. Do not cut any wires while all batteries are connected; remove and replace batteries while wearing nitrile gloves if using standard battery clips.*** Drawer-type battery holders do not necessitate the use of gloves.

### Circuit
![image](https://raw.githubusercontent.com/petmar0/RayCatcher/master/CRDetect.png "Detector Circuit")

In this circuit diagram, **R** is the sense resistor, usually about 1 kΩ, and **V** is the bias voltage. The bias voltage should be less than the turn-on voltage (usually either 95 or 65 VDC depending on the type of bulb being used), but should be high enough that a cosmic ray can trigger the circuit, causing a current to flow through the resistor. This is usually about 80-94 VDC, and can be supplied by a bank of 9-volt batteries, or a DC-DC converter that has a sufficiently large capacitor across it to absorb all transients.

## Construction
### Parts Needed
- 9-10 9-volt Batteries
- 9-10 9-volt Battery Holders
- Neon Bulb
- 1 kΩ Resistor
- BNC Female Connector
- 10 kΩ Trimpot
- Red Binding Post
- Black Binding Post

All of these can be found in the [Wish List](https://www.sparkfun.com/wish_lists/90984). Note that there are two options for battery holders. The less expensive one certainly works, but ***the more expensive one is safer***, as it allows separation of the battery mechanically with no shock risk.
### Tools Needed
- Soldering Iron
- Solder
- Wire Cutter
- Wire Stripper
- Tweezers
- Hot Glue Gun
- Hot Glue

### Assembly
1. Begin by clipping the end connectors off of the 9-volt battery holders.
2. Strip about 5-10 mm of insulation off of the end of each wire.
3. Twist the red (+) wire of one connector and the black (-) wire of another together.
4. Hold the joint in a pair of tweezers while soldering it together.
5. Repeat until all of the 9-volt connectors have been soldered in this fashion into a line.
6. Solder the 1 kΩ resistor across the two wires on the female BNC connector.
7. Glue over the 1 kΩ resistor on the bottom of the BNC connector.
8. Connect the ground (outer) wire from the BNC connector to the loose black (-) wire on the 9-volt connectors and solder it.
9. Connect the signal (inner) wire from the BNC connector to one of the two leads of the Neon bulb and solder it.
10. Connect the other lead of the Neon bulb to one of the two outer pins of the 10 kΩ trimpot and solder it.
11. Cut the other outer pin of the trimpot.
12. Attach the middle pin of the trimpot to the loose red (+) wire on the 9-volt connectors.
13. Connect the black (ground) lead from the battery connectors to the bottom of the black binding post and solder it.
14. Connect the red (+V) lead from the battery connectors to the bottom of the red binding post and solder it.
15. Put small globs of hot glue on each and every soldered connection.
16. Turn the trimpot all the way in the direction that is towards the remaining outside pin.
17. Connect the batteries to their connectors.

## Testing
### Tools Needed
- Oscilloscope, Arduino, Audio Recorder, or Other Output/Logging Device
- Smoke Detector or Propane Lamp Mantle as Radiation Source
- BNC-to-BNC or BNC-to-Dual Alligator Cable
- Nitrile Gloves

### Procedure
1. Connect the detector to the output or logging device using one of the above cables.
2. Allow for the unit to sit for a few hours with data being logged at as high of a sampling rate as possible.
3. Put on gloves.
4. Power down the detector by removing one battery.
5. Re-power the detector by reconnecting the battery.
6. Place smoke detector sensor or propane lamp mantle right over the neon bulb, and allow it to sit there for a few minutes.
7. Remove the radiation source, and remove gloves using [this method](http://youtu.be/DneVP5H48mY?t=24m33s).
8. Check the data: there should be some spikes in the signal several samples wide during the first few hours, while there should be no additional spikes during the time that the detector was exposed to the radiation source.

#### Troubleshooting
- If there is a greater rate of spikes in the region of the data after the radiation source is introduced, turn the trimpot a few degrees and try again until the rate is as low as can be.
- If at any point the neon bulb turns on, remove one battery to turn the detector off, rotate the trimpot a few degrees, and reattach the battery. If it comes back on, repeat this procedure.

## References
- [Wikipedia Article](http://en.wikipedia.org/wiki/Cosmic_ray)
- [National Geographic Article](http://news.nationalgeographic.com/news/2014/07/140709-space-cosmic-ray-hotspot-astronomy-science/)
- [ARMAS](http://sol.spacenvironment.net/~ARMAS/index.html)
- [Pierre Auger Observatory](http://www.auger.org)