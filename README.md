# Grammatica — Italian Verbs & Grammar

> **Catch-up sheet — read this first at the start of any new conversation.**
> It captures the aim, the current state, and the decisions already made, so we
> start on the same page and don't rebuild things that are settled.

---

## Aim

A single-file web app that **teaches Italian verb conjugation** (and the
supporting grammar) to a **complete beginner** — someone with no prior Italian
and no grammar background. It must be clear, simple, well structured, and
comfortable to use on an **iPad**. It is a **teaching tool first, a reference
second**.

## Who it's for

Absolute beginners. Assume **no knowledge of Italian or of grammar terms**.
Every concept is explained in plain English *before* any table is shown.

---

## Current state (last updated 28 July 2026)

- One self-contained file: **`index.html`** (identical copy: `italian-grammar.html`).
  No build step, no dependencies, runs offline, works as an "Add to Home Screen" app.
- **Four tabs:**
  - **Start here** — plain-English onboarding: what a verb is, what "conjugating"
    means, the three families, stem + ending, the six persons, what a tense is,
    and how to use the app.
  - **Reference** — soft pastel endings-pattern table + three-across colour-coded
    verb cards. Tense selector is sticky; every card is labelled with its tense.
    Tap 🔈 to hear a form; tap a card to see that verb in all tenses.
  - **Practice** — type or multiple-choice drills, accent bar (à è é ì ò ù),
    saved score/streak and a "my mistakes" review pool (browser local storage).
  - **Grammar** — sectioned side menu, ordered basic → advanced, starting with
    masculine/feminine.
- **Verbs:** 4 regular patterns (parlare, credere, dormire, capire) + 14 common
  irregulars, across **6 tenses/moods**: present, passato prossimo, imperfetto,
  futuro, condizionale, congiuntivo. Conjugations verified against Wiktionary.
- **Icon:** green "G" with a tricolore bar; embedded in the app + standalone PNGs.

## Locked design decisions (do NOT undo without checking first)

- **Soft pastel palette.** Strong/saturated fills were tried and **rejected** —
  they distract rather than help.
- **Teaching-first, beginner-first.** No jargon without a plain-English lead-in.
- **One colour = one meaning, across the whole site:**
  - Verb families: **-are green, -ere blue, -ire red, irregular amber**.
  - Stem = neutral grey; ending = the family's colour (kept subtle).
  - **io / tu / noi** consistency shown by **bold** (and underline for
    "shared by two"), *not* by strong colour bands.
  - Gender (Grammar only): **masculine violet, feminine pink** — never reused for verbs.
- **British English** throughout.
- Keep it a **single self-contained HTML file**.

## Files in this folder

- `index.html` — **the app** (the file that matters; GitHub Pages serves this one).
- `italian-grammar.html` — identical copy.
- `icon.png`, `apple-touch-icon.png`, `favicon-32.png` — icons.
- `icon-A.png`, `icon-C.png`, `icon-D.png`, `preview-*.png` — rejected icon options (safe to delete).
- `README.md` — this file.

## Hosting

- GitHub repo: **lewis182/Grammatica**. Pages URL once enabled:
  `https://lewis182.github.io/Grammatica/`. Re-upload `index.html` after each change.
- Local working folder: `E:\Italia Grammar`.

## How to resume in a new conversation

1. Make sure the `E:\Italia Grammar` folder is connected/selected.
2. Ask Claude to **read this README first**.
3. Then give the new instruction.

## Open ideas (discussed, not yet built)

- Plain-English intro + example sentence at the top of each tense in Reference.
- A "what next" step at the end of each Grammar lesson to keep guiding the learner.
- Example sentences per verb; a simple sentence-building exercise.
- Highlight the exact part of each irregular verb that breaks the rule.
- Spaced repetition in Practice.

---

## What's inside (summary)

A beginner-first Italian study app: a guided intro, a conjugation reference across
six tenses/moods, a practice/test mode, and a colour-coded grammar guide. Designed
for iPad — add it to the Home Screen to run full-screen and offline. Everything runs
client-side; there is no build step and no dependencies.
