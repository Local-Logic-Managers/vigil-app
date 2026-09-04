# Vigil

A concept demo for Vigil — a grade & homework watch app that syncs with the
systems a school already runs (Blackbaud, PowerSchool SIS, Canvas LMS, Google
Classroom), nudges the student day-to-day, and sends parents and teachers a
weekly progress letter with tailored study-habit suggestions.

Served via GitHub Pages at vigil.locallogicmanagement.com.

**This is a concept demo with sample data for one fictional student** — there
is no live school-system connection yet. See the "Connected sources" panel
on the Weekly report tab for the integrations this is designed for.

## Files
- `index.html` — the interactive demo (student view + weekly report view),
  single self-contained file, no build step.
- `CNAME` — GitHub Pages custom-domain config, points at
  `vigil.locallogicmanagement.com`.

## Deploying (same pattern as Kronos / Threshold / Warden)
1. Repo already lives at `LocalLogicManagers/vigil-app`, public, with these
   files at the root.
2. Settings → Pages → Deploy from a branch → `main` / `(root)` → Save.
3. Settings → Pages → Custom domain → `vigil.locallogicmanagement.com` → Save.
4. In Wix DNS (Dashboard → Domains → locallogicmanagement.com → DNS Records):
   add a CNAME record — Host `vigil`, Points to `locallogicmanagers.github.io`
   (same target every other subdomain uses).
5. Once DNS propagates, come back to Settings → Pages and check
   **Enforce HTTPS**.
