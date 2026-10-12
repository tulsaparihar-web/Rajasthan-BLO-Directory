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
