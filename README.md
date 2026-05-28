# Aspen CRM — Phase 1 Prototype

**Standalone clickable prototype** for the new Aspen Sales CRM. Single HTML file, no build step. Open `index.html` directly in any modern browser.

## What this is

A visual prototype of the **Phase 1 essentials** for the Aspen Sales CRM:

- **M1 Foundation** — login + shell + role switcher (Rep / Manager / Owner)
- **M2 Core CRM Objects** — Contacts, Accounts, Business Lines, Tasks
- **M4 Pipeline (basic)** — 7-stage visual kanban, manual transitions, Stage 6 manager gate
- **M5 Rep Dashboard (basic)** — action queue, KPI tiles, top carriers, my book of BLs
- **M9 Migration & Launch** — settings, users, Zoho migration status

## What this is NOT

- ❌ Not part of the Strata CMS prototype (`../da dashboard v2/`)
- ❌ Not a React app — single static HTML for easy sharing
- ❌ Not the production build — pattern reference only, code does not move forward
- ❌ Not Phase 2 — scoring engine, manager intelligence, client health monitoring, full reports all marked as "Phase 2" with a purple badge

## How to view it

Just double-click `index.html`. Loads in any browser. Uses:
- Tailwind via CDN (no install)
- Inter font from Google Fonts
- Inline SVG icons
- Vanilla JS for screen switching

## Visual parity with the CMS

This prototype intentionally mirrors the Strata CMS prototype (`../da dashboard v2/`) in:
- **Same colour palette** — brand-lime #7cb800, nav-navy #1a2b3c, status palette, text scale (all 60+ design tokens lifted from CMS `index.css`)
- **Same typography** — Inter, 400–800 weights
- **Same layout grammar** — 54px nav, 38px role switcher strip, ~228px sidebar, scrollable main
- **Same component idioms** — card patterns, KPI tiles, table styles, status pills

The CRM is architecturally a separate codebase but visually a sibling.

## Screens

1. **Dashboard (default)** — Rep Joe Rivera's daily home
2. **Pipeline** — 7-column kanban with sample BLs
3. **Accounts (Carriers)** — list view with carrier ranking + custom fields
4. **Account Detail** — Travelers Insurance with related BLs, contacts, activity
5. **Contacts** — list with status tiering (Unqualified / Qualified / Active / Inactive / Dead)
6. **Business Lines** — list of all BLs with stage + tier + priority
7. **BL Detail** — Travelers × CAT, with pipeline visual, BL fields, contacts, activity
8. **Tasks & Activities** — tasks panel + auto-logged calls/meetings/emails
9. **Manager Dashboard** — Stage 6 approval queue (the only hard gate) + rep performance
10. **Owner Dashboard** — Mark's cross-company view (Aspen + Optix together)
11. **Reports** — Phase 1 lean MVP set (10 reports)
12. **Settings & Migration** — Users, Zoho migration status, carrier universe

## Try the role switcher

The "View as" strip below the top nav lets you switch between:
- **Sales Rep** (default) — Joe Rivera's view
- **Manager** — Stephen Fry / Sales Manager
- **Owner (Mark)** — cross-company combined view

Each role lands on a different default screen showing what's role-appropriate.

## Phase 2 markers

Anywhere you see a **purple badge or panel labelled "Coming in Phase 2 · Aug 2026"**, that's functionality deliberately deferred — scoring engine, dormancy alerts, manager intelligence (9 views), client health, advanced reports, cadence automation.
