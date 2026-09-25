# Meridian Pulse — Video Concept Reel

A live, in-browser preview of two marketing video concepts built for a fictional global shipping brand, **Meridian**, designed as a portfolio piece for marketing/content roles in the shipping & logistics industry.

**[View the live demo →](https://hwushyam2005.github.io/Meridian_Pulse/)** *(add your GitHub Pages link here once deployed)*

---

## What this is

This project demonstrates two video treatments a marketing team at a global shipping company might commission:

1. **Product Launch Video — "Meridian Pulse"**
   A 45-second launch concept for a fictional real-time container-tracking app. Structure: pain-point hook → logo reveal → live tracking dashboard → proactive delay alert → trust stats → call to action.

2. **Talking-Head Recut Treatment**
   An overlay design system (lower-thirds, kinetic captions, pull-quotes) for repackaging an executive interview or webinar clip into a scroll-stopping social video.

This page is a **CSS-animation simulation** of both concepts' timing and structure, built to be quick to view and share (e.g. with recruiters) without needing any video software or CLI tools. It is not the final rendered video.

## Built with HyperFrames

The original video **compositions** (the real, renderable source) were authored for **[HyperFrames](https://github.com/heygen-com/hyperframes)** — an open-source framework by HeyGen that turns plain HTML/CSS into deterministic MP4 video, rendered via headless Chrome + FFmpeg. It's built so both humans and AI coding agents can write videos as code instead of using a timeline editor.

- HyperFrames repo: <https://github.com/heygen-com/hyperframes>
- License: Apache 2.0

This repo's HTML/CSS demo is a lightweight stand-in for that HyperFrames composition, so the concept can be viewed instantly in any browser or hosted for free on GitHub Pages. The actual `.mp4` deliverables would be produced separately by running the HyperFrames CLI (`npx hyperframes render`) against the original composition files.

## Files

| File | Purpose |
|---|---|
| `index.html` | Page structure and content — the two concept sections and their markup. |
| `style.css` | All visual styling and CSS `@keyframes` animations that drive both looping previews. |

The two are split for readability: `index.html` stays focused on content/structure, `style.css` holds all presentation and animation logic. `index.html` links to the stylesheet with a plain relative path (`<link rel="stylesheet" href="style.css">`), so both files must stay in the same folder for the page to render correctly.

## Viewing locally

Just open `index.html` in any browser (double-click it, or drag it into a browser tab). No build step, server, or install required — it's plain HTML/CSS.
