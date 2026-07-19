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

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — P1 solo main-channel batch

Stage B (P1-first) on **@mkbhd**, the main solo tech-review channel — the cleanest
Marques-attributed persona corpus. Batch size 8: drained the 8 oldest open P1 rows
(2013–2016 era). All 8 had English captions; **0 no-captions, 0 duplicates, 0 skipped,
no yt-dlp rate-limiting**. Second real ingest batch of the clone (16 L2 total now).

Videos (→ `wiki/sources/`): 2013-10-12 Apple iPhone 5s Review · 2014-08-31 The Truth
About Beats by Dre · 2014-12-08 Smartphone Awards: 2014 · 2015-10-09 Dope Tech #1:
Weapon · 2015-11-03 Dope Tech #2: Customs · 2015-12-19 Smartphone Awards: 2015 ·
2015-12-30 Dope Tech: Best of 2015 · 2016-01-08 Dope Tech: CES 2016.

**Attribution (solo channel).** Unlike the @Waveform ensemble batch, these are
single-presenter @mkbhd videos: Marques narrates throughout, so every page is
`attribution: solo` and the full transcript is Marques voice/persona data — no per-line
quarantine needed. Watched for guests/collab: none. The CES 2016 show-floor episode was
checked specifically for on-mic booth reps/demoers — there are none (Marques references
other YouTubers but no one else is quoted), so it too stays solo. All 8 pages carry ★
L3-candidate material.

Ledger: 8 rows @mkbhd L0→L2. Open after: **P1 105** (@mkbhd 103 + @WaveformClips 2),
P2 ~2667, shorts 363. @WaveformClips still holds its 2 fresh-upload P1 clips —
intentionally left open (clips must be deduped against parent @Waveform episodes, not yet
ingested). Ingest batches since last synthesis: 2 (checkpoint at 10 — no synthesis due).

Synthesis notes: 8 of 8 pages carry ★ L3-candidate material (synthesis debt), all needing
promotion into persona/topics at the next checkpoint. Durable persona signal captured:
his **earliest solo review methodology** (iPhone 5s — Touch ID/M7/camera verdict framing,
Android-vs-iPhone even-handedness); the **"you're mostly paying for brand/marketing, and
that's not automatically wrong"** consumer-value framework (Beats by Dre, margins vs
perceived value); the founding of the **annual Smartphone Awards** format plus 2014 and
2015 category winners, and the award CRITERIA as durable review values (battery over
thinness, no-compromise flagships, value/pricing as first-class, stock-Android preference);
the launch of the **Dope Tech** gear-showcase series and his **red-and-black studio
aesthetic** / "Team Crispy" image-quality identity + RED Weapon/Dragon and the Sigma
18-35 f/1.8 as his signature lens (production-filmmaking) and early dbrand/ColorWare vendor
ties; his dislike of **"year of the X"** framing and early conviction on **USB-C
inevitability** and **Tesla fleet-learning Autopilot** (Best of 2015); and his **"CES = a
glimpse of the future, not a shopping list" / hardware-ahead-of-its-content** trade-show
philosophy plus an early **Chevy Bolt as first real Tesla rival** EV take (CES 2016).
These are the first main-channel persona anchors and should corroborate/date-stamp the
@Waveform debt at the next synthesis pass.

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — P1 solo Dope Tech / iPhone 7 batch

Stage B (P1-first) on **@mkbhd**, the main solo tech-review channel. Batch size 8:
drained the next 8 oldest open P1 rows (all 2016) — seven **Dope Tech** episodes plus the
**iPhone 7 unboxing**. All 8 had English captions; **0 no-captions, 0 duplicates, 0
skipped, no yt-dlp rate-limiting**. Third real ingest batch of the clone (24 L2 total now).

Videos (→ `wiki/sources/`): 2016-02-12 Dope Tech: Crazy Speakers · 2016-07-14 Dope Tech:
Lightning Headphones · 2016-08-30 Dope Tech: Boosted Board 2 · 2016-09-14 iPhone 7
Unboxing: Jet Black vs Matte Black · 2016-10-08 Dope Tech: Self-Lacing Nike Mag ·
2016-10-11 Dope Tech: 8K RED Epic-W Unboxing · 2016-12-01 Dope Tech: Self Lacing Nike
HyperAdapt 1.0 · 2016-12-17 Dope Tech: Custom LED Clock.

**Attribution (solo channel).** All eight are single-presenter @mkbhd videos: Marques
narrates throughout, so every page is `attribution: solo` and the full transcript is
Marques voice/persona data — no per-line quarantine. Checked each for on-mic guests/
collaborators: none. People merely *referenced* but never heard on-mic (John of the "TLD"
channel re: the Orpheus and the HyperAdapt giveaway; the friend "Sam" who lent gear; the
person who lent the Nike Mag) were correctly left un-quarantined. The "Custom LED Clock"
turned out to be an off-the-shelf **LaMetric Time** he configures himself, not a
maker-built commission — still solo. No interview/collab episodes in this batch.

Ledger: 8 rows @mkbhd L0→L2. Open after: **P1 97** (@mkbhd 95 + @WaveformClips 2),
P2 ~2667 long-form, shorts 363. @WaveformClips still holds its 2 fresh-upload P1 clips —
intentionally left open (clips dedupe against parent @Waveform episodes, not yet
ingested). Ingest batches since last synthesis: 3 (checkpoint at 10 — no synthesis due).

Synthesis notes: 7 of 8 pages carry ★ L3-candidate material (synthesis debt); Nike Mag is
straight product coverage (no ★). Durable persona signal captured: his measured
**pre-iPhone-7 headphone-jack stance** (Lightning Headphones — concedes a matched Lightning
DAC can sound audibly better; objects on practical grounds, not audio quality) and the
**iPhone 7 headphone-jack-removal position** a month later (pragmatic/adapter-focused — the
$9 dongle replacement cost is the real friction, Lightning EarPods ≠ AirPods); his
**"shoot high-resolution now / cameras are computers attached to sensors"** production-craft
philosophy justifying 8K cinema-gear investment (RED Epic-W); the recurring **Dope Tech
format** as his vehicle for aspirational/novelty hardware (self-lacing Nike Mag & HyperAdapt
1.0, Boosted Board 2 e-mobility, high-end speakers, LaMetric clock); and his **jet-black vs
matte-black finish verdict** (special-edition jet black = scratch/fingerprint-prone; matte
= the "safe route") as an early durable review heuristic on premium finishes. All
attribution-clean (solo) and ready to corroborate/date-stamp the earlier @mkbhd + @Waveform
debt at the next synthesis pass.

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — P1 solo Dope Tech / Awards / iPhone X batch

Stage B (P1-first) on **@mkbhd**, the main solo tech-review channel. Batch size 8:
drained the next 8 oldest open P1 rows (late 2016 → early 2018) — the annual **Smartphone
Awards** (2016 + 2017), four **Dope Tech** episodes (Best Drones, 4K OLED Wallpaper TV,
Shot on Smartphones, and the two-part CES 2018 roundup), plus the **iPhone X unboxing**.
All 8 had English captions; **0 no-captions, 0 duplicates, 0 skipped, no yt-dlp
rate-limiting**. Fourth real ingest batch of the clone (32 L2 total now).

