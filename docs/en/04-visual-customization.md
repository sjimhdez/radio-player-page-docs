---
layout: default
title: Visual Customization
---

# Visual Customization

You can tailor the look of the player with theme colors, audio visualizers, and images. All options are per station and are set in **Settings → Radio Player Page Settings**.

**Previous:** [Program Schedule](03-program-schedule.html) · **Next:** [Multiple Stations](05-multiple-stations.html)

## Theme color

Eight color themes are available. All use a dark background; only the accent color changes.

| Theme    | Description        |
|----------|--------------------|
| Neutral  | Default gray accent |
| Blue     | Blue accent         |
| Green    | Green accent        |
| Red      | Red accent          |
| Orange   | Orange accent       |
| Yellow   | Yellow accent       |
| Purple   | Purple accent       |
| Pink     | Pink accent         |

Select the theme from the **Theme Color** dropdown for each station. The default is **Neutral**.

## Visualizers

Four real-time audio visualizations are available. They are loaded only when needed (lazy-loaded) and run only while audio is playing.

| Visualizer          | Type              | Description                    |
|---------------------|-------------------|--------------------------------|
| Oscilloscope        | Waveform (default)| Classic time-domain waveform  |
| Bars Spectrum       | Frequency         | Vertical frequency bars        |
| Amplitude Waterfall | Amplitude         | Cascading amplitude display   |
| Spectral Particles  | Frequency         | Particle-style frequency view  |

Select the **Visualizer** in the station settings. The default is **Oscilloscope**. Visualization requires browser support for the Web Audio API (all modern desktop and mobile browsers support it).

## Images

### Station logo

The **Logo Image** for the station is shown in the player and in system media controls (lock screen, notification, desktop media controls). Recommended size: **512×512 pixels** or larger. Set it in the station block under **Logo Image (Optional)**.

### Background image

The **Background Image** is displayed full-size behind the player. There is no fixed size; use an image that looks good at various screen sizes. Set it under **Background Image (Optional)**.

### Program logo

When you define programs in the [Program Schedule](03-program-schedule.html), you can attach an optional image to each program. Recommended size: **256×256 pixels**. Program logos appear in the schedule modal and in the All Programs modal.

## Notes

- **Responsive design** — The player layout adapts to desktop, tablet, and mobile.
- **iOS** — The volume slider is hidden on iOS because the system controls playback volume. HLS streams use the native Safari player when available.
- **Performance** — Visualizers and streaming libraries (e.g. for HLS/DASH) are loaded on demand to keep the initial page load light.

**Previous:** [Program Schedule](03-program-schedule.html) · **Next:** [Multiple Stations](05-multiple-stations.html)
