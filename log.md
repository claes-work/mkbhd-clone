# Log

_Append-only change record. Entry format: `## [YYYY-MM-DD] <type> | <title>` with_
_`<type>` ∈ `setup | plan | ingest | query | lint | persona-qa`._
_Ingest entries end with a synthesis-notes line (the synthesis-debt trail)._

## [2026-07-19] ingest | yt batch (@Waveform, 8) — first real ingest batch

First L2 ingest of the clone (corpus was 0 L2 before this). Stage B (P1-first) on
@Waveform, batch size 8: drained all 4 open @Waveform P1 rows — including the
fresh-upload P1 **"OnePlus is Dead… (In the US)" (2026-07-17)** — plus the 4 oldest P2
rows to fill the batch. All 8 had English captions; 0 no-captions, 0 duplicates, 0
skipped, no yt-dlp rate-limiting.

Videos (→ `wiki/sources/`): 2022-12-23 Wrapping Up 2022 + Blind Smartphone Test ·
2024-04-23 How One Small Company Saves Retro Tech · 2026-04-24 Tim Cooked and Now it's
John's Ternus · 2026-06-24 Explaining the NBA in Tech Terms · 2026-06-26 The Steam
Machine is Over $1000?! · 2026-07-03 Apple Raises Prices on Everything! · 2026-07-10
Nothing Beats Phone 4b with Ear 3a · 2026-07-17 OnePlus is Dead… (In the US).

**Attribution (ensemble channel).** These are multi-host Waveform episodes and the
transcripts are auto-captions with **no speaker labels**, so per-line attribution is
inherently uncertain. Each page confines the "Notable verbatim quotes (Marques)" bank
to lines that are unambiguously his (first-person self-reference to his reviews/channel,
or a co-host addressing "Marques" adjacent to the line); everything else is quarantined
in an "Unattributed / other-speaker material" section flagged `attribution: uncertain`
and does **not** train the persona. Marques-attributed quote counts per page: MYrfLmm 3,
v4FYdo **0** (guest-led Retro Tech interview — correctly yielded no Marques voice data),
Kf-67zx 4, 1YO2 2, voXcln 4, Mwllur 2, YgMNE4 3, 63m_fs 4. Co-hosts/guests (Andrew
Manganelli, David Imel, Adam Molina, Mariah, and episode guests) already have — or should
get — `wiki/entities/` context pages, not persona lines.

Ledger: 8 rows @Waveform L0→L2. Open after: **P1 113** (@mkbhd 111 + @WaveformClips 2),
P2 ~2567, shorts 363. @WaveformClips still holds its own fresh-upload P1 clip
(yt-SyR7RrXkqSs) — intentionally left open because clips must be deduped against their
parent @Waveform episodes, which are not yet ingested. Ingest batches since last
synthesis: 1 (checkpoint at 10 — no synthesis due yet).

Synthesis notes: 7 of 8 pages carry ★ L3-candidate material (synthesis debt) — Marques's
**blind-smartphone-camera-test methodology** and the durable principle *correct exposure
beats over-brightness/over-saturation* (Pixel 6A/5A winning years running); his
**"peak smartphone" / physics-is-real, buy-a-dedicated-camera** argument and the
CEO-interview insight that only the hardest strategic/moral calls escalate to a CEO
(Tim Cook episode); the **small-OEM structural-margin** thesis (why Nothing can't make a
flagship) and **"paperware until it ships"** EV-startup skepticism (Slate/Faraday/Roadster);
his **"reverse inflation" on editing-hardware cost**; the **platform-must-auto-surface
AI/provenance labels** and **de-monetize stolen short-form** stances; and the
**"next big thing after the iPhone"** AI-hardware framing. Most are attribution-to-confirm
against his solo-channel audio before promotion. Guest-led Retro Tech episode: no
persona value.