Videos (→ `wiki/sources/`): 2016-12-23 Smartphone Awards 2016 · 2017-01-18 Dope Tech: The
Best Drones · 2017-05-01 Dope Tech: The 4K OLED Wallpaper TV · 2017-06-28 Dope Tech: Shot
on Smartphones · 2017-10-31 Apple iPhone X Unboxing · 2017-12-20 Smartphone Awards 2017 ·
2018-01-11 Dope Tech of CES 2018 (Part 1) · 2018-01-14 Dope Tech of CES 2018 (Part 2).

**Attribution (solo channel).** All eight are single-presenter @mkbhd videos: Marques
narrates throughout, so every page is `attribution: solo` and the full transcript is
Marques voice/persona data — no per-line quarantine. The two CES show-floor episodes were
checked specifically for booth reps / demoers speaking on-mic (the usual quarantine risk
at a trade show): **none** — Marques narrates the whole floor walk solo. Collaborators
merely credited but never heard on-mic (e.g. "Dom" for drone shots) were correctly left
un-quarantined. No interview/collab episodes in this batch.

Ledger: 8 rows @mkbhd L0→L2. Open after: **P1 89** (@mkbhd 87 + @WaveformClips 2),
P2 2667 long-form (@mkbhd 1551 · @WaveformClips 623 · @Waveform 275 · @AutoFocus 120 ·
@TheStudio 98), shorts 363. @WaveformClips still holds its 2 fresh-upload P1 clips —
intentionally left open (clips dedupe against parent @Waveform episodes, not yet ingested).
Ingest batches since last synthesis: **4** (checkpoint at 10 — no synthesis due).

Synthesis notes: 7 of 8 pages carry ★ L3-candidate material (only the iPhone X *unboxing*
is un-flagged — first impressions, verdicts deferred to the full review). Two durable
threads strengthen this batch: (1) the annual **Smartphone Awards** franchise and its
per-category rubric (MVP = most-used phone, near-stock-Android optimization as recurring
tiebreaker, "best design" reframed as "best build") — two consecutive years now on record
(2016 Pixel XL MVP; 2017 Note 8 MVP / Pixel 2 best camera), a strong scorecard series to
distill; (2) a third + fourth **CES "glimpse of the future, not a shopping list"** data
point (2018 Parts 1-2) corroborating the 2016 CES framing — concept-vs-buyable filter,
"can't judge audio on a noisy floor" honesty, "~75% won't ship" test. Plus his subtractive
design-taste heuristic (Wallpaper TV: "remove everything until it stops looking like a TV")
and smartphone-camera philosophy ("Shot on X" ads are technically true but rig-heavy; a
phone never beats a DSLR on quality but always wins on being with you — enough to just
start). All attribution-clean (solo), ready for the next synthesis pass (debt now 4/10).

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — P1 solo reviews + Elon Musk / Bill Gates interviews

Fifth ingest batch. Drained 8 open P1 long-form rows from **@mkbhd**, oldest-first
(2018-04-03 → 2019-04-18), all to L2. One subagent per video wrote its own
`wiki/sources/` page; coordinator did ledger/index/log. **8 ingested, 0 skipped,
0 no-captions, 0 dup.** Captions fetched clean (no yt-dlp failures / rate limits).

Batch: Dope Tech: Camera Robots! (yt-UIwdCN4dV6w) · OnePlus 6 Review (yt-0PrUr3bQdwM) ·
Talking Tech with Elon Musk! (yt-MevKTPN4ozw) · Tesla Factory Tour with Elon Musk!
(yt-mr9kK0_7x08) · Smartphone Awards 2018! (yt-cpIEWsQpRMk) · Talking Tech & Saving the
World with Bill Gates! (yt-4mxXdCUXSSs) · Samsung Galaxy S10 Impressions! (yt-t9R7xx0joOU) ·
The Broken Galaxy Folds: Explained! (yt-vtqtyyGZvXM).

**Attribution — three interview/collab episodes handled per SUBJECT.md rules:** the two
Elon Musk videos (Talking Tech + Tesla Factory Tour) and the Bill Gates interview are
`attribution: interview`. Guests are context entities, NOT the subject — every substantive
Musk/Gates statement (Tesla/SpaceX engineering, "best part is no part," EV economics,
philanthropy/disease/AI-in-medicine) is quarantined to a non-persona "Unattributed /
other-speaker material" section and excluded from voice/beliefs training; only Marques's
own questions, framing, and self-description entered the voice bank. Recommended (not
created) `wiki/entities/` context pages for Elon Musk, Tesla, SpaceX, and Bill Gates —
recurring high-value context figures. The five remaining videos are solo, fully
Marques-attributed. Notable garble catch: Gates's "being able to jump over a garbage can"
was auto-captioned "believing Trump over a garbage can" — corrected, no political
reference. Other fixes logged per page (MKBHD misrenders, phone-model decimals, FANUC,
Roadster, Snapdragon 855, ultrasonic-fingerprint specs).

Pipeline after: **@mkbhd P1 79** (was 87), P2 1551, P3 38. Other channels unchanged
(@WaveformClips P1:2 held for dedup, @Waveform 292, @AutoFocus 120, @TheStudio 104).
Ingested L2=40, L3=0. Shorts open 363. Synthesis debt **5/10** (no checkpoint due).
Next iteration: continue Stage B on @mkbhd P1, oldest-first.

Synthesis notes: 7 of 8 pages carry ★ L3-candidate material. Durable threads sharpened:
(1) the annual **Smartphone Awards** franchise gains a third consecutive year (2018:
OnePlus 6T MVP, Note 9 best big, iPhone XS best small, Pixel 3 best camera, Mate 20 Pro
best-ever battery, Oppo Find X best design, Pocophone F1 best budget, Red Hydrogen One
biggest bust) — a strong multi-year scorecard series to distill; (2) an explicit
**price-to-value review lens** (OnePlus 6: "B+ camera, A+ for the price" — refusing to
grade a $529 phone on a flagship curve); (3) a **first-gen durability doctrine** (original
Galaxy Fold: "first-gen = public beta," robot fold-counts ≠ human longevity, soft-plastic
culprit); (4) **production-craft-as-core-value** (cinema camera robots, wants motion-control
in his own studio); (5) an **interview posture** (enthusiast-owner who does the research;
access-first, defer to the expert) visible across the Musk/Gates sit-downs. All persona-bound
material is Marques-attributed and attribution-clean; ready for the next synthesis pass.

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — P1 solo 2019 reviews + Retro Tech Game Boy doc

Sixth ingest batch. Drained 8 open P1 long-form rows from **@mkbhd**, oldest-first
(2019-04-19 → 2019-10-29), all to L2. One subagent per video wrote its own
`wiki/sources/` page; coordinator did ledger/index/log. **8 ingested, 0 skipped,
0 no-captions, 0 dup.** Captions fetched clean (no yt-dlp failures / rate limits).

