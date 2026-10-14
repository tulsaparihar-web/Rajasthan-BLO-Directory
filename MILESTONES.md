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
- **App label at this milestone:** `BLO and ERO`

### Added capabilities

- Dedicated BLO and ERO tabs in the bilingual interface.
- ERO directory bundled for offline use from `ERO_Details.xlsx`: 200 records across 41 districts.
- ERO filters limited to District and Assembly dropdowns.
- ERO results include officer name, office address, mobile, landline, and email.
- ERO search supports name, phone, office address, and email; results are paged.
- Call and Google Maps directions remain available when the relevant contact/location information exists.
- Room database upgraded to v4; existing BLO data is re-seeded alongside the ERO records on upgrade.

### Preserved behavior

The v1.0.0 milestone branch remains frozen and unchanged. BLO search, district/assembly/part filters, paging, offline data, bilingual UI, Call, and Directions remain in place.

## v1.2.0 — District DEO and DyDEO Directory

- **Status:** Implemented, merged to `main`; APK build and archive verification succeeded.
- **Pull request:** [#3 — Add DEO and DyDEO district-level tabs](https://github.com/tulsaparihar-web/Rajasthan-BLO-Directory/pull/3)
- **Merge commit:** `118d17d5f635bca8db4cec1d4dbc02098b8794c`
- **Verified build:** [GitHub Actions run 38533367130](https://github.com/tulsaparihar-web/Rajasthan-BLO-Directory/actions/runs/38533367130)
- **Build artifact:** `Rajasthan-BLO-Directory-APK`

### Added capabilities

- Added DEO and DyDEO tabs alongside BLO and ERO.
- Bundled the supplied DEO and DyDEO datasets offline: 41 records each, across 41 districts.
- Each new tab has a single District dropdown and a search textbox for officer name, phone, office address, and email.
- Results show officer contact details and office directions where available, with paging.
- DEO Call button is disabled as requested; calling remains enabled for DyDEO where a mobile number exists.
- Existing BLO and ERO functionality retained; ERO queries are isolated from DEO/DyDEO records.
- Room database upgraded to v5 to seed the new officer datasets after upgrade.
