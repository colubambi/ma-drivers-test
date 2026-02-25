# 🚗 Massachusetts Learner's Permit Practice Test

A full-featured practice test app for the Massachusetts RMV Learner's Permit exam — built using AI-assisted development.

**[Live Demo →](https://colubambi.github.io/ma-drivers-test)**

---

## Overview

This project was built to help people preparing for the Massachusetts RMV Learner's Permit written exam. It mirrors the real test format (25 questions, 25 minutes, 72% to pass) and includes questions drawn from the official MA Driver's Manual.

I built this as a hands-on demonstration of AI-assisted development — using Claude AI to implement features while I handled product design, requirements, UX decisions, and testing.

---

## Features

- **3 test modes** — Timed (real RMV format), Practice (no time limit), Adaptive (difficulty adjusts as you go)
- **5 question categories** — Full test, Signs & Signals, Laws & Regulations, Safety & Emergencies, Fines & Penalties
- **Per-question explanations** — every answer includes the relevant rule from the MA Driver's Manual
- **Hint system** — up to 3 hints per test that eliminate an incorrect option
- **Bookmarking** — flag questions mid-test to review later
- **Answer review** — full breakdown of every question after the test
- **Performance analytics** — accuracy rate, per-category breakdown, fastest/slowest question times
- **Score trend chart** — SVG chart tracking improvement across sessions (no libraries)
- **Test history** — last 10 tests saved locally with pass/fail tracking
- **Dark mode** — persistent across sessions via localStorage
- **Keyboard navigation** — arrow keys, number keys 1–4, Enter to submit
- **Export/import** — save your test history as JSON, restore on any device
- **Calendar export** — save test results as a `.ics` calendar event
- **Share results** — Web Share API with clipboard fallback
- **Responsive design** — works on mobile and desktop

---

## Technical Details

**Stack:** Vanilla HTML, CSS, JavaScript — zero dependencies, zero frameworks.

**Notable implementation choices:**
- CSS custom properties for theming — dark mode is a single `data-theme` attribute swap, no JS class toggling
- Per-question timing tracked via timestamps, enabling real fastest/slowest analytics
- Score trend rendered as hand-written SVG path (no Chart.js or similar)
- localStorage used for history, theme persistence, and backup/restore
- Keyboard accessibility with full ARIA roles on answer options

**File size:** Single `index.html`, ~2,600 lines.

---

## Development Approach

This project was built using **AI-assisted development** with Claude AI + Cline:

- I defined all features, UX requirements, and product decisions
- I directed the AI on what to implement and how
- I iterated through multiple versions based on testing and feedback
- I identified and fixed bugs in the analytics and answer review systems

This workflow — treating AI as an implementation tool while owning the architecture and product decisions — is increasingly how modern software gets built. This project is a practical demonstration of that.

---

## Running Locally

No build step needed. Just open the file:

```bash
git clone https://github.com/colubambi/ma-drivers-test.git
cd ma-drivers-test
open index.html   # or double-click the file
```

---

## About

Built by [Captain Babafemi Olubambi](https://github.com/colubambi) — aspiring DevOps Engineer based in Massachusetts.
