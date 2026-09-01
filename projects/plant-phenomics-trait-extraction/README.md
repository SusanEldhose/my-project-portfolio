# Automated Plant Trait Extraction from Images (Plant Phenomics)

Mini project for **RT 524 – Digital Agriculture and Advanced Analytics**, SART, IIT Guwahati.

- **Supervisor:** Dr. Dipankar Mandal, Assistant Professor, SART, IITG
- **Presented by:** Susan Eldhose (M.Tech, 2025–27) & Akanksha (PhD, 2025)
- **Date:** 21-04-2026

## Overview

Plant phenomics is the study of measuring and analyzing plant characteristics (traits) using digital tools and technology. This project builds an **automated plant analysis pipeline** that extracts leaf-level traits directly from time-lapse plant images, removing the need for manual measurement.

## Objectives

- Develop an automated plant analysis pipeline
- Measure:
  - Leaf count
  - Leaf length
  - Growth trends over time

## Methodology

The pipeline processes images in batches through the following stages:

1. **Image Segmentation** – Separates the plant from the background using:
   - **Lab color space** (uses green channel properties)
   - **Excess Green Index (ExG)** (highlights vegetation)
2. **Morphological Cleaning** – Removes noise from the segmented mask
3. **Skeletonization** – Reduces the plant to a 1-pixel-wide structure (centerline), enabling:
   - Leaf length calculation
   - Tip detection
4. **Tip & Noise Detection** – Filters edge tips and removes short branches from the skeleton
5. **Leaf Detection & Length Measurement** – Identifies individual leaves via bounding boxes and computes their length

## Results

For each observation day, the pipeline produces:

- **Leaf count per day** – number of leaves detected per observation
- **Individual leaf length** – length of each leaf, measured in pixels
- **Image segmentation output** – plant regions separated from the background
- **Skeletonized structure** – 1-pixel-wide leaf centerlines
- **Bounding boxes** – individual leaves identified and enclosed for visualization
- **Growth trend plot** – leaf count plotted against time to show the growth pattern

Sample results are shown across multiple observation windows (e.g., Day 001–09, Day 008–19, Day 070–11, Day 076–24, Day 104–24), tracking how leaf count and structure evolve over the plant's growth cycle.

## Future Applications

- Development of high-yield, stress-resistant crops
- Precision agriculture through real-time plant monitoring
- Early disease detection using image analysis
- Greenhouse automation and smart farming systems
- Crop growth prediction and yield estimation

## References & Credits

- Ref & Credit: Plant Vision Initiative / UNL


