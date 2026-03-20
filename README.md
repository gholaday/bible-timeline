# Kronos — Biblical Timeline Explorer

An interactive educational tool for exploring the story of Scripture from the Patriarchs through the early Church, set within the context of world history. Trace how Old Testament events connect to New Testament fulfillments, how doctrine developed through the Church Fathers, and how biblical history intersects with the rise and fall of empires.

## Features

### Timeline View
- Four parallel tracks — Old Testament, New Testament, Church History, and World History displayed along a horizontal, zoomable axis
- Color-coded era bands provide period context at a glance (Patriarchs, Exile, Life of Christ, Roman Empire, etc.)
- Events that overlap at the current zoom level are grouped into expandable clusters
- Mouse wheel zooms in/out; click-drag pans across 4,500 years of history
- Click any event for its full description, significance, key figures, and scripture references

### Connections View
- Parallel-column layout with OT & World events on the left, NT & Church events on the right, with flowing gradient ribbons between connected events
- 37 cross-references across 7 connection types: prophecy-fulfillment, type-antitype, quotation, thematic, covenant, doctrinal development, and historical echo
- Hover to explore — highlighting an event reveals all its connections; hovering a ribbon shows the connection details
- Two-panel detail modal with event description alongside detailed explanations of each connection

### Data
- 119 events spanning ~2000 BC to ~1000 AD
- 23 eras across all four tracks plus the intertestamental period
- 37 cross-references linking events across testaments and into church history

## Tech Stack

- Next.js 16 (App Router) + React 19 + TypeScript
- Tailwind CSS 4
- Framer Motion
- Custom SVG rendering
- Static TypeScript data files (no database)

## Getting Started

```bash
git clone https://github.com/gholaday/bible-timeline.git
cd bible-timeline
pnpm install
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000).
