#  Handheld Spectral Device for Leaf Chlorophyll Estimation

An affordable and portable spectral sensing device developed for the non-destructive estimation of leaf chlorophyll content and monitoring of plant health and stress.

---

## Overview

Development of a handheld spectral sensing system designed to measure leaf reflectance across the 350–850 nm spectral range. The device is intended to support the assessment of plant health, nutrient status, and stress conditions based on the spectral characteristics of leaves.

The system integrates the Hamamatsu C12880MA MEMS micro-spectrometer with an Arduino UNO development board, providing a compact and cost-effective alternative to conventional commercial spectroradiometric systems.

---

## Hardware Components

- **Spectral Sensor:** Hamamatsu C12880MA MEMS Micro-Spectrometer
  - Spectral range: 350–850 nm
  - Spectral resolution: approximately 15 nm
  - 288-pixel photodiode array

- **Microcontroller:** Arduino UNO (ATmega328P)

- **Communication Interface:** USB Type-A to Type-B cable for power supply and serial data transmission

---

## Software and Technologies

- **Arduino IDE (C/C++):** Used for microcontroller programming, sensor control, generation of clock and start signals, and acquisition of raw spectral data.

- **Processing Environment:** Used for graphical data acquisition and real-time visualization of spectral curves through serial communication.

- **Data Processing:** Excel and Python-based tools can be used for wavelength calibration, spectral averaging, data processing, and reflectance analysis.

---

## Key Features and Findings

- **Spectral Measurement:** Captures leaf spectral characteristics across the 350–850 nm range.

- **Vegetation Spectral Features:** Enables observation of characteristic vegetation reflectance patterns, including the green reflectance region and red-edge transition.

- **Chlorophyll Assessment:** Spectral absorption and reflectance characteristics can be used to support non-destructive estimation of leaf chlorophyll content.

- **Multi-Species Evaluation:** The system was evaluated across eight plant species:
  - Arrowhead
  - Chinese Evergreen
  - Jade Plant
  - Zebra Plant
  - Money Plant
  - Parlour Palm
  - Baby Rubber Plant
  - White Arali

---

## Future Enhancements

- Development of a custom 3D-printed enclosure for improved portability and field deployment.
- Integration of the PROSAIL radiative transfer model for automated chlorophyll quantification.
- Incorporation of Bluetooth or Wi-Fi connectivity for wireless data transmission.
- Development of a mobile-based interface for real-time spectral visualization and plant health assessment.

---

## Project Significance

Crop HySense demonstrates the potential of combining compact MEMS spectrometry with low-cost microcontroller technology to develop an accessible platform for non-destructive plant phenotyping, chlorophyll estimation, and precision plant stress monitoring.
