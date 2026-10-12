# Rajasthan BLO Directory — Milestones

## v1.0.0 — Approved Search Baseline

- **Status:** Approved by the user as the stable baseline for future enhancements.
- **Repository:** https://github.com/tulsaparihar-web/Rajasthan-BLO-Directory
- **Baseline commit:** `1d4bb19d141c22a1d1fb954b7ab9064a0c2e507b`
- **Build:** [GitHub Actions run 38233475069](https://github.com/tulsaparihar-web/Rajasthan-BLO-Directory/actions/runs/38233475069) — successful.
- **Artifact:** `Rajasthan-BLO-Directory-Improved-Search.zip` (contains the verified debug APK).
- **Frozen baseline branch:** `milestone/blo-directory-v1.0.0`

### Included capabilities

- Offline Room database seeded from the bundled BLO CSV.
- Hindi/English interface.
- Dedicated, scrollable search-results screen.
- Result count based on all matches and batched “Load more” paging.
- Refine-search and reset controls.
- Phone dialler action for available mobile numbers.
- Google Maps search/directions action for polling-station details.
- Unique IDs during import to prevent source rows from overwriting one another.
- Source CSV verified at build time: 61,362 data rows plus the header.

### Baseline rule

Treat the commit and `milestone/blo-directory-v1.0.0` branch as the approved reference version. Develop future features on the main development line, preserve existing behavior unless a change is explicitly agreed, and run the Android build before sharing each updated APK.

## v1.1.0 — BLO and ERO Directory

- **Status:** Implemented, merged to `main`, and verified by a successful Android build.
- **Merge commit:** `d6e41cff6a8e816ad91e93cc709d7ba3577d74f8`
- **Pull request:** [#1 — Add ERO tab to BLO and ERO Directory](https://github.com/tulsaparihar-web/Rajasthan-BLO-Directory/pull/1)
- **Verified build:** [GitHub Actions run 38237419581](https://github.com/tulsaparihar-web/Rajasthan-BLO-Directory/actions/runs/38237419581) — successful APK build and artifact verification.
- **App label:** `BLO and ERO`

### Added capabilities

- Dedicated BLO and ERO tabs in the bilingual interface.
- ERO directory bundled for offline use from `ERO_Details.xlsx`: 200 records across 41 districts.
- ERO filters limited to District and Assembly dropdowns.
- ERO results include officer name, user ID, office address, mobile, landline, and email.
- ERO search supports name, user ID, phone, office address, and email; results are paged.
- Call and Google Maps directions remain available when the relevant contact/location information exists.
- Room database upgraded to v4; existing BLO data is re-seeded alongside the ERO records on upgrade.

### Preserved behavior

The v1.0.0 milestone branch remains frozen and unchanged. BLO search, district/assembly/part filters, paging, offline data, bilingual UI, Call, and Directions remain in place.

