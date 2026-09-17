---
name: create-interpretation
description: "Records a user-made ruling/interpretation for a 6: Siege – The Board Game rules case not clearly covered by the rulebook (a home-rule or a past ambiguous-question ruling), saving it to interpretations.md. Only ever invoked explicitly by the user — never triggered automatically to fill a gap in a rules answer."
---

# Create an Interpretation

Target file: `../../interpretations.md`

This skill records a **user-made** ruling for a rules situation that
`rules/` doesn't clearly cover — either a deliberate home-rule, or a past
ambiguous question the user already ruled on and wants remembered for next
time. It never invents the ruling itself; it only captures a decision the
user has made (or is making right now) and its reasoning.

**Trigger:** only ever run this skill when the user explicitly asks to
create/save/record an interpretation (or accepts a suggestion to do so
from `answer-rules-question`). Never invoke it on your own initiative to
"fill in" an answer.

## Process

1. **Identify the three parts** of the entry from the conversation so far
   and from the user's request:
   - **Title** — a short, descriptive name for the question/situation.
   - **Ruling** — the actual decision (what happens / what's allowed).
   - **Explanation** — the reasoning behind the ruling.

2. **Ask the user directly for anything that isn't already clear.** It's
   common for the ruling to be obvious from context (e.g. the user just
   stated it) but the explanation to be missing, or vice versa — don't
   guess or invent either one. Use your best judgment to propose a
   concise **title**, but confirm it with the user rather than assuming.

3. **Check `interpretations.md` for an existing entry with the same or a
   very similar title/topic.** If one exists, ask the user whether this
   should replace/update that entry or be added as a new, separate one
   (e.g. a related but distinct case).

4. **Append the new entry** to `interpretations.md`, following the format
   documented at the top of that file:
   ```
   ## <Title>

   **Ruling:** <the decision>

   **Explanation:** <the reasoning behind it>
   ```
   Keep the ruling and explanation concise but complete — write full
   sentences, don't just paraphrase down to nothing.

5. **Confirm back to the user** what was recorded (title, ruling, and
   explanation), so they can correct anything before it's finalized.

## Notes

- This skill only ever writes to `interpretations.md` — it does not touch
  any file under `rules/`, which remains a verbatim reproduction of the
  physical rulebook.
- Interpretations recorded here are picked up by `answer-rules-question`
  when a future question matches one, and are clearly labeled there as a
  user interpretation rather than official rule text.
