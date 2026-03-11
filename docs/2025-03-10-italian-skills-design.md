# Italian Claude Code Skills — Design Document

## Overview

A collection of 7 Italian-themed Claude Code slash commands that are both
genuinely useful developer tools and a fun way to learn Italian idioms.

Each command maps a real Italian cultural concept to a practical development
workflow. The humor comes from the absurdity of the mapping being *correct* —
nonna's cooking logic actually applies to code architecture.

## Tone Guidelines

- **Deadpan delivery** — Claude applies Italian cultural logic completely
  seriously, as if this is the obvious way to reason about software.
- **No caricatures** — no fake accents, no "mamma mia" spam. The comedy is
  in specificity and genuine cultural references.
- **Rewarding knowledge** — an Italian laughs harder because they *know* that
  nonna, but everyone finds the advice genuinely useful.
- **Personality matched** — warm nonna energy for `/nonna-review`, elegant
  judgment for `/bella-figura`, baffled frustration for `/ma-che-vuoi`.

## Commands

### /al-dente — Code quality balance
- **Cultural root:** "Al dente" — pasta cooked firm, not soft. The right texture.
- **What it does:** Reviews code for over-engineering (too rigid) or fragility
  (too soft). Finds the balanced sweet spot.
- **Tone:** Professional chef. Calm, authoritative.

### /arrangiati — Workaround with what you have
- **Cultural root:** "L'arte di arrangiarsi" — the Italian art of making do
  with limited resources, born from generations of resourcefulness.
- **What it does:** Proposes solutions using ONLY existing dependencies and
  stdlib. No new packages allowed.
- **Tone:** Resourceful uncle who fixed a Vespa with a clothespin.

### /bella-figura — Make it presentable
- **Cultural root:** "Fare bella figura" — the deep Italian value of making a
  good impression, extending to how you present yourself and your work.
- **What it does:** Formatting, linting, naming review. Makes code presentable.
- **Tone:** Elegant, slightly judgmental. Spots socks-with-sandals energy.

### /coffee-break — Creative brainstorm pause
- **Cultural root:** The Italian coffee break — a sacred ritual of stepping
  away from work to recharge and let ideas come naturally.
- **What it does:** Steps back from the current approach. Proposes 3 alternative
  angles you haven't considered.
- **Tone:** Relaxed, lateral thinking. The bar counter at 10am in Naples.

### /dizionario — The cultural phrasebook
- **Cultural root:** "Dizionario" means dictionary.
- **What it does:** With no args, lists all commands with Italian origins and
  links. With an argument, deep-dives into that specific reference.
- **Tone:** Warm, educational. A friend explaining culture over dinner.

### /ma-che-vuoi — Explain confusing code
- **Cultural root:** The iconic Italian hand gesture (pinched fingers) meaning
  "what do you even want?" or "explain yourself."
- **What it does:** Identifies confusing code and explains it plainly. Calls out
  genuinely incomprehensible code directly.
- **Tone:** Genuinely baffled Italian demanding answers.

### /nonna-review — Gentle but firm code review
- **Cultural root:** The Italian grandmother — warm, caring, feeds you
  compliments before the truth. Never cruel, always right.
- **What it does:** Full code review focused on robustness: missing tests,
  error handling gaps, things that break at 2am.
- **Tone:** Warm nonna energy. Feeds you before the criticism.

## Repo Structure

```
italian-claude-code-skills/
  README.md
  LICENSE
  install.sh
  commands/
    al-dente.md
    arrangiati.md
    bella-figura.md
    coffee-break.md
    dizionario.md
    ma-che-vuoi.md
    nonna-review.md
  docs/
    cultural-references.md
```

## Installation

`install.sh` symlinks `commands/*.md` into `~/.claude/commands/`.
Running `git pull` in the repo auto-updates commands.
