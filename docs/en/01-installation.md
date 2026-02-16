---
layout: default
title: Installation
---

# Installation

This page covers the requirements and steps to install and activate Radio Player Page.

## Requirements

- **WordPress** 5.0 or later  
- **PHP** 5.6 or later  
- A **valid streaming URL** (Icecast, Shoutcast, HLS, DASH, or MP3)

For the best experience, use a modern browser. The audio visualizers use the Web Audio API, which is supported in current versions of Chrome, Firefox, Edge, and Safari (including iOS Safari 10+).

## Installation steps

1. **Upload the plugin** to the `wp-content/plugins/` directory, or install it from the **Plugins** screen (Add New → Upload Plugin or search for “Radio Player Page”).

2. **Activate the plugin** from the **Plugins** screen in WordPress.

3. Go to **Settings → Radio Player Page Settings**.

4. For at least one station:
   - Enter the **Streaming URL** (the full URL of your stream).
   - Select the **Player Page** (the WordPress page where the player should appear).
   - Click **Save Changes**.

5. **Open the assigned page** in your browser. The player loads automatically; you do not need to add any content or shortcode to the page.

## Important note

No configuration is needed on the WordPress page itself. The plugin uses WordPress’s `template_redirect` hook: when a visitor requests a page that is assigned to a station, the plugin serves a standalone HTML page with the player and stops the normal theme from loading. The page content and template you might have set are not used for that URL.

**Next:** [Configuration](02-configuration.html) — Set station name, theme, visualizer, images, and optional program schedule.
