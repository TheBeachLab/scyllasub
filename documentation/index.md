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
