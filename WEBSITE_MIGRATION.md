# Where Do We Eat website: website migration

Updated September 8, 2026.

## Canonical website

The public website is maintained in **[brianrenshaw-app-site](https://github.com/brianrenshaw/brianrenshaw-app-site)**, locally at `/Users/brianrenshaw/Projects/brianrenshaw-app-site`. Edit its `site/where-do-we-eat/` directory for future public website changes. App source and release management remain in this repository.

- App page / Marketing URL: https://brianrenshaw.app/where-do-we-eat/
- Support URL: https://brianrenshaw.app/where-do-we-eat/support/
- Privacy Policy URL: https://brianrenshaw.app/where-do-we-eat/privacy/
- Contact: contact@brianrenshaw.app
- App Store Connect app ID: `6808350718`
- User guide: https://brianrenshaw.app/where-do-we-eat/guide/

## Compatibility and releases

Previous website: https://brianrenshaw.github.io/where-do-we-eat-site/

Keep the existing GitHub Pages deployment enabled indefinitely. Old marketing/guide pages will redirect after HTTPS is validated at the new domain. Old privacy and support pages retain readable content and link to the new canonical page. Older installed app versions therefore continue to work.

App Store Connect URL changes are separate from website deployment. Update every existing platform/localization where editable; URL changes for released versions may wait for the next app release. Do not create or submit a new version solely as part of this migration. TestFlight URLs are maintained separately. No bundle identifiers, iCloud containers, URL schemes, data-collection declarations, or release states change.

## Deployment and verification

The new site is static HTML/CSS plus the existing browser game. GitHub Actions validates links, fragments, canonical URLs and font/assets, then deploys `site/`. Hover remains the DNS provider. Four apex A records point to GitHub Pages; `www` is a CNAME to `brianrenshaw.github.io`; existing MX/email settings remain unchanged.

Rollout is in progress. The central [migration log](https://github.com/brianrenshaw/brianrenshaw-app-site/blob/main/MIGRATION.md) is authoritative for HTTPS, legacy redirects, Apple read-back results, remaining release-dependent changes, and verification limits.

Website changes are committed separately from ongoing app work. Existing uncommitted app changes are preserved. Historical submission snapshots may contain the previous URLs; use the canonical values above for the next submission.
