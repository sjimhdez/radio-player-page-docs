---
layout: default
title: Configuration
---

# Configuration

All station settings are managed in **Settings → Radio Player Page Settings**. Each station has its own block of options; this page describes every field.

**Previous:** [Installation](01-installation.html) · **Next:** [Program Schedule](03-program-schedule.html)

## Where to configure

Open **Settings → Radio Player Page Settings** in the WordPress admin. You will see one or more station blocks. For each station you use, fill in at least **Player Page** and **Streaming URL**, then click **Save Changes** at the bottom of the page.

*[Figure: Settings page with general station options. Add screenshot as `../../assets/images/settings-general.jpg` when available.]*

## Fields per station

### Player Page (required)

The WordPress page where the player will appear. Select it from the dropdown. When someone visits that page’s URL, the plugin serves the standalone player instead of the theme. Each station must have a different page.

### Streaming URL (required)

The full URL of your audio stream (e.g. `https://example.com:8000/stream` or an HLS/DASH URL). Supported formats:

- Icecast and Shoutcast  
- HLS (`.m3u8`)  
- DASH (`.mpd`)  
- MP3 streams  

The plugin validates the URL on save and detects the stream type automatically for playback.

### Station Name (optional)

A display title for the station (e.g. “My Radio”). Maximum 64 characters. If left empty, the site title from **Settings → General** is used in the player and in system media controls.

### Theme Color

Dropdown with eight options: **Neutral**, **Blue**, **Green**, **Red**, **Orange**, **Yellow**, **Purple**, **Pink**. All themes use a dark background. Default is **Neutral**.

### Visualizer

Choose the real-time audio visualization: **Oscilloscope** (default, waveform), **Bars Spectrum**, **Amplitude Waterfall**, or **Spectral Particles**. Visualizers are loaded only when needed and run only while audio is playing.

### Logo Image (optional)

The station logo, shown in the player and in lock screen / system media controls. Recommended size: 512×512 pixels or larger. Use **Select Image** to choose from the media library and **Remove** to clear it.

### Background Image (optional)

A full-size image displayed behind the player. Use **Select Image** to set it and **Remove** to clear it.

### Program Schedule (optional)

A collapsible section to define **programs** (name, optional logo, optional descriptions) and a **weekly schedule** of time slots per day. The player then shows the current and next program and can announce the next one when it starts in 10 minutes or less. For full details, see [Program Schedule](03-program-schedule.html).

## Saving changes

Always click **Save Changes** at the bottom of the form after editing. Until you save, your changes are not stored and the player will not reflect them.

**Previous:** [Installation](01-installation.html) · **Next:** [Program Schedule](03-program-schedule.html)
