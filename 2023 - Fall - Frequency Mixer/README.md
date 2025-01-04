# Frequency Mixer
Built a frequency mixer that mixed a Colpitts Oscillator and a function generator output using a differential pair and tail current source as the mixer architecture on a bread board.

The final oscilloscope outputs can be seen in the report, as well as images for all the outputs. The Colpitts Oscillators was created in a previous project and has a frequency output of 4MHz and was chosen as the RF in this scenario (the input for the different pair structure). The function generator had an output waveform of 4.78MHz and was chosen as the LO in this scenario (the input for the tail current source). The output frequency of the mixer was 320kHz as expected.

A second experiment was done where the Colpitts Oscillator had a frequency of 4MHz, the function generator had a frequency of 4.6MHz, and the output frequency was 600kHz. Using this setup, a low pass filter was added at the end of the output to make the difference frequency the dominant frequency. 

The LTSpice files are also attached since the simulation files gave a starting point on what the final circuit should look like. In addition, the project description is also attahced.