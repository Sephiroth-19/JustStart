# 🕒 Non-24 Biological Clock (Custom Day-Length Clock)

A minimalist web app that simulates a **Non-24-hour circadian rhythm** — perfect for tracking or experimenting with delayed sleep cycles and custom “biological days”.

> 🌐 Live demo: [[https://sephiroth-19.github.io/non24-clock/](https://sephiroth-19.github.io/non24-clock/)](https://sephiroth-19.github.io/JustStart/)

---

## 🧭 Overview

This project provides a **fully client-side web clock** that visualizes time according to a **custom day length** (e.g., 25-hour day) rather than the normal 24-hour cycle.  
It allows users to define their own *biological midnight* and persist settings across sessions.

---

## ✨ Features

- 🕐 **Custom day length** (anywhere between 23 – 30 hours)
- 🎯 **Anchor time (“biological midnight”)** — set your own 00:00 reference
- ⏱ **Analog dial + digital time** display, dynamically updated
- 💾 **Persistent settings** stored locally (`localStorage`)
- 📱 **Responsive layout** (works on both desktop and mobile)
- 🔄 **Next 00:00 prediction** — shows when your next biological midnight occurs in local time
- ⚙️ **No server / no backend** — pure HTML + CSS + JavaScript
- ☁️ **Runs entirely on GitHub Pages**

---

## 🧩 How It Works

1. The app calculates biological time as a linear function of local real-time, using your chosen *day length* (in hours).  
2. When you set an **anchor point**, that local moment is treated as `00:00` in your custom cycle.  
3. The clock face is drawn dynamically with canvas (`<canvas>`), adjusted for your day length.  
4. Data such as day length and anchor time are stored in `localStorage`, so your settings persist after refresh.

---

## 🖥️ Tech Stack

| Layer | Technology |
|-------|-------------|
| Frontend | HTML 5, CSS 3, Vanilla JavaScript |
| Storage | Browser `localStorage` |
| Hosting | GitHub Pages |
| Visualization | HTML Canvas API |

---

## 🚀 Deployment

1. Clone this repository  
   ```bash
   git clone https://github.com/Sephiroth-19/non24-clock.git
   cd non24-clock
