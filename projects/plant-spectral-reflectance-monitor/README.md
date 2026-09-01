# Handheld Spectral Device for Chlorophyll Content Estimation

Mini project for RT 508 – Geospatial Technologies in Agro-Rural Sector, SART, IIT Guwahati.

* Submitted by: Harsh H Nair (254154004) & Susan Eldhose (254154009)

## Overview
A spectral device is an analytical instrument that measures the interaction of light with a material across different wavelengths to determine its physical or chemical composition. This project develops a low-cost, portable hyperspectral sensing device using the Hamamatsu C12880MA micro-spectrometer and Arduino UNO to capture leaf reflectance spectra and estimate chlorophyll content — a key indicator of plant vigor, nutrient availability, and biological stress levels — across eight different plant species.

## Objectives
* Design and develop a portable hyperspectral sensing device
* Measure leaf reflectance spectra and estimate chlorophyll content
* Ensure low cost, user-friendliness, and accuracy comparable to commercial devices

## System Design
* **Hamamatsu C12880MA** – Ultra-compact MEMS micro-spectrometer (350–850 nm range, 15 nm resolution, 288 pixels, SPI interface, 5 g weight)
* **Arduino UNO** – ATmega328P-based microcontroller board that interfaces with the sensor, executes code, and streams data (5V, 14 digital I/O, 16 MHz clock)
* **USB Type-A to Type-B Cable** – Connects Arduino to computer for power and data transfer
* **Arduino IDE** – Firmware programming and serial data acquisition
* **Processing Software** – Real-time visualization and interactive analysis of reflectance data
* **Microsoft Excel** – Data storage, averaging, graph plotting, and statistical analysis

## Methodology
1. Understand sensor and microcontroller operation
2. Program Arduino IDE and Processing software for data acquisition
3. Acquire and analyze digital reflectance data from leaf samples
4. Plot and interpret spectral graphs for chlorophyll estimation
5. Design and assemble a compact, enclosed handheld device

## Results
Reflectance spectra were captured across the UV-visible-NIR transition region for eight plant species:
* Arrowhead
* Chinese Evergreen
* Jade Plant
* Zebra Plant
* White Arali
* Money Plant
* Parlour Palm
* Baby Rubber Plant

All species exhibited the characteristic vegetation spectral signature (a green reflectance peak near 550 nm with chlorophyll absorption dips on either side). Succulent plants (Jade) showed higher visible reflectance than thin-leaved species.

## Conclusion
* Successfully designed a low-cost spectrophotometer for chlorophyll estimation
* Hamamatsu C12880MA sensor integrated with Arduino UNO provided accurate spectral measurements across the 340–850 nm range
* The device captured characteristic vegetation reflectance patterns with clear chlorophyll absorption features
* Spectral data was successfully acquired and visualized for eight plant species using Arduino IDE and Processing
* The system shows potential to evolve into a reliable, compact, farmer-friendly spectrometer for real-time plant health monitoring

## Future Applications
* 3D-printed enclosure for the sensor and microcontroller unit
* Development into a low-cost, portable handheld spectrophotometer product
* Application of the PROSAIL model for chlorophyll content estimation
* Integration with a mobile app or Bluetooth for real-time data transfer
* Extension of wavelength range into UV and NIR regions
* Material optimization and miniaturization for improved durability and portability

## References & Credits
* Jechow, A., et al. (2024). Characterizing and Implementing the Hamamatsu C12880MA Mini-Spectrometer for Near-Surface Reflectance Measurements of Inland Waters. *Sensors*, 24(19), 6445.
* Roman, A., et al. (2018). Multispectral satellite imagery and airborne laser scanning techniques for the detection of archaeological vegetation marks.

