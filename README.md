# STERIA — AI CSSD Specialist

Interactive educational experience for the **Sterilization Passport Journey**, International Sterile Processing Week 2026.
Central Sterile Services Department, King Khaled Eye Specialist Hospital.

Developed by the Digital Innovation Department. Content by the Central Sterile Services Department (Bodoor Megbel Alharbi, Sterilization Specialist).

**Live version:** https://YOUR-USERNAME.github.io/steria/

---

## What this is

A single web page with two paths:

- **Passport journey** — nine short stations following one reusable instrument from point-of-use handling to safe reuse, with a question at each stop and a progress record.
- **Ask STERIA** — 40 approved questions and answers about sterile processing, patient safety and digital CSSD.

It runs entirely in the browser. There is no server, no login and no database.

## Educational use only

This is an awareness and education tool. It does not replace CSSD professionals, hospital policy, validated cycles, or manufacturers' Instructions for Use. It contains no sterilization parameters, no exposure times, no temperatures and no patient-specific advice, and it never will — any process-specific value must come from approved hospital policy and the manufacturer's IFU.

## Privacy

The page collects nothing. No accounts, no forms, no patient information, no personal data. Progress through the journey is stored only in the visitor's own browser and is cleared when they leave. Analytics events, if a tracking tool is connected later, are anonymous counters only.

## Files

| Path | What it is |
|---|---|
| `index.html` | The whole experience. Open it in any browser. |
| `steria-content.json` | All the text — the 9 stations and the 40 questions. Edit this to change wording. |
| `IMPLEMENTATION.md` | Design, architecture, accessibility, analytics, backlog and timeline. |
| `assets/` | Character artwork, hospital logo and draft caption files. |
| `media/` | Where the video and narration files go. See `media/README.txt`. |

## Running it

Download or clone the repository and open `index.html`. Nothing to install.

To publish it, see **Settings → Pages** in this repository and serve from the `main` branch, root folder.

## Adding video and narration

Two switches near the top of the `<script>` block in `index.html`:

```js
const MEDIA_READY     = false;  // turn true once the .mp4 clips are in media/
const NARRATION_READY = false;  // turn true once the narration.mp3 files are in media/
```

Full instructions in `IMPLEMENTATION.md` §6 and §6b.

## Changing the content

All wording lives in `steria-content.json`. Edit it, commit, done — no code changes needed.

**Any change to the educational content must be reviewed and approved by CSSD before it is published.** Tag each approved version (for example `v1.0-approved-2026-09-01`) so it is always clear which wording the department signed off on.

## Credits

- Development: Digital Innovation Department, KKESH
- Content and CSSD expertise: Central Sterile Services Department — Bodoor Megbel Alharbi, Sterilization Specialist
- Character artwork: commissioned for this project

## Licence

To be confirmed by the hospital before public release. See the note in `CONTRIBUTING-NOTES.md`.
