# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static website for planning an Amsterdam trip (August 22-24, 2025). Written in Swedish. No build system, no dependencies, no package manager.

## Structure

- `index.html` — Home page with flight details and Airbnb address
- `activities.html` — Activities table with Google Maps links and weather tags (indoor/outdoor/covered)
- `restaurants.html` — Vegan/vegetarian restaurant cards with external links
- `style.css` — Shared stylesheet using CSS custom properties (--canal-blue, --warm-orange, etc.)
- `images/` — Restaurant photos (referenced by cards, with onerror fallback)
- `start.txt` — Original ChatGPT conversation used as source material

## Development

Open any HTML file directly in a browser. No server required. All pages share the same `style.css` and follow the same layout pattern: header, sticky nav, main content, footer.

## Conventions

- All content is in Swedish
- Interactive elements use `onclick` with `window.open()` for external links (Google Maps, restaurant websites)
- Responsive design via media queries at 768px and 480px breakpoints
- CSS grid with `auto-fit` and `minmax()` for card/grid layouts
