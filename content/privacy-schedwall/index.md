---
title: "SchedWall Privacy Policy"
date: 2026-03-18
draft: false
tags: []
---

# Privacy Policy for SchedWall

**Last updated:** March 18, 2026

SchedWall ("the App") is a schedule wallpaper generator for Android, developed by Saimai Lau.

## Data Collection

SchedWall does **not** collect, transmit, or share any personal data. All schedule data, settings, and images are stored **locally on your device** using Android SharedPreferences and internal storage.

## AI Scan Feature (Optional)

The App includes an optional "Scan Photo" feature that sends images to a third-party AI service for schedule recognition. The user chooses their provider and provides their own API key. Supported providers:

- **Anthropic (Claude)** — subject to [Anthropic's privacy policy](https://www.anthropic.com/privacy)
- **OpenAI (GPT-4o)** — subject to [OpenAI's privacy policy](https://openai.com/policies/privacy-policy)
- **Google (Gemini)** — subject to [Google's privacy policy](https://policies.google.com/privacy)

This feature:
- Is entirely opt-in and requires the user to provide their own API key
- Only sends data when the user explicitly initiates a scan
- Sends the image directly to the chosen provider's servers — the App developer does not have access to these images

## Calendar Access (Optional)

The App can optionally read from and write to your device's calendar to import or export schedule events. This feature:
- Requires explicit user permission (`READ_CALENDAR` / `WRITE_CALENDAR`)
- Only accesses calendar data when the user initiates a sync or export
- Does not transmit calendar data to any external server — all processing is on-device

## Permissions

The App requests the following Android permissions:
- **SET_WALLPAPER** — to set the generated schedule as the device wallpaper
- **INTERNET** — required only for the optional AI scan feature
- **READ_CALENDAR** — to import events from the device calendar (optional, requested at runtime)
- **WRITE_CALENDAR** — to export events to the device calendar (optional, requested at runtime)
- **READ_EXTERNAL_STORAGE** (Android 12 and below) — to read the current wallpaper when using the "Current Wallpaper" background option
- **VIBRATE** — for haptic feedback on successful actions

## Third-Party Services

Apart from the optional AI scan integration described above, the App does not integrate with any third-party services, analytics, or advertising platforms.

## Changes

This privacy policy may be updated from time to time. Changes will be posted on this page.

## Contact

If you have questions about this privacy policy, contact: **smlau2003@gmail.com**
