# HEIC to JPG support

Static support and privacy website for the native HEIC to JPG iPhone/iPad/Mac app.
No JavaScript, package install, build step, analytics, forms, functions or image uploads.
The original app-owned icon is copied from utility-apps; fonts are system fonts.

## Deploy on Vercel

Import the public `heic-to-jpg-support` repository into the existing Vercel Hobby team.
Use Framework Preset **Other**, repository root as Root Directory, no Build Command,
no Install Command, and the root as Output Directory (leave the default empty).
No environment variables are needed. Do not upgrade the plan.

`vercel.json` enables clean `/privacy` URLs and response security headers. Do not
add Vercel Analytics, Speed Insights or third-party scripts without updating the policy.

After deployment, check `/` and `/privacy` in a signed-out browser and on a phone;
check response headers, navigation, links, keyboard focus and expanded FAQ items.
The support target is `https://github.com/Zakariya1057/heic-to-jpg-support/issues/new`:
create that public repository with Issues enabled before advertising the link.
Use the deployed `/` as the support URL and `/privacy` as the privacy-policy URL.
No App Store link is included until the actual app record exists.

## Local preview

Run `python3 -m http.server 8765` in this directory. The static Python server serves
`/privacy.html`; Vercel serves the clean `/privacy` path. This server is local-only
preview infrastructure, not part of the site or the app.

## Content

- `index.html`: support, FAQ, public support link.
- `privacy.html`: policy effective 17 October 2026, distinguishing local app data from website hosting/support.
- `styles.css`: responsive system-font styling and visible keyboard focus.
- `assets/app-icon.png`: original native app icon.
- `vercel.json`: static routing and headers.

Review policy accuracy when app behavior, hosting or support processes change.
Never ask users to post private photos or personal information in public issues.
