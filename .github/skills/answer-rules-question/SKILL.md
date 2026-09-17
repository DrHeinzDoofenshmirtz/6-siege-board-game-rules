---
name: answer-rules-question
description: "Answers questions about the 6: Siege – The Board Game rules by looking up rules/_index.md and following \"See also\" references until the question is fully answered, citing the physical rulebook page(s) the answer came from, and consulting interpretations.md for previously recorded user rulings when the rulebook alone doesn't resolve the question. Use whenever the user asks how a rule works, what a rule means, or whether something is allowed under the rules."
---

# Answer a Rules Question

Entry point: `../../rules/_index.md`

This skill answers rules questions **strictly and objectively** from the
verbatim rule text in `rules/`. It never invents rulings or interpretations
of its own — that is the separate job of the `create-interpretation` skill.

A secondary source, `../../interpretations.md`, holds user-recorded
rulings (home-rules or past ambiguous questions the user already ruled
on). It is consulted only when the rulebook text itself doesn't clearly
resolve the question — see step 6 below.

## Process

1. **Extract concepts from the question** — not exact rulebook phrasing.
   (e.g. "can I shoot through smoke?" → concepts: shooting, smoke, line of
   sight, protection.)

2. **Match those concepts against `rules/_index.md`**, in this order of
   preference:
   - **Quick Index** term column (the rulebook's own vocabulary — best exact
     or near-exact matches).
   - **Glossary** terms (for concepts only defined inline, e.g. "Adjacency").
   - **Sections** list, as a topic-level fallback when no specific term
     matches well.

3. **Load the best-matching section file(s)** from `rules/` — each is
   small and self-contained, and starts with its own page tag(s)
   (`p. X` / `p. X–Y`).

4. **Follow "See also" references if the loaded content doesn't fully
   answer the question.** Each section ends with a plain line like:
   ```
   See also: protection, destroy, upper-floor-areas
   ```
   Each token is a filename stem in `rules/` (i.e. `protection` →
   `rules/protection.md`). Load any of those that seem relevant, and keep
   following further "See also" references until the question is answered
   or no new relevant sections are being introduced (don't re-visit a file
   already loaded).

5. **Once `operators.md` exists** (it doesn't yet — it will eventually
   contain all Operator profiles and their gadget/ability rules), also
   consult it for any question about a specific Operator's ability. Treat
   it as a second source alongside `rules/`, not as an out-of-scope case.

6. **If, after exhausting `rules/` (including "See also" trails), the
   rulebook text still doesn't clearly and fully resolve the question,**
   load `../../interpretations.md` in full (it's a single small file —
   read all of it, not a partial search) and check whether an existing
   entry's title/topic matches this question.
   - **If a matching entry exists**, use its **Ruling** to answer that
     part of the question, and include its **Explanation** — but see the
     "No interpretation invented by this skill, ever" and "Answer Format"
     sections below for how this must be clearly distinguished from
     rulebook text.
   - **If no matching entry exists**, don't invent one. Give the
     rulebook-only answer (or say plainly the rulebook doesn't cover it),
     and — only when the ambiguity looks like the kind a house-rule/
     interpretation could usefully settle — suggest to the user that they
     can record one with the `create-interpretation` skill, briefly
     naming the specific ambiguity that's unresolved.

7. **Compose the answer using only the verbatim rule text actually
   loaded**, plus any matched interpretation from step 6 — never
   extrapolate or fill gaps with the skill's own assumptions.

8. **Cite the page(s) the answer relies on.** Cite only the page(s) of the
   sections/excerpts whose text actually contributed to the answer — not
   every section that was merely visited along the way. If multiple
   sections each contributed a distinct fact, cite all of their pages,
   ideally tied to which part of the answer each supports. Any part of
   the answer drawn from `interpretations.md` is cited by its entry title
   instead of a page number (see Answer Format).

## Answer Format

A citation-free or bare-minimum answer is **not acceptable**. Every answer
must let the user go verify it in the physical rulebook themselves.

1. **Structure:**
   - Lead with a **direct answer** to the question.
   - Follow with **comprehensive supporting detail**: every relevant
     condition, exception, threshold, and closely related mechanic that was
     actually found in the loaded section(s) — a thorough answer is
     preferred over a minimal one, as long as everything stated is grounded
     in loaded rule text. Don't stop at a bare yes/no if the rulebook has
     more to say that's relevant.
   - Close with a **consolidated source list**, one line per page cited,
     each naming what part of the answer it supports, e.g.:
     ```
     Sources:
     - p. 19 — protection ratings and line of cover
     - p. 24 — how a disputed protection rating is checked via a challenge
     ```
   - If any part of the answer used a matched entry from
     `interpretations.md`, add it to the same list using its title
     instead of a page, clearly marked, e.g.:
     ```
     - Interpretation: "<Entry Title>" — <what it settles>
     ```

2. **Citations:**
   - Every distinct rule statement, numeric value, exception, or condition
     included in the answer must carry **its own inline page citation**
     right where it's stated (e.g. "...heavy protection (– 3 hits) (p. 19)."),
     not just one citation for the whole answer.
   - Cite a page only where it adds real traceability value (a rule
     statement, a number, an exception) — not on every single sentence of
     connective prose.
   - The consolidated source list at the end must match the inline
     citations used — same "only pages that actually contributed" rule
     from the Process section above, restated here as part of the answer's
     required shape.
   - If a relied-upon fact comes from an **assembled multi-excerpt
     section** (e.g. `gadget-icons`, which has separate `p. 26–27` and
     `p. 28` sub-tags), cite the specific sub-tag that fact came from, not
     the section's overall page range.

3. **No interpretation invented by this skill, ever:**
   - This skill never invents, guesses, extrapolates, averages multiple
     partial rules together, or offers a "most likely" ruling of its own.
     Keep a hard line between "the rulebook says X (p. Y)" and any implied
     reasoning — only ever restate/quote what's written.
   - **Surfacing an existing recorded interpretation is not the same as
     inventing one**, and is allowed: if step 6 of the Process found a
     matching entry in `interpretations.md`, use its Ruling and include
     its Explanation — but the answer must make unmistakably clear which
     part is rulebook text and which part is a **user interpretation**
     (e.g. "Per your recorded interpretation *"<Title>"*: <ruling>.
     Reasoning: <explanation>."). Never blend an interpretation into the
     prose as if it were rulebook text.
   - If no matching sections or interpretation cover the question,
     **say so plainly and stop there** — do not fill the gap with the
     skill's own logic. If the ambiguity looks like something a
     house-rule could usefully settle, suggest the user record one via
     the `create-interpretation` skill, naming the specific point that's
     unresolved. That's the only next step this skill offers; producing
     the ruling itself remains the user's call (via that skill), never
     this one's.

## Notes

- Exact handling of edge cases (e.g. Quick Index terms with no page, `—`)
  is still being designed — for now, stay conservative and objective:
  quote/cite the rules found, and be explicit if the rulebook doesn't
  pin something to a specific page.
- This skill's instructions are expected to be refined once tested against
  real questions.
