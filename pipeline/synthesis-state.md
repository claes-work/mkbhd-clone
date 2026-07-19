# Synthesis state

_Tracks the synthesis **high-water mark** so the synthesis loop never misses material and never
re-does work. Companion to the ingest ledger (`ledger.csv`). The detailed debt lives in `log.md`
as `Synthesis notes:` lines (every ingest batch appends one). See `tools/SYNTHESIS.md` for the loop
and `tools/synthesis_batch.py` for the driver._

## High-water mark
Synthesized through: **the first 10 ingest batches (74 L2 sources)** — the @Waveform year-end batch
plus the @mkbhd 2013–2020 P1 solo/interview corpus, log entries [2026-07-19] batches 1–10. Covers
`wiki/sources/` pages dated 2013-10-12 → 2026-07-17 that were L2 as of synthesis pass 1.

## Pending checkpoints
_(oldest first; the synthesis loop drains these top-down)_

## Done checkpoints
- [x] **Era: @Waveform + @mkbhd 2013–2020 P1 corpus (74 L2, batches 1–10)** — first synthesis pass.
  Drained the 10 accumulated `Synthesis notes:` lines: built all 7 `wiki/topics/` hubs, created
  `persona/beliefs.md` + `persona/voice.md` for the first time, extended `persona/biography.md`
  with dated 2013–2020 era anchors + Obama self-reported facts, and compiled
  `persona/system-prompt.md` **v1**. Done 2026-07-19 (synthesis pass 1).
