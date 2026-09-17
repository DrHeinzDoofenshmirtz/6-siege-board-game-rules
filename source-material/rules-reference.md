# 6: Siege – The Board Game — Rules Reference Guide

## About this guide

This is a **lookup-oriented reorganization** of `rules.md` (the rulebook,
transcribed in its original, learn-to-play order). No rule has been
reworded, interpreted, or changed — every rule below is copied verbatim from
`rules.md`. What has changed is the **structure**:

- Content is split into topical sections (one per rule subject) instead of
  the book's front-to-back reading order.
- Every section carries a **page reference** (`p. X` or `p. X–Y`) tracing it
  back to the physical rulebook, taken from the `--- Page N ---` markers in
  `rules.md` (each marker means everything after it, up to the next marker,
  is on that page).
- Where the rulebook's own **Index** (p. 34 of `rules.md`) shows that a term
  is discussed with real rule substance in more than one place, those
  verbatim excerpts are gathered together in one section (each excerpt still
  keeps its own page tag) instead of being scattered — see the "Cover /
  Protection" and "Icons used for gadgets" sections for examples.
- Every section ends with a **See also** line pointing to other sections
  that are genuinely related, so a reader can keep following the trail until
  a question is fully answered.
- This is currently a single file, but every section below is written to be
  self-contained, so it can be split into its own file later (its anchor id
  is its planned filename) without rewriting anything.
- Icon meanings (⚠️, ▲, ■, ⬟, 🔩, 🔌, 👁️, 🎯, 💀, ❗, etc.) are documented in
  `rules/icon-legend.md` and are not repeated here.

This guide only restructures `rules.md`. It excludes purely bibliographic
content that isn't a rule: the Introduction, the book's page-number Contents
list, the Components list, and the book's own page-number Index (that Index
is reused below as *data*, to build the Quick Index and cross-references,
then not carried over as a section itself). Individual Operators' special
gadget abilities are documented in `operators.md` (per `rules/icon-legend.md`) and
are out of scope here — this guide covers only the general rules in
`rules.md`.

## Quick Index (by rulebook term)

This mirrors the rulebook's own Index (p. 34), with an added column linking
each term straight to the relevant section(s) of this guide. Where the
rulebook's Index lists a term with no page (`—`), that is preserved as-is —
it means the rulebook itself doesn't define that term on a specific page.

