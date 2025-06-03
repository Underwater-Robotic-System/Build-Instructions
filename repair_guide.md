# Repair Guide 

The following is a simple repair guide for common issues and links to resources for fixing them.

## General Issues and Troubleshooting Tips

Things not turning on or staying on when they shouldn't. This section should help.

### Switching from Digital to Analog Mode

To test if the motors are malfunctioning a good place to start is by switching them back to analog mode. This means instead of using the Arduino to run the motors, the robot is simply using the electronic signals from the joystick potentiometer to control the movements.

First turn off the robot. Disconnect it completely from power. 

For analog mode, the sabertooth controller needs to be set to the correct pins/dip switch settings. Both controllers should have all the pins set to the "on" position. 

![Sabertooth Analog Pins](repair_guide_images/analogpins.PNG)

Finally to switch to analog mode all 4 jumpers need to be connected to the "C2" position as seen below.

![Jumpers Analog Position](repair_guide_images/sabertoothwiring.PNG)

If there is issues with the control box build refer back to the [Control Box Build Guide by SeaMate](https://docs.google.com/presentation/d/e/2PACX-1vRtIemncL3JVpDB7jIuYOOvCOdgGI8xzUyhYJl8N8HHexPyqrFNaqludSkgZgUaFctHBfSlmvy4tpxE/pub?start=false&loop=false&delayms=3000&slide=id.p)

If things are working in analog mode, then the issue is likely with the Arduino or the code. If things are not working in analog mode, then the issue is likely with the sabertooth controller or the motors or something hardware related.

### Reverting Back to Digital Mode from Analog Mode

To switch back to digital mode, the sabertooth controller needs to be set to the correct pins. 1,3,5 are on and 2,4,6 are off for both controllers.

![Sabertooth Digital Pins](repair_guide_images/digitalpins.PNG) 

**The 4 jumpers should be set to the "C1" position**.

If there are more issues with the control box being converted back to digital mode, refer to the [Control Box Build Digital Guide by SeaMate](https://docs.google.com/presentation/d/e/2PACX-1vSaJHo9mUlmZ_VFU7EeYjHr5jsFbRT6R-QFL30TU9lDHdw7xt-9oLNg8te0xLp8fXEJK5ztT22pUU_C/pub?start=false&loop=false&delayms=3000&slide=id.p1).

## Motor Issues

### Joystick Drift

If the joystick is drifting, it may be due to a bad potentiometer. You can tell this is an issue if one or more of the motors never fully turns off. The potentiometer is the component inside the joystick that detects the position of the joystick. If it is not working properly, it can cause the robot to drift in one direction or another. You can test this to see if there is any position the motors are fully stopping by gently moving the joystick in all directions and seeing if the motors stop or get any closer to stopping. This means the home setting of the joystick is not actually where the motors are stopping anymore. This can happen overtim by wear and tear on the joystick or if the joystick is dropped or damaged.

To fix this the best solution is to replace the joystick. You can buy the joystick separately or the whole kit from [SeaMate](https://seamate.org/collections/barracuda-rov/products/sabertooth-joystick-replacement-kit).

### Sabertooth Controller Issues

First check all the wires connected to the sabertooth. The sabertooth controller on the left controlls the left and right (horizontal) motors while the one on the right controls the crab and vertical motors. Check all the wires are secure in the sabertooth. 
They can loosen overtime since they are connected through a screw connection. Tighten the screws with the wires in the slots to ensure they are secure.

If the motors continue to not work and the sabertooth controller is flashing red or not working even with the pins the correct spots it may mean that the controller needs replaced. You can buy one separately or from [SeaMate](https://seamate.org/collections/barracuda-rov/products/sabertooth-joystick-replacement-kit).

Replacing the sabertooth requires unscrewing all the wires, taking out the PCB board carefully, and unscrewing the controller from the board. Use some **heatsink compound** on the back of the new controller before putting it in. This helps to make sure it does not overheat. Screw all the pieces and wires back in their original positions.

![Sabertooth Wiring](repair_guide_images/sabertoothwiring.PNG)

For more information on the sabertooth controller, refer to the [Sabertooth Powerpoint by SeaMate](https://docs.google.com/presentation/d/e/2PACX-1vRFP-ZPQkCo_Jx7r8_KIzDjlaPUm8ab588ryvPmsn5yvhOffjHJ8nfAnJD0QdS-N_Us_cYrgIzRN6ts/pub?start=false&loop=false&delayms=3000&slide=id.g15f7ea19d6_0_14).

## Camera Issues

## Sensor Issues

## Software Issues 
