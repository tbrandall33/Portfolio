# Two-Stage Op-Amp Amplifier/Filter Design

**Course:** EC EN 340 · **Term:** Fall 2026 · **Type:** Design project
**Tools:** NGSPICE

> **One-line summary:** "Designed a two-stage op-amp section that amplifies a 1-5 kHz signal while rejecting 100 Hz and 20 kHz noise."

## Context
The goal was to design a two-stage op-amp section that amplifies a 2 kHz current-source signal (and anything between roughly 1200 Hz and 3700 Hz) while attenuating 100 Hz and 20 kHz noise sources. Because the op-amp gain also amplifies the noise, the filters had to be chosen carefully. The design was verified in simulation against a netlist-based check requiring the output signal minus noise ("receiver strength") to exceed 0.2 V.

## My contribution
I approached many different topologies and filter setups to accomplish the necessary signal and noise difference. My ultimate setup contained two inverting operational
amplifiers with passive low pass filters placed on the feedback loops, and high pass filters placed in between stages. Other low pass filters were places near noise signals to attenuate as much as possible. 

## Result

(Porfolio/opamp-schematic.png)

The result came back with a Vs-Vn of about 2.4 V! Although these resistor/capacitor values may be difficult to find, and so I may go back to an older version with a 
similar design and more realistic values. 

## What went wrong, and what I changed
I had some difficuly with adjusting the passive low pass filters in the feedback loop. Changing those values regularly impacted my gain and affected my result. Eventually, bumping up the values a few magnitudes seemed to solve the issue.


