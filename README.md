# Water Level Indicator Using BC547 Transistors

A breadboard-based three-level water level indicator that uses water conductivity and BC547 NPN transistors to detect rising water levels and illuminate LED indicators.

## Overview
This project implements a simple water level monitoring system powered by a 9 V source. The design uses three sensing levels to indicate low, medium, and high water conditions. As the water rises and reaches each probe, the corresponding transistor switches on and drives an LED output.

The project demonstrates how a weak sensing current through water can be used to control a transistor as a switch, converting a physical water level into a clear electrical indication.

## Features
- Three-level water indication: low, medium, and high
- BC547 NPN transistors used as low-side switches
- LED-based visual output for each water level
- 9 V battery-powered design
- Breadboard implementation using discrete components
- Probe-based sensing using water conductivity

## Components Used
- 9 V battery
- 3 × BC547 NPN transistors
- 3 × 330 Ω resistors
- 3 × LEDs
- Assorted wires
- Breadboard

## How It Works
A common reference probe is placed near the bottom of the water container, while three sensing probes are placed at increasing heights. When water reaches a sensing probe, the water forms a conductive path between that probe and the common reference probe.

This conductive path allows a small base current to flow into the corresponding BC547 transistor. The transistor then switches on, allowing current to flow from the 9 V supply through the LED and current-limiting resistor to ground. As a result, the LED for that level illuminates.

As the water level rises, the LEDs turn on in sequence to show the current level.

## Engineering Concepts Used
- BJT transistor switching
- Low-side switching
- Water conductivity sensing
- Ohm’s Law
- LED current limiting with resistors
- Breadboard prototyping and hardware debugging

## Expected Behavior
- Low water level probe triggers the first LED
- Medium water level probe triggers the second LED
- High water level probe triggers the third LED
- LEDs illuminate progressively as water rises

## Files to Include in This Repository
- `README.md`
- `docs/project-report.pdf`

## Results
The completed circuit operated as a three-stage water level indicator. As water rose and reached each sensing probe, the corresponding LED turned on in sequence. The outputs remained stable during normal operation, indicating that the transistor switching behavior and current limiting were functioning as intended.

## Notes
This project was originally developed as a Circuit Theory I course project and later cleaned up for portfolio use.
