# Breadboard Layout and Testing

**Course:** EC EN 340 · **Term:** Fall 2026 · **Type:** Lab
**Tools:** Breadboarding, debugging, oscilliscope

> **One-line summary:** Built a normalized version of the schematic simulated on NGSPICE in a breadboard. Tested using oscilloscopes and waveform generators to input noise signals and power.


## Context

In this project, we were diving into the hands-on electrical components of our receiver board for our laser tag gun. A photodiode was included in our circuitry to capture incoming frequencies, but correct high and low pass filters allowed for amplification of correct player frequencies. Lots was learned about debugging, operational amplifiers, and oscilliscopes in this lab.

## My contribution

- I constructed a working version of our "power rails" for testing so that our op amps centered around 3.3V/2 instead of 0. Constituted of a voltage divider with large capacitors and resistors.
- I debugged our op amp setup, adjusting wiring for correct output voltage and current.
- I tested our board by wiring it to a power output, inputing a noise signal using a waveform generator, using an oscilloscope to analyze the FFT of the output signal, and a multimeter to test voltages around the board.

## Approach

A few changes were made as we worked. Our first setup included the use of two breadboards, to separate the power rails, and the operation amplifier/filters. Our photodiode direction also threw us for a loop at a few points. 

## Result

!First breadboard image: (Porfolio/breadboard.jpeg)

Testing against the gun showed our signal-noise voltage to be above 0.33V. Considering our player signal frequencies achieved voltages close to that number, I would say our project was successful at attenuating non-player frequencies and noise.

