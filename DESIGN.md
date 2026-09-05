---
name: DirectiveCraft
description: The controlled document a software studio issues when a claim must be checkable.
colors:
  ink: "#14304C"
  ink-sunk: "#10283F"
  rule: "#2E5175"
  rule-soft: "#23415F"
  chalk: "#EEF2F6"
  chalk-dim: "#A6C1D8"
  cyan: "#6FA6C8"
  signal: "#F26E4C"
typography:
  display:
    fontFamily: "Archivo, system-ui, 'Segoe UI', Roboto, sans-serif"
    fontSize: "clamp(2.15rem, 5.6vw, 3.5rem)"
    fontWeight: 700
    lineHeight: 1.07
    letterSpacing: "-0.021em"
  headline:
    fontFamily: "Archivo, system-ui, 'Segoe UI', Roboto, sans-serif"
    fontSize: "clamp(1.45rem, 3.4vw, 1.9rem)"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.015em"
  title:
    fontFamily: "Archivo, system-ui, 'Segoe UI', Roboto, sans-serif"
    fontSize: "clamp(1.02rem, 2vw, 1.2rem)"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "0.04em"
  body:
    fontFamily: "'Public Sans', system-ui, -apple-system, 'Segoe UI', sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.62
    letterSpacing: "normal"
  label:
    fontFamily: "'JetBrains Mono', ui-monospace, 'SFMono-Regular', Menlo, monospace"
    fontSize: "0.7rem"
    fontWeight: 500
    lineHeight: 1.7
    letterSpacing: "0.1em"
  data:
    fontFamily: "'JetBrains Mono', ui-monospace, 'SFMono-Regular', Menlo, monospace"
    fontSize: "clamp(1.2rem, 3.2vw, 1.6rem)"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "0.01em"
    fontVariation: "tabular-nums"
rounded:
  none: "0"
  hair: "1px"
spacing:
  pad: "clamp(20px, 5vw, 40px)"
  section: "clamp(34px, 4.5vw, 48px)"
  statement: "clamp(40px, 6vw, 64px)"
  col: "44rem"
  wide: "48rem"
components:
  action-primary:
    textColor: "{colors.signal}"
    typography: "{typography.label}"
    padding: "0 0 3px 0"
  readout-band:
    backgroundColor: "{colors.ink-sunk}"
    textColor: "{colors.chalk}"
    padding: "18px 22px 16px"
  readout-value:
    textColor: "{colors.chalk}"
    typography: "{typography.data}"
  clause-status:
    textColor: "{colors.signal}"
    typography: "{typography.label}"
  release-stamp:
    textColor: "{colors.signal}"
    typography: "{typography.display}"
    padding: "8px 28px 10px"
    rounded: "{rounded.none}"
---

# Design System: DirectiveCraft

## Overview

**Creative North Star: "The Controlled Document"**

The homepage is the artifact a studio issues when a claim must be checkable: a diazo
blueprint crossed with a QA release sheet, not a landing page. One saturated diazo-blue
ink owns the entire surface edge to edge. Structure is drawn, not decorated: a single
fixed 1px drafting-sheet frame inset from the viewport, a centred 48rem sheet whose
left and right edges are carried as hairlines through header, main, and footer, and
groups divided by whitespace and single hairline rules. Nothing is boxed, nothing is
carded, nothing floats.

Type does the ranking. A heavy Archivo display voice states the studio's one sentence
left-aligned; Public Sans carries the prose at a generous reading measure; JetBrains
Mono, tabular, carries every number, label, ordinal, and revision line so that data
always reads as instrument output. The lone warm accent — a diazo-print orange — is
rationed to things that are live or actionable: the FreqCraft link, inline links, the
clause PASS status, and the release-gate stamp. On a full screen it touches well under
a tenth of the surface.

This world explicitly refuses the centered dark hero with three principle cards and one
glowing CTA. It refuses gradients, glass, glow, drop shadows, rounded corners, and any
decorative imagery. Depth is tonal only: the recessed readout band is a half-step
darker than the ground.