Batch: Retro Tech: Game Boy (yt-Oy8zSYKkczI) · Dope Tech: The Probe Lens! (yt-jFZ0MFYup-o) ·
The Last (and First) Folding Phone! (yt-ROkXM3csNWY) · 5G: Explained! (yt-_CTUs_2hq6Y) ·
Dope Tech #20: Dual Screen Tech! (yt-XoH8no1MQWA) · iPhone 11 Review: Too Easy!
(yt-OoY7zp8GkLI) · This Is What Happens When You Re-Upload a YouTube Video 1000 Times!
(yt-JR4KHfqw-oE) · AirPods Pro Unboxing & Impressions! (yt-MrUhzYdcX6w).

**Attribution — one collab episode handled per SUBJECT.md rules:** *Retro Tech: Game Boy*
(yt-Oy8zSYKkczI) is not a solo piece but a mini-documentary — Marques narrates, but Casey
Neistat and several tech historians plus blindfold-test participants appear on camera. Marked
`attribution: interview`; every guest line quarantined to a non-persona "Unattributed /
other-speaker material" section, only Marques's narration and reactions entered the voice
bank. The other seven are solo, fully Marques-attributed. Caption-garble fixes logged per page
(Royole FlexPai captioned "Royal flex pie"/"Flex PI"; Laowa probe lens "probe blends", "M&Ms",
"B&H"; deployed Verizon mmWave really ~28/39 GHz vs. spoken 20–96 GHz range flagged; Dope Tech
#20 product names — ASUS ZenBook Pro Duo, LG V50, Sony WF-1000XM3/RX100 VII, Logitech MX
Master 3, Shure SM7B — normalized).

Pipeline after: **@mkbhd P1 71** (was 79), P2 1551, P3 38. Other channels unchanged
(@WaveformClips P1:2 held for dedup, @Waveform 292, @AutoFocus 120, @TheStudio 104).
Ingested L2=48, L3=0. Shorts open 363. Synthesis debt **6/10** (no checkpoint due).
Next iteration: continue Stage B on @mkbhd P1, oldest-first.

