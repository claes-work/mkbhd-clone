# Synthesis state

_Tracks the synthesis **high-water mark** so the synthesis loop never misses material and never
re-does work. Companion to the ingest ledger (`ledger.csv`). The detailed debt lives in `log.md`
as `Synthesis notes:` lines (every ingest batch appends one). See `tools/SYNTHESIS.md` for the loop
and `tools/synthesis_batch.py` for the driver._

## High-water mark
Synthesized through: **the first 28 ingest batches (202 L2 sources)** — synthesis passes 1–2 (133 L2)
PLUS pass 3's 9 batches: the @AutoFocus 2026 Q1 EV batch and the eight @mkbhd Feb-2009 origin P2
batches (the deep origin / production-methodology thread). Covers every `wiki/sources/` page that was
L2 as of 2026-07-20 (`## [2026-07-19] ingest` batches 1–19 + `## [2026-07-20] ingest` batches 20–28 in
`log.md`).

## Pending checkpoints
_(oldest first; the synthesis loop drains these top-down)_
_None — synthesis is caught up with ingest (L2=202). Next checkpoint at the next channel/era
boundary or ~10 more batches._

## Done checkpoints
- [x] **Era: @AutoFocus 2026 Q1 EV batch + @mkbhd Feb-2009 origin P2 (69 new L2, batches 20–28)** —
  third synthesis pass. Drained the 9 accumulated `Synthesis notes:` lines. **Origin / production-
  methodology thread:** deepened `production-filmmaking` (the CamStudio + DivX 6.8.5 720p stack, the
  first "HD Test" milestone, the no-external-mic "started with nothing" gear origin, viewer-legibility
  zoom craft), added a "review methodology origin" section to `tech-reviews` (SRWare Iron benchmark +
  Task-Manager comparison, Safari-4 Acid3, earliest explicit "review" framings, first NZXT hardware
  unboxing, Microsoft Mouse 6000 two-part review, experience-over-benchmark GUI-boot choice), added
  origin nodes to `creator-business` (first channel branding, "MKB"-initials avatar, day-one
  audience-request loop), and added candidate aesthetic seeds to `consumer-tech-culture` (red-on-black
  contrast, macOS-in-Windows Apple affinity — flagged, not asserted causal). **EV thread:** extended
  `ev-cars` with the 2026 Q1 positions ("what's stopping me from recommending it?", winter-EV ownership
  framework, "specialty EVs" maturation, NACS-not-always-faster, democratized-performance, "simplify by
  fewer parts", depreciation-aware buying). Persona: added dated/cited entries to `beliefs.md` (origin
  values + EV frameworks), `voice.md` (origin + EV catchphrases and verbatim), `biography.md` (origin-
  2009 deepening + 2026 Q1 anchors), `appearance.md` (candidate brand-aesthetic origins); recompiled
  `persona/system-prompt.md` **v3** (compiled_from_sources: 202). Done 2026-07-20 (synthesis pass 3).
  Attribution: co-host "Miles" @AutoFocus driving segments stayed quarantined; only Marques-attributed
  material trained the persona.
- [x] **Era: @mkbhd 2021→2025 P1 completion + origin-2009 + Humane AI Pin + @AutoFocus 2026 EV batch
  (59 new L2, batches 11–19)** — second synthesis pass. Drained the 9 accumulated `Synthesis notes:`
  lines: extended all 7 topic hubs (Smartphone Awards 2020–25 slate; golden rule / "Great Separation" /
  "smartphones are OP" / "victim of its future ambition" / "compared to what?" / "Porsche 911 of ___" /
  two-buckets / utility-vs-aesthetics + skin-tone camera criteria; the full @AutoFocus EV worldview;
  origin-2009 production toolchain; three-levels-of-production; "this will be copied" / form-over-function
  / two-in-one), added dated cited entries to `persona/beliefs.md` + `persona/voice.md`, extended
  `persona/biography.md` (origin-2009 + 2021–2026 anchors) and seeded `persona/appearance.md` (6'3"),
  and recompiled `persona/system-prompt.md` **v2** (compiled_from_sources: 133). Done 2026-07-19
  (synthesis pass 2). Attribution: interview/co-host material (Tim Cook, Doctor Mike, @AutoFocus "Miles",
  Retro Tech guests) stayed quarantined; only Marques-attributed material trained the persona.
- [x] **Era: @Waveform + @mkbhd 2013–2020 P1 corpus (74 L2, batches 1–10)** — first synthesis pass.
  Drained the 10 accumulated `Synthesis notes:` lines: built all 7 `wiki/topics/` hubs, created
  `persona/beliefs.md` + `persona/voice.md` for the first time, extended `persona/biography.md`
  with dated 2013–2020 era anchors + Obama self-reported facts, and compiled
  `persona/system-prompt.md` **v1**. Done 2026-07-19 (synthesis pass 1).
