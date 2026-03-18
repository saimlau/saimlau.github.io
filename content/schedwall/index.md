---
title: "SchedWall — User Manual"
date: 2026-03-18
draft: false
tags: []
---

# SchedWall User Manual

**SchedWall** turns your weekly schedule into a beautiful phone wallpaper. Add events manually, import from your calendar or ICS files, scan a photo with AI, customize the look, and set it as your wallpaper — all in one app.

---

## Getting Started

1. **Install** SchedWall from Google Play
2. **Add your first event** by tapping the **+** button
3. Fill in the title, location, day, and time
4. Your schedule appears in the wallpaper preview
5. Tap **Set as Wallpaper** to apply it

---

## Adding & Editing Events

### Manual Entry
- Tap **+** to open the event editor
- Enter a **title** (e.g., "AA 327") and **location** (e.g., "Ceras 300")
- Select the **day of week** (Mon–Sun)
- Toggle **All Day** for events without specific times
- Set **start** and **end** times using the time picker
- For **multi-day events**, select a different end day (e.g., Tue 10am to Wed 10am)
- Choose a **color** from the palette
- Set the event's **time zone** if different from your display timezone
- Tap **Save**

### Editing
- Tap any event in the **event list** below the preview to edit it
- Tap any event **on the wallpaper preview** itself to edit it directly

### Deleting
- Tap the **trash icon** on an event card to delete it

---

## Importing Events

### From Device Calendar
1. Tap **Sync Cal** (or **導入日曆** in Chinese)
2. Grant calendar permission if prompted
3. Select a **date range** (This Week, Next Week, 4 Weeks, or custom dates)
4. Tap **Sync** — found events appear with checkboxes
5. Uncheck any events you don't want, then tap **Import Selected**

### From ICS Files
1. Tap **ICS File** and select a `.ics` file from your device
2. Or tap an `.ics` attachment in email — SchedWall will appear in "Open with"
3. Review events with checkboxes and tap **Import Selected**

### AI Photo Scan
1. Tap **Scan** and pick a photo of a schedule (poster, flyer, printed timetable)
2. First-time setup: choose your **AI provider** (Claude, GPT-4o, or Gemini) and enter your API key
3. The AI extracts events from the image
4. Review with checkboxes and tap **Import Selected**

**API key sources:**
- Claude: [console.anthropic.com](https://console.anthropic.com)
- GPT-4o: [platform.openai.com/api-keys](https://platform.openai.com/api-keys)
- Gemini: [aistudio.google.com/apikey](https://aistudio.google.com/apikey)

---

## Exporting Events

Tap **Export Events** to share your schedule:
- **To Calendar** — writes selected events to your device's primary calendar
- **Share ICS** — generates an ICS file and opens the share sheet (email, Drive, etc.)

Both options let you select which events to export with checkboxes.

---

## Customization

Open **Settings** (gear icon in the top bar) to customize your wallpaper.

### Time Range
- **Auto-fit**: the grid automatically adjusts to show only the hours your events occupy
- **Manual**: set a fixed start and end hour (e.g., 8 AM to 6 PM)

### Visible Days
Toggle which days appear on the wallpaper. Default is Mon–Fri. Tap any day chip (Mon through Sun) to show or hide it.

### Display Timezone
Events are converted to this timezone on the wallpaper. Useful if you travel or have events in different timezones.

### Background
- **Solid Color** — uses the theme's background color
- **Current Wallpaper** — captures your current phone wallpaper as the background (the original is saved so re-applying won't stack schedules)
- **Choose Image** — pick any photo from your gallery. A crop/position screen lets you pan, pinch-zoom, and rotate the image. Tap the **rotate icon** for 90° steps or **0°** to reset

### Theme
Choose from 5 presets: **Default**, **Dark**, **Warm**, **Ocean**, **Forest**

Or customize individual colors:
- Background, Header, Grid Lines, Time Labels, Event Border, Event Text

Editing any color automatically saves as a **Custom** theme you can return to after trying presets.

### Font
- Choose from **default**, **sans-serif**, **serif**, or **monospace**
- Adjust **text size** with the slider (70%–150%)

### AI Scan Provider
Switch between Claude, GPT-4o, and Gemini. Each provider stores its own API key separately.

### Language
Switch the app language: **English**, **繁體中文**, **简体中文**, **Español**, **日本語**, **한국어**, or **System Default**

Changes apply instantly — no restart needed.

---

## Weekly Auto-Sync

In the **Sync Cal** dialog, toggle **Weekly auto-sync** to automatically:
1. Pull this week's events from your device calendar
2. Re-render the schedule wallpaper
3. Set it as your wallpaper

Runs once per week via Android's WorkManager. Battery-friendly — a few seconds of work, then sleeps.

---

## Tablet & Chromebook

- **Tablets** and **Chromebooks** get a side-by-side layout in landscape: preview on the left, controls and event list on the right
- **Phones** are locked to portrait for a better experience

---

## Wallpaper Tips

- The wallpaper is rendered at your phone's **exact screen resolution** for a pixel-perfect fit
- **Top and bottom margins** are left blank for the status bar and navigation bar
- Tap **Save to Gallery** to export the wallpaper as an image (saved to `Pictures/SchedWall/`)
- Long text in event blocks **wraps** automatically

---

## Permissions

| Permission | Purpose | When requested |
|---|---|---|
| SET_WALLPAPER | Set home & lock screen wallpaper | Automatic |
| INTERNET | AI photo scan feature only | Automatic |
| READ_CALENDAR | Import events from device calendar | On first sync |
| WRITE_CALENDAR | Export events to device calendar | On first export |
| READ_EXTERNAL_STORAGE | Read current wallpaper (Android 12-) | On background selection |
| VIBRATE | Haptic feedback on success | Automatic |

---

## Privacy

SchedWall stores everything **locally on your device**. No account required, no data collected. The optional AI scan sends images to your chosen provider's servers (Anthropic, OpenAI, or Google) using your own API key. See the full [Privacy Policy](/privacy-schedwall/).

---

## Support

For bug reports and feature requests: [smlau@stanford.edu](mailto:smlau@stanford.edu)
