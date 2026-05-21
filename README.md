# FMG Platform — UI Kit Specification

A self-contained single-page reference document for the Food Made Good Standard platform rebuild (SRA, April 2026).

## What this is

This is a static HTML file that runs entirely in the browser — no build step, no server, no dependencies to install. It documents:

- **All pages per user journey** — 8 journeys across Client, SRA Staff, and Shared flows, including pages not covered in the wireframes (MFA screen, read-only views, diff view, error states, etc.)
- **UI kit component inventory** — 45 components with states, variants, and WCAG 2.2 AA implementation requirements
- **Component usage map** — for every component, which journeys and pages it appears in

## Usage

Open `index.html` directly in a browser — no local server needed.

Or host it anywhere static: GitHub Pages, Netlify, Vercel, etc.

### GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your spec will be live at `https://[username].github.io/[repo-name]/`

## Contents

```
index.html   — Everything: React app, all data, all styles, self-contained
README.md    — This file
```

## Project context

- **Client:** The Sustainable Restaurant Association (SRA)
- **Platform:** Food Made Good Standard v2 MVP
- **Dev partner:** Yoyo Design
- **Date:** April 2026
- **Tech stack:** React 18 + .NET Minimal API + Azure SQL + Auth0

## Journeys covered

| # | Journey | Type |
|---|---------|------|
| J1 | Onboarding & Account Setup | Client |
| J2 | Completing a Submission | Client |
| J3 | Evidence Library | Shared |
| J4 | Assessment Authoring | SRA Staff |
| J5 | Submission Evaluation | SRA Staff |
| J6 | Feedback & Actions | Client |
| J7 | Dashboard, Reporting & Export | Shared |
| — | Shared / Global Pages | Shared |

## Component categories

- **Inputs** (17) — buttons, text inputs, textarea, radio, checkbox, toggle, select, combobox, date picker, file upload, slider, rich text, search, language selector
- **Navigation** (6) — sidebar nav, breadcrumb, tabs, pagination, step progress, assessment section nav
- **Feedback** (8) — toast, inline error, alert banner, auto-save indicator, progress bar, skeleton loader, empty state, star rating
- **Layout** (8) — card, modal, drawer, tooltip, popover, accordion, split panel, diff panel
- **Data display** (8) — data table, status badge, avatar, notification item, evidence card, score summary, stat card, timeline
- **Overlays** (5) — confirmation dialog, loading overlay, evidence preview, assign question modal, score override modal
