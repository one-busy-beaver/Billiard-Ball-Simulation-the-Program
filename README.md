# Billiard Ball Simulation the Program
A place to store the actual program of the billiard ball simulation project. To check out the Unity assets, see [this](https://github.com/catloaf-cafe/Billiard-Ball-Simulation).

## Functionality
regular ball, special ball, violation of causality...

## Demo
will insert

## Custom Input Type
### Regular Ball Quantity (int)
Parameter for the amount of regular balls you want. It can be adjusted during simulation. 
- Suggested Range: [0, 500]
### Velocity Constant (float)
Parameter for both regular and special balls. The default should be set to 1. Notice that the velocity is automatically scaled inversely to the total ball quantity, so this parameter is only modified when the user wants to make additional adjustments. 
- Suggested Range: [0, 5]
### Diameter Constant （float)
Parameter for both regular and special balls. Similar description as above. 
- Suggested Range: (0, 5]
### Special Ball Quantity (int)
Parameter for the amount of special balls you want. It can be adjusted during simulation. 
- Suggested Range: [0, 50]
### Force Constant (float)
Represents the strength of the force. Need not to be negative. The program automatically scales the force strength inversely to the total ball quantity, but additional modification is still needed. 
- Suggested Range:[0, 200]
### Force Radius (float)
Represents the radius of the force. Similar description as above. 
- Suggested Range: [0, 100]
### Moving Increment (double)
Represents the special balls' speed. Since special balls are programmed to not have velocity on their own, the user must specify the moving increment per frame. Notice that the "default" value is dependent on the screen size, so it varies from device to device.
- Suggested Range: [0, 5]
### Angle Increment (double)
Represents the special balls' deviation from its straight path ahead. Similar description as above.
- Suggested Range: [0, 5]

## Keyboard Controls:
### Setting Menu
- Space - resume 
- Return - reset 
### During Simulation
- Space - pause <br>
- "-", "+" - delete/add regular balls 
- "[", "]" - delete/add special balls 
### Both: 
- Escape - quit program 
