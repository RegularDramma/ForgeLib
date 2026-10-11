# ForgeLib — release readiness checklist

Status for v0.6.14-beta. This is an internal launch checklist, not a claim that every item is complete.

## Automated checks completed
- [x] JavaScript syntax checks for `app.js` and `admin.js`.
- [x] Main archive integrity.
- [x] Nested `creator-card-templates.zip` integrity and file listing.
- [x] All six catalog file paths exist in `downloads/`.
- [x] Corrected API starter snippet size metadata to 484 B.
- [x] Fixed RU/EN text for the free-resource counter and “Any” filter options.
- [x] Catalog import is capped at 2 MB and validates IDs, types, tags and localized text shapes.

## Must complete before public launch (release blockers)
- [ ] Run interactive browser tests on the actual public-hosting environment and check desktop/mobile layouts.
- [ ] Verify RU/EN switching, light/dark theme, search, every filter, sorting, empty state, resource detail pages and all download links.
- [ ] Verify the origin and redistribution rights for each bundled resource. The archive contains license labels but no evidence package proving rights; do not treat labels alone as proof.
- [ ] Add clear license/usage text and attribution where required; use an external source link instead of hosting a file if redistribution rights are uncertain.
- [ ] Test keyboard navigation, visible focus states, contrast and reduced-motion behavior.
- [ ] Choose the hosting provider/domain and test the deployed version before announcing it.
- [ ] Add privacy-conscious analytics only after deciding what data is collected and disclosing it appropriately.
- [ ] Keep `admin.html` local-only. Do not present it as a public secure admin: it has no server-side authentication or shared persistence.

## Known product limitations
- Catalog content is bundled into `data/catalog.js`; edits require a new deployment.
- Local admin edits are stored only in the current browser's `localStorage`.
- No user accounts, hosted uploads, payments, server-side analytics or backend are implemented.
- Bundled starter resources are small demo materials, not premium-quality packs.


## Recommended rollout
1. Keep this archive as a staging candidate.
2. Deploy to a temporary static-host URL.
3. Run the interactive checks above on desktop and mobile, including each download.
4. Confirm licensing/redistribution terms and keep evidence in the project folder.
5. Publish the beta link to a small test audience first; collect feedback without claiming premium-quality assets.
6. Fix critical issues before broad promotion.


## v0.6.15 Beta checks
- [ ] Browser-test Forge Space drag/drop with mouse and touch.
- [ ] Confirm local persistence after reload and browser restart.
- [ ] Confirm remove, clear, reorder, RU/EN and dark/light theme.
- [ ] Review mobile card and workspace layout.
- [ ] Full browser interaction testing is still required before public deployment.


## v0.6.16 Beta checks
- [ ] Verify the orbital background stays behind content on home, resource, and admin pages.
- [ ] Check text contrast and scroll behavior at desktop and mobile widths.
- [ ] Confirm the animation stops or becomes static with reduced-motion enabled.
- [ ] Review the light theme to ensure the artwork remains subtle.


## v0.6.24 Beta — functional rollback
- [x] Restored the v0.6.16 visual baseline and its animated orbital/crystal SVG; later visual redesigns are not carried forward.
- [x] Reduced drag auto-scroll speed and disabled downward auto-scroll while the pointer is over the drop board.
- [x] Pointer cancellation now cancels a drag rather than accidentally completing a drop.
- [x] Dragging a saved item may begin from its link area; ordinary clicks still open the resource unless the drag threshold is crossed.
- [ ] Browser-test drag/drop, reorder, click-to-open, remove, clear and persistence with mouse/touch.
