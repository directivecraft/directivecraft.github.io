# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Single-file static HTML/CSS per page (inline `<style>`, small inline vanilla JS). No
build step, no framework, no dependencies. Self-hosted fonts under `/assets/fonts`.
Deploys directly to GitHub Pages from `main`, folder `/` (root); `.nojekyll` present so
every file is served as-is. `CNAME` = `www.directivecraft.com`. Decision confirmed by
the user for the redesign: keep it single-file static HTML/CSS.

## Users

Primary: a prospective FreqCraft user who has heard of the app and is deciding whether
the people behind it can be trusted — someone who cares that a tool does not phone home,
is evaluating that claim rather than taking it on faith, and wants to see evidence of
engineering seriousness before they install or pay.

Secondary: a technically literate visitor (developer, tinkerer, privacy-minded reader)
who arrives at or is pointed to the `/testing` page and judges the studio by the rigor
of its release process.

Not a target: enterprise buyers, investors, or a general consumer audience.

## Product Purpose

Directive Craft LLC is an independent one-person software studio in Sheridan, Wyoming.
It builds focused tools that "do one thing exactly right" with no accounts, no ads, no
telemetry, and no data leaving the device — sold as a one-time purchase, not a
subscription. The website is the studio's hub: it states the philosophy, presents the
shipping product (FreqCraft), and is meant to scale as more products ship. Success =
a visitor understands what the studio stands for and why that is unusual, believes the
zero-data claim because the site shows its work, and clicks through to FreqCraft.

## Positioning

Precision tools that expose every parameter and collect zero data, published by a named
US LLC that documents its actual release-QA procedure in public (the `/testing` page
reproduces the real SOP, sanitized only of internal file paths). The combination —
consumer-grade polish, zero data collection, one-time purchase, and openly published
engineering process from a solo studio — is what a neighboring product could not
truthfully copy.

## Operating Context

- The site is read before installing or buying FreqCraft, often after finding the app on
  Google Play or hearing about it, to answer "are these people legit and is the
  no-tracking claim real."
- The `/testing` page functions as a standalone credibility artifact that may be linked
  to directly.
- Contact is email only (`contact@directivecraft.com`), assembled at runtime and never
  present in HTML source — this obfuscation must be preserved.

## Capabilities and Constraints

- Static hosting only (GitHub Pages). No server, no backend, no forms that submit
  anywhere, no database. Any interactivity is client-side vanilla JS.
- Current pages: `/` (homepage), `/testing/` (FreqCraft QA SOP), `/privacy/`,
  `/samples/` (redirect to `/testing/`). Sitemap and robots.txt present.
- This engagement redesigns the **homepage only**. `/testing/` and `/privacy/` keep
  their current design for now and would need a follow-up pass to match.
- Factual claims and numbers are preserved verbatim and none are invented. Current
  correct values (the local clone was stale; these come from the user and live site):
  - **211** automated tests (widget + unit, ~15 files) — not 56.
  - **0** data points collected by the app or the site.
  - **2** physical test devices in the release gate (Moto G7 Power / Android 10 —
    oldest supported; Moto G 2025 / Android 16 — newest supported).
  - **22** manual QA procedures.
  - One-time purchase, no subscription.
  - FreqCraft is **Android 1.1.0**, Flutter/Dart, package
    `com.directivecraft.freqcraft`, live on Google Play.
- FreqCraft in one line: a precision binaural and isochronic tone generator for Android
  — every Hz value visible, every parameter editable, multi-voice sessions, a live
  waveform visualizer, timed sessions with perceptual fades, 7 factory presets, and
  background audio that ducks rather than interrupts other apps.

## Brand Commitments

- Legal name **Directive Craft LLC**; wordmark **DirectiveCraft** (currently rendered
  with "Craft" in the accent color). The name is fixed. The diamond logo mark and the
  amber (`#FFB300`) accent are the incumbent visual world and are open to replacement in
  the redesign (the user did not pin them).
- Voice: precise, technical, plain, anti-hype. "Nothing hidden." States facts and
  numbers; does not use marketing superlatives, urgency, or growth-hacking devices.
- Wyoming / Sheridan origin is stated plainly as part of the identity.

## Evidence on Hand

- Real: the FreqCraft app on Google Play; the `/testing` QA SOP (real procedure, real
  version log, real disclosed defects — STOP teardown race, readout-overflow catch);
  the LLC registration (Sheridan, WY); self-hosted fonts.
- Real screenshots of FreqCraft exist in the sibling `freqcraft.github.io` repo
  (`assets/shots/`) if product imagery is wanted.
- Does NOT exist yet and must not be presented as shipping: any desktop product, any
  second app (others are in active development only), testimonials, customer names,
  press quotes, download/revenue numbers, pricing specifics beyond "one-time purchase."

## Product Principles

1. Show the work, don't assert it — every trust claim on the site should be backed by
   something a visitor can inspect (the testing page, the zero-dependency source, the
   privacy page's specifics).
2. Facts over adjectives — numbers, versions, and named devices carry the message; no
   hype vocabulary.
3. The studio is small and says so — solo, independent, Wyoming; this is a credential,
   not something to hide behind scale-implying language.
4. Zero data is literal — no analytics, no cookies, no third-party requests, no fonts
   from Google; the site must keep practicing what it claims.
5. Built to scale to a product line — the homepage is a studio hub, not a single-app
   landing page.

## Accessibility & Inclusion

No product-specific standard was established. Preserve semantic HTML, keyboard
operability, visible focus, and adequate contrast; the site is content-light and should
stay legible without JavaScript.
