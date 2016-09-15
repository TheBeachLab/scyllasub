# Project Scylla Documentation

## Environment
Strike 1: 200 atm  
Strike 2: 400 atm

## Geo-Location
In normal operation the messenger operates in dead-reckoning. When a precise location is required, the messenger pings to request position. Timer counter on. Pings must be sent at low frequency (less than a few hundred Hz).

The angels receive the ping and ping back with scheduled delays. If angels position is known and static no data is sent. The messenger receives the pings and derive the distance to the satellites: Speed of sound through media
[empirical formula](https://en.wikipedia.org/wiki/Speed_of_sound#Seawater).

1 angel -> sphere  
1 angels + height -> circle  
2 angels -> circle  
2 angels + height -> 2 points  
3 angels -> 1 point
