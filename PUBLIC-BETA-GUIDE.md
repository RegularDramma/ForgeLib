# ForgeLib — public beta rollout guide

This guide is for the first public test release. It does not replace the release blockers in `RELEASE-CHECKLIST.md`.

## Before upload
- [ ] Confirm that every bundled file may be hosted and redistributed under the displayed terms.
- [ ] Keep a copy of the license/source evidence for each resource.
- [ ] Run the syntax/archive/path checks listed in the release checklist.
- [ ] Do not upload `admin.html` as a production admin or promise that its edits publish to the site.

## Deploy as a static site
1. Create a new static-site project with the chosen hosting provider.
2. Upload the contents of this folder so `index.html` is at the site root (not inside an extra nested folder).
3. Use the provider's preview/staging URL first; a custom domain is not required for the initial test.
4. Open the staging URL in a desktop browser and a mobile browser.
5. Verify search, category filters, license/format filters, sorting, empty state, language/theme controls, all six resource detail pages, and each download.
6. Check browser console/network errors and ensure no links return 404.
7. Only after these checks pass, share the beta URL with a small test audience.

## What to tell early testers
- ForgeLib is an early free resource-library beta.
- The included files are starter/demo materials, not a premium asset pack.
- Ask testers what they searched for, what they expected to find, and which resources they would actually use.
- Collect feedback without requesting unnecessary personal data.

## Current limitations to disclose internally
- Static catalog: resource updates require a new deployment.
- No accounts, payments, backend uploads, shared admin, or server-side analytics.
- Download clicks are not proof that a file was successfully used.
- A public beta is not ready until rights and deployed-browser checks are complete.