Synthesis notes: 5 of 8 pages carry ★ L3-candidate material. Durable threads sharpened:
(1) a **minimalism / "withered technology" lineage** (Game Boy's cheap-durable-simple design
beating more powerful rivals → a straight line to Marques's later iPhone/"do less, better"
doctrine); (2) the **"being first doesn't matter if it sucks"** thesis + a **fold-in-beats-fold-out**
form-factor stance (Royole FlexPai as the cautionary first foldable); (3) an **early-adopter
verdict template** on bleeding-edge tech ("glimpse of the future, not ready, don't pay extra
yet" — 2019 5G, mmWave speed-vs-range brute-force node-density model); (4) **"a company can
shoot itself in the foot on features"** framing (Canon vs. Sony) surfacing again in Dope Tech
#20; (5) **branding skepticism** — "everything high-end is just called Pro now" (AirPods Pro).
Also a reusable **price-to-value review lens** (iPhone 11 "easy to recommend, most people buy
the base iPhone"; standing low-res-LCD critique) and a **production-craft demonstration**
(1000x re-upload experiment: generational YouTube re-encode loss — 720p lock-in, magenta drift,
audio drift). All persona-bound material is Marques-attributed and attribution-clean.

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — P1 solo Cybertruck + Retro Tech S1 docs

Stage B (P1, @mkbhd, oldest-first). Ingested 8 long-form to L2 — 1 solo Marques
(Tesla Cybertruck first drive, 2019-11-22) + the 7-part **Retro Tech Season 1** launch
(official trailer 2019-11-25; DynaTAC, Polaroid, Walkman, Sega Genesis, Macintosh,
Camcorder, all 2019-12-02). All 8 fetched clean (no 429, no no-captions, no dups).

Attribution: the Cybertruck video is **solo** (Marques vlog voice-over; Elon/Franz/Fisher
recounted by him, not separate speakers). The 7 Retro Tech episodes are **mixed / guest-led
documentaries** — Marques hosts/narrates but the substantive history/analysis is carried by
named interviewees. These transcripts are **professionally captioned WITH speaker labels**
(Marques:, Martin Cooper:, iJustine:, Ken Segall:, Bill Nye:, Casey Neistat, etc.), so guest
material was cleanly quarantined (paraphrased into Key claims, attributed by name) and only
confident-Marques narration/hands-on lines entered each page's voice bank. Ambiguous/unlabeled
banter flagged `attribution: uncertain`. No non-Marques speech reached persona/voice data.

Pipeline after: **@mkbhd P1 63** (was 71), P2 1551, P3 38. Other channels unchanged
(@WaveformClips P1:2 held for dedup, @Waveform 292, @AutoFocus 120, @TheStudio 104).
Ingested L2=56, L3=0. Shorts open 363. Synthesis debt **7/10** (no checkpoint due).
Next iteration: continue Stage B on @mkbhd P1, oldest-first.

Synthesis notes: 4 of 8 pages carry ★ L3-candidate material. New durable threads:
(1) a **Retro Tech / creator-origin self-narrative** — Marques explicitly locates his own
filmmaking/camera obsession in the 1984 JVC GR-C1 camcorder ("I still owe a lot of what I do
now to this"), and frames the whole series around how portable-personal tech "shrinks the
world" (DynaTAC); a first-person biography/beliefs thread worth promoting. (2) A **design-
provocation lens on the Cybertruck** — "at least we're not bored": a polarizing love-it/hate-it
design beats a safe cookie-cutter one — reusable articulation of his EV/industry-design taste.
(3) **Instant/analog craft appreciation** (Polaroid: "you have to frame it right and nail focus,
you can't change that later") reinforcing his photography-fundamentals stance. Most Retro Tech
substance is guest-sourced history (not persona-bound). Caption garbles flagged on pages:
Cybertruck "2024 F150" (likely mis-year in a 2019 clip) and "64-bit Gravis consoles" in the
Genesis episode — kept as spoken, flagged, no specs altered.

## [2026-07-19] ingest | yt batch (@mkbhd, 6) — P1 solo Dope Tech + Smartphone Awards 2019 + Bill Gates interview

Stage B (P1, @mkbhd, oldest-first). Batch of 8 selected; **6 ingested to L2**, 2 left
open on **429 rate-limit** (yt-x_R-qzjZrKQ 2020 iPad Pro review, yt-aXfiyuUziY0 iPhone SE
2020 review — retry next iteration). Not 3 consecutive failures, so the batch completed
normally. Pages: Dope Tech 8K OLED year-end (2019-12-21), Smartphone Awards 2019
(2019-12-24), Dope Tech of CES 2020 / Sony Vision-S (2020-01-09), Talking Tech with Bill
Gates (2020-02-14), Xiaomi Mi Mix Alpha impressions (2020-02-28), Dope Tech $3500
Devialet Phantom Reactor speaker (2020-06-09).

Attribution: five are **solo** Marques videos (all persona/voice data). The **Bill Gates
video is an interview** — Marques is the interviewer (persona data); Bill Gates is a guest
(context entity), so his substantive answers on climate, EVs, misinformation, and email are
**quarantined** under an `attribution: uncertain` / "NOT persona data" section and excluded
from persona training (auto-captions have no speaker labels → Gates attributed by context).
No non-Marques speech reached voice data. Flagged Bill Gates + Microsoft as candidate
`wiki/entities/` context pages for a later entity pass (not created here). Caption garbles
fixed across pages: "neil i patel"→Nilay Patel (The Verge), "porsche ti cam"→Porsche Taycan;
"snapdragon 85"→Snapdragon 855, "royal flex pie"→Royole FlexPai (Awards); 7680×4320 8K
pixel reconstruction (OLED); Devialet brand added in prose (never spoken in captions).

Pipeline after: **@mkbhd P1 57** (was 63; 2 held on 429), P2 1551, P3 38. Other channels
unchanged (@WaveformClips P1:2 held for dedup, @Waveform 292, @AutoFocus 120, @TheStudio
104). Open P1 total 59. Ingested **L2=62**, L3=0. Shorts open 363. Rate limits: 2×429 this
batch. Synthesis debt **8/10** (no checkpoint due). Next iteration: continue Stage B on
@mkbhd P1, oldest-first (retry the two 429 rows first).

Synthesis notes: 5 of 6 pages carry ★ L3-candidate material. New durable threads:
(1) **"bleeding-edge statement piece" evaluation lens** (8K OLED / Mi Mix Alpha) — an
impressive product nobody can fully exploit yet because the surrounding content/ecosystem
doesn't exist; "costs as much as a car but tech people might want it more than a car" —
a recurring MKBHD framing for early-adopter flagship/concept tech. (2) **Smartphone Awards
2019** is a canonical recurring format: full winner slate (PotY OnePlus 7 Pro; Best Camera
iPhone 11 Pro; Bust of the Year Pixel 4; Most Improved/Best Big ROG Phone 2; Best Compact
S10e; Best Budget Redmi K20 Pro; Design Galaxy Fold) + his evaluation-criteria framing —
worth an L3 topic note tracking year-over-year picks. (3) **Marques's interviewer posture**
with Bill Gates — prepared, primary-source-grounded (reads Gates's own annual letter back to
him), gently pointed ("what if you miss?", "as a youtuber I have to ask about youtube") —
reinforces the same "enthusiast who does the homework" interview stance seen in the Elon
Musk sit-down; an L3 persona thread. (4) **"tech as moving art" inclusion criterion** for
Dope Tech (Sisyphus kinetic table, rehoused Helios lens) — what qualifies something as
"dope" beyond specs. Most interview substance (Gates) is guest-sourced and NOT persona-bound.

## [2026-07-19] ingest | yt batch (@mkbhd, 5) — P1 solo 2020 reviews + Zuckerberg interview + 8K gaming

Stage B (P1-first) on **@mkbhd**, oldest-first, batch size 8. Retried the two rows the
previous batch left open on 429 first: **iPad Pro (yt-x_R-qzjZrKQ)** — the 429 cleared but
the only caption track fetched was music-only (`[music]`, 1 word), no speech captions, so
it can't be ingested without fabricating → marked **L1 no-captions (music-only; revisit)**;
**iPhone SE 2020 (yt-aXfiyuUziY0)** — **429 again**, left open for retry. One further
selection, **Dope Tech: Boston Dynamics Robot Dog (yt-s6_azdBnAlU)**, had no subtitles →
auto-marked L1 no-captions by the driver. The remaining 5 had good English captions and
were written to `wiki/sources/`.

Videos (→ 5 L2): 2020-06-23 iOS 14 Hands-On: Everything New! · 2020-07-18 Dope Tech: The
Biggest Ultrawide Monitor! (3X Pods giant-AirPods speaker, Asus ROG Zephyrus Duo, Samsung
Odyssey G9) · 2020-08-17 Dope Tech: The iPad Pro Killer?! (Xiaomi smart charging pad, Hachi
Infinite M1 projector [disclosed sponsorship], Galaxy Tab S7+) · 2020-09-16 Talking Tech
and The Metaverse with Mark Zuckerberg! · 2020-09-23 Can You Actually Game in 8K? (RTX 3090
Gameplay!).

**Attribution.** Four solo Marques videos (all persona/voice data). One **interview** —
the Mark Zuckerberg sit-down — handled like the Elon/Gates pages: Zuckerberg is a guest
(context entity), his substantive VR/AR answers are quarantined in an "Unattributed /
other-speaker material" section and excluded from persona training; only Marques's
questions/framing (8 verbatim quotes) train the voice. Zuckerberg + Facebook/Oculus flagged
for a later `wiki/entities/` context pass (not created here).

Pipeline after: **@mkbhd P1 50** (was 57: −5 L2, −1 iPad no-cap, −1 Boston no-cap; iPhone SE
429 still counted open). Open P1 total **52** (@mkbhd 50 + @WaveformClips 2 held for dedup).
P2 1551, P3 38 (@mkbhd). Other channels unchanged (@Waveform 292, @AutoFocus 120,
@TheStudio 104). Ingested **L2=67**, L3=0. Shorts open 363. Rate limits: **1×429** this
batch (iPhone SE). Synthesis debt **9/10** (no checkpoint due yet — a checkpoint/Stage S is
now one batch away). Next iteration: continue Stage B on @mkbhd P1 oldest-first (retry the
iPhone SE 429 first); expect a synthesis checkpoint to fall due shortly.

Synthesis notes: all 5 pages carry ★ L3-candidate material. New/reinforced durable threads:
(1) **"why now?" review lens** (iOS 14) — when a company ships an obvious/overdue feature,
ask what it waited to get right instead of just dunking on the lateness; plus his even-handed
Apple-vs-Android platform comparisons. (2) **Novelty-axis verdict** — "don't buy these for
the build quality, don't buy these for the sound quality, buy these for the immense flex"
(3X Pods): being explicit that a gadget can be worth it purely for novelty. (3) **"copied
Apple's homework but changed it up just a little bit"** — recurring Samsung/Android-borrows-
Apple framing (Galaxy Tab S7+), plus his standing "buy the Samsung tablet for the screen"
verdict. (4) **VR as "the next version of tech reviews"** — a genuine dated **2020 Marques
belief** ("put you in my shoes… you'll feel like you're in the car I'm driving"), persona-
relevant (frame as a 2020 view, not necessarily current); his prepared, self-checking
interviewer posture reinforces the Elon/Gates thread. (5) **"frame rate is king, but
resolution buys immersion"** + **"the tech works, the ecosystem isn't ready"** (8K/RTX 3090:
"the world of 8K gaming monitors doesn't really exist yet") — reinforces the prior batch's
"bleeding-edge statement piece" thread. (6) Sponsorship note: the Hachi projector segment is
a **disclosed** paid placement, stated up-front — a data point for the sponsorship-ethics
thread in SUBJECT.md. Most Zuckerberg interview substance is guest-sourced and NOT
persona-bound.

## [2026-07-19] ingest | yt batch (@mkbhd, 7) — P1 solo late-2020: iPhone 12 / AirPods Max / PS5 + Obama interview

Stage B (P1-first) on **@mkbhd**, oldest-first, batch size 8. One row rate-limited on the
first fetch — **iPhone SE 2020 (yt-aXfiyuUziY0)** returned HTTP 429 and was **left open**
for a later retry (not a hard failure; the other 7 fetched clean, so no 3-in-a-row stop).
The other 7 went to **L2**.

Videos (→ 7 L2): 2020-09-25 The Ultimate iOS 14 Homescreen Setup Guide! · 2020-10-20 iPhone
12 Unboxing + MagSafe Demo! · 2020-10-25 iPhone 12 Review: Just Got Real! · 2020-10-27
PlayStation 5 Unboxing & Accessories! (embargo: hardware-only) · 2020-12-10 AirPods Max
Unboxing & Impressions ($550) · 2020-12-16 Some Quick Advice from Barack Obama! (interview) ·
2020-12-16 AirPods Max Review: Luxury Listening!.

**Attribution.** Six solo Marques videos (all persona/voice data). One **interview** — the
Barack Obama BookTube exchange — handled like the Elon/Gates/Zuckerberg pages: Obama is a
guest (context entity), his answers quarantined in a "Quarantined — guest" section and
excluded from persona training; only Marques's interviewer framing + self-description train
the persona. That Obama page is a **high-value biography source** (self-reported: age 26 in
2020, channel started 2009, 10+ years, pro ultimate frisbee / NY Empire undefeated 2019,
avid golfer, NBA fan, attended the 2009 inauguration) and carries a dated diversity belief
(golf/ultimate/tech "not very diverse at a high level" → "the spotlight just a little bit
hotter as a Black man"). Obama = context entity, flagged for a later `wiki/entities/` pass
(not created here).

Pipeline after: **@mkbhd P1 43** (was 50: −7 L2; iPhone SE 429 still counted open). Open P1
total **45** (@mkbhd 43 + @WaveformClips 2 held for dedup). P2 1551, P3 38 (@mkbhd). Other
channels unchanged (@Waveform 292, @AutoFocus 120, @TheStudio 104). Ingested **L2=74**, L3=0.
Shorts open 363. Rate limits: **1×429** this batch (iPhone SE). Synthesis debt **10/10 — a
synthesis CHECKPOINT is now due**: this batch crosses the ~10-batch threshold, so the next
iteration should run **Stage S** (the first synthesis pass — fold the accumulated @Waveform +
@mkbhd 2013–2020 P1 debt into `wiki/topics/` hubs + build `persona/` beliefs/voice/biography
for the first time + compile `persona/system-prompt.md` v1) BEFORE resuming ingest. Retry the
iPhone SE 429 on the next Stage B.

Synthesis notes: strong ★ L3 material this batch. New/reinforced durable threads: (1)
**"the best technologies are invisible"** — an explicit, dated core Marques design principle
(iPhone 12 5G Smart Data Mode; ProMotion analogy) → promote to `persona/beliefs.md`. (2)
**scratch-vs-shatter inverse tradeoff** — a reusable durability-analysis framework (iPhone 12
Ceramic Shield), with his standing "I'll live my life / defer scratch truth to JerryRig­
Everything's Zack" posture. (3) **portless-iPhone prediction (2020)** — dated forecast off
MagSafe, worth logging for later "was he right?" tracking. (4) **no-charger-in-box critique**
with the USB-A/USB-C mismatch counter-argument — a citable position on Apple's environmental
framing. (5) **"two types of high-end headphones: reference/production vs luxury listening"**
— a reusable audio-review taxonomy (AirPods Max), plus the recurring **electric-car-cornering
weight analogy** and his **"I'm not an audiophile but I know what I like"** self-positioning.
(6) **Apple-review verdict shape**: premium execution + a few glaring quirks + "if you're in
Apple's ecosystem" = recommendation. (7) **iOS 14 "welcome to the party" stance** — even-
handed Apple-catches-up-to-Android framing. (8) Biography/voice from the Obama page (see
Attribution). Obama's own answers are guest-sourced and NOT persona-bound.

## [2026-07-19] lint | synthesis pass 1 — @Waveform + @mkbhd 2013–2020 P1 corpus (74 L2)

**First Stage S / first synthesis pass of the clone.** Drained the full accumulated
synthesis debt — all **10 `Synthesis notes:` lines** (batches 1–10, 74 L2 sources: the
@Waveform year-end/blind-test batch + the @mkbhd 2013–2020 P1 solo/interview corpus).
Promoted the genuinely-new durable material into `wiki/topics/` L3 hubs and built the
`persona/` product for the first time. No sub-agents (done in one agent context per the
run constraint). One writer, one file at a time.

**Topic hubs written (all 7 populated from stubs → dated, cited frameworks):**
- tech-reviews — two-axis camera model, price-to-value curve, "bust = expectations minus
  reality", "why now?", Apple-verdict shape, reference-vs-luxury audio taxonomy,
  dailies-every-phone, defers durability/benchmarks to specialists.
- smartphones — Smartphone Awards franchise (multi-year winner **table** 2014–2019),
  Blind Camera Test methodology (ELO, correct-exposure-beats-over-brightness),
  vertical-integration-beats-specs, finish heuristic, headphone-jack pragmatism, foldables.
- production-filmmaking — "camera = computer with a sensor", RED/RAW for craft,
  shoot-high-res-now, one-man-crew, photography fundamentals, re-encode-loss demo,
  creator origin.
- creator-business — margins + perceived value, Dope Tech thesis, novelty-axis, sponsorship
  disclosure, platform/creator-economy positions (attribution-to-confirm), channel self-def.
- ev-cars — Cybertruck "at least we're not bored" / source-critical demos, Chevy Bolt,
  Tesla fleet-learning, "paperware until it ships", electric-car-cornering analogy.
- tech-industry-commentary — "best technologies are invisible", scratch-vs-shatter,
  "tech works / ecosystem isn't ready", "bleeding-edge statement piece", CES philosophy
  (4 yrs), dated predictions (portless iPhone, USB-C), interviewer posture, CEO-escalation,
  peak-smartphone/small-OEM (attribution-to-confirm).
- consumer-tech-culture — Retro Tech "withered technology"/minimalism + creator origin,
  Dope Tech "tech as moving art", subtractive design, design-risk, branding skepticism,
  accessibility appreciation.

**Persona built for the first time:**
- `persona/beliefs.md` — created (was empty skeleton): Frameworks / Values / Opinions,
  all dated + cited; an "attribution-to-confirm (@Waveform)" bucket kept separate from firm
  beliefs; a "predictions to track" bucket.
- `persona/voice.md` — created (was empty skeleton): catchphrases ("dope", "anything with
  an on button", "forehead/chin", "your boy", "league of its own"), cadence, humor, and a
  cited verbatim quote bank (Marques-attributed only).
- `persona/biography.md` — extended with a "Corpus-derived anchors (2013–2020 era)" section:
  first-iPhone-review POV, RED/Team-Crispy identity, JVC-camcorder creator origin, and the
  dense Obama-BookTube self-reported block (age 26 in 2020, channel since 2009, NY Empire
  ultimate, golfer, NBA) + the dated diversity reflection. Marquee interviews indexed.
- `persona/appearance.md` — left empty (captions can't supply it; needs watched-video samples).

**Attribution discipline:** interview guests (Musk, Gates, Zuckerberg, Obama, Neistat) were
already quarantined at ingest and stayed OUT of persona — only Marques's own framing/voice
promoted. Ensemble-@Waveform findings whose per-line speaker is uncertain were promoted only
into the topic hubs and a clearly-labeled "attribution-to-confirm" bucket in beliefs, NOT the
firm belief set or system-prompt claims.

**Compiled:** `persona/system-prompt.md` **v1** (compiled_from_sources: 74) — first compile;
Persona mode (`/mkbhd`) can now load a clone. Coverage flagged strong on 2013–2020, hedge on
post-2021 (Auto Focus / Panels / Humane / Fisker / Tim Cook only lightly covered).

**Bookkeeping:** advanced the high-water mark in `pipeline/synthesis-state.md` (checkpoint moved
to Done, tagged v1); updated `index.md` (topics + persona sections). No ledger changes (synthesis
doesn't move L2→L3 rows; it promotes content). No rate limits, no errors, no fabrication.

Synthesis notes: none — synthesis debt fully drained (10/10 → 0). Next ingest batch starts a
fresh counter toward the next checkpoint (~10 batches or next channel/era completion). Resume
Stage B on @mkbhd P1 oldest-first next iteration (retry the iPhone SE 2020 yt-aXfiyuUziY0 429).

## [2026-07-19] ingest | yt batch (@mkbhd, 7) — P1 solo Smartphone Awards 2020 / iPhone-REALLY + Retro Tech S2 docs

Stage B (P1-first) on @mkbhd, oldest-first, batch size 8. The oldest P1, **iPhone SE
(2020) Review (yt-aXfiyuUziY0, 2020-04-22)**, hit HTTP 429 again on caption fetch — a
repeat offender across prior batches — so per instructions it was tried once, left open,
and NOT allowed to block the batch. Recorded a `429 rate-limited (repeated)` marker on
its ledger notes so the oldest-first selector stops re-drawing (and re-429-ing) it every
batch; it remains open (L0-discovered, P1) for a later retry. The other 7 rows all had
English captions → 7 L2 pages written. 0 no-captions, 0 duplicates, 0 skipped. **1× 429
(the one known-bad row); not a rate-limiting cascade** (safety rail not tripped).

Videos (→ `wiki/sources/`): 2020-12-23 **Smartphone Awards 2020!** (yt-e6_t26Q9aVM) ·
2021-03-05 **What I REALLY Think of the iPhone!** (yt-V7J9aMy_CFk) · 2021-03-17 **Dope
Tech: The Fastest Drone AND Car Yet!** (yt-syiQmaGZFXM) · 2021-04-13 **Retro Tech: Flying
Cars** (yt-ifI_fwg55k8) · 2021-04-14 **Retro Tech: Teleportation** (yt-tEmLMCPK8OE) ·
2021-04-15 **Retro Tech: Robots** (yt-nLeScEdf550) · 2021-04-16 **Retro Tech:
Hyperconnectivity** (yt-MhKiMPiZOdE).

**Attribution (mixed batch).** 3 solo Marques videos (Smartphone Awards, iPhone-REALLY,
Dope Tech) → fully persona/voice data. The 4 Retro Tech Season 2 episodes are produced
**documentaries** with heavy guest content, but — like the S1 Retro Tech docs — the
transcripts carry **reliable speaker labels**, so attribution is clean: each page's
Marques voice-bank is limited to labeled-Marques narration/hosting, and guest experts
(Gali Russell/Michael Ian Black/Omni Hoverboards; Vsauce2/Game Ranks/**Neil deGrasse
Tyson**; UrAvgConsumer/Mark Parsons; Chuck Nice/Sara Dietschy/NextMind) are paraphrased
as clearly-attributed key claims only — NOT persona data. Unlabeled "Dope or Nope" banter
lines were quarantined `attribution: uncertain`.

Synthesis notes: Genuinely-new, high-value persona material this batch (7 ★ L3-candidates
flagged for the next synthesis pass, NOT inline-promoted): (1) **"What I REALLY Think of
the iPhone"** is a landmark review-methodology source — the "review as a balancing act /
art of compression," "nine jobs in one," point-and-shoot-vs-manual camera framework,
app-support as his reason for carrying an iPhone, and the "glass is glass" anti-hype
stance (fits tech-reviews + creator-business + voice/beliefs). (2) The **Smartphone
Awards** annual-format + the **"premium mid-range ~$700 tier" 2020 thesis** (S20 FE MVP).
(3) The **Dope Tech Top Gear / Auto Focus partnership announcement** (2021-03-17) — a
datable biography node predating the Aug-2022 Auto Focus channel launch; plus his
first-person-POV production rationale. (4) Recurring **tech-optimist framing** across the
Retro Tech docs ("bring B to A instead of A to B"; "we already have our robot future — as
the Roomba"; "communication is the one sci-fi category that came true"; recreational
individual flight) — reusable beliefs/voice material.

## [2026-07-19] ingest | yt batch (@mkbhd, 6) — P1 solo 2021 iPhone 13 Pro / EVERY iPhone / Smartphone Awards + Pichai & Gates interviews
Stage B (P1, oldest-first, 2021+ era) on @mkbhd, batch size 8. Prepared 8; **6 ingested to
L2**, **1 skipped (429 rate-limit)** — `yt-ehv3zQAa9zM` Apple AirTags Unboxing (left open for
retry) — and **1 auto-marked L1 no-captions** — `yt-DyKQ7qtTJag` Tesla Model S PLAID
Impressions (no subtitles; not Whispered). The known repeated-429 iPhone SE 2020 row was
correctly NOT drawn (older, already excluded by the driver).

Pages written (all L2): 2021-04-17 Retro Tech: Smart Homes (`ccnlAVDXd7k`) · 2021-05-21
Talking Tech w/ Sundar Pichai (`n2RNcPRtAiY`) · 2021-10-02 iPhone 13 Pro Review
(`TnkdoEZhTbc`) · 2021-10-12 Reviewing EVERY iPhone Ever (`8FpPSMIB4uA`) · 2021-12-22
Smartphone Awards 2021 (`IDcyXtweHCw`) · 2022-03-02 Dope Tech: Weirdest Earbuds
(`-EZ_3Tq9a8c`). youtube-index footer 81→87; index.md 81→87.

**Attribution:** two non-solo items handled under the fidelity rules. (a) **Sundar Pichai**
video is a full 1:1 **interview** (`attribution: interview`) — only Marques's questions/
framing train the persona; all Pichai answers quarantined as CONTEXT for a future
`wiki/entities/sundar-pichai` page. (b) **Retro Tech: Smart Homes** is a **documentary**
(`attribution: mixed`) with an on-camera **Bill Gates** interview plus Dulcé Sloan (comedian)
and Sam Sheffer (YouTuber) segments — all guest lines quarantined; this is the 2nd Bill Gates
interview in the corpus. The Dope Tech end-card giveaway is a collab (Mr Who's The Boss +
dbrand) but no guest speaks, so nothing to quarantine there.

Synthesis notes: nothing landmark inline-promoted (debt logged for the next pass, checkpoint
at 10 batches). Genuinely-new/reusable material flagged with ★: (1) the **ProMotion /
high-refresh "you won't notice it until you go back to 60 Hz" thesis** + the **"minor
upgrades compound into greatness"** incremental-craft philosophy (iPhone 13 Pro), both
Marques-attributed and spanning smartphones + production-filmmaking. (2) A dense set of
**canonical MKBHD iPhone-line verdicts** (iPhone 4 = best design; iPhone X "opened Pandora's
box" on $1,000 phones; 6/6 Plus = best-selling ever; "the beginning of the end of small
phones"; "cheap phones are getting good") plus his **price-inflation / market-saturation
industry read** (Reviewing EVERY iPhone). ⚠️ Contradiction flagged on that page: he
misstates the iPhone 4S as "iOS 7" (it shipped on iOS 5) — do NOT promote that. (3) The
**Smartphone Awards 2021** canon — the deliberately-created "best small phone" category vs.
screen-size inflation, the pro-competition ethos ("moment of silence for LG"), and the "nail
the fundamentals" review value (MVP: Galaxy S21 Ultra). (4) Marques's **camera-evaluation
priority — skin tones + latitude** stated first-person in the Pichai interview (small but
datable review value). (5) The **"straight line" withered-tech-to-today** framing recurs in
Smart Homes (Clapper/X-10/Butler-In-A-Box → modern assistant; "sweet spot between the
Clapper and the Nest"), reinforcing the Game Boy minimalism doctrine.

## [2026-07-19] ingest | yt batch (@mkbhd, 7) — P1 solo 2022–23: iOS 16 / iPhone 14 Pro / Smartphone Awards 2022 + Dope Tech ×3
Stage B (P1, oldest-first, 2022+ era) on @mkbhd, batch size 8. Prepared 8; **7 ingested to
L2**, **1 skipped** — `yt-ehv3zQAa9zM` Apple AirTags Unboxing (left open, unchanged).

Pages written (all L2, all `attribution: solo`): 2022-07-11 iOS 16 Hands-On (`WfVF-Ec4naQ`) ·
2022-08-15 Dope Tech: Most Extreme Gaming Monitor (`MEiq0oCUb_8`) · 2022-09-14 iPhone 14 Pro
Review (`SdLShOCvVeM`) · 2022-09-30 Dope Tech: Hottest Laptop Design (`bFBIrkzy_gM`) ·
2022-12-27 Smartphone Awards 2022 (`5NjFuS_24v8`) · 2023-03-27 Dope Tech: Better than Expected
(`O-buiiyp_xU`) · 2023-04-01 Smartphone Awards Midseason 2023 (`17VcGk_-Ghc`). youtube-index
footer 87→94; index.md 87→94.

**Attribution:** all 7 are solo, Marques-fronted — no interview/collab episodes with other
speakers in this batch, so nothing quarantined. Two carry **disclosed paid sponsor segments**
(Samsung Odyssey Ark in the gaming-monitor Dope Tech; EcoFlow in the laptop Dope Tech) — those
praises are marked sponsor-context on the pages, not clean persona rankings. The 2023-04-01
Midseason Awards is an **April Fool's satire** video: ingested (not skipped) as a light L2
because it carries genuine citable signal, but the "S23 Ultra wins every category" bit is
quarantined as a joke; only the real early-2023 S23 Ultra praise, the real Space Zoom moon
skepticism, and the anti-misinformation PSA are persona-eligible (flagged on the page).

**Premise correction (AirTags):** the task flagged `yt-ehv3zQAa9zM` (AirTags) as a
"repeated-429" row to skip. In fact only the **iPhone SE 2020** row (`yt-aXfiyuUziY0`) carries
the `429 rate-limited (repeated)` ledger marker, and the driver correctly did NOT draw it
(older, auto-excluded). AirTags 429'd **once** last iteration and was left open for retry; this
iteration its captions **fetched OK** and it is now ingestable. Per the explicit skip directive
I left it untouched (still open, no page) rather than silently overriding — green-light it and
the next Stage B batch will pick it up cleanly.

**Rate limits:** 0 × 429 this iteration (all 7 caption fetches succeeded; safety rail not
tripped). No yt-dlp errors.

Synthesis notes: nothing landmark inline-promoted (debt logged; checkpoint at 10, now 3 batches
since synthesis pass 1). Genuinely-new durable material for the next synthesis pass: (1) the
**"this will be copied" industry-prediction** stance, stated at full strength on the iPhone 14
Pro's **Dynamic Island** (with the LG V10 precedent) — fits tech-industry-commentary. (2) The
**camera skin-tone accuracy critique** — "overexpose people with dark skin constantly, I would
know" — a signature, personal, recurring MKBHD position (→ smartphones/production-filmmaking +
persona/beliefs). (3) The **"form over function"** design-critique lens, stated at its purest on
the Dell XPS 13 Plus. (4) The **"two-in-one devices are always worse at one thing"** product
theory (Huawei Watch Buds). (5) Recurring **awards-as-tradition** framing + the **blind
smartphone camera test** method (photo-vote ≠ best-camera-system), and the iPhone's **4th-year**
camera-system win. (6) The recurring **USB-C-over-Lightning / ProRes-offload** complaint and the
**"iOS update matters as much as a new phone for iPhone 11+"** upgrade doctrine.

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — P1 solo 2023: $40k iPhone / Dyson Zone / Vision Pro / Solar Roof + iPhone 15 Pro
Stage B (P1, oldest-first) on @mkbhd, batch size 8. Prepared 8; **7 ingested to L2**,
**1 left open (429)** — `yt-ehv3zQAa9zM` Apple AirTags rate-limited on caption fetch this
run and was left open, unchanged (single 429, not the 3-consecutive safety rail).

Pages written (all L2): 2023-04-20 I Spent $40,000 to Unbox a Sealed Original iPhone
(`-BwUyTrU9fo`, solo) · 2023-05-15 This is the Dumbest Product I've Ever Reviewed / Dyson Zone
(`tFdnCzfJPJ0`, solo-with-guest) · 2023-06-06 Apple Vision Pro Impressions (`OFvXuyITwBI`, solo) ·
2023-07-03 Dope Tech: Nothing Phone 2 Redesign (`RM7SobH8ZO0`, solo) · 2023-07-29 Tesla Solar
Roof Review: Was It Worth It? (`UJeSWbR6W04`, solo) · 2023-09-13 iPhone 15/15 Pro Impressions
(`enR58PYHaWw`, solo) · 2023-09-28 iPhone 15 Pro Review (`cBpGq-vDr2Y`, solo). youtube-index
footer 94→101; index.md 94→101.

**Attribution:** six are clean solo Marques-fronted (all persona/voice data). The **Dyson Zone**
video (`tFdnCzfJPJ0`) is the one collab/interview episode: **Doctor Mike (Mikhail Varshavski)**
appears as a guest medical expert — his medical case (N95 vs no-seal, Brownian motion at
0.3 vs 0.1 micron, mucous-membrane/vasoconstriction risk, CDC accident-vs-respiratory stats) is
**guest-attributed and quarantined** (page `attribution: solo-with-guest`), NOT eligible for
beliefs.md/voice.md. **Barbara Corcoran** is credited (context, not present) for the loss-leader
concept — attribute the concept to her, its application to Marques. Other creators cited as
context only (not co-hosts / not quarantined dialogue): Cleo Abram (XR-stage collab),
JerryRigEverything, Dave2D, Mr. Mobile (the "camera differences are taste now" line is explicitly
borrowed from Mr. Mobile → attribute to him, Marques's endorsement his).

**Sponsorships (disclosed, marked sponsor-context on pages, not clean verdicts):** Eight Sleep
segments in the Nothing Phone 2 Dope Tech, the Solar Roof review, and the iPhone 15 Pro review
(recurring code MKBHD); Anker in the iPhone 15 impressions; and the $40k iPhone video is
**self-sponsored** (own MKBHD wallet / shop.mkbhd.com) — a creator-business data point, not a
third-party ad.

**Caption-garble flags:** heavy numeric garbling in the collector-auction figures ($40k iPhone)
and especially the **Solar Roof specs/costs** (array kW, Powerwall kWh, total system cost,
payback years) — all flagged with `⚠️ CONTRADICTION`/approximation callouts on the pages;
transcribe as approximate, cite the app/story not the spoken figure.

**Rate limits:** **1 × 429** this iteration (`yt-ehv3zQAa9zM` AirTags — reverted to 429 despite
the task noting it "now fetches fine"; left open for retry). Other 7 fetched OK; 3-consecutive
safety rail not tripped. No yt-dlp errors.

Synthesis notes: nothing landmark inline-promoted (debt now **4 batches** since synthesis pass 1;
checkpoint at 10). Genuinely-new durable material flagged ★ for the next synthesis pass:
(1) the **"branding explains it"** lens + **loss-leader / press-generation** frame for gimmick
products (Dyson Zone) — reinforces the **two-in-one law** already logged; (2) the **Porsche 911
"iterative refinement compounds over time"** review philosophy and the **"more power = more
horsepower, only matters if you use it"** frame (iPhone 15 Pro) — signature tech-reviews persona
material; (3) the **"series zero / first-gen defined by early adopters + developers"** lens and
the **"compared to what?" Apple-pricing** frame (Vision Pro); (4) the **"two buckets"** Apple-
analysis lens — new features are either seen-elsewhere or ecosystem-locked (iPhone 15);
(5) the **three-levels-of-production** model (Dope Tech XR stage) → production-filmmaking;
(6) the **"was it worth it?" long-term-review format** + EV/sustainability "bleeding edge =
expensive & rapidly evolving" framing (Solar Roof) → ev-cars. Attribution reminder for the pass:
keep Doctor Mike's medical reasoning out of persona data.

## [2026-07-19] ingest | yt batch (@mkbhd, 7) — P1 solo 2023–24: Cybertruck / Smartphone Awards 2023 / S24 Ultra / Vision Pro / Disney HoloTile / iPhone 16 + Tim Cook interview

Stage B ingest, @mkbhd P1 oldest-first, batch of 8 fetched → 7 ingested to L2, 1 left open (429).
New source pages (all L2):
- 2023-12-01 **Cybertruck** first-drive / 2nd impressions (ev-cars) — steer-by-wire + rear-wheel
  steer standout; "best in-car software that's not CarPlay/Android Auto"; explicitly NOT a review;
  Ridge sponsored; **solo**.
- 2023-12-19 **Smartphone Awards 2023** (smartphones) — annual awards format; MVP Pixel 8, Camera
  King iPhone 15 Pro; plateau + small-phone-eulogy theses; **solo**.
- 2024-01-26 **Galaxy S24 Ultra review** (smartphones) — "why buy anything else"; utility-vs-
  aesthetics camera framework; Galaxy AI / Circle to Search; "they need each other" (Samsung↔Google
  ↔Apple); 7-yr updates; Ridge sponsored; **solo**.
- 2024-01-31 **Using Apple Vision Pro** (tech-reviews) — part 1 of 2; "it's a VR headset, spatial
  computing is semantics"; killer app = the ecosystem; Mac Virtual Display; Personas / uncanny
  valley; first-person darker-skin-tone external-eyes observation; **solo**.
- 2024-04-26 **Disney HoloTile** (consumer-tech-culture) — Dope Tech-style exclusive; VR
  locomotion / motion-sickness (eyes-vs-inner-ear) explanation; **Lanny Smoot = context entity**;
  **solo**.
- 2024-06-12 **Talking Tech and AI with Tim Cook** (tech-industry-commentary) — **interview,
  attribution-gated**: Tim Cook is the guest, all his statements **quarantined** and excluded from
  persona; only Marques's framing/questions/self-reference (his prior "Apple never says AI" piece;
  "phone vs eyes" attention theme; blind-ranking format) feed the persona.
- 2024-09-10 **iPhone 16/Pro impressions** (smartphones) — "**The Great Separation**" thesis
  (hardware bump vs AI-software shipping later); restates the **golden rule: never buy for a
  promised future update**; 60 Hz-on-a-flagship gripe; AirPods Max "fake upgrade"; Anker sponsored;
  **solo**.

**Attribution note:** one **interview** in the batch (Tim Cook, WWDC 2024) handled per SUBJECT.md
ensemble/guest rules — speaker labels are clear in the transcript, so attribution is
high-confidence; Cook quarantined, only Marques trains the persona. Context entities newly
referenced: **Tim Cook / Apple** (interview guest), **Lanny Smoot / Disney Imagineering**
(HoloTile inventor), plus creator cameos **iJustine + Brian Tong** (Vision Pro FaceTime demo) —
all context, none persona data. Ledger domains/notes set per video; youtube-index + index counts
bumped 101 → 108.

**Rate limits:** **1 × 429** this iteration (`yt-ehv3zQAa9zM` AirTags — 429'd again as flagged;
left open with retry note, matching the iPhone SE 2020 precedent so it doesn't block auto-select).
7/8 fetched OK; 3-consecutive safety rail not tripped. No yt-dlp errors.

Synthesis notes: nothing landmark inline-promoted (debt now **5 batches** since synthesis pass 1;
checkpoint at 10). Genuinely-new durable material flagged ★ for the next synthesis pass:
(1) **"The Great Separation"** (hardware vs AI-software decoupling) + the restated **golden rule —
never buy for a promised future software update** (iPhone 16) → beliefs/tech-reviews;
(2) the **utility-vs-aesthetics camera-review framework** and **"they need each other"**
(Samsung↔Google↔Apple) + **"best argument against a $1,300 phone is that it's a $1,300 phone"**
(S24 Ultra) → smartphones/tech-reviews;
(3) **"Vision Pro is a VR headset; spatial computing is semantics"**, **"killer app = the
ecosystem"**, and the **first-person darker-skin-tone external-eyes** observation (Vision Pro) →
tech-reviews/consumer-tech-culture;
(4) the **plateau + small-phone eulogy + "hard to buy a bad phone now"** theses and the
Camera-King-vs-blind-test divergence (Smartphone Awards 2023) → smartphones;
(5) the **VR locomotion / motion-sickness** (eyes-vs-vestibular) teaching frame (Disney HoloTile) →
consumer-tech-culture;
(6) **Tesla has the best in-car software (non-CarPlay/Android Auto)** + the **"impressions ≠
review"** discipline (Cybertruck) → ev-cars/tech-reviews.
Attribution reminder for the pass: keep **Tim Cook's** answers out of persona data (interview guest).
