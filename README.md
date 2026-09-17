# 6: Siege – The Board Game — Rules Assistant

This repo is a structured, lookup-friendly rules reference for *6: Siege –
The Board Game*, built for use with GitHub Copilot CLI skills that answer
rules questions and record house-rule interpretations.

## Structure

- **`rules/`** — the active rules reference. `rules/_index.md` is the entry
  point (Quick Index, Glossary, Sections list); every other file is one
  topic/section, each carrying its physical rulebook page reference(s) and
  a "See also" trail to related sections. This is the only place skills
  read verbatim rule text from.
- **`interpretations.md`** — user-recorded rulings/home-rules for cases the
  rulebook doesn't clearly cover. Consulted only when `rules/` doesn't
  resolve a question, and always labeled as a user interpretation, never
  official rule text.
- **`icon-legend.md`** — maps the rulebook's graphical icons (e.g. hit dice
  colors, destruction ratings) to the emoji/text notation used in `rules/`.
- **`.github/skills/`** — the Copilot skills:
  - `answer-rules-question` — answers rules questions from `rules/`
    (falling back to `interpretations.md`), always with page citations.
  - `create-interpretation` — records a new entry in `interpretations.md`,
    only when explicitly requested by the user.
- **`rules-images/`** — page images of the original rulebook, kept for
  reference/verification.
- **`source-material/`** — complete rules files (`rules.md`: a full
  transcript of the rulebook; `rules-reference.md`: that transcript
  restructured into a reference). The active and usable rules are found in `rules/` — these are kept as source material for development and reference purposes.

## How it works

Ask a rules question and the `answer-rules-question` skill looks it up in
`rules/_index.md`, follows relevant sections, and answers with inline page
citations. To save a home-rule or a ruling for an ambiguous case, ask to
record an interpretation and the `create-interpretation` skill appends it to
`interpretations.md`.
