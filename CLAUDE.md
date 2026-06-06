# CLAUDE.md

Project: Personal academic website for Kumar P. Tripathy (hydroclimatic extremes, XAI, drought research).

## Stack
- Static site, single index.html (HTML + CSS + vanilla JS). No build step.
- Deployed on GitHub Pages.
- Fonts: Fraunces (display), Karla (body), JetBrains Mono (code).
- Theme: warm paper background, terracotta accent (#b1471a), teal for wet anomalies (#1f6f6b). Keep this palette.

## Structure
Four tabs, all in index.html, switched via JS (hash routing):
1. Home: bio, photo, education (one-liners), publications (one-liners, no DOI clutter), interests.
2. Research: cards (figure + short explanation + code snippet).
3. Blog: post cards. Later: separate markdown posts.
4. Software: interactive drought index explorer (FlashCAT demo). SPI is implemented client-side (Thom gamma fit, normal transform). EDDI-14/28, ESI, SESR, SMVI are stubbed as "coming soon".

## Rules
- Keep all content crisp. One-liners for education and publications.
- No em-dashes anywhere.
- Do not bloat: prefer editing index.html over adding frameworks. Ask before adding React/Vite/etc.
- The SPI demo math (gammaP, invNorm, computeSPIcell) is verified. Do not change without re-testing mean~0, sd~1.
- Real data later: precompute index fields in Python to JSON, load via fetch. Do not compute heavy indices in the browser beyond SPI.

## Owner preferences
- Direct, informal communication. No sycophancy.
- Publication-quality aesthetics. Avoid generic AI styling (purple gradients, Inter font).
