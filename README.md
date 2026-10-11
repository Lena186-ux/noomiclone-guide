# NoomiClone Guide

Independent English guide to NoomiClone. Original illustrations; no game files, third-party game assets, advertising or analytics.

## Build

`node build.mjs` builds eleven static content pages plus 404, sitemap and robots into `dist/`. No dependencies required. Current canonical origin is https://noomicloneguide.com. To switch after domain verification, use `SITE_URL=https://noomicloneguide.com node build.mjs` and set the same build environment variable in Vercel.

## Sources and limits

Reviewed 2026-10-11:
- https://jamesnorth.itch.io/noomiclone — author, HTML5/Unity, development status, four keyboard keys, official store links.
- https://play.google.com/store/apps/details?id=com.JamesWest.NoomiClone — Android listing and mobile features.
- https://apps.apple.com/us/app/noomiclone/id1546690510 — iOS listing and history.

The author offers an itch.io project-card widget. Permission for a third-party playable game iframe was not established; this site opens the author page instead. No hands-on gameplay results are claimed. Practice drills are editorial suggestions. Separate original/clone ancestry is not established by inspected primary sources. Browser build version and browser touch support remain unverified. The author's SIMMER link was not independently inspectable.

## Isolation

Use only this repository and its Vercel project. Never stage the parent workspace or reuse a sibling's `.vercel/project.json`. Contact corrections go to the public GitHub issue tracker. Domain purchase was confirmed on 2026-10-11.
