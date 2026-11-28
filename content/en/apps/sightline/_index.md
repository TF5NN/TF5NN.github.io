---
title: Sightline
summary: Terrain profiles for radio links. Place two points on the map and see whether the ground is in the way, and whether a radio link between them would probably work.
# A short description for the front page. One or two short sentences.
tagline: Terrain profiles. Place two points and see if a radio link between them will work.
# The day the app went on the site. The front page shows the four newest apps.
date: 2026-11-16
app_url: https://tf5nn.github.io/sightline/
# The app speaks English and Icelandic: the button opens it in the language being read here.
app_lang: true
repo_url: https://github.com/TF5NN/sightline
# Tags work the same as on posts. Write them in English in both languages.
tags: ["HAM radio", "LoRa", "Maps"]
weight: 30
---

Sightline draws the ground along the straight path between two points and the line of sight between the two antennas. It reads 2 m elevation data straight from the public ArcticDEM archive, so it works for Iceland and other land north of about 60°N.

## What it can do

- **Terrain profile** between any two points, with the Earth's curve included and blocked ground marked in red, on the chart and on the map.
- **Antenna heights** at both ends, for a mast, a roof or a handheld.
- **Radio link estimate**: choose a band, a radio and an antenna, and get the received signal, the margin and a plain verdict.
- **Presets** for 2 m and 70 cm FM and for 868 MHz LoRa mesh (MeshCore and Meshtastic), with your own figures under Advanced.
- **Fresnel zone** on the profile, with grazing stretches marked in amber.
- **Station layers**: show fixed stations on the map, starting with ÍRA's repeaters. Tap one to see how to work it, or use it as point A or B with its power, antenna and height filled in.
- **Stations seen from A**: with a station layer showing, placing point A colours each station by a first link estimate: green should work, amber is marginal, red unlikely. Iceland only.
- **Look around**: the skyline as seen from point A, with compass bearings, the stations and point B marked where they stand. Drag it to turn. Iceland only.
- **Works on a phone**: slide a finger along the profile to read the heights.
- **Light or dark**, following your device, with a button to switch. The choice carries over to the other apps.
- **Share a path**: the page address holds the whole setup.

## Good to know

The verdict is an estimate from a simple model. It has been right about ground blocking a path, and too optimistic on blocked paths in town. Read the margin as give or take 10 dB. [How it works and how far to trust it](https://tf5nn.github.io/sightline/how.html) has the details.

The terrain data is a surface model: buildings and trees count as ground, as they stood when the satellite images were taken.

Your points stay in your browser and in the page address.

## Credits

Terrain: ArcticDEM, Polar Geospatial Center (CC BY 4.0). Map: OpenStreetMap contributors.
