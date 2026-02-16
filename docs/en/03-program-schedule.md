---
layout: default
title: Program Schedule
---

# Program Schedule

The program schedule lets the player show **what is on air now** and **what is coming next**. You define programs (name, optional logo and descriptions), then assign them to time slots for each day of the week. The player uses your WordPress timezone and updates at the start of each minute.

**Previous:** [Configuration](02-configuration.html) · **Next:** [Visual Customization](04-visual-customization.html)

## What the player shows

- **Current program** — Under the station title: program name and time range (e.g. “Morning Show – 08:00–10:00”).
- **Upcoming program** — When the next program starts in 10 minutes or less, an announcement appears (e.g. “Coming up: Noon News in 5 min”).
- **Schedule modal** — A weekly view with the current day first and automatic scroll to the active program; “Back to today” and a close button.
- **All programs modal** — An alphabetical list of all programs with their weekly time slots. Program descriptions and extended descriptions are shown in these modals.

All times are based on the **WordPress timezone** (Settings → General). The “current time” in the player is the station’s time, not necessarily the visitor’s local time. When the station timezone differs from the visitor’s, the timezone clock in the player shows the station time and the offset.

## In the admin: Programs

Expand **Show Program Schedule** for the station. In the **Programs** section:

1. Click **Add Program** for each show you want to define.
2. For each program:
   - **Program name** (required if you use it in the schedule) — Short name shown in the player and in the schedule.
   - **Add Program Image** / **Change Image** — Optional logo; recommended size 256×256 px. Used in the player and in the schedule/modals.
   - Optional **description** and **extended description** (if you use the “Show more fields” area) — Shown in the schedule and All Programs modals.
3. Use **Remove Program** to delete a program. If it is used in any time slot, remove or change those slots first.

Validation: if a program is used in the schedule, it must have a name. The form will show an error and scroll to the first problem if you try to save with a missing name or invalid slots.

*[Figure: Admin program schedule panel with Programs and Schedule by day. Add screenshot as `../../assets/images/admin-schedule-panel.jpg` when available.]*

## In the admin: Schedule

In the **Schedule** section you assign programs to time slots for each day (Monday through Sunday).

1. For the desired day, click **Add Time Slot**.
2. In each slot:
   - **Select Program** — Choose one of the programs you defined.
   - **Start** and **End** — Use 24-hour format (HH:MM). For example, 2:00 PM is 14:00.
3. You can add multiple slots per day. Use **Remove Time Slot** to delete a slot.

### Rules

- **No overlapping slots** on the same day. If two slots overlap, both will show an error (e.g. “This time slot overlaps with: Morning Show”). Fix the times so they do not overlap.
- **Programs that cross midnight** are allowed. For example, a slot from 23:00 to 01:00 is valid; the plugin treats it as spanning midnight.
- Times are stored and displayed in 24-hour format. The player uses the WordPress timezone to decide which program is “now” and which is “next.”

The description under the schedule in the admin summarizes this: assign programs to time slots for each day; the player shows the current and next program and can announce the next one when it starts within 10 minutes; the display uses your site timezone and updates at the start of each minute.

*[Figure: Player with current program and optional “Coming up” announcement. Add screenshot as `../../assets/images/player-now-playing.jpg` when available.]*

*[Figure: Schedule or All Programs modal in the player. Add screenshot as `../../assets/images/program-modal.jpg` when available.]*

## Timezone

The “now” used for the current program and the “next” program announcement is the **WordPress site time** (Settings → General → Timezone). If your station broadcasts in a different timezone, set the WordPress timezone to that of the station. The timezone clock in the player (when visible) shows the station time and the difference from the visitor’s time.

**Previous:** [Configuration](02-configuration.html) · **Next:** [Visual Customization](04-visual-customization.html)
