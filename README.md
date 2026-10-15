# Qalmi — Ink & Canvas

> A quiet, offline-first writing desk: one self-contained file for drafting, organizing, reviewing, and exporting documents on your device.

**Open Qalmi free:** [arbabtalha.github.io/QALMI/QALMI.HTML](https://arbabtalha.github.io/QALMI/QALMI.HTML)

Qalmi runs in your browser with no sign-up and no paid service. Documents are stored locally in that browser; use **Storage and backups → Export all data** to keep a copy. Browser storage can be cleared or evicted.

## Start

Open `QALMI.HTML` in a modern browser, or serve the repository folder locally:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000/QALMI.HTML`. No environment variables or runtime packages are required. The complete app is in the single root-level `QALMI.HTML` file.

## Publish

GitHub Pages is configured to deploy the repository root from `main`; merge a change to `main` and Pages publishes it at the link above. No build command or secrets are required. `QALMI` is a working product name; trademark and custom-domain clearance have not been established.

## What works

Local documents and folders, templates, rich-text editing, autosave, snapshots, comments and review tools, search, supported file import/export (including DOCX), and browser-based print / Save as PDF. DOCX conversion is best-effort and reports limitations.

## Honest limits

This single-file edition has no account system, cloud sync, sharing, real-time collaboration, installable PWA, or offline app-shell startup. The live page needs an initial internet connection; already-open documents remain editable locally. Printing, pagination, spell-check dictionaries, and speech depend on the browser or device. The in-app **Feature coverage** ledger labels items WORKING, BLOCKED, or NOT IMPLEMENTED; the full specification is in `QALMI_INSTRUCTIONS.txt`.

## Checks

The inline JavaScript passes `node --check`; `npx --yes html-validate QALMI.HTML` passes; and a HappyDOM smoke/regression harness verified local persistence, core interactions, HTML sanitization, and a DOCX round-trip containing formatted text, a table, a link, and an embedded image. These checks do not replace full browser, mobile, accessibility, or office-suite QA.
