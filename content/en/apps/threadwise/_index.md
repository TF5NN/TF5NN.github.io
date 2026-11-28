---
title: Threadwise
summary: Screw thread tools for the workshop. Find out what an unknown thread is, get the figures to make it, and measure it over three wires.
# A short description for the front page. One or two short sentences.
tagline: Identify an unknown thread, get the figures to cut it, and measure it over three wires.
# The day the app went on the site. The front page shows the four newest apps.
date: 2026-11-20
app_url: https://tf5nn.github.io/threadwise/
# The app speaks English and Icelandic: the button opens it in the language being read here.
app_lang: true
repo_url: https://github.com/TF5NN/threadwise
# Tags work the same as on posts. Write them in English in both languages.
tags: ["Metalworking"]
weight: 40
---

Threadwise is three tools in one, all reading from one catalogue of 322 threads in eleven families: metric ISO, UNC/UNF/UNEF, Whitworth BSW/BSF, pipe threads G, R and NPT, metric taper (DIN 158, for grease nipples and plugs), Pg, metric trapezoidal Tr and metric buttress S.

## What it can do

The tabs follow the workshop: find out what you have, make it, measure it.

- **Find**: measure an unknown thread with a caliper and a pitch gauge, and get a ranked list of what it could be. It warns about look-alikes, and can work out the flank angle from two wire sizes, which tells Whitworth from unified without an angle gauge.
- **Make**: sizes to turn or bore, tap drills with the percentage of thread, and depth and infeed for single-point threading, straight in or on the compound.
- **Measure**: what the micrometer should read over three wires, with the limits for the tolerance class, and whether a part you have measured is in tolerance. You type the wire you actually have: it is never assumed.

Tap a result in Find to open it in Make, and Make's **Measure it** button takes it on to Measure. Every tab also works on its own, so skip any step you don't need.

## How far to trust it

Every number is checked against published tables, including the Icelandic *Töflubók*, and the checks are in the repository's validation folder. Where a standard's table has a gap, its formulas fill it and the app says so. Tolerances for Whitworth, Tr and S are not in yet: you type those by hand.

Threadwise is a free hobby project and I take no responsibility for the calculations, or for anything made, measured or accepted with them. Check anything that matters against the standard, with proper gauges.

## Licence

Creative Commons Attribution 4.0 (CC BY 4.0).
