# Underwater Positioning
In normal operation the ROV operates in dead-reckoning. When a precise location is required, the ROV pings to request position. Timer counter on. Pings must be sent at low frequency (less than a few hundred Hz).

The surface buoys receive the ping and ping back with scheduled delays. If buoys position is known and static no data is sent. The rov receives the pings and derive the distance to the buoys. Speed of sound through s
[empirical formula](https://en.wikipedia.org/wiki/Speed_of_sound#Seawater).

1 buoy -> sphere  
1 buoys + height -> circle  
2 buoys -> circle  
2 buoys + height -> 2 points  
3 buoys -> 1 point

Wikipedia entry about [Underwater acoustic positioning system](https://en.wikipedia.org/wiki/Underwater_acoustic_positioning_system)
