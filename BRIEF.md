# Portfolio Brief — Ofer Shahal

## Identity
- **Name:** Ofer Shahal
- **Title:** Geospatial Scientist & GIS Project Manager
- **Tagline:** "Turning spatial and transportation data into decisions that shape infrastructure."
- **Location:** Tel Aviv, Israel (hero/sidebar) — currently leading NSDI Zanzibar on assignment in Zanzibar, Tanzania
- **Languages:** Hebrew (native), English (fluent), Portuguese (good)
- **Contact:** shahalo@gmail.com · +972-50-240-7766 · linkedin.com/in/ofer-shahal · github.com/ofer-geo

## Goals
- Present work to two audiences: technical peers and institutional/government stakeholders
- Showcase maps, data products, and research alongside project management leadership
- Feel professional, minimal, and serious — not flashy

## Tech Stack
- **Framework:** Astro (static site)
- **Styling:** Plain CSS, `Inter` typeface, earth-tone palette (deep green accent, warm off-white background)
- **Deployment:** GitHub Pages
- **Maps/data assets:** static screenshots (PNG/JPG) in `public/maps/`, no live Leaflet/MapLibre embeds yet

## Site Structure (as built)
Single-page layout (`src/pages/index.astro`) with a persistent `Sidebar` (identity, contacts, languages) plus a `Hero` and tabbed panel content:

- **Hero** (`Hero.astro`) — name, eyebrow title, tagline, bio, CTAs (View Work / Download CV), stylised Israel map SVG
- **Tabs:**
  - **About** (`TabAbout.astro`) — bio + Tech Stack chips + Soft Skills chips
  - **Portfolio** (`TabPortfolio.astro`) — sub-navigated into three sections: *Data Science & Analysis*, *GIS Project Management*, *Maps & Geospatial Analysis*; each project card links to a dedicated page under `src/pages/projects/`
  - **Resume** (`TabResume.astro`), **Education** (`TabEducation.astro`), **Conferences** (`TabConferences.astro`)
- **Contact** (`Contact.astro`) — email/LinkedIn/GitHub links + footer
- Older standalone components (`About.astro`, `Work.astro`, `Projects.astro`, `CV.astro`) exist but aren't wired into `index.astro` — superseded by the sidebar/tab layout

## Current Project Pages (`src/pages/projects/`)
Data Science: `gtfs-transit-agent`, `escooter-cycling-thesis`, `bus-delay-prediction`, `train-stations-dashboard`, `scooter-supply-policy`
GIS PM: `zansdi`, `ogun-sdi`
Maps: `night-parking`, `contraflow`, `scooter-density`, `parking-policy`, `pride-events`, `service-frequency`

## Assets — status
- [x] CV (`public/cv.pdf`)
- [x] Map/chart screenshots in `public/maps/` (per-project, several each)
- [x] Project descriptions (title, role, tags, outcomes) — filled in per card
- [x] Thesis PDF (`public/thesis.pdf`), scooter policy paper (`public/Scooters_2024.pdf`)
- [ ] Profile photo — not used anywhere yet
- [ ] Interactive maps (Leaflet/MapLibre) — still static images only

## Tone & Voice
- Professional but human
- Confident without being boastful
- Technical detail where relevant (tags, methods, tools), plain language for institutional/PM-facing sections
