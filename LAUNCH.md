# Launch record — 2026-10-11

## Verified production

- Public URL and canonical origin: https://noomiclone-guide.vercel.app
- Repository: https://github.com/Lena186-ux/noomiclone-guide — public, main, issues enabled.
- Vercel project: noomiclone-guide; `prj_hwVRzFGIrxMtgXjnIblzuQ40UnaP`.
- Existing team: `team_5s6oVoWbOc9fBNOIw4er096N`.
- Final application deployment: `dpl_C4ksjo5hGz78Mus8yAyVZcH3gG9T`, Ready and production alias assigned.
- Application commit: `b260349` (launch documentation added afterward).
- Build: `node build.mjs`; 11 static content routes, custom 404, sitemap, robots, original SVG artwork and PNG social preview. No test suite added or run.
- All 11 production routes returned HTTP 200; sitemap returned 200/application/xml; robots returned 200/text/plain; unknown route returned 404.
- Browser QA: desktop and 390/768 px layouts reviewed; no horizontal overflow at those widths. Production FAQ expansion confirmed. Official destinations and per-route canonicals inspected.
- No third-party game assets, executable/source distribution, analytics scripts or advertising tags.

## Deployment workflow

GitHub integration failed in Vercel despite successful repository creation and CLI access. The site is published with the authenticated Vercel CLI; push alone does not currently deploy. Deploy from this directory with `vercel deploy --prod --scope a18720995650-6743s-projects` after building. Do not reuse a sibling project ID.

The CLI is currently at `/private/tmp/noomiclone-cli/node_modules/.bin/vercel`. GitHub CLI is at `/private/tmp/anyps5-gh/gh_2.102.0_macOS_arm64/bin/gh`. Temporary CLI paths may need replacement in later sessions. A stale global GitHub helper path was overridden in this repository only. Local credentials and `.env*` are ignored and not committed.

## Domain remains pending

Target: noomicloneguide.com. Parent chat checked availability and $17.29 first-year/renewal price at NameSilo on 2026-10-11. This is historical availability and pricing, not proof of purchase or current availability. Domain ownership was not confirmed in this chat. No DNS records were changed and no custom domain was added to Vercel.

Once purchase is confirmed, inspect the user's actual registrar account and current records. Add apex/www only to this project's Vercel configuration. Use the exact DNS values Vercel returns; preserve unrelated and mail records. Set SITE_URL=https://noomicloneguide.com in Vercel build environment, change the default origin in build.mjs, add a www-to-apex redirect, rebuild and redeploy. Verify HTTPS, redirects, sitemap and canonical origin before search submissions.

## Evidence and SEO methodology

Primary sources are documented in README.md and linked in website content. Author-provided embed endpoint offers an itch.io project-card widget; permission for a full third-party playable game iframe was not established. Site uses author/store outbound links. Browser touch inputs, browser build version and ancestry to another original game remain unverified. No hands-on gameplay claims are made.

Parent keyword selection and Oct 4–10 historical Trends comparison were reused; no live search-volume, KD, traffic or ranking claims appear on the site. Gefei `load_guide` / newwords: **2 credits** charged, request `req_e3c48b15c2aa42e0`. Shared 20-minute spend was reported as 33 credits, so further queries stopped. No additional Gefei queries made.

## Next steps after domain ownership

1. Bind custom domain and verify DNS/HTTPS; switch all canonical and sitemap origins together.
2. Verify GSC and Bing properties and submit sitemap. Neither was configured in this chat.
3. If desired, connect GA4/Clarity with privacy and consent behavior before loading vendor tags.
4. Grow source-linked long-tail guides using confirmed questions and version changes. Obtain creator permission and hands-on evidence before adding screenshots or advanced gameplay claims.
5. Pursue an advertising application once the site's content and audience support it. No ad approval, revenue, tracking ID or guaranteed traffic is claimed.
