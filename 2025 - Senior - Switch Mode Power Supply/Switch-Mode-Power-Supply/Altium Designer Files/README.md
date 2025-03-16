Note: The board is nearly finished, will be gerbered out soon, this is what the current board looks like. The final Altium project will be zipped here as well once the board has been gerbered out.

These are files from the Altium Designer for the Schematic and the Layout. If the schematic is difficult to see, it can also be viewed in the SMPS_Schematic.pdf file. 

# Schematic
## Page 1 - External
![Schematic_Page_1_External](/Altium%20Designer%20Files/Altium%20Images/Schematic_Page_1_External.png)

This page has all of the external connectors for the board: XT30 connectors for the input and channels, buttons, and potentiometers.

## Page 2 - Circuits
![Schematic_Page_2_Circuits](/Altium%20Designer%20Files/Altium%20Images/Schematic_Page_2_Circuits.png)

This page has most of the core circuitry for the SMPS Channel A & B. This includes diode bridge rectifier, 5V and 3V3 power lines, flyback converters, HV (from flyback) and LV (buck converter), current sense, over voltage protection, output A & B enable, parallel & series mode relays, voltage & current knobs, temperature sensor, feedback circuit, and the feedback transformer.

## Page 3 - MCU & USB
![Schematic_Page_3_MCU_USB](/Altium%20Designer%20Files/Altium%20Images/Schematic_Page_3_MCU_USB.png)

This page has the pins for both MCU A (Channel A) and MCU B (Channel B & C), as well as the USB2.0 circuitry to support USBC charging.

## Page 4 - Additional Circuits
![Schematic_Page_4_Additional](/Altium%20Designer%20Files/Altium%20Images/Schematic_Page_4_Additional.png)

This page has the rest of the circuits that didn't fit on the 2nd page. This includes voltage feedback from Channel B to A, fault indicator from Channel A to B, LEDs, and Channel B ON/OFF logic (more complicated due to independent, series, and parallel mode support).

# Layout
## Components 
![Layout_Components](/Altium%20Designer%20Files/Altium%20Images/Layout_Components.png)

This image shows all the components and all the traces on the board.

## Top Layer
![Layout_Top_Layer](/Altium%20Designer%20Files/Altium%20Images/Layout_Top_Layer.png)

This image shows all of the top layer polygon pours.

## Layer 1
![Layout_Layer_1](/Altium%20Designer%20Files/Altium%20Images/Layout_Layer_1.png)

This image shows all of the layer 1 polygon pours.

## Layer 2
![Layout_Layer_2](/Altium%20Designer%20Files/Altium%20Images/Layout_Layer_2.png)

This image shows all of the layer 2 polygon pours.

## Bottom Layer
![Layout_Bottom_Layer](/Altium%20Designer%20Files/Altium%20Images/Layout_Bottom_Layer.png)

This image shows all of the bottom layer polygon pours.

## 3D View
![Layout_3D](/Altium%20Designer%20Files/Altium%20Images/Layout_3D.png)

This image shows the 3D view of the board.