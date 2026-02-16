---
layout: default
title: FAQ
---

# Frequently Asked Questions

**Previous:** [Multiple Stations](05-multiple-stations.html) · **Back to:** [Documentation index](index.html)

## Do I need to configure anything on the WordPress page?

No. Once you assign a page to a station in **Settings → Radio Player Page Settings**, nothing else is required on the page itself. The plugin intercepts requests to that page and serves a standalone HTML page with the player. The page content, template, and any page settings are not used for that URL.

## Where can I get support or report issues?

Use the [WordPress.org support forum for Radio Player Page](https://wordpress.org/support/plugin/radio-player-page/) for questions, feature requests, and bug reports.

## Can I use this for commercial radio stations?

Yes. The plugin is free and open-source (GPLv2 or later) and can be used for both commercial and non-commercial stations.

## Where is the source code?

The source code is on [GitHub](https://github.com/sjimhdez/radio-player-page).

## What stream formats are supported?

The plugin supports:

- **Icecast** and **Shoutcast** — Traditional radio streaming protocols.
- **HLS** (`.m3u8`) — Adaptive streaming; iOS Safari uses native HLS support.
- **DASH** (`.mpd`) — Modern adaptive streaming.
- **MP3** — Standard audio streaming.

The plugin detects the stream type automatically and loads the right player (including optional libraries for HLS/DASH when needed).

## What languages does the player support?

The player interface is available in: English (US), Spanish, Spanish (Mexico), Russian, Dutch, Romanian, Swedish, Galician, and Danish. The language is chosen from the browser (HTML `lang` attribute, then stored preference, then navigator language), with a fallback to English.

## How does the sleep timer work?

You can set the player to stop playback after **30**, **60**, or **120** minutes. A countdown is shown while the timer is active. If you pause playback manually, the sleep timer is cancelled. The timer is only for automatically stopping playback; it does not affect the stream or the station.

## What happens when I uninstall the plugin?

When the plugin is **uninstalled** (removed from the site, not just deactivated), the `uninstall.php` script runs and removes the option `radplapag_settings` from the database. On multisite, it is removed from each site. The option is **not** removed when you only deactivate the plugin.

## Why doesn’t the stream load?

If the player does not start or the stream does not play:

1. **Check the URL** — In **Settings → Radio Player Page Settings**, ensure the **Streaming URL** is correct and reachable (try opening it in a new tab or in another player).
2. **CORS** — If your stream is on another domain, the server must allow requests from your site (CORS headers). Many streaming servers allow this by default; if not, you may need to configure the stream server.
3. **Browser console** — Open the browser’s developer tools (F12) and check the Console tab for errors. Network errors or blocked requests can indicate a wrong URL or CORS issue.
4. **Format** — The plugin supports Icecast, Shoutcast, HLS, DASH, and MP3. Unusual or protected streams may not work.

If the problem continues, describe your setup (stream type, URL format, and any error messages) in the [support forum](https://wordpress.org/support/plugin/radio-player-page/).

**Previous:** [Multiple Stations](05-multiple-stations.html) · **Back to:** [Documentation index](index.html)
