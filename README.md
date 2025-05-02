# Billiard Ball Simulation the Program
A place to store the actual program of the billiard ball simulation project. To check out the Unity assets, see [this](https://github.com/catloaf-cafe/Billiard-Ball-Simulation).

## Functionality
This project aims to simulate an instance of violation of causality. 

There are two balls in the system, regular balls and special balls. Regular balls are the ones that "obey and react" to the physical world. When there is an impact, these balls will bounce back as what we expect from the laws of physics. 

Special balls, on the other hand, won't be pushed back when they have an impact with regular balls. Instead, they will follow their original path, and only the regular balls will bounce back. They also won't come in contact with each other. Special balls are also designed to be able to attract or repel regular balls to create a larger violation of causality.

The user can control how many regular and special balls that are on the screen, and how fast they move, etc..

## Demo
will insert

## Custom Inputs and What They Mean
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

## Keyboard Controls
### Setting Menu
- Space - resume 
- Return - reset 
### In Simulation
- Space - pause <br>
- "-", "+" - delete/add regular balls 
- "[", "]" - delete/add special balls 
### Both: 
- Escape - quit program 
