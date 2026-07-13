# Changelog

All notable changes to the `team-maturity-self-locator` skill are recorded here.
The skill line is versioned independently from the research-suite documents.

## [1.2.0] - 2026-07

Leaner on-screen output; the saved `.txt` artifact is unchanged and complete. The assessment itself is unchanged. Backward-compatible.

- **Lean on-screen Snapshot**: in the chat, the Snapshot now shows a one-line reading frame + the Waypoint + the ADR core (Context / Decision / Why / Consequences + the owner/review blanks) + a two-line ADR-notes summary. The full POSTURE, the usage/license footer, and the ADR's closing explainer notes are written to the saved file and offered on request, no longer dumped inline.
- **Need-named on-request options** (never tool jargon): e.g. "Read the full Posture", "Am I allowed to use this with my team, or a client?", "What's an ADR, and how do I use this one?", each with a short why-it's-worth-it hook.
- **Close is a selection picker, not prose**, re-offered after each reveal so the reader can keep exploring, with a "Done, take the file" always present. (Picker caps at ~4 options, so items rotate rather than all showing at once.)
- **Anti-duplication guard**: emit each block exactly once; defends against a generation glitch that occasionally echoed the ADR/footer (or a waypoint tail) twice in the on-screen print. The saved file was always clean.

## [1.1.1] - 2026-07

Wording only, no behaviour or feature change. Backward-compatible.

- **License section clarified**: sharpened the wording on invoking vs bundling vs adapting the skill (invoking via your own agent isn't merging; only *adapting* triggers share-alike; attribution and non-commercial still apply), and cleaned the section's punctuation.
- **AI-tell read-out reworded**: when a "tell" axis is the floor but not at L1-L2, the skill now states the reading plainly and calmly, without the "danger zone" / "no alarm" phrasing that could still surface in the output. Keeps it modal, consistent with the tool's non-judgmental framing.
- **README**: the zoom bullet now reflects that the skill zooms into any floor axis with sub-structure (psychological safety, the three bounds, feedback, shared mental model), not psychological safety alone.

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
