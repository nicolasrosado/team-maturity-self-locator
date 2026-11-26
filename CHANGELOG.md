# Changelog

All notable changes to the `team-maturity-self-locator` skill are recorded here.
The skill line is versioned independently from the research-suite documents.

## [1.3.0] - 2026-11

Richer content and a sharper ADR; same assessment flow, same Waypoint format (v1). Backward-compatible: a Snapshot saved with 1.2.x loads unchanged.

- **Axis 1 (the three bounds) rated through three short questions**, one per bound (information: what we can know; cognition: what we can make sense of; time: when we can think it through). The axis takes the lowest of the three, never an average, and names the bound that pulls it down. Time is now spelled out on every rung (L5: time protected by the system).
- **What a level is made of**: "environment" and "culture" are now defined where the skill uses them (the environment = the organizational devices; the culture = the habits, norms and assumptions a team shares without deciding them), and a new explainer, on request, sets out the three spheres (environment, culture, actors; Alexandre-Bailly et al., 2016, Crozier & Friedberg), how a team relates to them level by level, and why AI, as a device, amplifies whatever culture it lands on.
- **Every rung illustrated**: the few rungs that had no concrete example now have one (axes 4 to 9), so a team can recognise itself.
- **A sharper ADR**: a short *Considered options* section (including "change nothing for now"), a *What we give up* line, where the discussion happens (a retro or a short meeting, not PR comments), who settles it if no consensus comes, and *Rejected* as a normal outcome to keep. The artifacts handed to a team (Snapshot, Waypoint, ADR) carry no third-party names; credits stay in the skill.
- **New moves and levers**, each credited: collective waiting when mobbing with AI (James Herr's team), a working agreement and "yes, and" to open a session, share the air, daily pairing (Steven Diamante), a safe-to-fail path for newcomers (time-to-autonomy, Julie Baillon), giving back to the digital commons at L5, and experimental ways to verify an agent's work.
- **Levers defined once**: the seven levers that were described twice (glossary and how-to) now have a single line each, with credit, a one-sentence definition and how to run it.
- **Credits re-checked**: sociable tests (Jay Fields, popularized by Martin Fowler), walking skeleton and ports & adapters (Alistair Cockburn), cognitive surrender (Steven Shaw & Gideon Nave, Wharton), anchoring (Tversky & Kahneman, 1974), and the speakers' practices named as the speakers follow them.
- **"An environment / a culture, not a verdict"** used consistently, including in the Posture block.
- **French answers about the licence** use the official Creative Commons names (*Partage dans les Mêmes Conditions*, never *à l'identique*), and share-alike is glossed as in the suite: any adaptation you share stays under the same licence.
- **Leaner file**: the token estimate and the in-file changelog were removed (full history lives here).

## [1.2.1] - 2026-11

Corrections only, no behaviour or feature change. Backward-compatible.

- **Attributions re-checked** against the talk transcripts and the cited sources: cognitive and intent debt credited to Margaret-Anne Storey (as cited by Dragan Stepanović); Ship / Show / Ask credited to Rouan Wilsenach (cited by William Bernting); breadcrumbs to James Herr's team; beads to Steve Yegge; Lopez's *black box* sourced to his article; Lopez's own wording restored ("more close to the decisions taken inside the code").
- **One wording fix**: collective ownership now reads "we missed it together, not just me" (the old "the team validated it" could suggest a bug was knowingly approved).
- **Share-alike spelled out** in the usage footer: any adaptation you share stays under the same licence, CC BY-NC-SA 4.0.

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
- **File naming**: saved snapshots are `<team-slug>_maturity-snapshot_<date>.txt` (team label first). Older `maturity-waypoint-*` files still load, the skill keys off the `BR-LOCATOR WAYPOINT` block, not the filename.
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
