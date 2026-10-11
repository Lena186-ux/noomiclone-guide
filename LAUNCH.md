# Launch record — 2026-10-11

## Verified production

- Custom canonical origin: https://noomicloneguide.com; original public alias retained at https://noomiclone-guide.vercel.app
- Repository: https://github.com/Lena186-ux/noomiclone-guide — public, main, issues enabled.
- Vercel project: noomiclone-guide; `prj_hwVRzFGIrxMtgXjnIblzuQ40UnaP`.
- Existing team: `team_5s6oVoWbOc9fBNOIw4er096N`.
- Final application deployment: `dpl_FnHEh8ELj5kP6ae9erqL5Ug23swS`, Ready and production alias assigned.
- Application commit: `56453ca` (launch documentation added afterward).
- Build: `node build.mjs`; 11 static content routes, custom 404, sitemap, robots, original SVG artwork and PNG social preview. No test suite added or run.
- All 11 production routes returned HTTP 200; sitemap returned 200/application/xml; robots returned 200/text/plain; unknown route returned 404.
- Browser QA: desktop and 390/768 px layouts reviewed; no horizontal overflow at those widths. Production FAQ expansion confirmed. Official destinations and per-route canonicals inspected.
- No third-party game assets, executable/source distribution, analytics scripts or advertising tags.

## Deployment workflow

GitHub integration failed in Vercel despite successful repository creation and CLI access. The site is published with the authenticated Vercel CLI; push alone does not currently deploy. Deploy from this directory with `vercel deploy --prod --scope a18720995650-6743s-projects` after building. Do not reuse a sibling project ID.

The CLI is currently at `/private/tmp/noomiclone-cli/node_modules/.bin/vercel`. GitHub CLI is at `/private/tmp/anyps5-gh/gh_2.102.0_macOS_arm64/bin/gh`. Temporary CLI paths may need replacement in later sessions. A stale global GitHub helper path was overridden in this repository only. Local credentials and `.env*` are ignored and not committed.

## Domain binding — 2026-10-11

Purchase confirmed in the user's authenticated NameSilo Domain Manager: noomicloneguide.com Active, created 2026-10-11, expires 2027-10-11. Both apex and www attached to this Vercel project. Vercel production deployment Ready and custom alias assigned.

DNS values came from the current Vercel domains verify response:

| Name | Type | Value | TTL |
| --- | --- | --- | --- |
| @ | A | 216.198.79.1 | 3600 |
| @ | A | 64.29.17.1 | 3600 |
| www | CNAME | 6dcea9cf6cf12f13.vercel-dns-017.com | 3600 |

NameSilo records were saved and confirmed after a reload. Six original parking A records were replaced; `_domainconnect` TXT was retained. No mail records were present. Prior records are in dns-before.json. Nameservers were not changed. DNS screenshot is saved outside the public repository in ../noomiclone-guide-evidence/dns-saved.jpg.

Canonical, Open Graph URLs, sitemap and robots origin now use https://noomicloneguide.com. www redirects to the apex through Vercel domain configuration (redirect=noomicloneguide.com, redirectStatusCode=308), preserving paths. The vercel.json host redirect alone returned 200 during verification, so the domain-level setting is the verified mechanism. At 19:18–19:19 Asia/Shanghai, authoritative and public DNS returned the new A/CNAME records. Vercel domains verify returned configured-correctly for both apex and www, with ownership verified and no conflicts. By 19:21, Vercel had issued an auto-renewing apex certificate (cert_LUleRUbtgXWeTInhyAN8rbcn), and both apex IPs returned HTTPS 200 with full normal certificate validation. www HTTPS returned 308 with Location https://noomicloneguide.com/controls/. Custom-domain homepage, controls, mobile, sitemap and robots were validated through Vercel endpoints using curl --resolve; canonical origin and all 11 sitemap URLs were correct. Ordinary local DNS/browser requests still hit cached parking addresses and failed TLS; no bypass or system DNS modification was used. Global cache convergence is not claimed.

## Evidence and SEO methodology

Primary sources are documented in README.md and linked in website content. Author-provided embed endpoint offers an itch.io project-card widget; permission for a full third-party playable game iframe was not established. Site uses author/store outbound links. Browser touch inputs, browser build version and ancestry to another original game remain unverified. No hands-on gameplay claims are made.

Parent keyword selection and Oct 4–10 historical Trends comparison were reused; no live search-volume, KD, traffic or ranking claims appear on the site. Gefei `load_guide` / newwords: **2 credits** charged, request `req_e3c48b15c2aa42e0`. Shared 20-minute spend was reported as 33 credits, so further queries stopped. No additional Gefei queries made.

## Remaining follow-ups

1. Ordinary local/browser DNS cache convergence remains pending; authoritative/public DNS, certificates, origin HTTPS and www redirects are verified.
2. Verify GSC and Bing properties and submit sitemap. Neither was configured in this chat.
3. If desired, connect GA4/Clarity with privacy and consent behavior before loading vendor tags.
4. Grow source-linked long-tail guides using confirmed questions and version changes. Obtain creator permission and hands-on evidence before adding screenshots or advanced gameplay claims.
5. Pursue an advertising application once the site's content and audience support it. No ad approval, revenue, tracking ID or guaranteed traffic is claimed.

Domain follow-up used no additional Gefei queries: 0 credits.
