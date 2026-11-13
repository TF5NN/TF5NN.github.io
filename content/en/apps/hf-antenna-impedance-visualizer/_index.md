---
title: HF Antenna Impedance Visualizer
summary: See how the feedpoint impedance of end-fed and dipole wire antennas changes with wire length and feedpoint position, across the HF bands from 160 m to 6 m.
app_url: https://tf5nn.github.io/HF-Antenna-Impedance-Visualizer/
repo_url: https://github.com/TF5NN/HF-Antenna-Impedance-Visualizer
weight: 10
---

An interactive, browser-based educational tool for amateur radio operators. It draws the impedance a wire antenna presents at its feedpoint, so you can see why some wire lengths are easy to match on several bands and others are not.

## What it can do

- **Eleven HF bands**, 160 m through 6 m, each one switchable.
- **Two modes.** End-Fed shows impedance against wire length. Dipole shows impedance against feedpoint position, from centre-fed to off-centre-fed.
- **Matching zones** shaded on the graph: 49:1, 9:1 with a tuner, and 1:1 for end-feds; 1:1, 4:1, 6:1 and a custom ratio for dipoles.
- **Sweet Spots** highlights wire lengths where several bands land inside a matching zone at once.
- **Antenna tuner** check with three presets and a custom range.
- **Counterpoise** and **velocity factor** controls, and height above ground in Dipole mode.

## What it does not cover

The tool models long wires, where standing waves decide the impedance. It is not valid for electrically short antennas or whips with loading coils. The [README on GitHub](https://github.com/TF5NN/HF-Antenna-Impedance-Visualizer#readme) explains why.

## Licence

Creative Commons Attribution 4.0 (CC BY 4.0).
