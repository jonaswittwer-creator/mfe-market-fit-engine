# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

MFE (Market Fit Engine) is a clickable prototype (Klickdummy) showing how a business consultant works through a dialog with a (simulated) AI to arrive at a reasoned market-entry recommendation. It is being built for the "Agentic Engineering" course. All content is in German.

The repo currently contains only planning docs (`briefing.md`, `PRD.md`, `tech-spec.md`, `design.md`) — no HTML/CSS has been written yet. These four docs are the source of truth and should be read in that order before building screens; implementation must follow them rather than introduce its own conventions.

## Stack and commands

Static HTML + CSS only. No framework, no build step, no package manager, no JavaScript required. There is nothing to install, build, lint, or test — pages are opened directly in a browser or served via GitHub Pages. Verify changes by opening the relevant `.html` file in a browser.

## Architecture

- One HTML file per screen; `index.html` is screen 1. Planned filenames (from `tech-spec.md`):
  `index.html` → `produktdefinition.html` → `ki-erstgespraech.html` → `marktvergleich.html` → `ki-empfehlung.html` → `praesentationsvorschau.html`.
- Single shared `styles.css` used by all screens.
- Navigation is plain `<a href="...">` links between files in the order above — no JS routing, no client-side state. "Weiter" links forward, "Zurück" links back (absent on screen 1).
- Every screen shows a progress indicator "Schritt X von 6".
- Login, the AI chat, market data, and export are all static/fixed content — there is no real backend, AI, or data processing to implement.

## Design system (see `design.md` for full detail)

- Base color: Anthrazit/Blauschwarz; accents: Petrol, Violett, Cyan, with a subtle neon glow on hover/active states (used sparingly, not as flat fills).
- Sans-serif font, minimum 16px body text.
- Colors must be defined as CSS custom properties in `:root` in `styles.css`, using the fixed token names from `design.md` (`--color-bg`, `--color-bg-elevated`, `--color-text`, `--color-text-muted`, `--color-accent-petrol`, `--color-accent-violet`, `--color-accent-cyan`, `--color-glow`, `--color-border`) — don't invent ad hoc color values outside these tokens.
- Formal address ("Sie"), never "Du".
- Numeric/data content must visibly carry a "Demo-Daten" label.
- Designed for desktop width 1440px; no horizontal scroll at that width; must stay readable (not necessarily fully usable) on mobile.
- All interactive elements (buttons, links) must be reachable via Tab.

## Scope boundaries (from `briefing.md` / `PRD.md`)

- V1 covers exactly the 6 screens above. 10 further screens from the overall concept are explicitly out of scope for now and, when tackled, are meant to go through separate branches + PRs each — don't fold them into this work.
- No real AI integration, no real market data, no real login/accounts (login is a demo password `12345678`), no real export (preview only) — do not add real implementations for these; fixed/static content is correct and intentional here.

Lies design.md, bevor du Farben, Schriften oder Layout änderst. Halte diese Datei unter etwa 200 Zeilen.
