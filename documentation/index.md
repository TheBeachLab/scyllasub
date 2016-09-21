# Project Scylla Documentation

## Roadmap

### Hardware
* 1 Preliminary sketch design
* 2 Preliminary scale model design in Solidworks
* 3 Fabrication and design iteration
* 4 Design Solidworks full scale prototype with autonomous movement
* 5 Fabrication, testing and design iteration
* 6 Load sensing equipment
* 7 Survey testing
* 1 Pressure issues
* 1 Hydrodynamics
* 1 Energy
* 1 Communications
* 1 Positioning

### Software and electronics
* 1 Subroutines design
* 1 Electronics design
  * Sensing
  * Data acquisition (HD images)
  * Battery Management circuit
  * Controlling ROV (wired/ wireless)
* 2 Coding
* Debug button or Diagnostic utility


### Data processing
* Cartography tools: Qgis...
* Data processing and postprocessing
* Data visualization


## Environment
* Seawater
* Light conditions: pitch black
* Pressure (round 1): 200 atm  
* Pressure (round 2): 400 atm
* Temperature: unknown
* Currents: unknown
* Survey area shape: unknown
* Altitude: unknown but will be limited
* Suspended particles, fish (may objestruct maneuvering)

## Geo-Location
In normal operation the messenger operates in dead-reckoning. When a precise location is required, the messenger pings to request position. Timer counter on. Pings must be sent at low frequency (less than a few hundred Hz).

The angels receive the ping and ping back with scheduled delays. If angels position is known and static no data is sent. The messenger receives the pings and derive the distance to the angels. Speed of sound through s
[empirical formula](https://en.wikipedia.org/wiki/Speed_of_sound#Seawater).

1 angel -> sphere  
1 angels + height -> circle  
2 angels -> circle  
2 angels + height -> 2 points  
3 angels -> 1 point

##  Buoyancy Control
Usually, in a submarine the buoyancy is controlled with the help of ballast tanks, which can be filled with water or air to adjust the overall density of the vehicle. In submarines, this is done with the help of compressed air onboard. We need a ballast tank or we need to make sure that the vehicle's center of mass, at all times is lower, this is a must to ensure the stability (if we want the vehicle to have prefered orientation). We can lower the center of mass by moving all the heavy parts like the battery and other heavy parts like the main motor to the lower side of the vessel.

Anyway these are the methods to control the buoyancy of the vessel I (sibu) can think about. Feel free to add or edit.
* 1 Carry a  compressed air cylinder this can be very small depending on how long we plan to keep the vessel underwater, in operation. I guess it could be as small as a 100gm CO2 cartridge, which expands to about 25L at atmospheric pressure. This is by far the simplest and easiest method I can think about.
* 2 Carry a chemical/s than can generate gas on demand, by letting chemicals mix or react with water. Other possibilities are chemicals that release gas on heating.
* 3 Generate steam to build up pressure and expel water from the ballast tank.
* 4 Electrolysis to generate hydrogen and oxygen.
* 5 The ballast tank can be made as pistons and vacuum could be made to reduce the average density of the vessel.

Method 1 is tried and tested to be reliable. Requires almost zero energy consumption. But we have to carry the gas and the amount limits our operational freedom.

Method 3 & 4 are slow and consumes lot of energy, and very much energy inefficient.

Method 2 could be either slow or way too fast that it becomes dangerous. It may be very difficult to precisely control the amount of gas required. 

A temperature dependent Reversible chemical reaction between gaseous chemical species, generating a massive or liquid/solid product, could be a novel concept, but we have to think about the energy consumption.

Method 5 is also feasible, except the requirement for a high power/torque motor to power the piston and a strong cylinder and seal which can withstand the pressure.
