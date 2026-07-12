# Changelog

All notable changes to the `team-maturity-self-locator` skill are recorded here.
The skill line is versioned independently from the research-suite documents.

## [1.1.0] - 2026-07

Output renamed and the skill made self-explanatory about usage rights. Backward-compatible.

- **Output → "Team Maturity Snapshot"**: the whole generated artifact now has a self-describing header (names it + lists its sections) and a usage-and-license footer. Sections: Posture + Waypoint + ADR. The position block keeps the name **Waypoint**.
- **The skill now answers usage/license questions** ("can I use it with a client? via my agent? bundle it?") plainly and non-judgmentally, from an embedded, self-contained license section: own team vs paying clients, the *outputs-not-intentions* rule, and call vs bundle vs adaptation.
- **File naming**: saved snapshots are `<team-slug>_maturity-snapshot_<date>.txt` (team label first). Older `maturity-waypoint-*` files still load — the skill keys off the `BR-LOCATOR WAYPOINT` block, not the filename.
- Non-judgmental framing preserved; the assessment flow is unchanged; past waypoints re-ingest.

## [1.0.0] - 2026-07

Initial public release, extracted into its own repository as the canonical source
of truth for the skill.

- Interactive 9-axis self-location on the Bounded-Rationality Maturity Scale.
- Level computed as the floor (lowest axis), never an average.
- Psychological-safety deep-dive (Clark's four stages) when that axis is the floor.
- Floor-matched levers drawn from the companion ebook's toolbox.
- Non-judgmental framing throughout: environments, not verdicts; suggest, never impose.
- EN / FR support.
