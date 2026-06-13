# Display settings

Used on firmware version 1020

<!-- markdownlint-disable MD013 -->

## Game

### Game: DisplayPort1

| Key               | Value | Explanation                                                                                                                                                           |
| ----------------- | ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Refresh Rate      | 240   | The panel's native maximum at 5120×1440. DisplayPort1 carries the Windows PC (RTX 4090), which supports DSC, so it can drive the full 240 Hz within DP 1.4 bandwidth. |
| Black Equalizer   | 13    | Lifts detail in dark areas so figures hiding in shadow stay visible. 13 is the neutral midpoint — higher values wash out blacks, lower values crush shadow detail.    |
| Adaptive-Sync     | On    | Enables VRR (FreeSync Premium Pro / VESA Adaptive-Sync) so refresh tracks the GPU's frame rate, removing tearing without the input lag V-Sync adds.                   |
| Virtual Aim Point | Off   | Overlays a static crosshair on screen. Off — a screen-drawn aim point is a competitive-integrity gray area and not wanted here.                                       |

### Game: DisplayPort2

| Key               | Value | Explanation                                                                                                                     |
| ----------------- | ----- | ------------------------------------------------------------------------------------------------------------------------------- |
| Refresh Rate      | 120   | macOS has poor support for DSC, limit to 120 Hz to stay within DP 1.4-spec bandwidth.                                           |
| Adaptive-Sync     | On    | Enables VRR so refresh tracks the source's frame rate, removing tearing without the input lag V-Sync adds.                      |
| Virtual Aim Point | Off   | Overlays a static crosshair on screen. Off — a screen-drawn aim point is a competitive-integrity gray area and not wanted here. |

## Picture

| Key            | Value       | Explanation                                                                                                                                   |
| -------------- | ----------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Picture Mode   | Custom      | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9)                                                              |
| Brightness     | 50          | SDR backlight level, set to a comfortable level for the room. Has no effect in HDR, where luminance is driven by the content's metadata.      |
| Contrast       | 75          | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9)                                                              |
| Sharpness      | 60          | The neutral midpoint — no added edge enhancement or softening. Above 60 introduces halos around edges, below 60 blurs the native 1:1 image.   |
| Color          | (see below) |                                                                                                                                               |
| Eye Saver Mode | Off         | Warms the white point to cut blue light, which shifts color away from the calibrated target. Off to preserve the Custom/RTINGS white balance. |

### Color

#### Color: SDR

| Key        | Value  | Explanation                                                                      |
| ---------- | ------ | -------------------------------------------------------------------------------- |
| Color Tone | Custom | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9) |
| Red        | 46     | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9) |
| Green      | 53     | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9) |
| Blue       | 48     | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9) |
| Gamma      | Mode1  | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9) |

#### Color: HDR

| Key        | Value  | Explanation                                                                                                                      |
| ---------- | ------ | -------------------------------------------------------------------------------------------------------------------------------- |
| Color Tone | Custom | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9)                                                 |
| Red        | 87     | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9), with gain increased to account for SDR content |
| Green      | 100    | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9), with gain increased to account for SDR content |
| Blue       | 91     | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9), with gain increased to account for SDR content |

## PIP/PBP

| Key          | Value | Explanation                                                                                                                  |
| ------------ | ----- | ---------------------------------------------------------------------------------------------------------------------------- |
| PIP/PBP Mode | Off   | Splits the panel between two inputs. Off so the active source gets the full 5120×1440 canvas instead of a partitioned slice. |

## OnScreen Display

| Key          | Value   | Explanation                                                                            |
| ------------ | ------- | -------------------------------------------------------------------------------------- |
| Language     | English | OSD menu language.                                                                     |
| Display Time | 20 sec  | How long the OSD stays on screen after the last joystick input before auto-dismissing. |

## System

| Key                    | Value        | Explanation                                                                                                                                                        |
| ---------------------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Infinity Core Lighting | (see below)  |                                                                                                                                                                    |
| Local Dimming          | Auto         | Sourced from [RTINGS](https://www.rtings.com/monitor/reviews/samsung/odyssey-g9)                                                                                   |
| 🎧 Volume              | 50           | Output level for the monitor's 3.5 mm headphone jack, kept at the midpoint default.                                                                                |
| Dynamic Contrast       | Off          | Continuously pumps backlight and contrast to match scene content, which crushes detail and causes visible brightness swings. Off for a stable, calibrated picture. |
| Off Timer Plus         | (see below)  |                                                                                                                                                                    |
| PC/AV Mode             | (see below)  |                                                                                                                                                                    |
| Auto Source Switch     | Off          | Stops the monitor from jumping to a newly active input. Off so it holds the chosen source instead of grabbing focus when the other input wakes.                    |
| Key Repeat Time        | Acceleration | Controls how the OSD joystick repeats when held — Acceleration speeds up as you hold, for quicker navigation through long menus.                                   |
| Power LED On           | Working      | Showing the power LED when the display is off seems backward to me.                                                                                                |
| VRR Control            | Off          | Enabling this reduces flicker when frame rates are unstable but drastically increases latency, so we leave it Off.                                                 |

### Infinity Core Lighting

| Key          | Value          | Explanation                                                  |
| ------------ | -------------- | ------------------------------------------------------------ |
| Lighting     | On             | Enables the rear-facing RGB ring on the back of the panel.   |
| Light Effect | Static         | Holds a single solid color rather than cycling or animating. |
| Color        | Row 1 Column 7 | The chosen static color from the palette grid.               |

### Off Timer Plus

| Key       | Value       | Explanation |
| --------- | ----------- | ----------- |
| Off Timer | (see below) |             |
| Eco Timer | (see below) |             |

#### Off Timer

| Key       | Value | Explanation                                  |
| --------- | ----- | -------------------------------------------- |
| Off Timer | Off   | Disables the fixed-countdown auto power-off. |

#### Eco Timer

| Key       | Value | Explanation                                                                        |
| --------- | ----- | ---------------------------------------------------------------------------------- |
| Eco Timer | Off   | Disables the auto power-off that triggers after a stretch of darkened/idle screen. |

## PC/AV Mode

| Key          | Value | Explanation                                                                                                                         |
| ------------ | ----- | ----------------------------------------------------------------------------------------------------------------------------------- |
| HDMI         | PC    | Treats the input as a PC source: full RGB range (0–255), 4:4:4 chroma, and 1:1 pixel mapping with no overscan, so text stays sharp. |
| DisplayPort1 | PC    | Treats the input as a PC source: full RGB range (0–255), 4:4:4 chroma, and 1:1 pixel mapping with no overscan, so text stays sharp. |
| DisplayPort2 | PC    | Treats the input as a PC source: full RGB range (0–255), 4:4:4 chroma, and 1:1 pixel mapping with no overscan, so text stays sharp. |

<!-- markdownlint-enable MD013 -->
