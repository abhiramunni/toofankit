# ToofanKit — Cyclone & Storm Preparedness, Calmly Done

**Live:** https://abhiramunni.github.io/toofankit/

Cyclone Akvan is heading for the Andhra coast (landfall expected Friday 20 November 2026, between Nellore and Tuni). ToofanKit turns cyclone panic into a checklist: a live landfall countdown, four timed preparation phases, a family-size emergency kit, a home lock-down list, a family plan, the emergency numbers that matter, plain-language guides, and a 60-second storm drill quiz.

## What it does

- **Live landfall countdown** — days, hours, minutes and seconds to Cyclone Akvan's expected landfall (Fri 20 Nov 2026, ~12:00 IST), with the IMD status as reported 16 Nov 2026 and a note to check IMD for the latest.
- **Readiness dial** — a 0–100% ring computed from all 48 checks (20 phase tasks, 20 kit items, 8 home tasks), with a per-area breakdown.
- **Four timed phases** — Watch (72+ hours), Stock up (48h), Lock down (24h), Stay put (landfall). Tap a phase to open its tasks; each task has a plain-language "why".
- **Emergency kit builder** — 5 groups (water & food, light & power, documents & money, health, tools & safety) with quantities that scale automatically to your family size (e.g. water = 9 L per person for 3 days).
- **Home lock-down checklist** — 8 jobs, from trimming branches to sandbags at the door.
- **Family plan** — a meeting point and one out-of-town contact, saved on-device, plus ICE contacts with tap-to-call and add/remove.
- **Emergency numbers** — 112 (national emergency), 100 police, 101 fire, 108 ambulance, 1077 district control room — all tap-to-call — plus an IMD colour-code explainer (green / yellow / orange / red).
- **Six plain-language guides** — before, during and after the storm, the eye, flooding, and evacuation.
- **Storm drill quiz** — 6 questions with explanations; best score is saved.
- **Copy readiness summary** — a plain-text summary to share with the family. Remove-samples and erase-all included. Everything is stored in localStorage on the device; no account, no uploads.

## Design

Warm editorial palette (ivory paper, espresso ink, bronze and terracotta), Fraunces + Inter, a full-screen cinematic intro with tap-to-skip (quick on return visits), AI-generated storm-coast and emergency-kit photography with slow Ken Burns drift, and a 3-step onboarding coach.

## Notes

- Cyclone details are from IMD reporting on 16 November 2026. For live warnings, always check [mausam.imd.gov.in](https://mausam.imd.gov.in) and follow your district administration. In a real emergency, call **112**.
- This is a preparedness helper, not an official alert.

## Tech

Single self-contained `index.html` — no backend, no build step, localStorage only. Tested with headless jsdom (see `qa-test.js`).
