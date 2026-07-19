# Synthesis state

_Tracks the synthesis **high-water mark** so the synthesis loop never misses material and never
re-does work. Companion to the ingest ledger (`ledger.csv`). The detailed debt lives in `log.md`
as `Synthesis notes:` lines (every ingest batch appends one). See `tools/SYNTHESIS.md` for the loop
and `tools/synthesis_batch.py` for the driver._

## High-water mark
Synthesized through: **the first 19 ingest batches (133 L2 sources)** — synthesis pass 1's 74-source
2013–2020 corpus PLUS pass 2's 9 batches: the @mkbhd 2021→2025 P1 completion, the origin-2009 era,
the Humane AI Pin landmark, and the first @AutoFocus (2026 EV) batch. Covers every `wiki/sources/`
page that was L2 as of 2026-07-19 (`## [2026-07-19] ingest` batches 1–19 in `log.md`).

## Pending checkpoints
_(oldest first; the synthesis loop drains these top-down)_
_None — synthesis is caught up with ingest (L2=133). Next checkpoint at the next channel/era
boundary or ~10 more batches._

## Done checkpoints
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
