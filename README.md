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

## Using this under the license

See [`LICENSE`](LICENSE) (full legal code) and [`NOTICE`](NOTICE) (copyright and credits). This is a documentation / prompt artifact (a Claude skill written in Markdown), not executable software.

This work is released under **CC BY-NC-SA 4.0**. In plain terms:

- **BY (attribution)** — credit the author (Nicolas Rosado) whenever you share, publish, or redistribute it (or an adaptation). Purely private use publishes nothing, so there's nothing to attribute then.
- **NC (non-commercial)** — no use "primarily directed toward commercial advantage or monetary compensation." NC is about the **use, not the user**: no selling it, paywalling it, or bundling it into a paid product — but a **company using it internally, for its own team, is completely fine** (NC is not "no businesses").
- **SA (share-alike)** — if you *modify or adapt* the tool, the adapted part must stay under the same CC BY-NC-SA license (so the spirit keeps travelling).

**The real question is not "standalone or wired into an agent?" — it's "for your own team, or for paying clients?"**

**Using it — for whom:**

| Use case | Under the free license? |
|---|---|
| Your own team, internal use | ✅ Yes |
| A local read to inform your own view, even for a team you consult (nothing shipped out) | ✅ Yes — a permission the author grants |
| A client deliverable, a paid product / service, or reselling it | ❌ Commercial — not allowed under the free license; you need the author's permission first |
| Sharing or publishing something based on it | ✅ Yes, with attribution |

**Running, distributing or modifying the skill:**

| Use case | Under the free license? |
|---|---|
| Run it **standalone** (installed, invoked directly) | ✅ Yes |
| Run it **via your own agent, unmodified** (a *combination*) | ✅ Yes — your agent code stays under your terms; the skill keeps its CC BY-NC-SA license |
| **Bundle a copy** into your own agent / product to ship to others (*aggregation*) | ✅ if non-commercial **and** you credit the author (the copy stays CC BY-NC-SA); ❌ in a paid product / service → ask the author |
| Bundle it into an **existing agent under another license** | Coexists fine (*aggregation*, side by side): ✅ if non-commercial and that license can host an NC component; ❌ if the agent is paid, or its license can't host NC → ask the author |
| **Modify / translate / adapt** the skill (an *adaptation*) | ✅ Yes — but the adapted part stays under CC BY-NC-SA (*share-alike*); you can't merge it into another license or relicense it |

**A few principles behind the tables:**
- **Outputs, not intentions.** The client line turns on what actually gets *shipped*, not on what you mean to do: free as long as nothing that comes out of it is delivered to a client, sold, or built into a paid offering. It holds for the skill's own output too (the **Team Maturity Snapshot** — its Waypoint and proposed ADR): keep it for your own or your team's reading; hand it to a client as a paid deliverable or sell it, and it's commercial. Concretely: ✅ you run it and read the result to shape your own thinking → fine; ❌ a report built from it goes into a paid client deliverable → commercial; ❌ it's embedded in a paid product or service → commercial.
- **Coexist ≠ merge.** Placing the skill unmodified beside your own code lets the two licenses coexist — your code stays yours, the skill stays CC BY-NC-SA. What you can't do is *merge* it into another license or relicense it; CC BY-NC-SA also can't live inside something that must stay commercially usable.
- **One constant across every case:** the skill copy always stays CC BY-NC-SA, attribution applies whenever you distribute, and NC gates **anything commercial** — a paid product or service, a client deliverable, **marketing or promotional use, or a site that earns ad revenue** — → you need the author's permission.
- **Cited authors keep their rights.** The license covers Nicolas Rosado's original text only. The thinkers and practitioners quoted or built upon (Simon, Edmondson, Clark, Team Topologies / Skelton & Pais, Stepanović, Storey, Westrum, and the named speakers) keep their own rights — reproduced under the right of quotation. You can't relicense them, and you can't re-attribute their ideas or words to yourself; credit stays with them.
- **The local-read permission** is granted by the author as the rights holder, on top of the license; the CC BY-NC-SA license itself is unchanged (not a modified or custom license).

For a commercial or client use case: it isn't granted by default — ask the author's permission first (it may or may not be granted). The aim of this work is to help teams, not to sell.
