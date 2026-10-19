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

## MOV to MP4 pages

The independent MOV app's support and policy pages are `mov-to-mp4/index.html`
and `mov-to-mp4/privacy.html` (policy effective 18 October 2026). Intended deployed
URLs are [MOV support](https://heic-to-jpg-support.vercel.app/mov-to-mp4) and
[MOV privacy](https://heic-to-jpg-support.vercel.app/mov-to-mp4/privacy). Verify both
live routes after deployment; their presence in source does not establish publishing.
These pages reuse the static styling and make no app-upload/backend promise.

## PDF to Word pages

The independent PDF app's support and privacy sources are `pdf-to-word/index.html`
and `pdf-to-word/privacy.html`, with policy effective 19 October 2026. The original
native icon is copied into `assets/pdf-app-icon.png`. Intended routes:
[PDF support](https://heic-to-jpg-support.vercel.app/pdf-to-word) and
[PDF privacy](https://heic-to-jpg-support.vercel.app/pdf-to-word/privacy).

These pages describe local PDF/OCR conversion to editable DOCX, actual formatting
limits, Files-only access and best-effort temporary cleanup. They reuse existing
static CSS and security headers; no scripts, forms, dependencies or app-upload
service were added. Source preparation does not establish deployment, App Store
availability or published App Privacy answers. Verify both live routes and native
app footer navigation after deployment. Never request private document attachments
in public GitHub issues. Do not alter HEIC/MOV policy facts as part of PDF updates.
The PDF support page publishes the authorized email `zakaria2011@live.no` and
keeps GitHub issues as an optional public route; its policy discloses both channels.
