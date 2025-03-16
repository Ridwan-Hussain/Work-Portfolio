# Switch Mode Power Supply

This is a GitHub repo displaying all the files for the 2025 Cooper Union senior project, including the LTSpice simulations, and any final design files (block diagram, schematic, layout, etc.) for any boards manufactured. 

## Goals
The goal of this senior project is to make a Switch Mode Power Supply that can:
- Be SAFE (the 120V from the wall will be stepped down to 24V using a transformer)
- Do AC-DC conversion so it can be used as a lab bench power supply
- Have 2 independent channels that range from 1-20V and 0-3A
- Support series and parallel mode for these channels
- Have a constant USB-C 5V 3A output
- Be power efficient
    - Based on the lab bench Gwinstek SMPS SPD-3606, a good target efficiency is 50%
- Low voltage ripple (<1%)

## Circuitry
Some of the circuitry for the project include:
- Safety Circuits
    - Common choke
    - Zener diodes
    - (@ilona you got this part)
    - OCP
    - UVP
- Diode Rectifier
- Flyback converter
- Buck converter
- Opto-Isolators
- Power MOSFETs and power relays
- USB-C controller
- Feedback loop using an error amplifier
- 3 isolated grounds

## Firmware
Arduino IDE Setup:
- ESP32 Dev Module Board Type
- Upload Speed: 115200

# Contributors
This project was done by a group of three friends:
- Azra Rangwala (EE'25)
- Ilona Lameka (EE'25)
- Ridwan Hussain (EE'25)
