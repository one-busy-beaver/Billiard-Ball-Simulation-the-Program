# Billiard Ball Simulation the Program
A place to store the actual program of the billiard ball simulation project. To check out the Unity assets, see [this](https://github.com/catloaf-cafe/Billiard-Ball-Simulation).

## Functionality
regular ball, special ball, violation of causality...

## Custom Input Type and Suggested Range: 
- Regular Ball Quantity: int, [0, 500]
  - Parameter for the amount of regular balls you want. It can be adjusted during simulation. 
- Velocity Constant: float, [0, 5]
  - Parameter for both regular and special balls. The default should be set to 1. Notice that the velocity is automatically scaled inversely to the total ball quantity, so this parameter is only modified when the user wants to make additional adjustments. 
- Diameter Constant: float, (0, 5]
  - Parameter for both regular and special balls. Similar description as above. 
- Special Ball Quantity: int, [0, 50]
  - Parameter for the amount of special balls you want. It can be adjusted during simulation. 
- Force Constant: float, [0, 200]
  - Represents the strength of the force. Need not to be negative. The program automatically scales the force strength inversely to the total ball quantity, but additional modification is still needed. 
- Force Radius: float, [0, 100]
  - Represents the radius of the force. Similar description as above. 
- Moving Increment: double, [0, 5]
  - Represents the special balls' speed. Since special balls are programmed to not have velocity on their own, the user must specify the moving increment per frame. Notice that the "default" value is dependent on the screen size, so it varies from device to device.
- Angle Increment: double, [0, 5]
  - Similar description as above.

## Keyboard Controls:
### In the Setting Menu
- Space - resume 
- Return - reset 
### During Simulatio
- Space - pause <br>
- "-", "+" - delete/add regular balls 
- "[", "]" - delete/add special balls 
### Both: 
- Escape - quit program 