| Term | Page(s) | Reference Guide section(s) |
|---|---|---|
| ⚠️ (extra movement point) | 17 | [Move](#move) |
| Action | — | [Operator Actions](#operator-actions), [Activating an Operator](#activating-an-operator) |
| ACTION — Destroy | 15, 16 | [Destroy Action](#destroy) |
| ACTION — Run | 18 | [Run](#run) |
| ACTION — Move | 18 | [Move](#move) |
| ACTION — Overwatch | 20 | [Overwatch Action](#overwatch) |
| ACTION — Shoot | 18 | [Shoot Action](#shoot) |
| ACTION — Use Tactical Gadget | 22 | [Use Tactical Gadget Action](#use-tactical-gadget) |
| ACTION — Use a Special Gadget effect | 22 | [Use a Special Gadget ACTION Effect](#use-special-gadget-action) |
| Activation (Operator) | 14, 15 | [Gameplay Sequence](#gameplay-sequence), [Activating an Operator](#activating-an-operator) |
| Adjacency | 7 | [Main Floor](#main-floor) |
| Application (App) | 2, 12 | [Setup Sequence](#setup-sequence), [Game Speed Setting](#game-speed-setting) |
| Area capacity | 7, 8, 9 | [Main Floor](#main-floor), [Partitions](#partitions), [Upper Floor Areas](#upper-floor-areas) |
| Barricade | 8, 19 | [Partitions](#partitions), [Protection](#protection) |
| Breach | 8, 23 | [Partitions](#partitions), [Destroy Action](#destroy) |
| Camera | 28 | [Tactical Gadgets for Defenders](#defender-gadgets) |
| Challenges | 24 | [Challenges](#challenges) |
| Charge cube | 12, 22 | [Squad Selection](#squad-selection), [Use Tactical Gadget Action](#use-tactical-gadget), [Use a Special Gadget ACTION Effect](#use-special-gadget-action) |
| Deployment | 13 | [Deployment](#deployment) |
| Destruction rating ⚠️🟧⬟ | 23, 26 | [Destroy Action](#destroy), [Icons Used for Gadgets](#gadget-icons) |
| Door | 7, 23 | [Room](#room), [Destroy Action](#destroy) |
| Eliminated (Operator) | 10 | [Operator Status](#operator-status) |
| Exchange of fire | 21 | [Overwatch Action](#overwatch) |
| Fortified Entryway | 28 | [Tactical Gadgets for Defenders](#defender-gadgets) |
| Fortified wall | 8, 19 | [Partitions](#partitions), [Protection](#protection) |
| Free action | 20 | [Free Action](#free-action) |
| Free space | 7 | [Main Floor](#main-floor) |
| Gadgets | 11, 25 | [Operator Profile](#operator-profile), [General Remarks on Gadgets](#gadgets-general) |
| Gameplay sequence | 14 | [Gameplay Sequence](#gameplay-sequence) |
| Heavy wall | 8, 19 | [Partitions](#partitions), [Protection](#protection) |
| Hidden (Operator) | 10, 15 | [Operator Status](#operator-status), [Activating an Operator](#activating-an-operator) |
| Hit dice | 11 | [Operator Profile](#operator-profile) |
| Holed wall | 8, 19 | [Partitions](#partitions), [Protection](#protection) |
| In play (Operator) | 10 | [Operator Status](#operator-status) |
| KEYWORD — Overlays | 27 | [Gadget Effect Keywords](#gadget-keywords) |
| KEYWORD — Line of sight | 27 | [Gadget Effect Keywords](#gadget-keywords) |
| KEYWORD — Throwable | 27 | [Gadget Effect Keywords](#gadget-keywords) |
| KEYWORD — Deployable | 27 | [Gadget Effect Keywords](#gadget-keywords) |
| KEYWORD — Wave | 27 | [Gadget Effect Keywords](#gadget-keywords) |
| KEYWORD — Setup | 7, 27 | [Gadget Effect Keywords](#gadget-keywords), [Partitions](#partitions) |
| KEYWORD — Vertical | 7, 27 | [Room](#room), [Gadget Effect Keywords](#gadget-keywords) |
| Leaning position | 17, 19, 26 | [Leaning](#leaning), [Protection](#protection), [General Remarks on Gadgets](#gadgets-general) |
| Light wall | 8, 19 | [Partitions](#partitions), [Protection](#protection) |
| Line of cover | 19 | [Protection](#protection) |
| Line of sight | 6, 9, 25 | [Line of Sight](#line-of-sight), [Upper Floor Areas](#upper-floor-areas), [Checking Lines of Sight](#checking-lines-of-sight) |
| Limited components | 29 | [Limited Components](#limited-components) |
| Located 🎯 | 9 | [Operator Status](#operator-status) |
| Main floor | 7 | [Main Floor](#main-floor) |
| Missions | 5, 11 | [Aim of the Game](#aim-of-the-game), [Setup Sequence](#setup-sequence) |
| MODULE — Forward Planning | 5, 30 | [Forward Planning Module](#forward-planning-module) |
| MODULE — Advanced Tactics | 30 | [Advanced Tactics Module](#advanced-tactics-module) |
| MODULE — Competitive Gaming | 31 | [Competitive Gaming Module](#competitive-gaming-module) |
| Multiplayer mode | 31 | [Multiplayer Mode](#multiplayer-mode) |
| 'No App' variant | 29 | ['No App' Variant](#no-app-variant) |
| Obstacle | 8, 19 | [Partitions](#partitions), [Protection](#protection) |
| Occupied space | 7 | [Main Floor](#main-floor) |
| Operator profile | 11 | [Operator Profile](#operator-profile) |
| Overwatching (Operator) | 10, 20 | [Operator Status](#operator-status), [Overwatch Action](#overwatch) |
| Partitions | 8, 23 | [Partitions](#partitions), [Destroy Action](#destroy) |
| Perimeter space | 7, 13 | [Room](#room), [Deployment](#deployment) |
| Protection | 19 | [Protection](#protection) |
| Range | 11, 18 | [Operator Profile](#operator-profile), [Shoot Action](#shoot) |
| Reaction | 22, 24 | [Use a Special Gadget ACTION Effect](#use-special-gadget-action), [Operator Reactions](#operator-reactions) |
| Recruit | 31 | [Multiplayer Mode](#multiplayer-mode) |
| Reroll token | 29, 32 | [Reroll](#reroll), [Rapid Deployment (Multiplayer)](#rapid-deployment-multiplayer) |
| Reveal (hidden Operator) | 10, 21 | [Operator Status](#operator-status), [Overwatch Action](#overwatch) |
| Riposte | 22 | [Riposte](#riposte) |
| Room | 7 | [Room](#room) |
| Room 🔲 | 7, 27 | [Room](#room), [Gadget Effect Keywords](#gadget-keywords) |
| Shield 🛡️ | — | [Operator Profile](#operator-profile), [Protection](#protection) |
| Shot | 18, 21, 22 | [Shoot Action](#shoot), [Overwatch Action](#overwatch), [Riposte](#riposte) |
| Space | 7 | [Main Floor](#main-floor) |
| Stamina | 11 | [Operator Profile](#operator-profile) |
| Straightening up | 18 | [Leaning](#leaning) |
| Strength rating ⚠️🟧⬟ | 23, 26 | [Destroy Action](#destroy), [Icons Used for Gadgets](#gadget-icons) |
| Structural element | 8 | [Partitions](#partitions) |
| Stunned 💀 | 9 | [Operator Status](#operator-status) |
| Tactical gadgets | 28 | [Tactical Gadgets for Defenders](#defender-gadgets), [Tactical Gadgets for Attackers](#attacker-gadgets) |
| Tactical inventory | 12, 22 | [Squad Selection](#squad-selection), [Use Tactical Gadget Action](#use-tactical-gadget) |
| Timer | 12, 15, 18, 24 | [Game Speed Setting](#game-speed-setting), [Activating an Operator](#activating-an-operator), [Shoot Action](#shoot), [Challenges](#challenges) |
| Upper floor area | 8, 18, 20, 21 | [Partitions](#partitions), [Leaning](#leaning), [Overwatch Action](#overwatch) |
| Window | 7, 23 | [Room](#room), [Destroy Action](#destroy) |
| Wound 💀 | 11 | [Operator Profile](#operator-profile) |

## Glossary (terms defined inline, without their own section)

Some rulebook terms are defined in a sentence or two *inside* a larger
section rather than under their own heading. These entries give the exact
verbatim definition plus a link to the full section it lives in.

- **Adjacency** *(p. 7)* — "Spaces with a shared boundary are said to be
  adjacent if a line of sight can be drawn between them. This means that a
  space can be adjacent to the 8 spaces around it." See [Main Floor](#main-floor).
- **Occupied space / Free space** *(p. 7)* — "Spaces can contain no more
  than one Operator and one gadget. A space with an Operator or an obstacle
  in it is 'occupied'. Spaces containing no Operator or obstacles are
  'free'." See [Main Floor](#main-floor).
- **Perimeter space** *(p. 7)* — "The dark green spaces around the edges of
  the game board (referred to as 'perimeter spaces') represent the
  approaches to the building. These perimeter spaces are never part of a
  room." See [Room](#room).
- **Structural element** *(p. 8)* — "This type of space represents an
  impassable structural element. This space is surrounded by sections of
  heavy wall. Structural elements can never be targeted, and no game
  components can be placed there." See [Partitions](#partitions).
- **Entryway space ◈** *(p. 8)* — "An entryway space ◈ is a space on the main
  floor to which a few additional rules apply." See [Partitions](#partitions)
  for the full definition and rules.

## Sections (in this guide's topical order)

*Core concepts & victory*
[Core Concepts](#core-concepts) · [Aim of the Game](#aim-of-the-game)

*The environment*
[Game Areas](#game-areas) · [Environment](#environment) · [Line of Sight](#line-of-sight) ·
[Main Floor](#main-floor) · [Room](#room) · [Partitions](#partitions) ·
[Upper Floor Areas](#upper-floor-areas)

*Operators*
[Operators](#operators) · [Operator Status](#operator-status) · [Operator Profile](#operator-profile)

*Setup*
[Setup Sequence](#setup-sequence) · [Squad Selection](#squad-selection) ·
[Game Speed Setting](#game-speed-setting) · [Deployment](#deployment)

*Playing the game*
[Gameplay Sequence](#gameplay-sequence) · [Activating an Operator](#activating-an-operator) ·
[Operator Actions](#operator-actions)

*Operator actions*
[Move](#move) · [Leaning](#leaning) · [Run](#run) · [Shoot Action](#shoot) ·
[Protection](#protection) · [Free Action](#free-action) · [Overwatch Action](#overwatch) ·
[Riposte](#riposte) · [Use Tactical Gadget Action](#use-tactical-gadget) ·
[Use a Special Gadget ACTION Effect](#use-special-gadget-action) · [Destroy Action](#destroy)

*Reacting & resolving disputes*
[Operator Reactions](#operator-reactions) · [Challenges](#challenges) ·
[Checking Lines of Sight](#checking-lines-of-sight)

*Gadgets*
[General Remarks on Gadgets](#gadgets-general) · [Icons Used for Gadgets](#gadget-icons) ·
[Gadget Effect Keywords](#gadget-keywords) · [Tactical Gadgets for Defenders](#defender-gadgets) ·
[Tactical Gadgets for Attackers](#attacker-gadgets)

*Other rules & variants*
[Other Important Rules](#other-important-rules) · [Fairplay and Pauses](#fairplay-and-pauses) ·
[Effects and Rules](#effects-and-rules) · [Limited Components](#limited-components) ·
['Back in the Box'](#back-in-the-box) · [Reroll](#reroll) · ['No App' Variant](#no-app-variant)

*Special Ops modules*
[Special Ops Modules](#special-ops-modules) · [Forward Planning Module](#forward-planning-module) ·
[Advanced Tactics Module](#advanced-tactics-module) · [Competitive Gaming Module](#competitive-gaming-module)

*Multiplayer*
[Multiplayer Mode](#multiplayer-mode) · [4 Players: 2 v 2](#four-players-2v2) ·
[Rapid Deployment (Multiplayer)](#rapid-deployment-multiplayer) · [3 Players: 2 v 1](#three-players-2v1)

*Other*
[Alternative Profiles](#alternative-profiles) · [Hints and Tips](#hints-and-tips)

---

## Core Concepts {#core-concepts}
*p. 5*

In *6: Siege – The Board Game*, each player commands a squad of Operators.
Players are either attackers or defenders, each with unique means of
achieving victory.

The **attacker** begins the game outside the building complex, whereas the
**defender** is hidden inside.

Games last up to 6 rounds, each organized in 5 phases:

1 – Attacker's first activation phase
2 – Defender's first activation phase
3 – Attacker's second activation phase
4 – Defender's second activation phase
5 – Upkeep phase

During each activation phase, players take turns to activate some of their
Operators, each able to perform one movement action and two additional
actions.

Use your Operators' weapons to try to eliminate opposing Operators that
stray into line of sight.

You can also use gadgets and actions to re-shape the terrain, by breaching
walls, barricading doors, or tossing a smoke grenade into a room, for
example.

Making your way to the upper floor lets you move around more discreetly.
Operators can also overwatch areas, instantly firing at any opponents that
come into sight! Operators can also gain protection from a wall or obstacle
by leaning.

The action unfolds within a limited time, managed by an app.

**See also:** [Gameplay Sequence](#gameplay-sequence), [Aim of the Game](#aim-of-the-game)

## Aim of the Game {#aim-of-the-game}
*p. 5–6*

Win the game by either fulfilling the chosen mission's victory conditions or
eliminating all members of the opposing squad. If the last remaining
Operator in both squads is eliminated during the same activation, nobody
wins.

There are three types of mission, each with a specific objective:

- **Control mission:** The attackers and defenders compete for control over
  areas in order to score victory points. We recommend the Control mission
  for new players, as it is ideal for learning the game.
- **Bomb mission:** The attackers must defuse one of two interconnected
  bombs. The defenders' goal is to stop them.
- **Hostage mission:** The attackers' objective is to extract a hostage from
  the play area. The defenders must prevent them.

These missions are described in greater detail in the *Mission Guide*.

To give you a taste of what awaits you in *6: Siege – The Board Game*, the
following example shows a phase in a game round during which the attacker is
activating 3 of their Operators with the aim of taking up a position inside
a room in the Consulate.

[DIAGRAM]

Example: Attacker activation sequence (1 — Thermite, 2 — Ash, 3 — Sledge)

1. Thermite destroys the barricade (⚠️1). He deploys a drone, which then
   moves. The drone scans the room around it: Bandit receives a 🎯 Located
   marker.
2. Ash moves in front of the barricade. As Bandit has been located, Ash has
   a line of sight through the barricade. She shoots at Bandit, eliminating
   him. Ash resumes her movement, reaching the upper floor via an entryway
   space.
3. Sledge destroys the barricade (⚠️1). He moves, then leans into an opening
   in the room to overwatch the hallway facing him.

**See also:** [Setup Sequence](#setup-sequence), [Core Concepts](#core-concepts)

## Game Areas {#game-areas}
*p. 6*

The following play areas are arranged around the game board (aka 'the
environment'):

- Defending squad's tactical area
- General supply
- Attacking squad's tactical area

**See also:** [Environment](#environment), [Squad Selection](#squad-selection)

## Environment {#environment}
*p. 6*

Each side of the game board depicts a building, referred to as the
environment. Only one floor of this building, the 'main floor', is shown in
full. The building's other floors are represented by two upper floor areas
(one for the defender, the other for the attacker). The main floor is
divided into a grid of square spaces. Walls or barricades are present on the
boundaries between some of these spaces.

[DIAGRAM]

**See also:** [Main Floor](#main-floor), [Upper Floor Areas](#upper-floor-areas), [Line of Sight](#line-of-sight)

## Line of Sight {#line-of-sight}
*p. 6–7*

Line of sight interacts with all game components, and the environment in
particular. Some actions and game effects require a line of sight (for
example, an Operator needs a line of sight to their target when shooting).

*Definition*

A line of sight is an imaginary straight line linking the central dots in
two spaces that is not broken by any of the following elements:

- a partition;
- a space containing a Smoke or Gas overlay;
- a space containing an Operator, other than the targeted space.

Operators can draw a line of sight in any direction at all times.

*Checking line of sight*

During the game, players are not allowed to check lines of sight using an
LoS Ruler or other means, except when challenging an opponent's claimed line
of sight (see Challenges, p. 24).

[DIAGRAM]

Example: Line of sight

1. Mute has line of sight to Thermite, as the imaginary line between the
   centers of the spaces containing these two Operators is not broken by a
   partition, an overlay, or another Operator.
2. He does not have line of sight to IQ, however, as the line between the
   centers of their respective spaces is broken by a partition (marked with
   a dot in the diagram).

**See also:** [Checking Lines of Sight](#checking-lines-of-sight), [Challenges](#challenges), [Partitions](#partitions), [Upper Floor Areas](#upper-floor-areas), [Shoot Action](#shoot)

## Main Floor {#main-floor}
*p. 7*

*Spaces on the main floor*

[DIAGRAM]

A game component in a space fully occupies that space. When targeting a
space containing a game component, target the space's central dot.

*Adjacent spaces*

Spaces with a shared boundary are said to be adjacent if a line of sight can
be drawn between them. This means that a space can be adjacent to the 8
spaces around it.

[DIAGRAM]

Example: Adjacency

- Lines of sight to spaces having a shared boundary with the space occupied
  by Smoke.
- Spaces considered adjacent to Smoke's space.
- Spaces not considered adjacent to Smoke's space.

*Area capacity*

Spaces can contain no more than one Operator and one gadget. A space with an
Operator or an obstacle in it is 'occupied'. Spaces containing no Operator or
obstacles are 'free'.

**See also:** [Room](#room), [Partitions](#partitions), [Move](#move), [Line of Sight](#line-of-sight)

## Room {#room}
*p. 7–8*

A room consists of a group of spaces inside a perimeter represented by a
dotted outline on the game board. Some gadgets affect a whole room. Actions
performed in any space in the room will be subject to the gadget's effects.

*Room 🔲 (room icon)*

An additional rule applies to rooms that have 🔲 icons in their corners:
Operators on the upper floor may perform an action with a **Vertical** gadget
targeting any space in a room.

[DIAGRAM]

Example: Room

- Room perimeter
- These icons show that this is a 🔲 room

*Perimeter space*

The dark green spaces around the edges of the game board (referred to as
'perimeter spaces') represent the approaches to the building. These
perimeter spaces are never part of a room.

[DIAGRAM]

Decorative elements printed on the game board are not obstacles, walls,
windows, or icons, and have no impact on the game. This means that gameplay
is unaffected by pot plants, parapets, guard rails, and other decorative
features.

The wall's thickness and the chair have no influence on gameplay.

*Door and window*

Operators can move through doors and windows, which also do not block line
of sight.

These elements can be fortified by erecting a barricade (see Barricades,
p. 8).

*Door*

[DIAGRAM]

A door is represented by one or two sections marked with a cross. All doors
shown directly on the game board are 'open'.

*Window*

[DIAGRAM]

A window may occupy either 1 or 2 space sections.

NOTE Moving through a window costs 1 extra movement point (see Move, p. 16).

**See also:** [Partitions](#partitions), [Gadget Effect Keywords](#gadget-keywords), [Move](#move), [Deployment](#deployment)

## Partitions {#partitions}
*p. 8*

Walls and barricades are collectively referred to as 'partitions'.

All partitions except Holed walls block line of sight.

*Walls*

[DIAGRAM]

A space section covered by a wall is a 'wall section'. A wall consists of
one or more wall sections, in some cases leading to a protruding wall. A
wall is represented by a white outline (which is part of the wall).

Walls of all types are impassable to Operator movements.

There are four types of wall.

[DIAGRAM]

**Heavy wall:** May provide heavy protection to Operators (see Protection,
p. 19). Heavy walls are indestructible.

*Area capacity:* Wall-mounted gadgets (see Gadget, p. 25) can only be
mounted on heavy wall sections. A wall section can only accommodate one
gadget, which belongs to the space into which it faces. No other gadgets can
be deployed at that space.

[DIAGRAM]

**Fortified wall:** Provides the same level of protection as a heavy wall,
but can be destroyed by gadgets with the ⬟3 destruction rating.

[DIAGRAM]

**Light wall:** May provide light protection to Operators (see Protection,
p. 19). This type of wall can be destroyed by a gadget or an Operator with
the 🟧2 or ⬟3 destruction rating.

[DIAGRAM]

**Holed wall:** Provides the same level of protection as a light wall, but
does not block line of sight. This type of wall can be destroyed by a gadget
or an Operator with the 🟧2 or ⬟3 destruction rating.

NOTE Holed walls are only used in the game's expansions.

*Barricades*

Barricades may be placed over doors and windows printed on the game board.
Barricades may provide light protection to Operators (see Protection,
p. 19).

[DIAGRAM]

Barricaded Door standee / Barricaded Window standee

A barricade is represented by a standee placed on a door or window.

Barricades can be destroyed by a gadget or an Operator with the ⚠️1, 🟧2, or
⬟3 destruction rating.

*Breach*

[DIAGRAM]

A Breach standee represents the rubble from a destroyed wall. It covers and
replaces one or more destroyed wall sections.

Breaches do not block line of sight.

NOTE Moving through a breach costs 1 extra movement point (see Move, p. 16).

*Obstacle*

[DIAGRAM]

Obstacles can occupy a single space or extend over multiple spaces. They are
indestructible, do not block line of sight, and may provide light protection
to Operators.

NOTE Scaling an obstacle costs 1 extra movement point (see Move, p. 16).

*Structural element*

[DIAGRAM]

This type of space represents an impassable structural element. This space
is surrounded by sections of heavy wall.

Structural elements can never be targeted, and no game components can be
placed there.

*Entryway space* ◈

[DIAGRAM]

An entryway space ◈ is a space on the main floor to which a few additional
rules apply.

All Operators can use gray entryway spaces to move to or from an upper floor
area. Blue entryway spaces can only be used by **attackers** (see Moving
between floors, p. 18).

The following components can only be placed on entryway spaces:

- an Entryway Overwatch token (see Overwatch action, p. 20). Operators treat
  entryway spaces as neutral if they either have no Entryway Overwatch
  token, or one deployed by their own squad. For the **defender**, blue
  entryway spaces are not neutral;
- a Fortified Entryway token (see Gadgets, p. 25), subject to the area
  capacity of one gadget per space.

**See also:** [Protection](#protection), [Destroy Action](#destroy), [Upper Floor Areas](#upper-floor-areas), [Leaning](#leaning), [Icons Used for Gadgets](#gadget-icons)

## Upper Floor Areas {#upper-floor-areas}
*p. 8–9*

Each squad has an upper floor area consisting of two spaces. These spaces
represent the existence of other floors of the building, allowing Operators
to move around more quickly, shoot, or deploy gadgets from an upper floor
area.

*Space in an upper floor area*

[DIAGRAM]

Only defenders may use orange spaces; blue spaces are exclusively for
attackers.

Spaces in upper floor areas are not considered to be adjacent to each other
or adjacent to the entryway spaces on the main floor.

However, some actions and reactions may be performed from an upper floor
area into entryway spaces or 🔲 rooms.

*Area capacity*

Each space in an upper floor area can accommodate no more than one Operator
(represented by a miniature or a Hidden Operator token).

*Line of sight*

An Operator in an upper floor area has line of sight to all gray entryway
spaces. Note that the line of sight extends no further than the entryway
space. An **attacker**'s Operator in an upper floor area also has line of
sight to all blue entryway spaces.

This line of sight may be blocked by:

- an opposing Entryway Overwatch token;
- a Fortified Entryway token;
- a Smoke or Gas overlay.

NOTE Operators in entryway spaces do not have line of sight to the upper
floor.

**See also:** [Partitions](#partitions), [Line of Sight](#line-of-sight), [Overwatch Action](#overwatch), [Leaning](#leaning)

## Operators {#operators}
*p. 9*

Each player leads a squad of Operators, hand-picked from special forces
units of various nationalities.

*Operator representation*

Each Operator is represented in the tactical area by a miniature on the game
board (for a revealed Operator) or by their 2 Hidden Operator tokens.

[DIAGRAM]

Ash's miniature (revealed) / Mute's Hidden Operator token (decoy side /
portrait side) — marks showing the front of the Operator and the
overwatched direction.

NOTE Rules that mention an Operator's miniature also apply to Operators
represented on the board by a Hidden Operator token.

**See also:** [Operator Status](#operator-status), [Operator Profile](#operator-profile)

## Operator Status {#operator-status}
*p. 9–11*

An Operator's status can be changed during the game.

Some statuses are indicated by a marker. Each miniature or token
representing an Operator can have only one Status marker of each type.

*Status marker: Located*

[DIAGRAM]

Operators become Located when hit by a Shoot action. They may also be
Located by a drone, camera, or special gadget. Place a 🎯 Located marker on
their miniature base.

Revealed Operators that receive a 🎯 marker.

Line of sight to Located Operators **is no longer broken** by light walls,
barricades, and spaces containing a Smoke or Gas overlay.

*Status marker: Stunned*

[DIAGRAM]

Operators may be Stunned by a flashbang grenade or a special gadget. Place a
Stunned marker on their miniature base. Operators that perform a Shoot
action while Stunned roll two 🟡 yellow Hit dice instead of the dice they
would normally roll.

*Status marker: Overwatch*

[DIAGRAM]

While overwatching, an Operator can Riposte during the opposing Operator
activation phase (see Overwatch action, p. 20).

*Eliminated / In play*

[DIAGRAM]

An Operator who sustains a number of wounds 💀 equal to or greater than
their Stamina stat is eliminated. Remove their miniature and all items on
their profile and put them back in the box. Flip the Operator profile to
show its 'Eliminated' side. Any gadgets deployed in the environment by the
eliminated Operator remain in play.

Twitch's profile — 'Eliminated' side.

Operators are considered to be 'in play' until they are eliminated.

*Revealed / Hidden Operators*

The **attacker**'s Operators begin the game revealed (i.e. represented by
miniatures).

The **defender**'s Operators, on the other hand, are initially hidden! Each
Hidden Operator is represented on the game board by two Hidden Operator
tokens: a decoy, and a portrait indicating their true location. The
defender may secretly look at their Hidden Operator tokens at any time.

Like an Operator miniature, the two Hidden Operator tokens each occupy a
space, blocking line of sight.

- **Revealing a hidden Operator – By the defender:** The defender may decide
  to reveal a hidden Operator at any time, in order to perform certain
  actions or reactions. This does not cost an action.

  NOTE An overwatching hidden Operator who decides to Riposte is
  automatically revealed before the shot is resolved (see Riposte, p. 22).

  NOTE A hidden Operator wishing to perform a **REACTION** enabled by a
  special gadget effect may do so by spending a Charge cube, with no need to
  reveal themselves.

- **Revealing a hidden Operator – By the attacker:** The attacker may, at
  any time and without spending an action, ask the defender to reveal a
  Hidden Operator token in the following situations:

  - if the **hidden Operator** is in direct line of sight of one of their
    own **Operators** (not just in a space that they are overwatching). The
    defender may challenge the validity of the claimed line of sight (see
    Challenges, p. 24);
  - if the **hidden Operator** sustains one or more wounds;
  - if **one of their Operators** uses a gadget that locates **hidden
    Operators**.

[DIAGRAM]

Example: Operator revealed by a line of sight — Ash is entering a space
where she has line of sight to one of Smoke's Hidden Operator tokens.

[DIAGRAM]

Example: Operator revealed by a drone — Ash has deployed a drone, which
enters the room containing one of Smoke's Hidden Operator tokens. The
drone scans the token's true nature.

[DIAGRAM]

Example: Operator revealed by a wound — Ash has thrown a grenade into an
area containing one of Smoke's Hidden Operator tokens. Reveal the token if
he sustains one or more wounds from the grenade.

**See also:** [Overwatch Action](#overwatch), [Riposte](#riposte), [Challenges](#challenges), [Activating an Operator](#activating-an-operator), [Operator Profile](#operator-profile)

## Operator Profile {#operator-profile}
*p. 11*

*WEAPONS*

**Range categories:** Weapons can have a short (1-3 spaces), medium
(4-6 spaces) or long range (7 or more spaces). The range category affects
the number and color of Hit dice rolled for a shot.

**Hit dice:** On average, a yellow die 🟡 rolls 1 hit, versus 1.5 hits for an
orange die 🟠 and 2 hits on a red one 🔴. When shooting at a target with
protection, do not roll any dice with a lightning symbol (e.g. 🟡⚡).

[DIAGRAM]

Example Operator profile card (Blitz, attacker):

- WEAPONS — RANGE 1-3: 🟡🟡🟡⚡ | 4-6: 🟠🟠🟠⚡ | 7+: 🔴🔴⚡
- FLASH SHIELD CHARGES 🧊🧊 — **ACTION** → Deployable — All Operators in the
  room containing the targeted space receive a Stunned marker, except
  Blitz.
- 🛡️ Shield icon present
- RUN 2
- DESTROY ⚠️
- STAMINA 💀5

*SPECIAL GADGETS*

Each Operator has a unique special gadget, as shown on their profile.

**Gadget name and related icons**

**Gadget effect(s):** effects preceded by the **ACTION** icon require the
Operator to spend an action in order to apply them. Effects preceded by the
**REACTION** icon are generally triggered during the opponent's activation
phase and do not cost an action. Effects with neither the **ACTION** nor
**REACTION** icon are permanent, and remain active at all times.

Some effects have one or more keywords (see Gadgets, p. 25).

**Charge cube slots:** Some actions and reactions require an Operator to
spend a 🧊 Charge cube.

**Shield:** Operators with the 🛡️ icon on their profile have permanent light
protection against shots (see Protection, p. 19).

**Stamina:** The number of wounds 💀 that must be inflicted to eliminate an
Operator.

**Destroy:** The destruction-rating icons (⚠️/🟧/⬟) shown on an Operator's
profile indicate their destruction rating when they perform the Destroy
action.

*Run:* This number (2 or 5) indicates the number of additional movement
points granted by the Run action. Operators with the '–' character cannot
run.

*Effects of revealing a hidden Operator*

Place the revealed hidden Operator's miniature in the space that contains
the token indicating their true position. Leave the orientation (indicated
by the marker on the token) unchanged and keep any status markers.

Place an Overwatch marker on the front of the miniature base, showing the
previously overwatched direction, unless the revealed Operator is currently
in their activation phase.

Then put the two Hidden Operator tokens back in the box.

These operations are not actions, and do not trigger reactions (see
Operator reactions, p. 24).

[DIAGRAM]

**See also:** [Protection](#protection), [Destroy Action](#destroy), [Operator Status](#operator-status), [Run](#run), [Shoot Action](#shoot), [Gadget Effect Keywords](#gadget-keywords)

## Setup Sequence {#setup-sequence}
*p. 11–12*

The setup phase is an integral part of the *6: Siege – The Board Game*
experience. Your choices at this stage in selecting Operators for your squad
and deploying them to the game board will have a critical impact on the
game.

*Mission selection*

In the *Mission Guide*, choose an environment and select a mission (Control,
Bomb, or Hostage).

NOTE For your first few games, we recommend picking the Control mission and
the Consulate environment (see *Mission Guide*).

Place the game board representing the chosen environment in the middle of
the table. Place the device on which you installed the app near the game
board, together with the 2 LoS Rulers and 7 Hit dice.

Form the general supply near the game board. Put all Breach standees, Wound
tokens 💀, Located 🎯 and Stunned 🟡 markers in the supply, along with the
Drone marker and all the overlays. Place the Round Tracker marker on the
first space (0) on the Round Tracker.

Put an obstacle of the appropriate shape in each obstacle location.

[DIAGRAM]

Example: Obstacle setup

Lastly, set up the following required components, as instructed in the
selected mission (see *Mission Guide*):

- Bomb, Hostage, or Control tokens and miniatures specific to the selected
  mission;
- Barricade standees;
- 5 Camera miniatures (oriented as instructed);
- 3 Barbed Wire tokens (except for Control missions);
- 2 Fortified Entryway tokens (except for Control missions).

**See also:** [Squad Selection](#squad-selection), [Game Speed Setting](#game-speed-setting), [Deployment](#deployment), [Aim of the Game](#aim-of-the-game)

## Squad Selection {#squad-selection}
*p. 12*

Decide who will play as the **attacker** and who will be the **defender**.

Players simultaneously and secretly form their respective squads, picking 5
of the Operators available for their role (i.e. attacker or defender).

*Rapid deployment*

*(Not to be confused with the "Rapid Deployment" multiplayer rules — see
Rapid Deployment (Multiplayer), p. 31–32.)*

You can save time by playing with the pre-made squads shown for each mission
in the Starter Zone section of the *Mission Guide*.

Each player then sets up their tactical area, consisting of:

- 5 Operator profiles representing their chosen Operators. Place an
  Activation token under each profile, Operator-available side up;

[DIAGRAM]

Activation tokens – 'Operator available' side

- a personal supply, with a Reroll token, Entryway Overwatch tokens and
  Leaning standees;
- a Tactical Inventory board: each player secretly places Charge cubes in
  whichever free slots they choose. The **defender places 4 cubes** in this
  way, and the **attacker places 6**. The **attacker** also places 3 Charge
  cubes in the slots for drones. Players then simultaneously reveal their
  choices. The defender now has access to four tactical gadgets for the
  whole game, compared with nine for the attacker.

[DIAGRAM]

Example: Tactical inventories after setup

Players collect any standees, miniatures, or tokens associated with the
gadget described on each Operator profile. For now, store these components
on the Operator profile.

[DIAGRAM]

Some Operator profiles have slots for Charge cubes: place a Charge cube in
each slot.

Charge cube slot for IQ's gadget.

[DIAGRAM]

Some profiles have a slot for an activatable Gadget: place the appropriate
Activatable Gadget token in the slot, 'Ready' side up.

Slot for Montagne's Activatable Gadget token.

NOTE Feel free to use the named Base Rings to help you recognize the
Operators on the game board until you are familiar with their appearance.

**See also:** [Setup Sequence](#setup-sequence), [Use Tactical Gadget Action](#use-tactical-gadget), [Rapid Deployment (Multiplayer)](#rapid-deployment-multiplayer)

## Game Speed Setting {#game-speed-setting}
*p. 12–13*

*Managing game time and the app*

For an even more immersive gaming experience, we recommend playing
*6: Siege – The Board Game* with the companion app. If you are unable to use
the app, or prefer not to, refer to the 'No App' variant (see p. 29).

Open the app. Set the number of players and enter their names. Each player
then selects one of the four available speed settings (1 – Beginner, 2 –
Chill, 3 – Standard, or 4 – Extreme).

[DIAGRAM]

The speed setting affects the deployment time and game time allocated to
each Operator. For a balanced game, players should choose the same setting.
However, a veteran player can play with a handicap by picking a more
demanding speed setting than their less experienced opponent.

NOTE **For your first few games,** we recommend playing with no time limit,
or choosing speed setting 1 (Beginner) in the app.

**See also:** ['No App' Variant](#no-app-variant), [Setup Sequence](#setup-sequence)

## Deployment {#deployment}
*p. 13–14*

[DIAGRAM]

*Rapid deployment*

*(Not to be confused with the "Rapid Deployment" multiplayer rules — see
Rapid Deployment (Multiplayer), p. 31–32.)*

You will find ready-to-play deployments for each mission in the Starter
Zone section of the *Mission Guide*. To use one of these pre-made
deployments, tap the SKIP DEPLOYMENT button in the app and copy the
deployment as shown. No time limit applies.

Tap the DEPLOYMENT button.

During their deployment:

- Players must comply with the applicable area capacity and gadget
  positioning rules (see Gadget Deployment, p. 25);
- Operators may be placed in a leaning position (see Leaning, p. 17).

*Defender's deployment*

When playing as the defender, deploy your Operators and gadgets in the
order shown below. Operators and gadgets cannot be placed in perimeter
spaces.

1. The defender may reposition or remove from the game board up to 5 of the
   following components set up during the Mission Selection step:
   - cameras;
   - barbed wire;
   - fortified entryways;
   - barricades.

   NOTE If you move a barricade, you must redeploy it to the same type of
   location (for example, a two-section Barricaded Door standee can only be
   placed on a two-section Barricaded Door location).

2. Then place all your special gadgets that have the **Setup** keyword.
3. If you have chosen Bulletproof Camera and/or Deployable Shields in your
   tactical inventory, remove the corresponding cubes from your inventory,
   collect the same number of Bulletproof Camera miniatures and/or
   Deployable Shield standees from the box, and place them on the game
   board.
4. Then place your 10 Hidden Operator tokens on free spaces on the board,
   or in orange spaces on the upper floor. For each space in the defender's
   upper floor area that contains a Hidden Operator, also place the
   Entryway Overwatch token bearing that Operator's name on an entryway
   space. When the defender's deployment time has run out, or if the
   defender taps the CONTINUE TO ATTACKER'S DEPLOYMENT button in the app,
   it is the attacker's turn to deploy their assets within the set time
   limit.

*Attacker's deployment*

When the defender has finished their deployment, the attacker places their
5 Operators and their Overwatch marker in perimeter spaces.

The **attacker** cannot deploy Operators to their upper floor area.

NOTE Never resolve reactions or reveal hidden Operators during the
deployment phase. You must wait until the attacker's first activation
phase.

*Deployment timeout*

If the time allotted to a squad runs out before they have completed their
deployment, collect any game components not yet set up and put them back in
the box.

[DIAGRAM]

**See also:** [Squad Selection](#squad-selection), [Room](#room), [Leaning](#leaning), [Gameplay Sequence](#gameplay-sequence), [Rapid Deployment (Multiplayer)](#rapid-deployment-multiplayer)

## Gameplay Sequence {#gameplay-sequence}
*p. 14–15*

Games last up to 6 rounds, each organized in 5 phases:

1 – Attacker's first activation phase
2 – Defender's first activation phase
3 – Attacker's second activation phase
4 – Defender's second activation phase
5 – Upkeep phase

Each player must complete their two activation phases within a limited
time, defined by the number of their Operators still in play at the start
of the round. Players allocate this time between their activation phases as
they see fit.

The player carrying out their activation phase is known as the 'active
player', and their opponent is the 'passive player'.

When activating an Operator, the active player flips that Operator's
Activation token to show its 'Operator activated' side.

[DIAGRAM]

Activation token 'Operator available' side / Activation token 'Operator
activated' side

*1 – Attacker's first activation phase*

[DIAGRAM]

The attacker moves the Round Tracker marker forward one space, and the
defender starts the attacker's timer by tapping the TAP TO START ROUND 1
button.

The attacker fully activates between **1 and 3** of their Operators still
in play, in any order.

Then the attacker taps CONTINUE TO DEFENDER'S OPERATORS to start the
defender's timer.

NOTE If a player with a squad of 3 or more Operators activates all their
Operators during their first activation phase, they will skip their second
activation phase.

NOTE If a player with a squad of 5 Operators chooses to activate only 1
Operator during their first activation phase, they will be able to activate
only 3 of their 4 available Operators in their second activation phase.

*2 – Defender's first activation phase*

[DIAGRAM]

The defender fully activates between **1 and 3** of their Operators still in
play, in any order.

Then the defender taps CONTINUE TO ATTACKER'S OPERATORS to start the
attacker's timer.

*3 – Attacker's second activation phase*

The attacker fully activates **between 0 and 3** of their Operators in
play, in any order, provided they were not activated during their first
activation phase.

Then the attacker taps CONTINUE TO DEFENDER'S OPERATORS to start the
defender's timer.

*4 – Defender's second activation phase*

The defender fully activates **between 0 and 3** of their Operators in play,
in any order, provided they were not activated during their first
activation phase.

Then the defender taps UPKEEP to end the activation phases.

*Activation timeout*

When a player's activation time expires during one of their activation
phases:

- if one of their Operators was in the process of performing an action,
  complete the action, unless it was a movement action, in which case,
  leave the Operator in the last space entered before the timer expired;
- that player cannot activate any more Operators;
- they may still react, but can no longer take time to think first.

NOTE If the attacker's time expired during their first activation phase,
the defender plays both of their activation phases, one after the other.

*5 – Upkeep phase*

Check the mission's victory conditions (see *Mission Guide*). A player wins
the game if they have achieved any of the victory conditions: tap the END
GAME button.

Otherwise, remove any Located markers, Stunned markers, and/or overlays
from the game board, returning them to the general supply.

Players flip their Operators' Activation tokens to show their 'Operator
available' side, and reset all Activatable Gadget tokens to their 'Ready'
side.

For each Operator eliminated during the current round, tap one of the
outlines in the relevant squad in the app. The app then automatically
adjusts the activation time available to each player for the coming round.

Then begin a new round by tapping NEXT ROUND, or OVERTIME where applicable.

[DIAGRAM]

Repeat the process for each subsequent round until a victory condition is
met.

[DIAGRAM]

**See also:** [Activating an Operator](#activating-an-operator), [Game Speed Setting](#game-speed-setting), [Aim of the Game](#aim-of-the-game)

## Activating an Operator {#activating-an-operator}
*p. 15–16*

After flipping the Activation token to show its 'Operator activated' side,
the Operator may perform up to **three actions**, in any order: 1 Move
action, and 2 other actions.

Operators are not allowed to perform the same action twice.

The available actions vary according to whether the Operator is revealed or
hidden.

*Actions available to a revealed Operator (miniature)*

Revealed Operators can perform the following actions:

- Move;
- Run;
- Shoot;
- Overwatch;
- Use Tactical Gadget;
- Use a Special Gadget **ACTION** effect;
- Destroy.

These actions are described in the Operator Actions section.

*Actions available to a hidden Operator (tokens)*

While hidden, Operators may only perform the following actions: Move, Run,
and lastly, Overwatch (which is performed automatically).

If you want a hidden Operator to perform any other actions, you must first
reveal the Operator during their activation phase. Once revealed, the
Operator may spend any remaining actions as a revealed Operator.

**Example:** Smoke, who is hidden, performs a Move action. He then wants to
Shoot an opposing Operator. To do so, he must reveal himself and spend an
action to Shoot. He may then perform a final action, which can be anything
except Move or Shoot, which he has already performed.

[DIAGRAM]

**See also:** [Operator Actions](#operator-actions), [Operator Status](#operator-status), [Gameplay Sequence](#gameplay-sequence)

## Operator Actions {#operator-actions}
*p. 16*

| Action | Revealed Operators | Hidden Operators | From the main floor | From an upper floor area |
|---|---|---|---|---|
| Move *(movement)* | ✅ | ✅ | Spend up to 5 movement points. | Spend 1 movement point to access the main floor via a ◈, then spend any remaining movement points. |
| Run *(movement)* | ✅ | ✅ | Spend up to 5 movement points, depending on the Operator's profile. | — |
| Overwatch | ✅ | ✅ | Reorient the Operator. Overwatch spaces in the Operator's line of sight, in the direction indicated by their Overwatch marker. | Place an Entryway Overwatch token on a neutral ◈. OR Dispute an ◈ overwatched by the opponent. |
| Shoot | ✅ | ❌ | Shoot at an Operator situated in line of sight. Locate 🎯 the targeted Operator. | — |
| Use Tactical Gadget | ✅ | ❌ | Apply the effect of a gadget in the tactical inventory. | Perform one of these three actions in a neutral ◈. |
| Destroy | ✅ | ❌ | Remove destructible elements from the game board, if they are in a line of sight and you have the required destruction rating. | (see left) |
| Use a Special Gadget **ACTION** effect | ✅ | ❌ | Apply a Special Gadget **ACTION** effect. | Apply a Special Gadget **ACTION** effect in a neutral ◈. OR Apply a Special Gadget **ACTION** effect of a **Vertical** gadget in a 🔲 room. |

[DIAGRAM]

*(This table is the rulebook's own summary, printed just before the detailed
rules for each action begin — see the individual action sections below for
the full rules.)*

**See also:** [Move](#move), [Run](#run), [Shoot Action](#shoot), [Overwatch Action](#overwatch), [Use Tactical Gadget Action](#use-tactical-gadget), [Destroy Action](#destroy), [Use a Special Gadget ACTION Effect](#use-special-gadget-action)

## Move {#move}
*p. 16–17*

An Operator performing this action has 5 movement points, which can be spent
on moving and leaning.

*Moving an Operator*

An Operator may enter orthogonally or diagonally adjacent spaces (see
Adjacent spaces, p. 7), at a cost of 1 movement point per space.

[DIAGRAM]

Example: Moving into an adjacent space — To reach space **B**, Sledge must
spend 2 movement points. This movement is not possible, as spaces **A** and
**B** are not adjacent.

The following restrictions apply to this movement:

- Operators cannot enter a space occupied by an opposing Operator.
- An Operator can move through a space occupied by a squad-mate, but can
  never spend their movement there;
- An Operator can move through a breach or window. Doing so costs 1 extra
  movement point ⚠️.

*Passing an obstacle*

Operators must spend 1 extra movement point ⚠️ to climb onto an obstacle as
they enter one of its spaces. Entering another space occupied by the same
obstacle, or moving off the obstacle, costs only 1 movement point.

Operators can never pause or end their movement in a space containing an
obstacle.

[DIAGRAM]

Example: Moving and passing an obstacle — To reach space **A**, Sledge must
spend 6 movement points (requiring him to use the Run action, see p. 18),
whichever route he takes. Whenever Sledge passes an obstacle or moves
through a window, he must spend an additional 1 movement point (shown by
the ⚠️ icon).

*Movement by hidden Operators*

The defender allocates the movement points for an Operator's Move (or Run)
action freely between the two Hidden Operator tokens.

*Pausing a Move action*

Players may pause a Move action after entering a free space, perform one or
two available actions, and then resume their movement, spending their
remaining movement points in the normal way. The active player still counts
each movement step separately and announcing the number of remaining
movement points.

An Operator can pause a Move action multiple times during the same
activation.

**See also:** [Leaning](#leaning) (Move and floor-changing rules continue there — see "Moving between floors"), [Partitions](#partitions), [Run](#run)

## Leaning {#leaning}
*p. 17–18*

Operators (whether revealed or hidden) on the main floor can lean to gain a
line of sight while remaining protected.

For 1 movement point, an Operator can lean into a **free orthogonally
adjacent space**.

Move the Operator's miniature into the space into which they are leaning,
and place their Leaning standee in the space from which they are leaning.

Operators cannot lean through breaches or windows, or over obstacles.

[DIAGRAM]

Example: Leaning — Mute before leaning / Mute in the leaning position.

- ✅ Spaces into which Mute can lean
- ❌ Spaces into which Mute cannot lean
- Obstacle / Breach

A leaning Operator occupies 2 spaces on the game board: the one containing
their miniature, and the one containing their Leaning standee.

An Operator leaning between two rooms is considered to be present in both.

An Operator can be targeted by targeting either their miniature or their
Leaning standee.

*Important note*

- Leaning standees never block line of sight.
- Operators cannot move while leaning.
- A leaning Operator uses the space containing its miniature when
  performing actions that require line of sight.
- Leaning has the same effects on gameplay as entering a space. For
  example, if an Operator leans into a space overwatched by an opposing
  Operator, the opposing Operator can Riposte.

*Straightening up*

Straightening up (i.e., exiting the leaning position), also costs 1
movement point. Operators may straighten up in two ways:

- either move the miniature into the space containing the Leaning standee,
  and return the standee to the owner's supply;
- or leave the miniature in its current space and return the Leaning
  standee to the owner's supply. The Operator is considered to have entered
  the space that now contains their miniature.

NOTE Leaning and straightening up have the same effects as entering a
space, potentially triggering a Riposte from an overwatching opposing
Operator (see Riposte, p. 22).

*Moving between floors*

Operators must use an entryway space to move between floors.

*Moving from the main floor to an upper floor area*

An Operator on the main floor that enters an entryway space during a
movement action can spend 1 movement point to move into one of the two
spaces in their designated upper floor area.

If neither space in their upper floor area is free, the Operator must remain
on the main floor.

Once in their upper floor area, the Operator cannot spend any remaining
movement points or perform another movement action.

*Moving from an upper floor area to the main floor*

An Operator in their upper floor area may spend 1 movement point to move to
an entryway space on the main floor.

Operators that leave their upper floor area cannot return to it during the
same activation.

**See also:** [Move](#move), [Protection](#protection), [Riposte](#riposte), [Upper Floor Areas](#upper-floor-areas), [Partitions](#partitions)

## Run {#run}
*p. 18*

`RUN 2` — The Run action lets an Operator make an extra movement during
their activation phase. It grants either 2 or 5 movement points, depending
on the value shown on the Operator profile, which can be spent for a
conventional Move action.

NOTE: Operators with a Run value stated as '–' cannot perform this action.

**See also:** [Move](#move), [Operator Profile](#operator-profile)

## Shoot Action {#shoot}
*p. 18–19*

An Operator can perform a Shoot action, targeting an opposing Operator
situated in line of sight. The Operator performing a Shoot action is known
as 'the shooter'.

*Shooting through game elements*

As line of sight to Located Operators is not broken by light walls,
barricades, and overlays, they can be targeted by shots fired through these
elements.

1. Tap ⏸ to pause the timer. Then announce which opposing Operator they are
   aiming at ('the target'). State whether or not the target has protection
   (light or heavy, see Protection, p. 19).

   *Pausing the timer to perform an action:* Pause the timer whenever a
   game effect requires a dice roll.

   The player controlling the targeted Operator:
   - either states that they approve the line of sight and protection
     conditions declared by the shooter, in which case play proceeds
     directly to the next step;
   - or indicates that they do not approve the conditions declared by the
     shooter, challenging the shot (see Challenges, p. 24).

2. Calculate the distance from shooter to target: count each space between
   the shooter and the target, including the target's space but not the
   shooter's space. Pick the shortest path and ignore ⚠️ when calculating
   the distance.

   [DIAGRAM]

   Example: Range calculation — Blitz is shooting at Smoke, at a range of 4
   spaces. (Blitz's line of sight; Range calculation)

   After calculating the distance in spaces, refer to the Operator profile
   to determine the equivalent range category.

   The range affects the number and color of Hit dice rolled for a Shoot
   action. If the target has protection, do not roll any dice with a
   lightning symbol ⚡.

   Treat shots fired from an upper floor area into an entryway space as
   **short range**.

3. Roll all the allowed Hit dice and add up the Hit 💥 symbols to determine
   the total number of hits inflicted on the target.

   If the targeted Operator is protected (see Protection, p. 19), modify the
   hit total as follows:
   - Subtract 2 hits if the target has light protection;
   - Or subtract 3 hits if the target has heavy protection.

4. The final result indicates the hits inflicted on the targeted Operator,
   who sustains 1 wound 💀 per hit. Place the corresponding number of Wound
   tokens on their profile.

   An Operator is eliminated immediately if the total number of Wound
   tokens on their profile equals or exceeds their Stamina stat (see
   Operator status, p. 10).

   If the targeted Operator remains in play, place a Located 🎯 marker on
   their miniature's base, even if they sustained no hits.

5. Tap ▶ to restart the timer.

**See also:** [Protection](#protection), [Challenges](#challenges), [Operator Profile](#operator-profile), [Line of Sight](#line-of-sight), [Operator Status](#operator-status), [Overwatch Action](#overwatch)

## Protection {#protection}
*p. 19–20*

A targeted Operator may gain light protection (– 2 hits) or heavy
protection (– 3 hits) if the **shooter's line of sight** passes through any
of the following elements (see table opposite):

| Element through which the line of sight passes | Additional condition | Protection |
|---|---|---|
| Obstacle | The target must be situated **in a space adjacent** to the obstacle. | Light protection: – 2 hits |
| Holed wall | — | Light protection: – 2 hits |
| Barricade | — | Light protection: – 2 hits |
| Light wall | — | Light protection: – 2 hits |

Operators with **2 or more sources of light or heavy protection** are
considered to have heavy protection. This means that a maximum of 3 hits
may be subtracted from an opponent's shot.

Protection **only** applies to hits inflicted by shots.

*Protection for leaning Operators*

A leaning Operator is represented by two game components. When a shot
targets either of these two components, a second line (in addition to the
line of sight) must be drawn to determine the targeted Operator's
protection rating.

This second line runs from the shooter to the targeted Operator's non-
targeted component, and is not blocked by any game elements. This line is
known as the **line of cover**. Each different element through which the
line of sight and the line of cover pass protects the targeted Operator.

As the line of cover is never blocked, additional elements grant protection
if the targeted Operator is leaning. Use the following information to
determine the protection provided by elements along the line of cover, as
well as the elements listed in the previous table:

| Element through which the line of cover passes | Protection |
|---|---|
| Heavy wall | Heavy protection: – 3 hits |
| Fortified wall | Heavy protection: – 3 hits |
| Squad-mate carrying a shield 🛡️ | Light protection: – 2 hits |

[DIAGRAM]

Example: Leaning Operator — Smoke is shooting at Ash, who is in the leaning
position. She gains heavy protection as the line of cover between Smoke and
Ash's Leaning standee passes through a heavy wall.

[DIAGRAM]

Ash is shooting at Smoke, who is Located and leaning. Smoke gains heavy
protection from a combination of 2 sources:
- the line of sight passes through a light wall;
- the line of cover also passes through an obstacle adjacent to him.

[DIAGRAM]

Protection example: Obstacle — Ash is shooting at Smoke. Smoke has light
protection, as he is adjacent to an obstacle and Ash's line of sight to him
passes through that obstacle.

*Operators carrying a shield* 🛡️

Operators with the 🛡️ icon on their profile have permanent light protection
against shots.

**See also:** [Shoot Action](#shoot), [Leaning](#leaning), [Partitions](#partitions), [Challenges](#challenges), [Operator Profile](#operator-profile)

## Free Action {#free-action}
*p. 20*

Some actions cause players to perform other actions, which are treated as
free actions. Reactions are also free actions.

Free actions never count towards the total of 3 available actions when
activating an Operator.

A free action never triggers a Riposte, unless the initial action that led
to it does.

[DIAGRAM]

HEARTBEAT SENSOR — **ACTION** → Wave OR Vertical — The targeted Operator
receives a 🎯 marker.

**ACTION** → Vertical — Perform a Shoot action (short range, light
protection) targeting the Located Operator.

**Example:** During his activation phase, Pulse spends only one of his 3
actions to perform the Use a Special Gadget **ACTION** effect action with
his heartbeat sensor. Once completed, this action may prompt a reaction by
an opposing Operator, but the ensuing Shoot action is free and never
triggers a reaction.

For his second action, Pulse can therefore perform any other action,
including Shoot, except Use a Special Gadget **ACTION** effect, which he has
just used.

**See also:** [Operator Reactions](#operator-reactions), [Riposte](#riposte), [Activating an Operator](#activating-an-operator)

## Overwatch Action {#overwatch}
*p. 20–22*

An Operator can use the Overwatch action to:

- **From the main floor:** overwatch an area comprising multiple spaces in
  the Operator's line of sight, extending in the direction shown by their
  Overwatch marker;
- **From an upper floor area:** overwatch one entryway space.

The Operator is said to be 'overwatching', and the area or entryway space
thus covered is 'overwatched'.

During the opposing squad's activation phases, the overwatching Operator can
Riposte in spaces in an overwatched area (see Riposte, p. 22).

*Overwatched status marker*

The overwatched status is indicated by an Overwatch marker placed in front
of an overwatching Operator situated on the main floor, or by an Entryway
Overwatch token in the case of an Operator on the upper floor.

[DIAGRAM]

Thermite with his Overwatch marker / Mute's Hidden Operator token with
Integrated Overwatch marker.

When an Operator performs the Overwatch action from the main floor, point
their miniature in the overwatched direction, then place an Overwatch
marker in front of it, in one of the four sections of the space containing
the miniature.

[DIAGRAM]

Example: Overwatch marker orientation — ✅ Correct positioning / ❌ Incorrect
positioning.

When an Operator performs the Overwatch action while in a leaning position,
place the Overwatch marker in front of their miniature. The marker cannot be
placed between the Operator miniature and their Leaning standee.

*Ending overwatch*

An overwatching Operator that performs an action during their activation
loses their overwatch status: remove their Overwatch marker (unless the
Operator is hidden) or their Entryway Overwatch token from the board and
return it to their personal supply.

NOTE Overwatch markers and Entryway Overwatch tokens are not removed from
the game board during the upkeep phase.

*Overwatching from the main floor*

Revealed and hidden Operators do not perform Overwatch actions from the
main floor in exactly the same way.

- **Revealed overwatching Operator:** The Operator covers a 180° arc
  extending forward from the space section covered by their Overwatch
  marker. The Operator overwatches all spaces inside the arc that are in
  their **line of sight**.
- **Hidden overwatching Operator:** Hidden Operators automatically conclude
  their activation with an Overwatch action: reorient their Hidden Operator
  tokens to show the overwatched direction. The Operator covers a 180° arc
  extending forward from the space section covered by their Overwatch
  marker (which is incorporated into the Hidden Operator token).

[DIAGRAM]

Example: Overwatched area — ✅ Spaces overwatched by Smoke. ❌ Spaces not
overwatched by Smoke.

While overwatching, Smoke monitors all spaces in line of sight that are
located forward of the imaginary line extending the space section covered
by his Overwatch marker (→).

*Overwatching from an upper floor area*

Revealed and hidden Operators do not perform Overwatch actions from the
upper floor in exactly the same way.

*Revealed overwatching Operator*

From an upper floor area, an Operator can only overwatch one entryway
space. Choose the entryway space that you want your Operator to overwatch,
then:

- if the entryway space does not already contain an Entryway Overwatch
  token, place your Operator's Entryway Overwatch token in it. Your
  Operator is now overwatching the space;
- if the entryway space already contains an Entryway Overwatch token
  belonging to your squad, you may replace it with your Operator's Entryway
  Overwatch token. Return the removed token to your supply;
- if the entryway space already contains an opposing Entryway Overwatch
  token, your Operator disputes the entryway space. The player owning the
  existing token may agree to remove it from the game board, allowing your
  Operator to take over in the normal way, with no other effects.
  Otherwise, an exchange of fire is triggered between the two Operators
  (see below).

If a disputed Entryway Overwatch token belongs to a hidden Operator, that
Operator must reveal themselves. If the Entryway Overwatch token was a
decoy, remove their Entryway Overwatch token and replace it with the
disputing Operator's token.

*Hidden overwatching Operator*

A hidden Operator that ends their activation with at least one of their
Hidden Operator tokens in their upper floor area automatically performs the
Overwatch action on an entryway space, or attempts to do so by disputing an
entryway space overwatched by an opposing Operator. Hidden Operators must
reveal themselves before disputing an entryway space.

NOTE If a Hidden Operator token moves to an upper floor area that already
contains the Operator's second Hidden Operator token, you may redeploy the
Operator's Entryway Overwatch token at the end of their activation.

*Exchange of fire*

During an exchange of fire, the active player pauses the timer ⏸.

Their Operator may perform a free Shoot action (short range, heavy
protection) targeting the Operator that owns the disputed Entryway
Overwatch token.

After this shot:

- If the passive player's Operator is still in play:
  - leave their Entryway Overwatch token in place;
  - they may also perform a free Shoot action (short range, heavy
    protection) targeting the Operator disputing the space occupied by
    their Entryway Overwatch token.
- If the passive player's Operator is eliminated:
  - put their Entryway Overwatch token back in the box;
  - replace it with the active Operator's Entryway Overwatch token.

On completing the exchange of fire, the active player taps ▶ to restart the
timer.

*Shot*

The term 'shot' may refer to a Shoot action, a Riposte or an exchange of
fire. Whenever a player's Operator fires a shot, perform all the steps for a
Shoot action (see Shoot action, p. 18), allowing for the range and
protection requirements applicable to exchanges of fire.

**See also:** [Riposte](#riposte), [Shoot Action](#shoot), [Upper Floor Areas](#upper-floor-areas), [Operator Status](#operator-status), [Partitions](#partitions)

## Riposte {#riposte}
*p. 22*

An Overwatch action may lead to a Riposte, which can only be triggered
during the opposing player's activation phase.

A Riposte is a free Shoot action. Do not remove the Overwatch token or
marker after a Riposte.

Hidden Operators must reveal themselves when launching a Riposte.

*Riposte from the main floor*

An Operator overwatching from the main floor may Riposte **whenever** an
opposing Operator:

- enters a space that they are overwatching;
- is present in a space that they are overwatching **after** completing an
  action.

NOTE It is possible to Riposte when an opposing Operator moves into a space
on the main floor that contains an obstacle.

*Riposte from an upper floor area*

An Operator overwatching from their upper floor area may Riposte (short
range) **whenever** an opposing Operator:

- enters an entryway space that they are overwatching;
- is present in an entryway space that they are overwatching after
  completing an action.

NOTE There is no limit to the number of times an Operator can Riposte
during an opponent's activation phase.

[DIAGRAM]

Example: Riposte

1. Ash leans into a space that is overwatched by Smoke.
2. Smoke Ripostes. After resolving the shot, Ash is still in play.
3. For her second action, Ash shoots at Smoke.

Smoke survives, and can therefore Riposte against Ash a second time.

**See also:** [Overwatch Action](#overwatch), [Free Action](#free-action), [Operator Reactions](#operator-reactions), [Leaning](#leaning)

## Use Tactical Gadget Action {#use-tactical-gadget}
*p. 22*

Each Charge cube in a tactical inventory represents the potential to
perform a Use Tactical Gadget action.

To perform a Use Tactical Gadget action, you must spend a Charge cube from
the desired gadget: remove the Charge cube from your inventory and put it
back in the box. Target the space where you want to use the gadget. Apply
the gadget's effect from the targeted space.

Tactical gadget Charge cubes can be spent by any of the Operators in a
squad.

The effects of some tactical gadgets involve performing a Destroy action.
Treat this as a free action.

**See also:** [Squad Selection](#squad-selection), [Tactical Gadgets for Defenders](#defender-gadgets), [Tactical Gadgets for Attackers](#attacker-gadgets), [Destroy Action](#destroy)

## Use a Special Gadget ACTION Effect {#use-special-gadget-action}
*p. 22–23*

Special gadgets can only be used by the Operator that owns them.

An Operator performing the Use a Special Gadget **ACTION** effect action may
apply one of their special gadget's effects preceded by the **ACTION** icon
(the same icon is used for both attackers and defenders).

If the **ACTION** icon is preceded by a struck-out Charge cube slot 🧊❌, you
must spend a Charge cube from the relevant Operator profile in order to
apply the effect. Put the spent Charge cube back in the box.

*Permanent effect of special gadgets*

Special gadget effects not preceded by **ACTION** or **REACTION** (see
Operator reactions, p. 24) are permanent. They are applied with no need to
spend an action, and remain active at all times.

Some effects require you to perform one or more actions. These are free
actions.

**See also:** [Operator Profile](#operator-profile), [Operator Reactions](#operator-reactions), [Free Action](#free-action)

## Destroy Action {#destroy}
*p. 23–24*

`DESTROY ⚠️` — An Operator performing the Destroy action applies the
destruction rating shown on their Operator profile to all destructible
elements (i.e., with a strength rating) in the targeted space.

Some gadget effects also require the Operator to perform a free Destroy
action when they are applied, in which case, the gadget's destruction
rating will be stated in the effect.

*Targeting Destroy actions performed by Operators*

When performing a Destroy action, the Operator must target the central dot
in a space in line of sight.

*Determining the affected elements*

The following elements can be affected by a Destroy action in a space:

- the gadget (if any) in the targeted space;
- all partitions in the targeted space.

NOTE If you perform a Destroy action in a space containing an Operator, the
action does not affect any gadgets present on that Operator's profile (in
the form of miniatures or Charge cubes).

*Location of partitions*

A one-section partition belongs to 2 orthogonally adjacent spaces.

A two-section partition is treated as a single component. It belongs to 4
orthogonally adjacent spaces.

[DIAGRAM]

✅ Spaces that affect the partition if targeted

*Required destruction rating: ⚠️1 🟧2 ⬟3*

Operator profiles show a destruction rating ⚠️/🟧/⬟, applicable when the
Operator uses the Destroy action.

Compare the destruction rating against the targeted element's strength
rating. There are three possible strength ratings: ⚠️1, 🟧2, and ⬟3.

The ⚠️1 destruction rating destroys gadgets and partitions with the ⚠️1
strength rating.

The 🟧2 destruction rating destroys gadgets and partitions with the ⚠️1 or
🟧2 strength rating.

The ⬟3 destruction rating (gadget effect only) destroys gadgets and
partitions with the ⚠️1, 🟧2, or ⬟3 strength rating.

Elements with no strength rating, such as obstacles and heavy walls, are
indestructible.

*Bulletproof (gadgets only)*

The Bulletproof 🔩 attribute does not apply to Destroy actions performed by
an Operator in exactly the same way as free Destroy actions triggered by a
gadget effect.

- **Destroy action performed by an Operator:** This action will destroy a
  Bulletproof 🔩 gadget only if the Operator performing it is adjacent and
  has the necessary destruction rating.
- **Destroy action triggered by a gadget effect:** Consider only the
  targeted gadget's strength rating, ignoring any Bulletproof 🔩 attribute.

*Consequences of destruction*

If the destroyed game element is:

- **a gadget**, put it back in the box;
- **a single or double barricade**, put it back in the box, revealing the
  two space sections that it previously occupied. The space section(s)
  thus revealed represent a (single or double) door or window;
- **a single or double wall**, place a breach where the destroyed wall was
  located. The breach size should match the number of sections in the
  destroyed wall.

[DIAGRAM]

Example: Performing a Destroy action — From his current space, Sledge:

1. can destroy the camera (on the left), as he has a line of sight to the
   central dot in the space into which the camera is pointing;
2. can destroy the light wall (on the right), as he has a line of sight to
   the space containing the targeted partition, and has the necessary
   destruction rating 🟧2 (shown on his profile);
3. cannot destroy either of the signal disruptors, as he has no line of
   sight to the relevant spaces.

**See also:** [Partitions](#partitions), [Icons Used for Gadgets](#gadget-icons), [Line of Sight](#line-of-sight), [Use Tactical Gadget Action](#use-tactical-gadget)

## Operator Reactions {#operator-reactions}
*p. 24*

There are two types of reaction to an action by an opposing Operator:

- **Riposte**, which is a shot fired by an overwatching Operator (see
  Overwatch action, p. 20);
- **Gadget effect with a REACTION icon.** If the **REACTION** icon is
  preceded by a struck-out Charge cube slot 🧊❌, you must spend a Charge
  cube from the relevant Operator profile in order to apply the effect. Put
  the spent Charge cube back in the box. An Operator reacting to an action
  (or to another reaction) may only use their special gadget effect once.

When in a position to react, you are responsible for announcing exactly
when you want to perform a reaction. If you want to take a moment to
consider whether or not to react, you must first tap the timer so that your
own time is counting down.

*Switching the timer when a reaction is triggered*

Before triggering a reaction, the passive player taps CONTINUE TO
ATTACKER/DEFENDER'S OPERATORS. This stops the active player's timer and
starts their own timer. The passive player may at this point take some time
to decide whether or not to react, but their own timer will be ticking
down! After making their decision, the passive player taps CONTINUE TO
ATTACKER/DEFENDER'S OPERATORS in the app to restart the active player's
timer. Normal play then resumes.

If two or more of your Operators are able to react, resolve each reaction
in full (applying all effects), one after the other in any order.

A reaction is a free action (see Free action, p. 20).

**See also:** [Riposte](#riposte), [Free Action](#free-action), [Use a Special Gadget ACTION Effect](#use-special-gadget-action)

## Challenges {#challenges}
*p. 24–25*

*What actions can be challenged?*

**Shots**

Shots by Operators can always be challenged. Players then check the
conditions announced by the active player.

**Other game effects**

All game effects (other than shots) that require line of sight may also be
challenged.

*Challenge sequence*

**Challenging a shot**

1. Use a LoS Ruler to check whether the line of sight is valid (see
   Checking lines of sight, p. 25).

   - ✅ **If the line of sight is confirmed to be valid:** complete the
     shot. Then check the target's actual protection rating, if necessary,
     drawing a line of cover to the leaning target:
     - ✅ if this matches the value announced by the shooter, the stated
       protection rating is confirmed and must be applied when resolving
       the shot;
     - ❌ if it does not match the value announced by the shooter, ignore
       the stated protection rating and apply the actual protection rating
       when resolving the shot.
   - ❌ **If the line of sight is found to be invalid:** the shot has no
     effect. If it was the result of a Shoot action, the action is still
     spent.

2. Apply the consequences of the challenge.

   - ✅ **If both of the conditions announced by the challenged player are
     confirmed,** that player may:
     - either immediately add 30 seconds to their own timer;
     - or deduct 30 seconds from the opponent's timer.
   - ❌ **If either or both of the conditions declared by the challenged
     player are invalidated,** their opponent chooses between adding 30
     seconds to their own timer or deducting 30 seconds from the challenged
     player's timer.

   Tap the '– 30 seconds' or '+ 30 seconds' button in the app.

3. Apply the effects of the shot, where applicable. Then tap the ▶ button.

**Example:** Monica, playing as the attacker, announces to her opponent
(Ron) that her Operator Blitz is going to shoot at Mute, who has heavy
protection. She pauses her timer. Ron thinks the line of sight to Mute is
invalid. He decides to challenge the action, in order to verify the
conditions announced by Monica.

Ron uses a LoS Ruler to check the line of sight from the Operator to their
target. The check confirms his suspicion: the line of sight between Blitz
and Mute is blocked by a heavy wall. As the line of sight was invalid, the
challenge is resolved in Ron's favor, and he opts to immediately deduct 30
seconds from Monica's timer. Even though it failed, Blitz's Shoot action is
still spent. With the challenge over, Monica taps ▶ and resumes her
activation.

**Challenging other game effects**

The challenging player pauses the timer ⏸.

Resolve game effect challenges using the same procedure as for shots,
skipping the protection rating check and related consequences.

If an action is challenged and the line of sight found to be invalid, the
action (and Charge cube, where applicable) is still spent. If the line of
sight for a **REACTION** is found to be invalid, the Charge cube is still
spent.

**See also:** [Checking Lines of Sight](#checking-lines-of-sight), [Shoot Action](#shoot), [Protection](#protection), [Line of Sight](#line-of-sight)

## Checking Lines of Sight {#checking-lines-of-sight}
*p. 25*

**LoS Ruler positioning:** The line along the middle of the LoS Ruler must
completely cover the relevant two central dots.

NOTE Sometimes, this process requires you to move game elements. Where
possible, temporarily place them in spaces adjacent to their original
spaces.

Line of sight is considered to pass through a game element if any part of
the element (however small) protrudes beyond the centerline on the LoS
Ruler.

[DIAGRAM]

Validity of a line of sight — Valid line of sight / Invalid line of sight

**See also:** [Challenges](#challenges), [Line of Sight](#line-of-sight)

## General Remarks on Gadgets {#gadgets-general}
*p. 25–26*

*Gadget deployment*

Players deploy various types of gadgets, while setting up the game or
during Operator activation phases.

Where the effect of a gadget is to place a miniature or token on the board,
the targeted space must be free. When deploying gadgets, a capacity limit of
one gadget per space applies.

*Ground-deployed gadgets*

Ground-deployed gadgets are represented by a token, which can be placed in
any space on the main floor.

*Wall-mounted gadgets*

[DIAGRAM]

Wall-mounted gadgets are represented by a miniature, which can be placed on
any section of heavy wall on the main floor. However, unlike barricades,
which belong to two spaces, a wall-mounted gadget belongs to a single
space, determined by the gadget's orientation.

When you deploy a wall-mounted gadget, you must therefore orient the gadget
with its front facing the targeted space.

Note: It is not possible to deploy 2 wall-mounted gadgets on the same heavy
wall section.

*Using a wall-mounted gadget*

[DIAGRAM]

Camera facing into the space on the right / Camera facing into the space on
the left

*Other gadgets*

Gadgets not represented by a physical component placed on the game board do
not count towards a space's capacity limit.

**Example:** A grenade can be thrown onto a Barbed Wire token.

*Hits*

If a gadget uses Hit dice, tap ⏸ to pause the timer while you roll the dice
and apply their effects.

Note: Protection applies only to hits inflicted by shots. Hits inflicted by
Hit dice rolled for a frag grenade are never mitigated by protection.

*Activatable gadgets*

[DIAGRAM]

Slot for Montagne's Activatable Gadget token.

Some special gadgets are activatable, and require an Activatable Gadget
token. The corresponding token slot is shown on the owner's Operator
profile. Cover it with an Activatable Gadget token ('Ready' side up) during
setup.

Use of activatable gadgets is not restricted, but the owning Operator must
activate a gadget in order to use it. These gadgets have a **ACTION** effect
containing the icon, which lets you flip the Activatable Gadget token to
reveal its 'Activated' side.

While the gadget is activated, its effect applies. During the upkeep phase,
reset all Activatable Gadget tokens to their 'Ready' side.

*Multi-space areas of effect*

Some gadgets affect an area consisting of multiple spaces extending from a
targeted space. These spaces are collectively referred to as an 'area of
effect' which is described in the gadget effect.

Gadget effects are applied to an area of effect as follows:

- Apply the effect simultaneously to all spaces in the area of effect;
- Unless otherwise stated, the effect applies to Operators in both squads;
- Roll the dice separately for each Operator required to roll Hit dice.
  (Roll the Hit dice only once for a leaning Operator, even if both spaces
  that they occupy are inside the area of effect);
- If the area of effect is a room, apply the effect to all spaces in the
  room (including any spaces not in line of sight of the Operator using
  the gadget);
- Some gadgets have the **Overlay** keyword. Their area of effect is the
  area occupied by the overlay (see Overlays, below).

**See also:** [Icons Used for Gadgets](#gadget-icons), [Gadget Effect Keywords](#gadget-keywords), [Operator Profile](#operator-profile), [Leaning](#leaning)

## Icons Used for Gadgets {#gadget-icons}
*p. 26–28 (this topic's own heading appears twice in the rulebook; both verbatim occurrences are gathered here, each keeping its own page tag)*

*p. 26–27*

| Category | Icon | Meaning |
|---|---|---|
| Attribute | 🔩 | **Bulletproof** — The only way to remove this gadget from the game board is to perform a Destroy action with the appropriate destruction rating from an adjacent space, or to use a gadget with the necessary destruction rating. |
| Attribute | 🔌 | **Electronics** — Some gadget effects only affect this type of gadget. |
| Attribute | 👁️ | **Always Visible** — Lines of sight targeting this gadget are not blocked by Operators or by Smoke or Gas overlays. |
| Strength | ⚠️1 | Gadgets or partitions with this strength rating can be destroyed by gadgets and Operators with the ⚠️1, 🟧2, or ⬟3 destruction rating. |
| Strength | 🟧2 | Gadgets or partitions with this strength rating can be destroyed by gadgets and Operators with the 🟧2 or ⬟3 destruction rating. |
| Strength | ⬟3 | Gadgets or partitions with this strength rating can be destroyed by gadgets with the ⬟3 destruction rating. |
| Destruction | ⚠️1 | This gadget or Operator destroys partitions and gadgets with the ⚠️1 strength rating. |
| Destruction | 🟧2 | This gadget or Operator destroys partitions and gadgets with the ⚠️1 or 🟧2 strength rating. |
| Destruction | ⬟3 | This gadget destroys partitions and gadgets with the ⚠️1, 🟧2, or ⬟3 strength rating. |

*p. 28*

Some gadget names are followed by icons representing an attribute possessed
by the gadget.

The strength ratings ⚠️1 and 🟧2, and the Bulletproof 🔩 attribute, apply
only to the Destroy action performed by an Operator (see Destroy action,
p. 23) — not to ⬟3 (that destruction rating only appears on gadget
effects, never on an Operator profile), and not to free Destroy actions
triggered by a gadget effect, which ignore the Bulletproof 🔩 attribute
entirely (see "Bulletproof (gadgets only)" under Destroy action, p. 23–24).

**Electronics** 🔌: Some gadget effects apply only to this type of gadget.

**Always Visible** 👁️: Lines of sight targeting this gadget are not blocked
by Operators or by Smoke or Gas overlays.

**See also:** [Destroy Action](#destroy), [General Remarks on Gadgets](#gadgets-general), [Gadget Effect Keywords](#gadget-keywords)

## Gadget Effect Keywords {#gadget-keywords}
*p. 27–28*

Some gadgets use one or more keywords to succinctly describe their
conditions of use.

*Setup*

Deploy this gadget during the setup sequence.

Gadgets placed on the game board must comply with space and wall section
area capacity.

*Overlays (Fire / Smoke / Gas)*

[DIAGRAM]

Fire overlay — Area of effect of an overlay

This gadget has an associated overlay. The overlay shows the gadget's area
of effect, which covers either 2 or 4 spaces, depending on the overlay.

[DIAGRAM]

Spaces in the overlay — Overlays area of effect

*Overlay placement*

You must place the widest possible overlay. One of the spaces occupied by
the overlay must be the space targeted by the gadget. Overlays must not
pass through partitions, breaches, windows, or obstacles.

Multiple overlays cannot have overlapping areas of effect.

If the 2-space overlay cannot be validly placed, the gadget cannot target
the desired space.

[DIAGRAM]

Example: Overlay placement — Overlay 1 is not validly positioned, as it
overlaps a wall. Overlay 2 is not valid either, as it passes through an
obstacle and its area of effect overlaps that of overlay 3. Overlays 3 and
4 are correctly positioned.

Remember to remove overlays from the game board and return them to the
general supply during the upkeep phase.

*Line of sight*

This gadget must target a space in line of sight.

Remember that an Operator in an upper floor area has line of sight to all
gray entryway spaces.

*Throwable*

This gadget must be thrown: target a space in line of sight, within a
maximum range of 6 spaces. Operators and Smoke or Gas overlays do not block
this line of sight.

*Using a Throwable gadget from an upper floor area*

An Operator in a space in their upper floor area may toss a Throwable
gadget into a neutral entryway space on the main floor, as they have a line
of sight to it.

*Deployable*

An Operator may deploy a Deployable gadget in an adjacent space.

*Using a Deployable gadget from an upper floor area*

An Operator in a space in their upper floor area may deploy a Deployable
gadget in a neutral entryway space on the main floor, as if it were
adjacent.

*Wave*

This gadget must target a space within a maximum range of 4 spaces (as if
the Operator were performing a Shoot action), ignoring any partitions,
Operators, and Smoke or Gas overlays.

*Using a Wave gadget from an upper floor area*

Gadgets used from an upper floor area affect only the targeted neutral
entryway space.

*Vertical*

This gadget must be used from an upper floor area. It can target any
space in a 🔲 room.

*Drone*

This gadget is Deployable. Once deployed, it can move, spending up to 5
movement points. Drones cannot pass obstacles, enter spaces containing a
Barbed Wire token, or move to upper floor areas. They can, however, enter
spaces occupied by Operators.

On ending its movement, the drone scans the room around it. All opposing
Operators in the room receive a 🎯 marker.

NOTE A hidden Operator that receives a 🎯 marker is automatically revealed.

[DIAGRAM]

Drone marker — Players may use the Drone marker in the general supply to
show the drone's movement, returning the marker to the supply on completing
the scan.

NOTE The Drone marker serves merely as a pointer and does not count towards
area capacity. Drones can therefore enter spaces that already contain a
gadget.

**See also:** [General Remarks on Gadgets](#gadgets-general), [Room](#room), [Line of Sight](#line-of-sight), [Upper Floor Areas](#upper-floor-areas), [Tactical Gadgets for Attackers](#attacker-gadgets)

## Tactical Gadgets for Defenders {#defender-gadgets}
*p. 28*

**Fortified Entryway** 🔴

*Setup*

A Fortified Entryway is a ground-deployed gadget, which must always be
placed in an entryway space. When an entryway space is fortified, it is no
longer treated as an entryway space until the Fortified Entryway token is
removed from the game board by a gadget with the ⬟3 destruction rating
(used from the main floor or an upper floor area).

**Barbed Wire** 🔩⚠️1

*Setup*

Barbed Wire is a ground-deployed gadget. **Attackers** entering a space
containing a Barbed Wire token must immediately end their activation. A
Drone gadget cannot be deployed in or enter a space containing a Barbed
Wire token.

**Deployable Shield** 🔩🟧2

*Setup*

Deployable Shields are ground-deployed gadgets that are treated as
obstacles, but can be destroyed. They have the Bulletproof 🔩 attribute and
a 🟧2 strength rating.

**Camera** 🔌👁️⚠️1

*Setup*

A Camera is a wall-mounted gadget. It covers the whole room in which its
miniature is placed. An opposing Operator that enters a space in a room
containing a Camera, or ends an action in one, receives a Located 🎯 marker
(even if they are not in the camera's line of sight).

**Bulletproof Camera** 🔌👁️🔩⚠️1

*Setup*

A Bulletproof Camera is deployed and behaves exactly like a standard
Camera, except that it also has the Bulletproof 🔩 attribute.

**Nitro Cell**

*Throwable*

A Nitro Cell inflicts hits in an area of effect. Specifically, it inflicts
the hits rolled on 🔴🔴 to an Operator located in the targeted space, and the
hits rolled on 🟠 to any Operators in spaces adjacent to the targeted space.

**Impact Grenade**

*Throwable*

Perform a Destroy 🟧2 action in the targeted space.

**See also:** [Gadget Effect Keywords](#gadget-keywords), [Icons Used for Gadgets](#gadget-icons), [Destroy Action](#destroy), [Partitions](#partitions)

## Tactical Gadgets for Attackers {#attacker-gadgets}
*p. 28–29*

**Breach Charge** 🔴

*Deployable*

Perform a Destroy 🔴 action in the targeted space. Like any other gadget
with the ⬟3 destruction rating, a Breach Charge can target a space
containing a Fortified Entryway token, from an upper floor area or from the
main floor.

**Tactical Drone** 🔌

*Drone – Deployable*

Tactical Drones are governed by the rules defined for the Drone keyword
(see Drone, p. 27).

**Frag Grenade**

*Throwable*

Perform a Destroy ⚠️1 action in the targeted space. Any Operator in that
space takes the hits rolled on 🟡🟡.

Perform a Destroy ⚠️1 action in spaces adjacent to the targeted space.
Operators in such spaces take the hits rolled on 🟡.

**Flashbang Grenade**

*Throwable*

Operators in the targeted space or spaces adjacent to it immediately
receive a Stunned marker.

**Smoke Grenade**

*Throwable – Smoke overlay*

Spaces occupied by the Smoke overlay block lines of sight, except for lines
of sight to Always Visible 👁️ gadgets or Located Operators.

NOTE An Operator in a space containing a Smoke overlay will have all of
their lines of sight blocked, unless their target has been Located.

**Claymore** ⚠️1

*Deployable*

A Claymore is a ground-deployed gadget. When deploying a Claymore, orient
the token with the arrow pointing to an orthogonally adjacent space. A
hidden Operator cannot move into a space targeting a Claymore.

A Claymore is tripped:

- if an opposing Operator enters the space containing its token or the
  space targeted by its arrow;
- if it is destroyed.

When a Claymore is tripped, Operators in the space containing the Claymore
token or spaces adjacent to it immediately take the hits rolled on 🔴🔴.
Then put the Claymore token back in the box.

**See also:** [Gadget Effect Keywords](#gadget-keywords), [Destroy Action](#destroy), [Tactical Gadgets for Defenders](#defender-gadgets), [Operator Status](#operator-status)

## Other Important Rules {#other-important-rules}
*p. 29*

This section contains some rules not directly linked to the sequence of
play, but which are crucial for ensuring that every game of 6: Siege — The
Board Game.

**See also:** [Fairplay and Pauses](#fairplay-and-pauses), [Effects and Rules](#effects-and-rules), [Limited Components](#limited-components), ['Back in the Box'](#back-in-the-box), [Reroll](#reroll)

## Fairplay and Pauses {#fairplay-and-pauses}
*p. 29*

At any time during deployment and play, players may request a pause to
resolve any rule interpretation issues. Simply tap the Pause ⏸ button.
When the issue has been resolved, tap Play ▶ to restart the timer.

**See also:** [Challenges](#challenges), [Game Speed Setting](#game-speed-setting)

## Effects and Rules {#effects-and-rules}
*p. 29*

Some effects, particularly those described on Operator profiles, conflict
with or modify the normal rules of 6: Siege — The Board Game. Such effects
prevail over the normal rules.

**See also:** [Operator Profile](#operator-profile)

## Limited Components {#limited-components}
*p. 29*

If you are supposed to place a game component but no more are available,
no substitutes are allowed. The desired action is no longer available.

**See also:** ['Back in the Box'](#back-in-the-box)

## 'Back in the Box' {#back-in-the-box}
*p. 29*

When game components are put back in the box, they can no longer be used
until the end of the game.

**See also:** [Limited Components](#limited-components), [Destroy Action](#destroy)

## Reroll {#reroll}
*p. 29*

Each player has a single-use Reroll token. When shooting, you may declare
your intention to use your Reroll token after rolling the dice. On
spending this token, you keep any one die and must reroll all the others.
Add together the results shown on the rerolled dice and the retained die
(if any), and apply this new result. Put the spent Reroll token back in the
box.

**See also:** [Shoot Action](#shoot), [Rapid Deployment (Multiplayer)](#rapid-deployment-multiplayer)

## 'No App' Variant {#no-app-variant}
*p. 29–30*

*(The rulebook prints this topic under two consecutive headings — the
timing-table intro and the full variant rules. Both are gathered here as one
section, each part keeping its own page tag.)*

*p. 29*

If you are unable to use the app, or prefer not to, you can use two
conventional stopwatches or a chess clock (or replicate a smartphone app),
replicating the specified settings.

| Speed setting | Defender/attacker deployment time | Time per Operator |
|---|---|---|
| Beginner | 20 minutes / 10 minutes | 120 seconds |
| Chill | 15 minutes / 5 minutes | 90 seconds |
| Standard | 15 minutes / 5 minutes | 60 seconds |
| Extreme | 8 minutes / 3 minutes | 45 seconds |

Alternatively, you can play the 'No App' variant.

*p. 29–30*

This variant changes some of the game's core rules. During the setup
phase, place the 10 Bonus tokens in the general supply. Deployment and
activation are not subject to time limits.

When you win a challenge (see Challenges, p. 24), instead of gaining or
losing time you receive a Bonus token, which you should place:

- '+1 action' side up, on the profile of one of your Operators that is
  either in the process of being activated or has not yet been activated;
- or '–1 action' side up, on any opposing Operator that is either in the
  process of being activated or has not yet been activated.

No more than two Bonus tokens may be placed on a particular Operator
profile. If the same Operator profile has a '+1 action' and a '–1 action'
token, they cancel each other out. Return both tokens to the supply.

An Operator beginning their activation with 1 or 2 '+1 action' tokens may
perform one or two bonus actions. Every action selected by the Operator,
including bonus actions, must be different. On completing the Operator's
activation phase, remove the '+1 action' tokens from their profile and
return them to the general supply.

An Operator beginning their activation with one '–1 action' token on their
profile has one fewer action than normal. On completing the Operator's
activation phase, remove the '–1 action' token from their profile and
return it to the general supply. When an unactivated Operator receives a
second '–1 action' token, immediately flip their Activation token to show
its 'Operator activated' side; it will not be possible to activate that
Operator during the current round.

When an Operator receives a token during their activation phase,
immediately apply its effect: +1 or –1 action. If they receive a second
'–1 action' token, end their activation immediately (after resolving the
current action and any challenge, where applicable). On completing the
Operator's activation phase, remove the '–1 action' token from their
profile and return it to the general supply.

If you win a challenge but no Bonus tokens remain in the general supply,
take any Bonus token already placed on an Operator profile and place it,
either side up, on an Operator profile of their choice.

During the upkeep phase, return all Bonus tokens to the general supply.

[DIAGRAM]

**See also:** [Game Speed Setting](#game-speed-setting), [Challenges](#challenges), [Activating an Operator](#activating-an-operator)

## Special Ops Modules {#special-ops-modules}
*p. 30*

Three Special Operations rules modules make 6: Siege — The Board Game even
more tactical. We recommend waiting until you have mastered the basics
before introducing them. These modules can be used individually or in
combinations.

**See also:** [Forward Planning Module](#forward-planning-module), [Advanced Tactics Module](#advanced-tactics-module), [Competitive Gaming Module](#competitive-gaming-module)

## Forward Planning Module {#forward-planning-module}
*p. 30*

The Forward Planning module gives the defender far greater control over
the environment during the Setup phase.

During the Mission Selection step, carry out the setup process without
placing any Bomb miniatures or Hostage tokens.

Then start the timer and continue with the defender's deployment, making
the following changes:

- the defender places the Bomb miniatures or Hostage tokens in any
  permitted spaces (as defined in the Mission Guide);
- the defender may reposition or remove from the game board up to 10
  (rather than the usual 5) components set up during the Mission Selection
  step;
- the defender may place 1 Fortified Wall token on any section of light
  wall;

  [DIAGRAM]

  Fortified Wall tokens

  NOTE When a fortified wall (represented by a token) is destroyed, replace
  it with a breach of the same size.

- the defender may place up to 3 Breach standees on any sections of light
  or fortified wall.

**See also:** [Deployment](#deployment), [Partitions](#partitions)

## Advanced Tactics Module {#advanced-tactics-module}
*p. 30–31*

*New Hide action*

[DIAGRAM]

The defender's revealed Operators can perform a new action: Hide.

When a revealed Operator spends one of their actions to Hide, put their
miniature back on their Operator profile, replacing it with the two Hidden
Operator tokens, stacked together face-down.

Operators with a 🎯 marker cannot perform the Hide action.

If an Operator has a 🎯 marker, add the corresponding marker to the stack
of Hidden Operator tokens.

When placing these two tokens, orient them in the same direction as the
miniature that they are replacing.

Operators with stacked tokens cannot lean or change their orientation.
Operators cannot perform the Hide action while leaning.

NOTE The stacked Hidden Operator tokens may henceforth be moved separately
during movement actions. If they separate after receiving a 🎯 marker,
assign a marker to each Hidden Operator token.

When a hidden Operator is revealed, return their Hidden Operator tokens to
their profile, rather than putting them back in the box.

*Overwatch action variant*

In this module, Overwatch is a free action, performed automatically. This
gives attackers more margin for maneuver, while also making things easier
for the defenders (who might use the actions thus saved to Hide, for
example).

Play the game without Overwatch markers. During setup, leave the Overwatch
markers in the box, but keep the Entryway Overwatch tokens. Immediately
before ending an Operator's activation, the controlling player reorients
the Operator's miniature or Hidden Operator tokens to indicate the
overwatched direction.

[DIAGRAM]

The 180° overwatch arc is defined by the visible markings on miniature
bases and Hidden Operator tokens.

Operators that end their activation in an upper floor area overwatch an
entryway space, or attempt to do so by disputing an entryway space overwatch
by the opponent. This means that entryway spaces are always disputed at the
end of an Operator's activation.

**See also:** [Operator Status](#operator-status), [Overwatch Action](#overwatch), [Leaning](#leaning)

## Competitive Gaming Module {#competitive-gaming-module}
*p. 31*

The Competitive Gaming module introduces some alternative settings for
your games.

*Best-Of-Three match*

This module lets you play a match consisting of two or three games played
with the same mission and environment.

The first to score two victories wins the match.

Assign the attacker and defender roles randomly before starting the first
game. Swap roles for the second game.

If you have to play a third, tie-breaker game, determine the roles
randomly, as before.

*Operator selection*

During the Squad Selection phase preceding each game, you can refine your
strategy and attempt to weaken your opponent's hand by banning certain
Operator picks.

Put the banned Operator profiles back in the box for the current game.

This draft phase is a four-step process:

1. The attacker picks 1 Operator, then bans 1 opposing Operator. The
   defender then does likewise.
2. The attacker picks 2 Operators.
3. The defender picks 2 Operators, then bans 1 opposing Operator. The
   attacker then does the same.
4. The defender picks 2 Operators.

**See also:** [Squad Selection](#squad-selection), [Aim of the Game](#aim-of-the-game)

## Multiplayer Mode {#multiplayer-mode}
*p. 31*

You can also play 6: Siege — The Board Game with three or four players.
Some rules are tweaked in this mode: the game functions with pairs of
players and introduces an Operator with no special gadget, the Recruit.

As well as providing logistical support, the Recruit becomes a better
shooter as the game progresses. The Recruit starts the game with a fairly
harmless profile but, if protected, can become a major asset to their
squad.

**See also:** [4 Players: 2 v 2](#four-players-2v2), [Rapid Deployment (Multiplayer)](#rapid-deployment-multiplayer), [3 Players: 2 v 1](#three-players-2v1)

## 4 Players: 2 v 2 {#four-players-2v2}
*p. 31*

*Setup*

When the squads have been picked, each player chooses 2 Operators to
control during the game. This pair is known as a 'section'.

Beginning with the attackers, each squad's players choose 1 of the 2
available Recruit profiles. Place the selected profile in the squad's
tactical area, with reach of both players.

Place 6 Charge cubes in the designated locations on each Recruit profile.

The players in a squad agree which tactical gadgets to choose, and how to
deploy the Recruit.

NOTE When playing in teams, additional time is allocated to each Operator,
to allow for better coordination between the two sections.

| Speed setting | Defender/attacker deployment time | Time per Operator |
|---|---|---|
| Beginner | 20 minutes / 10 minutes | 150 seconds |
| Chill | 20 minutes / 10 minutes | 120 seconds |
| Standard | 15 minutes / 5 minutes | 90 seconds |
| Extreme | 15 minutes / 5 minutes | 60 seconds |

**See also:** [Squad Selection](#squad-selection), [Rapid Deployment (Multiplayer)](#rapid-deployment-multiplayer), [3 Players: 2 v 1](#three-players-2v1)

## Rapid Deployment (Multiplayer) {#rapid-deployment-multiplayer}
*p. 31–32*

The Starter Zone section of the Mission Guide includes suggestions for
pre-made sections.

*Gameplay sequence*

Each player is responsible for their own section and special gadgets.

The gameplay sequence is different in multiplayer mode.

**Phase 1: First activation by the attackers.**

The attackers agree which section to activate first. The player
controlling that section activates both their Operators. They may also
choose to activate the attacking squad's Recruit.

**Phase 2: First activation by the defenders.**

The defenders agree which section to activate first. The player
controlling that section activates both their Operators. They may also
choose to activate the defending squad's Recruit.

**Phase 3: Second activation by the attackers.**

Activate the attackers' second section. The active player may activate the
attackers' Recruit, if it has not already been activated.

**Phase 4: Second activation by the defenders.**

Activate the defenders' second section. The active player may activate the
defenders' Recruit, if it has not already been activated.

**Phase 5: Upkeep phase**

A new option is available during the upkeep phase, before beginning a new
round. Tapping the 'Level Up Recruits' button grants 1 minute to upgrade
your Recruits.

[DIAGRAM]

*Leveling up the Recruit*

Upgrade your Recruit's effectiveness in any one range category: each squad
removes a cube from the desired range category on their Recruit's profile
and puts it back in the box. Remove the first available cube (from left to
right) in the chosen range category. This reveals a new die, to be rolled
in future Shoot actions by the Recruit.

If the Charge cube slot shows a 🔌 icon, leveling up the Recruit also
grants an extra Charge cube in the tactical inventory. In such cases,
instead of putting the removed cube back in the box, place it in a free
slot in the squad's tactical inventory.

[DIAGRAM]

Leveling up the Recruit — TACTICAL INVENTORY

**Important note:** If a Recruit ends their activation in an upper floor
area, ignore the effect of the 🔌 icon.

When the one-minute timer expires, the squads simultaneously reveal their
choice. Put any unassigned Charge cubes back in the box.

*Notes on multiplayer rules*

**Reaction**

Reactions by Operators or Recruits may be declared by either player in a
squad.

**Challenging line of sight**

Any player may challenge a line of sight drawn by the opposing squad.

**Communication**

During deployment, the players in a squad may communicate freely including
leaving the table for a private discussion, but they are not allowed to
pause the deployment timer.

During the game, each squad may communicate freely, but only during its own
activation phases.

Defenders may look at their squad-mate's Hidden Operator tokens.

**Important note:** When you are the first player to activate your
Operators during a round, the timer will be running for both you and your
squad-mate.

**Reroll token**

The Reroll token is shared by the two squad-mates in each squad. It can
still only be used once.

**Eliminated sections**

If a section and the squad's Recruit are eliminated, the player controlling
the eliminated section will not be able to activate any Operators. That
player can still help by analyzing the situation and advising their
squad-mate.

**See also:** [4 Players: 2 v 2](#four-players-2v2), [Challenges](#challenges), [Reroll](#reroll), [Operator Reactions](#operator-reactions)

## 3 Players: 2 v 1 {#three-players-2v1}
*p. 32–33*

Two attackers face off against one defender.

The attackers play using the rules for the 2 v 2 game mode. The defender
also adopts the 2 v 2 rules, but their squad is not split into sections.
The defender may activate their 4 Operators and their Recruit in any order
(as with the core rules).

**See also:** [4 Players: 2 v 2](#four-players-2v2), [Rapid Deployment (Multiplayer)](#rapid-deployment-multiplayer)

## Alternative Profiles {#alternative-profiles}
*p. 33*

You cannot play an Operator character and their alternate version
simultaneously: doing so might raise gameplay balance issues, but more
importantly, would tear a hole in the space-time continuum! Last but not
least, the game only contains one copy of each Operator-specific
component.

**See also:** [Squad Selection](#squad-selection), [Operator Profile](#operator-profile)

## Hints and Tips {#hints-and-tips}
*p. 33–34*

*Squad composition tips*

Although every Operator is unique, they can be described in terms of
generic skills. The 'Operator List' lets you quickly assemble a squad,
prioritizing the skills most useful for the upcoming mission.

For example, for a Hostage mission, the attackers might want to pick
Operators with the 'Runner' skill, whereas defenders may prefer a squad
containing Operators with the 'Time-waster' skill. Squad can be versatile
or highly specialized, as you prefer. However, it is always a good idea to
include at least one Operator with the 'Breacher' skill in your squad,
allowing you to move through the environment more easily.

*Tactical recommendations*

6: Siege — The Board Game is a game where every action counts. Your
Operators are accomplished professionals who know how to plan and execute
an assault! As each side has its own tactical advantages, here are a few
tips to help you prepare for your first few games.

First and foremost, regardless of whether you are playing attack or
defense, never forget that every action counts. A single shot can have
devastating consequences: mindlessly charging into battle is rarely a
viable option.

Next, one of the game's core concepts is its destructible environment.
Keep in mind that the environment can change, and that some shots
penetrate certain types of partition. Exploit this to weaken your opponent
without overexposing your Operators, or to open up escape routes.

Lastly, manage your time wisely! Try to think about your tactical options
and possible openings while your opponent is playing. This approach lets
you make best use of your time and commit fewer tactical errors.

**Defender**

As the defender, trust in your defenses: your goal is to delay the
attacker's advance. Don't be afraid to lie in wait, using your Hidden
Operator tokens to instill doubt, rather than seeking a confrontation.

If you open up a flaw in your defenses, you can be sure the attacker will
exploit it.

Respond to any openings produced by the attacker creating new entryways.
Adjust your approach to avoid unpleasant surprises. When defending a room,
it is usually a better idea to control the approaches than to hole up in
a last stand. Defending a wider perimeter gives you more options!

Once you have gained a solid understanding of the defender's role, you
will be able to adopt a more aggressive defensive posture and cut the
ground from under your opponent's feet.

**Attacker**

You always have the initiative, but that's no reason to charge in guns
blazing! Be patient. Games often last 5 or even 6 rounds. Prepare your
assault methodically, and create fallback opportunities by demolishing
destructible terrain features and taking out enemy gadgets.

Don't expose yourself without good reason. Even though your Operators are
more deadly at medium and long range, the defender will often wait for
you to approach. An overwatching defender can sometimes eliminate you
before you even finish your action.

Coordinated action by multiple Operators is the key to taking your
opponent by surprise. You also have a Tactical Inventory that can simplify
an assault, if used wisely. You have a tactical toolkit of gadgets to use
and abuse, including drones and breach charges to blast through fortified
entryways.

**See also:** [Squad Selection](#squad-selection), [Partitions](#partitions), [Overwatch Action](#overwatch)

