# Changelog

## v0.6.25-beta — unified cosmic hero and brand mark
- Added a single panoramic cosmic scene as the home hero background.
- Disabled the previous orbit-SVG backdrop rather than layering the new art over it.
- Added a standalone geometric brand emblem and HTML-rendered ForgeLib wordmark.
- Switched the interface accent palette to violet/magenta; catalog cards remain neutral and use content-specific previews.
- Left the new scene static for this stage; background animation is deferred until the new layout is reviewed.

## v0.6.24-beta — functional rollback to animated orbital baseline

- Rebased visual styling and animated background on v0.6.16, before the later large-scene redesigns.
- Kept the later drag-and-drop usability fixes where they were programmatic rather than cosmetic: gentler edge auto-scroll, no downward auto-scroll while over the drop target, safe pointer-cancel handling, and drag initiation from saved-item links without breaking ordinary clicks.
- Existing catalog validation, escaped dynamic content, restricted local download paths, filters, sorting, RU/EN switching, theme switching and local workspace persistence remain from the baseline.

# Changelog — ForgeLib v0.6.16-beta

- Corrected the API starter snippets file size metadata (484 B).
- Limited catalog JSON imports to 2 MB and strengthened structural validation, including unique IDs and description/tag types.
- Escaped dynamic catalog text before inserting it into public resource cards and detail pages.
- Restricted downloadable resource paths to local `downloads/` paths; URL schemes, backslashes, and path traversal are rejected.
- Escaped dynamic values in the local admin resource list.
- Added basic structural validation and a 1,000-item limit for imported catalog JSON.
- Added sorting by title A–Z and recently updated; newest sorts by descending resource ID (the admin assigns the next ID to new items).
- Updated the displayed catalog version and README to match the archive version.
- Kept the admin explicitly local-only; no backend, server-side authentication, or public upload functionality was added.

## Validation

- JavaScript syntax checks: passed.
- Main ZIP integrity: verified after packaging.
- Bundled resource paths and nested ZIP integrity: verified during packaging.
- Full interactive browser testing: not completed in this environment.


## v0.6.14-beta
- Fixed Russian localization of the free-resource counter label.
- Localized the “Any” option in the license and format filters for RU/EN.
- Clarified that this archive is a public-beta candidate and that launch still depends on rights review and deployed browser checks.


## v0.6.15-beta
- Replaced the green/charcoal accent system with black, violet and dark-pink tones; coordinated light theme.
- Added persistent Forge Space workspace for mixed catalog resources.
- Added eased pointer-follow dragging with grab-offset preservation, drop feedback, add/remove/clear and manual reorder.
- Added mobile layout and reduced-motion accommodations for the workspace.


## v0.6.16-beta
- Added a custom SVG cosmic crystal/orbital background behind the site.
- Added slow full-turn animation with a fixed viewport layer so it remains in the background while the page scrolls.
- Reduced background opacity on smaller screens and in light theme; respects `prefers-reduced-motion`.
- Updated catalog version metadata.
