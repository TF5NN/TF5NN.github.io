---
title: Instructions
weight: 10
---

1. [Open the app](https://tf5nn.github.io/sightline/). The map opens on Iceland.
2. Tap the map to place point A, then point B. Drag a pin to move it. **My location** puts a point where you are.
3. The profile appears under the map: the ground along the path and the line of sight between the antennas. Ground above the line is red.
4. Set the **antenna height** at each end, in metres above the ground.
5. Press **Estimate radio link** and choose a band, a radio and an antenna. The verdict and the numbers behind it appear above the choices.
6. If the two ends are different stations, tick **Different station at each end**.
7. To share or save a path, copy the page address.

## Reading the profile

Move the pointer along the profile, or slide a finger along it on a phone, to read the distance and the ground height at each spot.

- **Blue line**: the line of sight from antenna to antenna.
- **Red**: the ground is above the line.
- **Amber**: the ground is below the line but close to it. Shown with the radio side open.
- **Shaded band**: the Fresnel zone, the space around the line that the signal actually uses.

## Reading the verdict

| Margin | Verdict |
|---|---|
| 20 dB or more | Solid |
| 10 to 20 dB | Good |
| 0 to 10 dB | Marginal |
| below 0 dB | Unlikely |

The margin is how far the received signal is above the weakest signal the receiver can use. Read it as give or take 10 dB.

## Your own figures

**Advanced**, inside the radio side, has the numbers behind the lists: frequency, transmit power in watts or dBm, antenna gain, cable loss and receiver sensitivity. For LoRa you can set the spreading factor and bandwidth. Type over any of them to use your own.

## More

[How it works and how far to trust it](https://tf5nn.github.io/sightline/how.html) explains the model, the terrain data, and how the results have compared with real links.
