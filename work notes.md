# PRESSURE SENSORS

Measurements:  
0.730 V -> 0.0 Bar  
0.926 V -> 0.5 Bar  
1.131 V -> 1.0 Bar  
1.275 V -> 1.5 Bar  
1.444 V -> 2.0 Bar  
1.605 V -> 2.5 Bar  
1.768 V -> 3.0 Bar  
1.951 V -> 3.5 Bar  

Output is linear and has the same slope as in datasheet.
It's possible to recalculate values with ESPHome filters.

## 1.2 MPa sensor
datasheet: 0.5V -> 0 Bar, 4.5V -> 12 Bar  
p = k*x + b  
k = (4.5 - 0.5) / (12 - 0) = 0.333(3)

## 0.5 MPa sensor
datasheet: 0.5V -> 0 Bar, 4.5V -> 5 Bar  
p = k*x + b  
k = (4.5 - 0.5) / (5 - 0) = 0.8
