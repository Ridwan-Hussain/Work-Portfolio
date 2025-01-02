# Brake-by-Cable for Autonomy Lab
The purpose of the Brake-by-Cable (BBC) board was to support the new braking motor on the Polaris Gem e2 for the IGVC Competition. The PCB housed the motor controller to adjust the speed of the motor, as well as have a boost converter to power the brake pressure sensor, parking brake, and interfaced with the ESP32 base board to help control the braking power of the car. 

The motor was controlled mainly using the (Pololu 2991 motor controller)[https://www.pololu.com/product/2991]. The main considerations for this part was making sure the motor controller can be directly interfaced with the ESP32, creating large enough traces and power planes so the motor can draw 5A+ if needed, and making sure the two power planes are isolated from each other.

The main considerations for the brake pressure sensor was to ensure it could be powered properly, which required a boost converter to convert the 12VDC to 17VDC, and increasing the viable data range of the brake pressure sensor. This was achieved using a cascaded OpAmp circuit where the first stage was an non-inverted OpAmp and the second stage was an difference amplifier. This allows the voltage to be increased and the base voltages to be decreased, so the voltage range can go from 0.7V-2V to 0.2V-2.3V, abiding by the ESP32 ADC range.

The main considerations for the parking brake is making sure the parking brake is activated when there is no power from the ESP32 by utilizing an electromagnet, and allowing the parking brake to go down if the nodes are turned on.

## LTSpice Simulations
- Files that include the simulations used to test the ADC range for the brake pressure line for better voltage range for the ESP32.

## PCB Files
- Files that include images of the PCB Schematic and Layout, as well as a zip of the final EasyEDA files for the PCB. The images are displayed below. 

![Schematic](./PCB%20Files/Schematic_BBCPCB-v2.0.1_2024-04-30.png)

Image displaying the final schematic. The different circuit parts can be seen in the different blocks.


![Layout TOP](./PCB%20Files/Layout_TOP_BBCPCB-v2.0.1_2024-04-30.png)

Image displaying the final layout on the top layer. The routing and different planes can be seen here.


![Layout BOT](./PCB%20Files/Layout_BOT_BBCPCB-v2.0.1_2024-04-30.png)

Image displaying the final layout on the bottom layer. The routing and different planes can be seen here.


![Layout 2D](./PCB%20Files/Layout_2D_BBCPCB-v2.0.1_2024-04-30.png)

Image displaying the final 2D layout. The various silkscreen can be more easily be seen here.


![Layout 3D TOP](./PCB%20Files/Layout_3D_TOP_BBCPCB-v2.0.1_2024-04-30.png)

Image displaying the final 3D layout on the top side. This displays an accurate image of how the final looked.


![Layout 3D BOT](./PCB%20Files/Layout_3D_BOT_BBCPCB-v2.0.1_2024-04-30.png)

Image displaying the final 3D layout on the bottom side. This displays an accurate image of how the final looked.