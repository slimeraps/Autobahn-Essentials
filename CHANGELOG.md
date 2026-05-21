# Changelog

All notable changes to the Autobahn Essentials theme.

## 6.0.0 — 2026-05-21

### Added
- New **AE.Blog** page template (`templates/page.ae-blog.json`) and section (`sections/page-ae-blog-autobahn.liquid`) that auto-feeds from the `autobahn-blog` Shopify blog, showing the latest 10 posts newest-first.
- "View blog history" button on the AE.Blog page that appears once the source blog has more than 10 posts, linking to Shopify's built-in blog archive at `/blogs/autobahn-blog`.
- Theme-editor **Blog source** picker on AE.Blog so the source blog can be changed without code edits.

### Changed
- **Builds page** (`sections/page-builds-autobahn.liquid`) stripped down to hero-only. The page will be redesigned as a gallery in a future release.

### Removed
- Manual "Build card" theme-editor blocks from the Builds page (vehicle / title / text / 3 part tags). Cards are now driven by published blog posts on the AE.Blog page instead of hand-maintained blocks.
- Grid, "Submit a build" CTA, and associated settings from the Builds page schema.

### Admin steps required after deploy
- Create a new page in Shopify admin titled "AE.Blog" and assign it the `page.ae-blog` template.
- Add an "AE. Blog" item to the main menu pointing to the new page, placed to the right of Builds.
- In the Customize editor, delete any leftover invalid blocks under the Builds page.

## Prior releases

Releases 0.1 through 5.5 are tracked via git tags only.
