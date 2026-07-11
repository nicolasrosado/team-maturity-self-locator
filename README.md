# team-maturity-self-locator

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

> **A Claude skill.** An interactive, non-judgmental self-assessment that locates a software
> team on the **Bounded-Rationality Maturity Scale** (Nicolas Rosado) and suggests the single
> highest-leverage next move. A *living tool*, continuously improved.

**Skill command:** `/team-maturity-self-locator` · **Version 1.0.0** · Free gift to the community (**CC BY-NC-SA 4.0**)

> This repository is the **canonical source of truth** for the skill.

Part of the Bounded-Rationality research suite (white papers, an ebook, the scale, and this
self-locator). Everything lives here:
<https://nicolasrosado.github.io/aiagents-montreal/research/bounded-rationality/>

## Follow along

- **Star** or **watch** this repo to be notified of new versions, no need to check back.
- Found something off, unclear, or an idea to improve it? **Open an issue.** The right to make
  mistakes this work advocates for applies to its author too, so constructive feedback on any
  inconsistency is warmly welcome.

## Install

The skill is a single file. Place it so it sits at:

```
~/.claude/skills/team-maturity-self-locator/SKILL.md
```

For example:

```bash
git clone https://github.com/<your-account>/team-maturity-self-locator.git
mkdir -p ~/.claude/skills/team-maturity-self-locator
cp team-maturity-self-locator/SKILL.md ~/.claude/skills/team-maturity-self-locator/
```

To stay in sync with updates, you can symlink instead of copying:

```bash
mkdir -p ~/.claude/skills/team-maturity-self-locator
ln -sf "$(pwd)/team-maturity-self-locator/SKILL.md" ~/.claude/skills/team-maturity-self-locator/SKILL.md
# then `git pull` in the repo picks up new versions automatically
```

*(Only `SKILL.md` is loaded by Claude.)*

## Run

In Claude Code (or any Claude that loads skills), type:

```
/team-maturity-self-locator
```

Then answer the questions. The skill walks your team through **9 axes**, computes your **floor**
(your level = the lowest axis, not an average), and suggests **one** next move, framed as a team
experiment, never a verdict. No setup, no account, **nothing leaves the conversation**.

## What it does

- Walks the 9 axes one at a time (with an example for each), in your language (EN/FR).
- Computes the level as the **lowest** axis, not an average.
- Zooms into **psychological safety** (Clark's four stages) when that's your floor.
- Suggests 1 to 2 **levers** matched to the floor (drawn from the companion ebook's toolbox).
- Stays **non-judgmental**: it's the *environment*, not the people; suggest, never impose.

## Requirements

Claude with skills support (e.g. Claude Code). No other dependencies.

## License and credit

See [`LICENSE`](LICENSE) (full legal code) and [`NOTICE`](NOTICE) (copyright and credits).
**CC BY-NC-SA 4.0**: read it, share it, translate it, build on it;
credit the author, keep it non-commercial, share alike. This is a documentation / prompt
artifact (a Claude skill written in Markdown), not executable software.

Built on Nicolas Rosado's original framework. The named lenses (Simon, Edmondson, Clark,
Skelton & Pais, Stepanović, Storey, Westrum, and others) are credited where they appear, not
owned.
