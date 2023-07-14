# Build-Instructions

Step-by-Step Building Guide

## Content

- [Barracuda robot](#barracuda-robot-build-instructions)
  - [Tool List](https://docs.google.com/spreadsheets/d/1VwJwuMHgYOP06yRYR0DLT3_j4Y_BDbTCyc3LyoblmyQ/edit?usp=sharing)
  - [Part One: Design and Build Frame](#part-one-design-and-build-frame)
  - [Part Two: Propulsion System](#part-two-propulsion-system)
  - [Part Three: Power System](#part-three-rov-power-system)
  - [Part Four: Analog Control System](#part-four-analog-control-system)
  - [Part Five: Connect the Tether System to the Control System](#part-five-connect-the-tether-system-to-the-control-system)
  - [Part Six: Waterproofing the Camera](#part-six-waterproofing-the-camera)
  - [Part Seven: Digital Control System](#part-seven-digital-control-system)
  - [Part Eight: Programming the ROV](#part-eight-programming-the-rov)
- [Triggerfish robot](#triggerfish-robot-build-instructions)
- [Sensor system](#sensor-system)
  - [Part One: setup](#part-one-set-up)
  - [Part Two: Probes calibration](#part-two-probes-calibration)
  - [Part Three: Control box](#part-three-control-box)
  - [Part Four: Connecting Multiple sensors to one Arduino uno serial port](#part-four-connecting-multiple-sensors-to-one-ardunio-uno-serial-port)
  - [Part Five: Connect sensors to the frame](#part-five-connect-sensors-to-the-frame)
  - [Part Six: Extract the data to CSV file](#part-six-extract-the-data-to-csv-file)

## Parts

### Robot 1: Barracuda

- 1x 12V DC Power Supply w/power pole outlet + GFCI
- 1x SeaMATE TriggerFish (Rev 4)/Barracuda (Rev 1) Video System Kit (2 cameras)
- 1x SeaMATE Barracuda ROV Kit (Rev 1-AD)

### Robot 2: TriggerFish

- 1x SeaMATE TriggerFish (Rev 4)/Barracuda (Rev 1) Video System Kit (2 cameras)
- 1x 12V DC Power Supply w/power pole outlet + GFCI
- 1x SeaMATE TriggerFish (Rev 4) to Barracuda (Rev 1) Upgrade Kit
- 1x SeaMATE TriggerFish ROV Kit (Rev 4-AC)

## Barracuda Robot Build Instructions

[Barracuda Tool List](https://docs.google.com/spreadsheets/d/1VwJwuMHgYOP06yRYR0DLT3_j4Y_BDbTCyc3LyoblmyQ/edit?usp=sharing)

### Part One: Design and Build Frame

Tools and Parts needed:

- PVC Cutter
- Rubber Hammer
- 3/8 inch drill bit and drill
- 1/2 inch drill bit and drill
- 12 ft. 1/2 inch PVC pipe (preferably thin-wall)
- 9 pieces of 90-degree elbow ½ PVC socket by socket
- 2 pieces of ½ inch PVC cross socket by socket by socket by socket
- 12 pieces of ½ inch PVC T socket by socket by socket
- 1 piece of PVC T ¾ by ½ by ¾ , ½ is the center hole, socket by socket by socket
- 2 pieces of 3/4 in x 1/2 in PVC Reducer (no threads)
- 1 piece of ¾ inch PVC tap socket
- 2 pieces of 3/4 inch PVC 5 cm long
- Saw

Using the video [Build a Remotely Operated Vehicle (ROV) at Home!](https://www.youtube.com/watch?v=Lnr5YlBl550) as a reference as well as [SeaMate](https://seamate.org/) we designed a frame for the tethered ROV. We initially only designed the frame to hold 3 motors but we altered the design to hold 4 because that is how many our kit came with. In total, we have two forward-facing propellers, a crab propeller, and a vertical propeller.

The image we used for reference from [SeaMate](https://seamate.org/):

<img src="/images/reference.png" alt="Reference Image" width="50%" height="50%">

Our original design:

<img src="/images/design1.jpg" alt="First Design Image" width="50%" height="50%">

Altered Design to feature four propellers:

<img src="/images/design2.jpg" alt="Altered Design Image" width="50%" height="50%">

1.Cut the 12 ft. 1/2 inch PVC pipe into various pieces using the PVC Cutter:

- 2 pieces 20 cm long  
- 2 pieces 15 cm long (10cm x 2 + 3cm x 2 long)
- 2 pieces 12 cm long
- 8 pieces 10 cm long
- 3 pieces 7 cm long
- 5 pieces 5 cm long
- 9 pieces 3 cm long

2.Drill a 3/8 inch hole into the 3/8 inch PVC tap socket

3.On the side of one of the 5 cm long 3/4 inch PVC use a saw to cut a slit about a 1/2 inch wide

4.Follow the design to build the frame. Remember to use the rubber hammer to secure the  pipes in place

Our Finished Frame:

<img src="/images/frame.jpg" alt="Frame Image" width="50%" height="50%">

### Part Two: Propulsion System

Tools and Parts needed:

- Flat-head screwdriver
- Hot-glue gun
- Heat shrink
- Barracuda Motor and Propeller Kit

Follow the ["Motors and Propellers" presentation](https://docs.google.com/presentation/d/1mcP4J4Q2bmahoEIpsOrDUR52icu5sXS-rw9jk4Rwi88/pub?start=false&loop=false&delayms=3000&slide=id.gae2819d7c9_2_0) from [SeaMate](https://seamate.org/) to attach and secure the propellers to the motors. Images are provided by [SeaMate](https://seamate.org/).

1. Start by attaching the motor mounts
2. Remove the impeller
3. Follow the ["Attaching Propellers to the Motors" video](https://vimeo.com/461891032/d2fa00bc51) to properly attach the propellers to the motors. Remember to use the Loctite on the tip of the bolt to ensure that the propeller bolt does not spin out.

For the next step, we created the tether management system. The system recommended in ["Propulsion System: Creating the Tether Management Cross For PVC Frames"](https://docs.google.com/presentation/d/1OqQ49ZD1G6fhgH34ldpA0NPWfAKPs6clWxlLNhh0xcE/pub?start=false&loop=false&delayms=3000&slide=id.g1c265fea39_2_47) utilizes a PVC cross. Our system, however, does not and uses a straight PVC connector.

Cross PVC tether management system from ["Propulsion System: Connecting the tether to the motors"](https://docs.google.com/presentation/d/1_93HPWE-aPsy9pZsqfuzoopn1yeF3Gt1c8lFXxB4B6g/pub?start=false&loop=false&delayms=3000&slide=id.g1c61d8a3e2_2_47):

<img src="/images/cross_pvc.png" alt="Cross PVC tether management system" width="50%" height="50%">

Our PVC tether management system:

<img src="/images/outsideoftether.jpg" alt="Tether management system" width="50%" height="50%">

For the next step, solder the motor wires to the tethers. Following the ["Propulsion System: Connecting the tether to the motors"](https://docs.google.com/presentation/d/1_93HPWE-aPsy9pZsqfuzoopn1yeF3Gt1c8lFXxB4B6g/pub?start=false&loop=false&delayms=3000&slide=id.g1c61d8a3e2_2_47) presentation, connect the tether to the motors. Remember to put the heat shrink around the tether before soldering so you can apply it after to waterproof the wire. Use hot glue around the wires and put the heat shrink over it and heat it. The glue should reheat and form around the wires.

Our waterproofing of the tethers:

<img src="/images/waterproofoftether.jpg" alt="Waterproof of Tether" width="50%" height="50%">

### Part Three: ROV Power System

Tools and Parts needed:

- Soldering iron
- Solder/ Solder and Seal Connectors
- Wire Strippers
- Wire cutters
- Hot Glue and a hot-glue gun
- Heat gun
- Heat shrink
- Anderson Power pole Crimper (No generic brand of crimper will work)
- Barracuda Power Kit

We followed the ["Power System: Creating Your Power Wires" presentation](https://docs.google.com/presentation/d/e/2PACX-1vRB_owLvyuNd8iDSV75_4woGGFtWirwWUzcAqRzxTVrHXuVxsgL9y21wm49XkIXBWbFYfJHqMubGQvk/pub?start=false&loop=false&delayms=3000&slide=id.g16b0f7ed38_2_47) for putting together our ROV Power System.

Steps:

1. For the first step solder the red wire from the fuse to the red power wire and waterproof the connection. To waterproof the connection before soldering together the wires slide the heat shrink over the fuse wire. Then solder the wires together and put hot glue over the connection. Put the heat shrink over the solder and heat it. The glue should reheat and cover the joint. For more information on waterproofing connections, you can look over the ["Soldering Wires and Waterproofing Connections" presentation](https://docs.google.com/presentation/d/e/2PACX-1vTPJ1hrOKJDOTHoj9DG1P2_QryKL_gfk6RzKkA6mBRk2MNgf4Fkmfli536027sqzH-LtXmxUy9lx1P4/pub?start=false&loop=false&delayms=3000&slide=id.p4). Alternatively, you can use the solder and seal connectors over the wires to connect and waterproof them. We choose to use the solder and seal connectors for the power cord.
2. Next crimp on the Anderson Powerpoles. Strip approximately 0.75 cm from the end of the wire that needs to be crimped. Take one of the metal crimps and insert it with the hook side down into the hole between '30' and '45'. Squeeze the handle to slightly hold onto the metal piece but do not crush it. Then insert the stripped wire and squeeze the Anderson Powerpole crimper until the handle releases. Repeat this for each end of the wire.
3. Put the hook into the plastic housing and push it down to lock it in place.

Anderson Powerpole crimper:

<img src="/images/anderson.jpg" alt="Anderson Powerpole crimper" width="50%" height="50%">

Our power cord connections:

<img src="/images/powercord.jpg" alt="Our power cord connections" width="50%" height="50%">

### Part Four: Analog Control System

Tools and Parts needed:

- Soldering iron
- Solder
- Wire Strippers
- Wire cutters
- Metric rule
- Large and small Phillips head and flat-head screwdrivers
- Jeweler's screwdrivers
- Anderson Power pole crimper (No generic brand of crimper will work)
- Regular crimper
- Needle nose pliers
- Solder sucker
- The MATE Barracuda ROV kit and video monitor

Following the ["Constructing the Barracuda Control Box in Analog Mode" presentation](https://docs.google.com/presentation/d/e/2PACX-1vRtIemncL3JVpDB7jIuYOOvCOdgGI8xzUyhYJl8N8HHexPyqrFNaqludSkgZgUaFctHBfSlmvy4tpxE/pub?start=false&loop=false&delayms=3000&slide=id.p) we put together the analog control box system. Remember when soldering to check the polarity of the parts before putting them into the main PCB.

1. Start on the main PCB and follow the ["Constructing the Barracuda Control Box in Analog Mode" presentation](https://docs.google.com/presentation/d/e/2PACX-1vRtIemncL3JVpDB7jIuYOOvCOdgGI8xzUyhYJl8N8HHexPyqrFNaqludSkgZgUaFctHBfSlmvy4tpxE/pub?start=false&loop=false&delayms=3000&slide=id.p).
2. After finishing the main PCB construct the backplate board.
3. Solder the tether piece to the colored wires on the backplate.
4. Connect the watt meter and the joysticks to the acrylic pieces. Use the Anderson Powerpole crimper on the ends of the wires connected to the watt meter.
5. Connect the monitor to the backboard. Connect the power wires and video input into the proper connections
6. Put everything in place into the Barracuda control box. Attach the backboard to the control box using the given nuts and bolts. Attach the monitor to the top lip using Velcro. You can leave the blue PCB out for now because we will be soldering it again later.

Analog Main Board:

<img src="/images/blueboard.jpg" alt="Blue PCB" width="50%" height="50%">

Analog backboard front before connecting to the tether:

<img src="/images/backboardfront.jpg" alt="Backboard Front" width="50%" height="50%">

Analog backboard back before connecting to the tether:

<img src="/images/backboardback.jpg" alt="Backboard Back" width="50%" height="50%">

Analog system after connecting to the tether:

<img src="/images/afteranalog.png" alt="After Analog soldering" width="50%" height="50%">

Attach the backboard:

<img src="/images/attachbackboard.jpg" alt="Backboard" width="50%" height="50%">

Attach the monitor:

<img src="/images/attachmonitor.jpg" alt="Monitor" width="50%" height="50%">

### Part Five: Connect the Tether System to the Control System

When connecting the tether system to the control system you have to solder the eight colorful wires of the tether to the tether connector. Each wire has a corresponding pin on the connector. Follow the chart provided in the ["Control System: Connecting the tether to the TF 4.0 / Barracuda control box"](https://docs.google.com/presentation/d/e/2PACX-1vRmrSRmjQVziOMXkgDid8x8DRKmTxXSncry5jPP_hHe7w-SiogroOXmtn4SQ5PWtV8lacbkS3eCdnta/pub?start=false&loop=false&delayms=3000&slide=id.g1c61c68843_4_66) presentation.

Image of the pins provided by ["Control System: Connecting the tether to the TF 4.0 / Barracuda control box"](https://docs.google.com/presentation/d/e/2PACX-1vRmrSRmjQVziOMXkgDid8x8DRKmTxXSncry5jPP_hHe7w-SiogroOXmtn4SQ5PWtV8lacbkS3eCdnta/pub?start=false&loop=false&delayms=3000&slide=id.g1c61c68843_4_66):

<img src="/images/tetherconnector.png" alt="Tether Pins" width="50%" height="50%">

After connecting the tether you can plug in the system to test the motors. The four lights on the blue PCB will light up when the corresponding motor is moving. Use the joysticks to move the motors and test different speeds.

Testing the motors:

<img src="/images/ourmotors.gif" alt="Motors GIF" width="50%" height="50%">

### Part Six: Waterproofing the Camera

Tools and Parts needed:

- Video System Kit - 2 Camera from SeaMate
- 5-minute epoxy, we used [Gorilla 2 Part Epoxy, 5 Minute Set](https://www.amazon.com/Gorilla-Epoxy-Minute-ounce-Syringe/dp/B01M7VD07W/ref=sr_1_5?crid=3MVHT4WJMP0K6&dchild=1&keywords=5+minute+epoxy&qid=1610756667&sprefix=5+minute+epoxy%2Caps%2C283&sr=8-5)
- Acrylic gap filler, we used [IPS Weld-On 16 Acrylic Plastic Cement](https://www.amazon.com/IPS-Weld-Acrylic-Plastic-Cement/dp/B0149IFA9O/ref=sr_1_12?crid=2FEZKY6KF46N7&dchild=1&keywords=acrylic+glue&qid=1610756924&sprefix=acrylic+g%2Caps%2C301&sr=8-12)
- [Envirotex-Lite slow curing epoxy](https://www.amazon.com/Environmental-Technology-16-Ounce-Pour-Finish/dp/B000LNS9CW/ref=sr_1_8?crid=DLLXQ4XHO3HR&dchild=1&keywords=envirotex+lite&qid=1610757028&sprefix=envirote%2Caps%2C279&sr=8-8)
- 3 plastic cups
- Stir sticks
- Toothpicks
- Protective gloves
- Clean, well-ventilated, and protected area
- 5% white vinegar solution (in case you have to remove uncured epoxy from your skin)

By following the ["Creating a Ruggedized Waterproof Camera" presentation](https://docs.google.com/presentation/d/e/2PACX-1vRrlYFWUx8csrGhwCbVJPvuaqN2EGDLD4UUQ7FA8KJXNQRPEpY4xKNoAaWuSK1Vagv4G1HJcjQ5s-JH/pub?start=false&loop=false&delayms=3000&slide=id.p4) we waterproofed the camera.

Waterproofing the Camera Materials:

<img src="/images/waterproofingmaterials.jpg" alt="Waterproofing the Camera Materials" width="50%" height="50%">

Steps:

1. Remove the protective lens cover and brackets from the camera
2. Prepare the clear plastic disk by drawing an X on the plastic covering. Remove the plastic cover from the other side of the plastic disk, this will act as a circular lens.
3. Use the 5-minute epoxy to attach the camera lens to the plastic disk. Seal the lens so that there are no gaps for the slow-curing epoxy to get through. Do not cover the camera lens with epoxy either or you will lose vision. The ["Waterproofing a Camera 1: Epoxying the disk over the lens" video](https://vimeo.com/437484941/fc75689ada) was a very helpful resource for this step.
4. After securing the camera to the plastic disk you have to glue the lens onto the tube. Use the Acrylic gap filler glue to secure the tube to the disk and use enough to fill all the holes. If there are gaps the slow-curing epoxy will leak. Wait 1-2 hours for the glue to dry. Repeat the gluing process again until there are no gaps left, and let dry overnight. The ["Waterproofing a Camera 2:  Inserting the camera into the acrylic tube" video](https://vimeo.com/437487451/83b6e1d827) is what we used as a resource for this step.
5. Next insert the cable into the tube. Start by attaching the tether cable to the camera and plugging it in. The red and yellow connectors need to be secured into the tube and will be submerged in the epoxy. Twist the wires into a package until they can be inserted into the acrylic tube and do so.
6. The next step is to mix and pour the slow-curing epoxy. The epoxy we used is 2-part and directs you to mix equal amounts of both parts. Stir the epoxy for about 3-5 minutes and pour into the tube. Wait overnight for it to cure. You can watch the ["Waterproofing a Camera 3:  Pouring epoxy"](https://vimeo.com/437486428/14f4e19c03) video to see how they poured their epoxy into the tube.

Waterproofing the Camera after Step 3:

<img src="/images/waterproofcam1.jpg" alt="Waterproofing the Camera Step 3" width="50%" height="50%">

Waterproofing the Camera after Step 4:

<img src="/images/waterproofcam2.jpg" alt="Waterproofing the Camera Step 4" width="50%" height="50%">

Waterproofing the Camera after Step 5:

<img src="/images/cableintube.jpg" alt="Waterproofing the Camera Step 5" width="50%" height="50%">

<img src="/images/tether.gif" alt="Tethers in the Tube gif" width="50%" height="50%">

Waterproofing the Camera after Step 6:

<img src="/images/afterpouring.jpg" alt="Waterproofing the Camera Step 6" width="50%" height="50%">

<img src="/images/singlecamera.jpg" alt="Single Camera" width="50%" height="50%">

### Part Seven: Digital Control System

Using the ["Installing Components to Convert the Barracuda from Analog to Digital" presentation](https://docs.google.com/presentation/d/e/2PACX-1vRGQ4dE5oen7Kwpmbd7KRCxd7AtzV-uXCo0KpaTwT5Yzs5sOymx5Vyh6EKPKEWbZbH0UaDV7fXbUJDf/pub?start=false&loop=false&delayms=3000&slide=id.p1) we converted the analog electronics to digital to make it capable of being programmed and to add Bluetooth.

Tools and Parts needed:

- Soldering iron
- Solder
- Wire Strippers
- Wire cutters
- Solder sucker
- Digital System Kit from SeaMate
- Needle-nosed pliers

Steps:

1. Install the Arduino. Start by soldering the resistors R11 - R14 onto the board. Using the 40-pin header strip, insert the long ends of the pins into the Arduino headers. Fit the Arduino into the Barracuda Control Board. You may need to tape the Arduino to the board and then solder the 32 pins.
2. Solder the Arduino 9V Power Supply. Solder all the parts into the board including the 1000 ohm resistor, LED, and capacitors C2,C3, and C7.
3. Test the power system by reconnecting the system to power. The power LED should light up green if the system is good.
4. Solder in the 12C display connector piece.
5. Plug the Arduino USB cable into the box.
6. Solder the relay devices on the left side of the blue PCB. Also, solder the LEDs and fuse holder.
7. Put the Bluetooth HC-05 in place and solder the Bluetooth and resistors R11-R14 for the Bluetooth. Before soldering the Bluetooth HC-05 the pins will not be at the correct angle of 45 degrees to the board so use the needle-nosed pliers to angle the board into the right place. To see how to bend the pins correctly the ["Installing the Bluetooth" video](https://vimeo.com/543361284/c9fdbb2f1a) is very helpful.

After soldering the Arduino into the board:

<img src="/images/arduinoinboard.jpg" alt="Arduino" width="50%" height="50%">

After soldering the relay system into the board:

<img src="/images/relaysystem.jpg" alt="Relay system" width="50%" height="50%">

### Part Eight: Programming the ROV

Prepare your ROV to take digital commands.

1. Start by downloading the Arduino Software (version 1.8.15 or later) and installing the control program for the Barracuda [Download Link](https://www.arduino.cc/en/software). You can optionally download the software, MIT A12, which allows your ROV to be controlled via Bluetooth on an Android phone [Download Link](https://www.google.com/url?q=https://appinventor.mit.edu/explore/get-started&sa=D&source=editors&ust=1686157110234992&usg=AOvVaw0bAEwxUN1TN1yHN-OP9nPD).
2. Switch the four jumpers to the two left-most posts to cover pins 1 and C on each 3-pin header connector.
3. Set the DIP Switches to the proper settings following this chart. If you would like to know more you can follow the [Sabertooth Dip Switch Wizard](http://www.dimensionengineering.com/datasheets/SabertoothDIPWizard/start.htm).

<img src="/images/dipswitch_settings.png" alt="DIP Switch Settings" width="50%" height="50%">

4. Next download the [MATE control sketch](https://files.materovcompetition.org/docs/resources/Barracuda/code/CUDA-Arduino-Joystick-Control.ino).
5. Now connect the LCD display to the four pins of the 12C Display. Make sure to connect the GND to GND, VCC to +5V, SDA to SDA, and SCL to SCL.
6. Next download the [Display Test Sketch](https://files.materovcompetition.org/docs/resources/Barracuda/code/CUDA-DISPLAY-TEST-1.ino). See if the test works, it should display characters 0123456789ABCEDEG on row 0 and FEDCBA9876543210 on row 1 one at at a time.
7. You can download the library files after testing your display. The first one is for the motor controller, [DimEng Sabertooth.zip](https://files.materovcompetition.org/docs/resources/Barracuda/code/). The second library is for the 12C liquid crystal display [Liquid Crystal 12C-1.zip](https://files.materovcompetition.org/docs/resources/Barracuda/code/).
8. Test the Relay with the [relay test sketch](https://files.materovcompetition.org/docs/resources/Barracuda/code/CUDA-RELAY-TEST-1.ino). The relays will toggle on relay 1 for 2 seconds and turn it off. Then it will toggle on the second relay for 2 seconds and turn it off. The LCD displays the state of the relays.
9. (OPTIONAL) If you downloaded the software to control the ROV with an Android phone you can test it using the [Bluetooth Test Sketch](https://files.materovcompetition.org/docs/resources/Barracuda/code/CUDA-Bluetooth_Relay_Test.ino). The commands are as follows. 0 turns relay 1 on, 1 turns relay 1 off, 2 turns relay 2 on, 3 turns relay 2 off.
10. You are now ready to edit your basic Arduino program to control your ROV.

Test the LCD step 6:

<img src="/images/testlcd.gif" alt="LCD Test" width="50%" height="50%">

Test the Motors step 7:

<img src="/images/motortest.gif" alt="Motor Digital Test" width="25%" height="25%">

### Part Nine: Adding a Video Camera System

[ADDING A CAMERA TO THE BARRACUDA CONTROL BOX](https://docs.google.com/presentation/d/e/2PACX-1vRJjvGWgH24Xj1KYbRpok7Kht3LrysZ1Clu1u61WIKA2NfJ5kuueQJWUdK1OY4nEr65P3OiVYW8rf7m/pub?start=false&loop=false&delayms=3000&slide=id.g1c61c68843_4_66)

## TriggerFish Robot Build Instructions

We followed a very similar process for the Triggerfish Robot as we did the Barracuda however, a few adjustments were made. Instead of drilling holes into corner PVC pieces, we went to the alternative of using T-shaped PVC pipe at the corners of the frame. This allowed steadier water flow and for the robot to fill up faster. We also only used one camera instead of two.

## Sensor system

### Part One: Set up

Tools and Parts needed:

- [ENV-SDS Kit from Atlas Scientific](https://atlas-scientific.com/kits/env-sds-kit/)
- Flow meter
- Tethers
- Waterproof material
- [Extension cables](https://atlas-scientific.com/cables/3-meter-sma-male-to-sma-female-extension-cable/)
- Electronics storage container
- Arduino
- PVC T
- PVC reducer
- PVC circle opening
- Hot glue and hot glue gun

First set your sensors into the preferred mode. We kept ours in UART mode for compatibility with the Arduino and for calibration. You can use this [Instructibles guide](https://www.instructables.com/UART-AND-I2C-MODE-SWITCHING-FOR-ATLAS-SCIENTIFIC-E/) to see the 3 different methods to switch modes.

### Part Two: Probes calibration

Next calibrate your probes

- It is easier to do calibration in UART mode with continuous readings enabled. Calibration can be trickier in I2C mode but you can do it in either mode.

[Switch mode guide](https://www.instructables.com/UART-AND-I2C-MODE-SWITCHING-FOR-ATLAS-SCIENTIFIC-E/)

![UART and I2C mode](/images/UART-I2C-Mode.jpg)

- Make sure to calibrate with all the cable extensions attached. We used these [Extension cables](https://atlas-scientific.com/cables/3-meter-sma-male-to-sma-female-extension-cable/) 3 meter-long cables however we had to also order an extra [connector](https://atlas-scientific.com/connectors/female-bnc-to-male-sma-connectors/) for the temperature sensor specifically.

[Tips for calibrate probes](https://www.instructables.com/TIPS-FOR-USING-ATLAS-SCIENTIFICS-SENSORS-SOME-DOs--1/)

#### pH probe

- pH probe has red color: [EZO pH circuit dataset](https://files.atlas-scientific.com/pH_EZO_Datasheet.pdf)

- Enable continuous reading mode: type `C,1` in the Serial Monitor, you know the sensor in continuous reading mode when the led is blinking

- Follow this tutorial on how to calibrate your pH sensor: [video tutorial](https://how2electronics.com/interfacing-atlas-scientific-ph-sensor-with-arduino-via-uart-i2c/)

<img src="/images/pH%20calibration.jpg" alt="pH calibration" width="50%" height="50%">

- Code and wiring: [pH probe calibration](https://files.atlas-scientific.com/Arduino-Uno-pH-sample-code.pdf)

- Calibration steps: [Atlas Scientific EZO PH Calibration Procedure](https://www.instructables.com/Atlas-Scientific-EZO-PH-Calibration-Procedure/)

#### Dissolve oxygen (DO) probe

- Dissolve oxygen (DO) has yellow color: [EZO DO circuit dataset](https://files.atlas-scientific.com/DO_EZO_Datasheet.pdf)

- Code and wiring: [DO probe calibration](https://files.atlas-scientific.com/Arduino-Uno-DO-sample-code.pdf)

- Calibration steps: [Atlas Scientific EZO DO Calibration Procedure](https://www.instructables.com/Atlas-Scientific-EZO-DO-Calibration-Procedure/)

#### Oxidation-reduction potential (ORP) probe

- ORP probe has blue color: [EZO ORP circuit dataset](https://files.atlas-scientific.com/ORP_EZO_Datasheet.pdf)

- Code and wiring: [ORP probe calibration](https://files.atlas-scientific.com/Arduino-Uno-ORP-sample-code.pdf)

- Calibration steps: [Atlas Scientific EZO ORP Calibration Procedure](https://www.instructables.com/Atlas-Scientific-EZO-ORP-Calibration-Procedure/)

#### Conductivity probe (EC)

- Conductivity has green color: [EZO EC circuit dataset](https://files.atlas-scientific.com/EC_EZO_Datasheet.pdf)

- Code and wiring: [EC probe calibration](https://files.atlas-scientific.com/Arduino-Uno-EC-sample-code.pdf)

- Calibration steps: [Atlas Scientific EZO EC Calibration Procedure](https://www.instructables.com/Atlas-Scientific-EZO-EC-Calibration-Procedure/)

#### Temperature sensor (RTD)

- Temperature sensor has the pink wire: [EZO RTD dataset](https://files.atlas-scientific.com/EZO_RTD_Datasheet.pdf)

- Code and wiring: [Temperature sensor calibration](https://files.atlas-scientific.com/Arduino-Uno-RTD-sample-code.pdf)

- Calibration can be done at any value, a simple method is to calibrate the probe in boiling water (100 degree Celsius)

#### Flow meter

### Part Three: Control box

- Drill holes into a plastic box to fit all your electronics. We repurposed a container from an Arduino kit.

TODO ADD PICTURES of the schematic diagram

### Part Four: Connecting Multiple sensors to one Arduino Uno serial port

- Electronically connect the sensors to the port expander and to the Arduino UNO.

- Instruction: [Connecting Multiple sensors to one Arduino Uno serial port](https://www.instructables.com/HOW-TO-EXPAND-ONE-SERIAL-PORT-INTO-EIGHT/)

<img src="/images/port_expander.jpg" alt="port expander" width="50%" height="50%">

### Part Five: Connect sensors to the frame

Attach the camera using the PVC TODO:

### Part Six: Extract the data to CSV file

We use the Python code to extract the data from Arduino serial monitor to csv file. We get this Python code from one online tutorial [Arduino Data Logger (CSV) with Sensors and Python](https://www.learnrobotics.org/blog/arduino-data-logger-csv/). This is the link to our code for this project: [ardunio_to_csv.py](/src/python/ardunio_to_csv.py). You will need to install the pyserial library (`pip install pyserial`) to run this code. Remember to close the Arduino Serial Monitor before running the code.

### Part Seven: Testing

We tested our ROV in a large pool. However, keep in mind that water with chemicals in it such as chlorine and salt water are corrosive and so it is highly recommended that you rinse your ROV with fresh water after testing in corrosive water.

<img src="/images/testing1.jpg" alt="Pool Testing" width="50%" height="50%">

<img src="/images/testing2.jpg" alt="Pool Testing" width="50%" height="50%">

<img src="/images/pooltestingfinal.gif" alt="Pool Testing" width="50%" height="50%">

## References

- [SeaMate](https://seamate.org/)
- [Underwater Robotics Textbook Download](https://drive.google.com/file/d/1fA1dZfQog4u1yjC6PknGXwDlu9EICpK3/view?usp=share_link)
- [Build a Remotely Operated Vehicle (ROV) at Home!](https://www.youtube.com/watch?v=Lnr5YlBl550)
- [Atlas Scientific](https://atlas-scientific.com/)
