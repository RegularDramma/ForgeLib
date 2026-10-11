# ForgeLib v0.6.25 Beta

ForgeLib is a static, free-first digital-resource library prototype. This beta is intended for public usability testing, not as a complete commercial marketplace.

## Run locally

For a quick local preview, open `index.html` in a modern browser. For the most reliable testing, serve this folder through a local static HTTP server.

## Public pages
- `index.html` — home and resource catalog
- `resource.html?id=1` — resource detail page

## Visual update in v0.6.25
- Replaced the previous animated orbital SVG backdrop with one unified cosmic scene behind the hero.
- Added a separate geometric ForgeLib emblem; the wordmark remains real HTML text for clean rendering and accessibility.
- Shifted brand accents from green to violet while keeping resource thumbnails content-specific and card surfaces neutral.
- The new background is intentionally static in this version. Motion effects should be designed only after reviewing the new composition in the page.

## Beta functionality
- Free resource catalog
- Search by title, tags, category, format and description
- Category filters, license/format filters, and sorting by newest, title, and recently updated
- Dedicated resource pages and real file downloads
- RU/EN switch and dark/light theme
- Responsive layout
- The public catalog shows only resources with downloadable files; no fake paid products or purchase flow are shown

## Included resources
The catalog currently contains six free starter resources. Before public launch, review every file, description, attribution and license. Do not publish third-party content unless its license permits the intended use.

## Local admin prototype
`admin.html` and `admin.js` remain for local experimentation only. They use browser `localStorage`; edits are not published to other visitors and this is not a secure server-side admin system. The public navigation does not link to the local admin.

## Known limitations
- No accounts, backend, hosted uploads, payments or server-side analytics.
- Changes made in the local admin do not update the public catalog for other users.
- The catalog is static and changes must be included in a new deployment.

## Security and publication notes
- Dynamic catalog text is HTML-escaped before rendering; local download links are restricted to relative paths without traversal or URL schemes.
- Admin imports have basic shape/size validation. The local admin remains a prototype and must not be exposed as a production admin.
- Included license labels are metadata, not proof of ownership or redistribution rights. Verify rights and keep source/attribution evidence before public distribution.
- Automated checks in this revision cover JavaScript syntax, archive integrity, nested ZIP integrity, catalog file-path existence, and selected metadata consistency. A full interactive cross-browser/manual UI test is still outstanding.

## Public beta gate
This archive is a **candidate** for public beta, not a declaration that the site is already production-ready. Before announcing it, complete the must-do items in `RELEASE-CHECKLIST.md`, especially file/rights review and a deployed-browser smoke test. If a resource's redistribution terms are unclear, remove its download or replace it with an external source link until clarified.

## Suggested next step
Deploy a staging copy to a static host and test it on desktop and mobile. Only then announce the public beta. Add privacy-conscious analytics for searches, resource opens, download clicks and zero-result searches after deciding what is collected and disclosing it appropriately.


## v0.6.15 Beta — Forge Space
- Reworked the visual palette to a black / violet / dark-pink system, including a coordinated light theme.
- Added Forge Space: locally persisted resource collection, drag-and-drop from catalog, add/remove/clear controls, and drag reordering.
- Drag preview follows the pointer with eased motion while preserving the original grab offset.
- The collection stores resource IDs and order in this browser only; it is not synchronized across devices.
- Full page-transition effects remain intentionally deferred until the new styling and workspace behavior are reviewed.


## v0.6.16 Beta — animated orbital backdrop
- Added a custom SVG illustration with a faceted violet crystal, magenta orbital rings, floating fragments and soft nebula glow.
- The backdrop rotates slowly behind the interface, stays fixed while scrolling, and is dimmed to preserve text and card contrast.
- Reduced animation and background intensity for mobile, light theme, and users who prefer reduced motion.
- The background is a lightweight local asset (`assets/forge-orbit.svg`); it requires no external image host or network request.
