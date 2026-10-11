# Morning Routine — Official Landing Page

The official showcase website and interactive web simulator for the **Morning Routine** Android application.

Hosted live on GitHub Pages:  
**[https://del0x3.github.io/morning-routine-site/](https://del0x3.github.io/morning-routine-site/)**

---

## Overview

This repository contains the static source code for the product landing page. The site introduces the core philosophy of Morning Routine, provides a live in-browser touch simulator, breaks down the lockscreen interaction flow, and hosts links to official release builds.

Associated Android Application Repository:  
**[github.com/del0x3/morning-plan](https://github.com/del0x3/morning-plan)**

---

## Features

1. **Interactive In-Browser Simulator:**
   - A desktop and mobile-responsive smartphone mockup that runs the Excalidraw routine flowchart in pure web technologies.
   - Visitors can press and hold cards (`Wake Up`, `Wash Up`, `Drink Water`, `Step Outside`) to experience the animated 650ms fill gesture before locking into a checkmark (`✓`).
   - Long-press to reset tasks back to unchecked.
   - Hand-drawn callout arrows guide visitors to interact with the mockup.

2. **Visual Step-by-Step Walkthrough:**
   - Detailed breakdown of the morning routine sequence:
     - 01: Display turns on (clean canvas overriding system clock and notifications).
     - 02: Hold-to-confirm gesture (accidental tap protection).
     - 03: Decision branching with optional pathways.
     - 04: Swipe-to-unlock directly to Samsung One UI PIN or fingerprint scanner.

3. **High-Resolution Device Comparison:**
   - Direct visual comparison between the Gemini concept board and real screen captures from a physical Samsung Galaxy running Android 15 / 14.

4. **Technical Architecture Overview:**
   - Explains Android Keyguard Window APIs (`showWhenLocked`, `turnScreenOn`), Compose Canvas rendering, and strict offline zero-telemetry architecture.

5. **Direct APK Downloads:**
   - One-click download links connecting directly to GitHub Releases.

---

## Technical Stack

- Semantic HTML5
- Tailwind CSS (responsive layout and utilities)
- Typography: Inter (clean UI) + Kalam (hand-drawn felt marker script)
- Vanilla JavaScript (zero framework dependencies, lightweight hold-and-fill event listeners)
- GitHub Pages (static edge CDN deployment)

---

## Local Development

Preview locally using any static web server:

```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve .
```

Open `http://localhost:8000` in your web browser.

---

## License

Released under the [MIT License](https://opensource.org/licenses/MIT).
