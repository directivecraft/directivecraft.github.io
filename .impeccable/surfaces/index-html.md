---
version: 1
slug: "index-html"
primary_target: "index.html"
related_targets: []
---

# Surface brief — directivecraft.com homepage

Scope: homepage (`index.html`) only. `/testing/` and `/privacy/` keep their current design this pass.
Visitor mode: Persuade.
Audience: a prospective FreqCraft user checking whether the studio is real and the zero-data claim is true; secondary technical readers who judge by the `/testing` SOP.
Action: believe the studio is rigorous and independent; click through to FreqCraft.
Proof on hand: 211 automated tests, 0 data points, 2 named release devices, one-time purchase, the public `/testing` SOP with disclosed defects, LLC in Sheridan WY.
Constraints: single-file static HTML/CSS, no build step, GitHub Pages, zero third-party requests, email obfuscated at runtime, all numbers verbatim, name "DirectiveCraft" fixed.
Memorable moment: the gate stamp resolving to PASS as the readouts settle.
Unresolved: whether `/testing` + `/privacy` get a matching pass; whether PRODUCT.md/DESIGN.md should be git-ignored so Pages doesn't serve them.

## Direction contract

THESIS: The homepage is a controlled document — the artifact a studio issues when a claim must be checkable — not a landing page. It refuses the centered dark hero with three principle cards and one glowing CTA.

OWN-WORLD: One saturated diazo-blue ink owns the full page (#15304C ground, #EDF1F4 chalk text, #7FA8C9 pale-cyan secondary rule/label, #E4572E signal accent for live/actionable only). A control-block masthead (document no., revision, gate stamp). Groups separated by whitespace and hairline rules, never boxed. Numbers set as fixed tabular readouts with unit labels in a mono face; body in a technical grotesque; display in a document/redaction-grade face. No third-party assets.

STORY: Visitor understands DirectiveCraft is one named studio that publishes checkable software; believes it because every claim carries its evidence inline; acts by opening FreqCraft (the one accent link).

FIRST VIEWPORT: Masthead row — wordmark + doc no. left, "REV 2026-09 · SHERIDAN WY" right, thin rule under. Then the title line (studio's one sentence) at large display size, left-aligned. Below it a readout band: 211 TESTS / 0 DATA POINTS / 2 DEVICES / 1× PURCHASE, tabular, unit labels beneath. Bottom-left of the fold: the gate stamp resolving to PASS. Primary action ("Open FreqCraft →") in #E4572E, inline in the reading column, not a floating button.

FORM: Controlled document (diazo blueprint + QA release gate). Candidate 3 of 7 on the grounded list. Seed key 3d53d3f5, kind assigned, code-led.

FINISH: unreviewed and undocumented is unfinished; this build ends with the finish review, the verdict, DESIGN.md, and every shipping raster carrying its provenance
