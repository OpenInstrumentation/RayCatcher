# Cosmic Ray Detector
## Overview
This project seeks to create an inexpensive cosmic ray detector capable of sensing rays greater than 1 GeV in energy.

![image](http://auger.physics.wisc.edu/images/crspectrum.gif "Cosmic Ray Spectrum")


### Circuit
![image](https://doc-10-08-docs.googleusercontent.com/docs/securesc/ha0ro937gcuc7l7deffksulhg5h7mbp1/ajgfdcd2852n11kftaq7gkg63tteg2ic/1405454400000/01745336737108954122/*/0B52gk5ma9b0EdnQtSU9ZU3hiMDQ?h=16653014193614665626&e=download =400x "Detector Circuit")

In this circuit diagram, **R** is the sense resistor, usually about 1 kΩ, and **V** is the bias voltage. The bias voltage should be less than the turn-on voltage (usually either 95 or 65 VDC depending on the type of bulb being used), but should be high enough that a cosmic ray can trigger the circuit, causing a current to flow through the resistor. This is usually about 80-94 VDC, and can be supplied by a bank of 9-volt batteries, or a DC-DC converter that has a sufficiently large capacitor across it to absorb all transients.

### Construction
