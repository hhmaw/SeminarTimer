# SeminarTimer

[![Open in browser](qr_link.png)](https://htmlpreview.github.io/?https://github.com/hhmaw/SeminarTimer/blob/main/timer.html)

**SeminarTimer** is a single-file fullscreen timer web app designed for classroom or presentation use. It provides a normal countdown mode and a configurable **Teacher Mode** that auto-schedules presentations, Q&A, switching, and breaks based on planned time.

---

## 🚀 Features

- **Fullscreen countdown timer** with large digits
- **Keyboard controls** for quick operation
- **Teacher Mode** (scheduled sessions + auto breaks)
- Breaks inserted based on **planned elapsed time** (not wall clock)
- Settings are saved to **localStorage** (persist across reloads)

---

## 🧭 How to run

1. Open `timer.html` in a browser (double-click or host via local server).
2. Use the UI or keyboard shortcuts to start and control the timer.

---

## 🎛️ Controls

| Key | Action |
|-----|--------|
| Space | Start / pause |
| R | Reset |
| ↑ / ↓ | Add / subtract 1 minute |
| ← / → | Add / subtract 10 seconds |
| F | Toggle fullscreen |

---

## 🧑‍🏫 Teacher Mode

Enable **Teacher mode** in the settings panel to activate a schedule system.

### Schedule components
- **Presentation** (user configurable duration)
- **Questions** (after each presentation)
- **Switch time** (between students)
- **Breaks** (auto inserted after X minutes of **planned** instruction)

### Notes
- Breaks are inserted based on the sum of the planned segment durations, not the timer’s actual run time.
- If a break should land between questions and the next presentation, the app will insert it there.

---

## ⚙️ Settings & Presets

Open the settings panel by clicking the legend text at the bottom of the screen.

### Adjustable settings
- Default timer (minutes)
- Play gong when time hits 0
- Total presentations
- Presentation duration
- Question duration
- Switch duration
- Break interval (min)
- Break length (min)

### Presets
- Use **Save** in the config panel to store the current settings as a preset.
- Presets are identified by a short readable name based on the settings (e.g., `N20m_G` or `T20m_G_P8x10m_...`).
- Select a preset from the dropdown to apply it immediately.
- Delete presets using the **Delete** button.

Settings and presets are stored automatically in the browser.

---

## 📝 File structure

- `timer.html` — single-file app containing HTML/CSS/JS

---

## License

This project is provided as-is for personal and classroom use.
