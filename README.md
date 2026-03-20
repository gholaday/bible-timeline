# Chronos — Biblical Timeline Explorer

An interactive timeline that traces the story of Scripture from the Patriarchs through the early Church, set within the context of world history. Explore how Old Testament events connect to New Testament fulfillments, how doctrine developed through the Church Fathers, and how biblical history intersects with the rise and fall of empires.

## Features

### Timeline View
- **Four parallel tracks** — Old Testament, New Testament, Church History, and World History displayed along a horizontal, zoomable axis
- **Era bands** — Color-coded periods (Patriarchs, Exile, Life of Christ, Roman Empire, etc.) provide context at a glance
- **Event clustering** — Events that overlap at the current zoom level are grouped into expandable clusters
- **Zoom and pan** — Mouse wheel zooms in/out; click-drag pans across 4,500 years of history
- **Event detail cards** — Click any event for its full description, significance, key figures, and scripture references

### Connections View
- **Parallel-column layout** — OT & World events on the left, NT & Church events on the right, with flowing gradient ribbons between connected events
- **37 cross-references** across 7 connection types: prophecy-fulfillment, type-antitype, quotation, thematic, covenant, doctrinal development, and historical echo
- **Hover to explore** — Hovering an event highlights all its connections; hovering a ribbon shows a tooltip with the connection label, type, and scripture references
- **Two-panel detail modal** — Click an event to see its description alongside detailed explanations of how it connects to other events

### Data
- **119 events** spanning from ~2000 BC to ~1000 AD
- **23 eras** across all four tracks plus the intertestamental period
- **37 cross-references** linking events across testaments and into church history
- All data is static TypeScript — no database, no API calls

## Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) 18+
- [pnpm](https://pnpm.io/)

### Install and Run

```bash
git clone https://github.com/gholaday/bible-timeline.git
cd bible-timeline
pnpm install
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Build for Production

```bash
pnpm build
pnpm start
```

## Tech Stack

- **Next.js 16** (App Router) + **React 19** + **TypeScript**
- **Tailwind CSS 4** for styling
- **Framer Motion** for animations (ribbon draw-in, panel transitions, event card entrances)
- Custom SVG for timeline rendering and connection ribbons
- Static data files (no database)

## Project Structure

```
app/                    Next.js pages and layout
components/
  timeline/             Timeline axis, era bands, event dots, event cards, clustering
  connections/          Connections view, ribbon canvas, event columns, modal
  controls/             Header, track toggles, zoom controls, era jumper
data/                   Static event, era, and cross-reference datasets
lib/                    Types, constants, timeline math utilities
docs/plans/             Design documents
```

## Visual Design

The interface uses a "Sacred Codex" aesthetic — warm parchment tones, serif typography, and muted earth colors inspired by illuminated manuscripts.

- **Palette**: Parchment background (#F7F2E8), warm surface (#EDE7D9), deep text (#2C2416)
- **Fonts**: Playfair Display (headings), Source Serif 4 (body), DM Sans (UI), DM Mono (data)

## License

This project is open source. Feel free to use, modify, and distribute.
