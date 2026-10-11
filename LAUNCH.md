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
- No third-party game assets, executable/source distribution, advertising tags. GA4 and Clarity are optional after visitor consent (see configuration below).

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

## Search and analytics configuration — October 11, 2026

- GSC domain `sc-domain:noomicloneguide.com` and URL prefix `https://noomicloneguide.com/` verified by DNS. TXT @ `google-site-verification=TH0bUuBpuan6NySiJLsP3Ovqg1GJt84e4vLvoaAtA2c`, TTL 3600; existing DNS retained.
- Sitemap `https://noomicloneguide.com/sitemap.xml` submitted; initial report says Unable to fetch, 0 discovered. Re-submitted after homepage live test passed. Submission is not confirmation of indexing.
- GSC live homepage test at 19:37 Asia/Shanghai: URL can be indexed. Homepage indexing request returned a temporary submission error; not claimed successful.
- Bing HTTPS site added and HTML meta verification deployed. Sitemap submitted and initially Processing; 0 discovered. Later Bing UI network requests returned ERR_FAILED; final processing result not verified.
- GA4 under existing SwitchSpines account 403173714: NoomiClone Guide property 558437910, web stream 16105947576, measurement ID G-6FYLHG2HR4. Timezone China (GMT+8), currency USD. Enhanced measurement: page views, scroll, outbound click, file downloads enabled; search/forms/video disabled. Google signals and user-provided data remain off. Advertising personalization disabled for all 307 regions.
- GSC domain resource linked successfully to GA4 NoomiClone Guide Web in the same account.
- `official_play_click` registered as a code-created key event, once per session, no default monetary value. `official_store_click` and `guide_navigation` are emitted by consent-aware code; neither means a game was played or installed.
- Clarity project yw130kv1um (NoomiClone Guide), URL https://noomicloneguide.com/, entertainment category. Strict text masking confirmed. Consent v2 grants analytics storage only, denies advertising storage.
- Global analytics.js and privacy dialog deployed once per document. Neither vendor script loads before consent. Visitors can select either service, reject both, or withdraw through footer Privacy settings. Choices retained for 180 days; withdrawal clears first-party analytics cookies and reloads to stop previously loaded services. Tracking limited to canonical hostname, avoiding preview traffic.
- Updated privacy policy, Google/Bing verification meta tags, and CSP vendor allowlists deployed.
- Deployment dpl_5rgaUAsRtoC5B581CAJidceXW3fz READY, aliased to noomicloneguide.com. Production source verified with full TLS validation through Vercel address, including both search verification tags and analytics.js.
- All 11 routes, sitemap.xml, robots.txt and analytics.js returned HTTPS 200 through verified Vercel origin.
- Build, JS syntax and diff whitespace checks passed. Browser verified desktop privacy dialog, rejection and reopening on production Vercel alias, with no vendor scripts on preview hostname. New viewport override did not alter observed DOM dimensions, so new mobile consent QA remains unverified.
- Latest normal local HTTPS/browser still fails TLS because local resolver returns old NameSilo parking addresses. Authoritative and Cloudflare DNS return Vercel addresses; Google public resolver still had parking addresses. HTTPS certificate validated without bypass at both Vercel IPs and www redirected 308 to apex preserving path. Google live test independently accessed the canonical homepage.
- GA4 realtime receipt and Clarity live recording not yet verified: local canonical browser access is blocked by DNS cache. Do not count source presence or preview visits as received analytics.
- Account screenshots saved outside the public repository in ../noomiclone-guide-evidence/.

## Remaining verification

1. Normal local canonical HTTPS after DNS caches expire.
2. GSC sitemap successful fetch, Bing sitemap completed processing, and homepage indexing request retry.
3. GA4/Clarity real consented canonical-browser receipt, independent consent/withdrawal browser QA, and mobile consent layout.