**Key Characteristics:**
- One diazo-blue ground, edge to edge; no second surface colour, only a darker sunk band.
- Drawn structure: fixed sheet frame, hairline rules, carried sheet edges — never boxes.
- Mono for every number, label, and ordinal; data reads as instrument output.
- Accent rationed to live/actionable elements only.
- One authored motion moment (the PASS stamp); everything else static and JS-optional.

## Colors

A single saturated diazo-blue owns the page; everything else is a tint, a hairline, or the one rationed warm accent.

### Primary
- **Diazo Print Orange** (`{colors.signal}` #F26E4C): The only warm colour. Applied to live or actionable elements exclusively — the "Open FreqCraft" action, inline prose links, the clause `PASS` status labels, the release-gate stamp and its inner keyline, `::selection` background, and the `:focus-visible` outline. Never used for headings, structure, decoration, the logo mark, or ordinals.

### Neutral
- **Diazo Blue Ground** (`{colors.ink}` #14304C): The page background, full bleed. The world's base ink.
- **Sunk Blue** (`{colors.ink-sunk}` #10283F): A half-step darker recessed band — the readout instrument strip and the scrollbar track. The only tonal depth cue in the system.
- **Rule Blue** (`{colors.rule}` #2E5175): Primary hairlines — sheet left edge, readout top/bottom borders, titleblock/footer separators, scrollbar thumb.
- **Soft Rule Blue** (`{colors.rule-soft}` #23415F): Fainter hairlines — sheet right edge, the fixed drafting-sheet frame, intra-group dividers, clause and cell separators.
- **Chalk** (`{colors.chalk}` #EEF2F6): Primary text — headings, body emphasis, readout values, wordmark.
- **Dim Chalk** (`{colors.chalk-dim}` #A6C1D8): Secondary text, blue-tinted rather than gray — standfirst, intros, clause detail, body paragraphs, meta lines, "In development" heading.
- **Diazo Cyan** (`{colors.cyan}` #6FA6C8): Tertiary — mono field labels, clause ordinals (§1), entry ordinals (001), the footer revision line, the 2px masthead/footer rule, and the logo mark strokes.

### Named Rules
**The Live-Only Accent Rule.** `#F26E4C` marks things that are live, passing, or clickable — nothing else. If an element is not a link, a pass status, or the release stamp, it is chalk, dim chalk, or cyan. On any given screen the accent covers under 10% of the surface; the rarity is the signal.

**The Blue-Tinted Neutral Rule.** There is no gray in this system. Every "neutral" is a blue. Secondary text is `#A6C1D8`, not a desaturated gray.

## Typography

**Display Font:** Archivo (variable 400–800; fallback system-ui, 'Segoe UI', Roboto, sans-serif)
**Body Font:** Public Sans (variable 400–700; fallback system-ui, -apple-system, 'Segoe UI', sans-serif)
**Label/Mono Font:** JetBrains Mono (400/500; fallback ui-monospace, 'SFMono-Regular', Menlo, monospace)

**Character:** Archivo is a tight, grotesque display face used heavy and confident; Public Sans is a neutral government-grade text face; JetBrains Mono is the instrument readout. The pairing reads as an engineering document that respects the reader's time.

### Hierarchy
- **Display / H1** (Archivo 700, `clamp(2.15rem, 5.6vw, 3.5rem)`, line-height 1.07, letter-spacing -0.021em): The studio's one sentence. Left-aligned, `max-width: 19ch`, `text-wrap: balance`. Mobile floor `clamp(2rem, 8.5vw, 2.6rem)`. Also the wordmark at 1.06rem.
- **Headline / entry H3** (Archivo 700, `clamp(1.45rem, 3.4vw, 1.9rem)`, letter-spacing -0.015em): Register entry names (FreqCraft). Muted variant is 600 in dim chalk for not-yet-shipped entries.
- **Title / H2** (Archivo 700, `clamp(1.02rem, 2vw, 1.2rem)`, letter-spacing 0.04em, UPPERCASE): Section headers.
- **Clause name** (Archivo 600, 0.98rem, letter-spacing 0.03em, UPPERCASE): The § register clause names.
- **Stamp** (Archivo 800, `clamp(2.6rem, 8vw, 4rem)`, letter-spacing 0.06em): The single release-gate PASS stamp. The only use of weight 800.
- **Body** (Public Sans 400, 16px, line-height 1.62): Prose. Emphasis is weight 500 in chalk. Reading measures: standfirst 54ch, intro 58ch, clause detail / readout note 62ch, entry paragraphs 58ch.
- **Standfirst** (Public Sans 400, 1.06rem, line-height 1.66, dim chalk): The one paragraph under H1.
- **Data value** (JetBrains Mono 500, `clamp(1.2rem, 3.2vw, 1.6rem)`, `tabular-nums`): Readout cell numbers; secondary fraction in `small` at 0.72em dim chalk.
- **Label** (JetBrains Mono 500, 0.7rem, letter-spacing 0.08–0.12em, UPPERCASE, cyan): Field keys (Doc/Sheet/Rev), readout cell labels.
- **Meta / mono line** (JetBrains Mono 400, 0.72–0.8rem): Titleblock values, entry meta, clause status, ordinals, footer links, footer revision line.

### Named Rules
**The Mono-For-Number Rule.** Every numeral a visitor might check — test counts, versions, device counts, dates, ordinals, revision lines — is set in JetBrains Mono with `tabular-nums`. Numbers never appear in the display or body face.

**The Left-Aligned Statement Rule.** The H1 is left-aligned and capped at 19ch. It is never centred and never full-measure.

## Layout

The page is a single centred sheet: `--wide: 48rem`, `margin: 0 auto`, with `border-left: 1px var(--rule)` and `border-right: 1px var(--rule-soft)` carried independently by `header`, `main`, and `footer` so the sheet edge runs unbroken the full length of the page. Prose blocks are further constrained to `--col: 44rem` via a `.col` wrapper; horizontal padding is `--pad: clamp(20px, 5vw, 40px)` applied by an inner `.sheet` wrapper (never on the sheet border element itself).

A fixed 1px drafting-sheet frame (`body::before`, `inset: 9px`, `border: 1px solid var(--rule-soft)`) sits above content at `z-index: 5`; it tightens to `inset: 5px` at ≤720px.

Vertical rhythm is section-driven, not an 8px grid: `section.block` padding `clamp(34px, 4.5vw, 48px)`, the statement block `clamp(40px, 6vw, 64px)` top, contact `clamp(44px, 7vw, 64px)`. Consecutive blocks are separated by a single `1px var(--rule-soft)` top border. The masthead and footer are separated from the body by a `2px var(--cyan)` rule.

Groups are divided by whitespace plus hairline rules only. No group is boxed, filled, or shadowed. The one filled region is the readout band (`var(--ink-sunk)`, full sheet width, hairline top and bottom).

**Responsive (single breakpoint, 720px):**
- Titleblock: 4-column grid (`1fr auto auto auto` with left-border dividers) collapses to a single column; fields switch from stacked to inline key/value rows.
- Readout: 4-column grid becomes 2×2, with borders reassigned so interior hairlines stay coherent.
- Clause register: ordinal column narrows `3.2rem → 1.9rem`, column-gap `20px → 12px`; detail reflows under the name.
- Entries, gate, contact, footer: already single-column; unchanged.
- Verified at 375/390/414px with zero horizontal overflow.

## Elevation & Depth

No shadows. The system is flat by rule. The single `text-shadow` on the stamp is a 1px same-hue optical thickener, not a cast shadow, and there are no `box-shadow` declarations anywhere.

Depth is tonal and singular: the readout band is painted `var(--ink-sunk)` (#10283F), one half-step below the #14304C ground, and bracketed by hairline rules to read as a recessed instrument strip. That is the only "layer" in the design. Everything else — sections, entries, the gate, the footer — sits on the base ground and is separated by rules and space alone.

### Named Rules
**The Drawn-Not-Lifted Rule.** Structure is expressed with 1px rules and a fixed frame, never with elevation. If a region needs to feel distinct, it gets a hairline border or the sunk-band tint — never a shadow, never a radius.

## Shapes

Rectilinear and hard-edged throughout. Corner radius is `0` on every structural element: sheet, bands, stamp, action underline. The only non-zero radius in the stylesheet is a `1px` softening on the `:focus-visible` outline.

The form vocabulary is the hairline: 1px rules (`var(--rule)` / `var(--rule-soft)`) for structure, a 2px cyan rule for the two major document seams (under the masthead, above the footer), a 3px solid signal border for the release stamp with a 1px inset signal keyline (`.stamp::after`). Borders carry meaning by weight and colour, not by style — all are solid.

The one deliberate geometric gesture is the release stamp's `rotate(-3.5deg)`; nothing else on the page is rotated or skewed.

The logo mark is a thin-stroke diamond (cyan, 1.25px) with an interior crosshair and a chalk centre dot — drawn at the same hairline weight as the page structure, in the tertiary colour, never in the accent.

## Components

### Primary Action (`.act`)
- **Character:** A mono, understated command-line prompt — not a button.
- **Shape:** No background, no radius. A `1px solid var(--signal)` bottom border with `padding-bottom: 3px`.
- **Type/Color:** JetBrains Mono 500, 0.9rem, letter-spacing 0.02em, in `var(--signal)`; a trailing `→` in a `.arr` span.
- **Hover:** Bottom border thickens to 2px (padding compensates to 2px so text doesn't shift); the arrow translates `translateX(4px)` over 0.16s. No colour change.
- Used for "Open FreqCraft" and "Contact the studio". There is no secondary or ghost button in this system.

### Inline Link (`a`)
- `var(--signal)` text, 1px underline at `text-underline-offset: 0.18em`, underline colour starts at 55% signal and animates to full signal on hover over 0.15s. Text colour does not change.

### Readout Band (`.readout` / `.cell`)
- **Character:** An instrument strip reporting studio measurements.
- **Surface:** `var(--ink-sunk)`, full sheet width, `1px var(--rule)` top and bottom.
- **Grid:** `repeat(4, 1fr)`; cells divided by `1px var(--rule-soft)` left borders (first cell borderless, flush left). Collapses to 2×2 at ≤720px.
- **Cell:** cyan uppercase mono label (0.7rem, letter-spacing 0.08em) above a chalk mono value (`clamp(1.2rem,3.2vw,1.6rem)`, 500, `tabular-nums`); a secondary fraction rendered in `small` at 0.72em dim chalk.
- **Note (`.readout-note`):** dim-chalk 0.82rem line below the grid, hairline top, max 62ch, carrying one inline link.

### Clause Register (`.clause`)
- **Character:** A checkable commitments ledger — § / name / status / detail.
- **Grid:** `3.2rem 1fr auto` (ordinal / name / status), with the detail spanning columns 2–4 on a second row. Each clause has a `1px var(--rule-soft)` top border; the last also has a bottom border. Baseline-aligned.
- **Ordinal (`.no`):** cyan mono 0.78rem, `tabular-nums` (`§1`).
- **Name:** Archivo 600 uppercase, 0.98rem, chalk.
- **Status (`.status`):** signal mono 0.72rem, letter-spacing 0.14em (`PASS`).
- **Detail:** dim-chalk 0.92rem, max 62ch.

### Register Entry (`.entry`)
- **Character:** A numbered catalogue record of what has shipped.
- **Heading:** Archivo 700 `clamp(1.45rem,3.4vw,1.9rem)` with a leading `.ord` — cyan mono 0.7rem, letter-spacing 0.1em, nudged `translateY(-0.15em)`. Ordinal is cyan, never accent.
- **Muted variant (`h3.muted`):** dim chalk, weight 600 — for entries not yet shipped ("In development").
- **Meta line:** JetBrains Mono 0.74rem dim chalk, ` · `-separated facts.
- **Links row (`.links`):** mono 0.8rem, wrap, `gap: 8px 22px`.
- **`.entry-next`:** `margin-top: 30px`, hairline top — separates the shipped record from the in-development note.

### Release Gate / Stamp (`.gatemark` / `.stamp` / `.cap`)
- **Character:** The single dramatic object on the page — a rubber-stamped ship decision.
- **Stamp:** Archivo 800, `clamp(2.6rem,8vw,4rem)`, letter-spacing 0.06em, in `var(--signal)`; `3px solid var(--signal)` square border with a `1px` inset signal keyline (`::after`, 45% signal); `rotate(-3.5deg)`; 1px same-hue `text-shadow` thickener.
- **Caption (`.cap`):** mono 0.76rem dim chalk; product name in `b` is chalk 500, block display.
- **Motion:** When `.gatemark` scrolls into view (IntersectionObserver at 0.35 threshold, plus a scroll/resize fallback), the `.armed` class triggers `stamp-in` (560ms, `cubic-bezier(0.16, 1, 0.3, 1)` — exponential ease-out, from `rotate(-7deg) scale(1.22)` opacity 0) and `cap-in` (620ms, 120ms delay, slides up 6px). Both are `both`-filled and render fully without JS. Under `prefers-reduced-motion: reduce` all animation is removed and the stamp is static.

### Masthead Titleblock (`.titleblock`)
- **Character:** A drawing's title block — Doc / Sheet / Rev control fields.
- **Grid:** `1fr auto auto auto`; the wordmark then three `.tb-field` columns divided by `1px var(--rule-soft)` left borders with 20px gutters. `2px var(--cyan)` rule under the whole header.
- **Field:** cyan uppercase mono key (0.7rem, letter-spacing 0.12em) above a dim-chalk mono value (0.8rem, `white-space: nowrap`).
- **Wordmark:** diamond SVG mark (cyan hairline) + "DirectiveCraft" in Archivo 700, 1.06rem, chalk. Mark and text both chalk/cyan — never accent.
- **Mobile:** single column; fields become inline key/value rows.

### Footer (`.foot-top` / `.foot-links` / `.foot-rev`)
- `2px var(--cyan)` top rule. `.foot-top` is a space-between flex row: `.foot-mark` (Archivo 700, 0.92rem, dim chalk) and `.foot-links` (mono 0.78rem). `.foot-rev` is a cyan mono 0.72rem line with a hairline top — the document revision stamp ("Rev 2026-09-05 · Sheridan, Wyoming · No tracking on this page").

### Browser Surfaces
- `::selection`: `var(--signal)` background, `#1A1A1A` text.
- `:focus-visible`: `2px solid var(--signal)` outline, `outline-offset: 3px`, `border-radius: 1px`.
- Scrollbar: 12px, `var(--ink-sunk)` track, `var(--rule)` thumb with a 3px sunk-colour border; `scrollbar-color: var(--rule) transparent` for Firefox.

## Do's and Don'ts

### Do:
- **Do** keep one blue ground edge to edge; if a region must recede, use `var(--ink-sunk)` (#10283F) and hairline brackets, nothing else.
- **Do** set every checkable numeral in JetBrains Mono with `tabular-nums` — counts, versions, dates, ordinals, revision lines.
- **Do** ration `#F26E4C` to live/actionable elements only: links, the primary action, `PASS` status, the release stamp. Keep it under 10% of any screen.
- **Do** carry the sheet's left (`var(--rule)`) and right (`var(--rule-soft)`) edges on every top-level region — header, main, footer — so the 48rem sheet reads as continuous.
- **Do** divide groups with whitespace and a single 1px rule; use the 2px cyan rule only for the masthead and footer seams.
- **Do** keep prose within its measure: 44rem `.col`, ~54–62ch per block.
- **Do** left-align the display H1 and cap it at 19ch.
- **Do** let one authored motion moment (the PASS stamp) carry all the drama; everything else gets link/arrow micro-transitions at most, and must render fully without JS and be static under `prefers-reduced-motion`.

### Don't:
- **Don't** box, card, fill, or shadow a content group. No `box-shadow` anywhere; depth is the one sunk band only.
- **Don't** add corner radius to structural elements. Rectilinear, hard-edged; radius `0` except the 1px focus-outline softening.
- **Don't** put a number in the Archivo or Public Sans face, or introduce a gray — every neutral is a blue.
- **Don't** use the accent on the logo mark, ordinals, headings, or structure. The mark and ordinals are cyan.
- **Don't** centre the H1 or build a centered dark hero with principle cards and a glowing CTA — that is the explicit anti-reference.
- **Don't** add gradients, glass, glow, drop shadows, or decorative imagery.
- **Don't** introduce a second button style; the primary action is a mono underline, and there is no secondary/ghost variant.

## Scope

This system now governs all three built pages: `index.html`, `/testing/` (the
FreqCraft QA SOP), and `/privacy/`. The Space Grotesk and Inter `@font-face`
blocks remain in `assets/fonts.css` only as dead declarations (no page references
them) and can be removed once nothing else depends on them.

### Extension pages — `/testing/` and `/privacy/`

Both inherit the homepage tokens, masthead, sheet, footer, and readout band
unchanged. Page-specific components and one sanctioned adaptation:

- **Titleblock `Doc` values** are suffixed per sheet: `DC-000` (home),
  `DC-000-T` (testing), `DC-000-P` (privacy). The third field is `Home / ← Back`
  instead of `Rev`.
- **`/privacy/` fact readout** is the readout band at `repeat(3, 1fr)` (six
  boolean facts: Cookies/None … Account required/No). Values are chalk mono, not
  accent — "None" is a state, not an action.
- **`/testing/` procedure readout** is the readout band at `repeat(5, 1fr)`
  (211 / 22 / 02 / Sev / Written).
- **Phase divider (`.phase`)** — a `2px var(--cyan)` top rule (the same weight as
  the masthead/footer seam) with an Archivo 700 `clamp(1.2rem,3vw,1.6rem)` name.
  Marks the SOP's major parts (Automated coverage, Phase A, Phase B).
- **Test register (`.test`)** — the clause-register pattern extended: a bordered
  mono `.test-id` chip + Archivo `.test-title` on one row, then `.test-purpose`,
  a `.steps` checklist (1px cyan square markers via `::before`), and one or more
  `.result` lines. Hairline top border between tests, never boxed.
- **`.result` accent adaptation** — on the homepage the `PASS` status is the
  accent because it is rare. On `/testing/` a pass is the norm across ~20 tests,
  so **`.result` (pass) is neutral**: a 1px cyan left rule and a cyan mono label.
  **`.result.fail` / `.result` blockers take the signal** (1px signal left rule,
  signal label) because a failure is the one actionable thing on the page;
  **`.result.note`** uses a `var(--rule)` rule and dim label. This keeps the
  Live-Only Accent Rule intact — signal still marks "look here / act".
- **`.envbox`** — a mono config block on `var(--ink-sunk)`, 1px `--rule-soft`
  border with a 2px `--rule` left edge, `overflow-x: auto`.
- **`.gaps` table** — a real data table: cyan uppercase mono `th` on
  `var(--ink-sunk)`, 1px `--rule-soft` cell borders, wrapped in
  `.gaps-wrap { overflow-x: auto }` so it scrolls inside the sheet on mobile.
- **`.version-log`** — mono change-log block, same surface treatment as `.envbox`.
- No canvas, no background animation, no scroll-triggered motion on these two
  pages; the only JS is the runtime email assembly (with a `<noscript>` address
  fallback on `/testing/`).
