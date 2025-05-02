# Billiard Ball Simulation Program
A place to store the actual program of the billiard ball simulation project. To check out the Unity assets, see [this](https://github.com/catloaf-cafe/Billiard-Ball-Simulation).

### Custom Input Type and (Suggested) Range: 

Regular Ball Quantity: int, [0, 500] <br>
Velocity Constant: float, [0, 5] <br>
Diameter Constant: float, (0, 5] <br>

Special Ball Quantity: int, [0, 50] <br>
Force Constant: float, [0, 200] <br>
Force Radius: float, [0, 100] <br>
Moving Increment: double, [0, 5] <br>
Angle Increment: double, [0, 5] <br>

### Input Explanation: 

Regular Ball Quantity: Parameter for the amount of regular balls you want. It can be adjusted during simulation. <br>

Velocity Constant: Parameter for both regular and special balls. The default should be set to 1. Notice that the velocity is automatically scaled inversely to the total ball quantity, so this parameter is only modified when the user wants to make additional adjustments. <be>

Diameter Constant: Similar description as above. <br>

Special Ball Quantity: Parameter for the amount of special balls you want. It can be adjusted during simulation. <be>

Force Constant: Represents the strength of the force. Need not to be negative. The program automatically scales the force strength inversely to the total ball quantity, but additional modification is still needed. <be>

Force Radius: Similar description as above. <be>

Moving Increment: Represents the special balls' speed. Since special balls are programmed to not have velocity on their own, the user must specify the moving increment per frame. Notice that the "default" value is dependent on the screen size, so it varies from device to device. <be>

Angle Increment: Similar description as above. <br>

### Keyboard Controls:

Setting Menu: <br>
&emsp; Space - resume <br>
&emsp; Return - reset <br>

During Simulation: <br>
&emsp; Space - pause <br>
&emsp; "-", "+" - delete/add regular balls <br>
&emsp; "[", "]" - delete/add special balls <br>

Both: <br>
&emsp; Escape - quit program <br>
