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

## [2026-07-19] ingest | yt batch (@mkbhd, 5) — P1 solo: Smartphone Awards 2024 & 2025 / iPhone 17-Air / Dope Tech Revisited / Xiaomi SU7
Ingested 5 open P1 long-form @mkbhd rows to L2 (five `wiki/sources/` pages; index + youtube-index
bumped 108→113). Written sequentially by the coordinator (no sub-agents this run). All five are
**solo, Marques-fronted → persona/voice data**; no interview/collab/ensemble attribution needed.
Selection also auto-marked two 2008 golf P2 rows `no-captions` (yt-fjhmnWFsr3s, yt-PD5igzFB8iY) and
left one P1 open on a yt-dlp error (**yt-k_vD2S49INE "Retro Tech: Wearables"** — 1 error, not a rate-
limit streak). The 2020 iPhone SE / AirTags P1 rows were already excluded (prior 429s), untouched.
Pages: 2024-12-19 Smartphone Awards 2024 (10th; S24 Ultra PotY) · 2025-09-10 iPhone 17/Pro/Air
impressions · 2025-11-21 Dope Tech Revisited · 2025-12-05 Xiaomi SU7 "are we cooked?" · 2025-12-08
Smartphone Awards 2025 (iPhone 17 MVP + iPhone 16 Bust).
Synthesis notes: rich, mostly-new — all five flagged ★ L3-candidates. (1) **Smartphone Awards
philosophy**: MVP = "the story that represents the year," explicitly NOT the best-specs phone; the
recurring "phones are all big now / death of the small flagship" thesis (Note-4-vs-modern stat);
the **diminishing-returns value framework**; the "boring = elite" Scottie-Scheffler framing of the
S24 Ultra → smartphones/tech-reviews. (2) **2024→2025 arc to reconcile**: iPhone camera streak he
called "closer than ever" to being broken in 2024 IS broken in 2025 (Oppo Find X9 Pro); the base-
iPhone-should-be-complete critique finally resolved (iPhone 17 = both Most Improved AND MVP, while
stripped iPhone 16 = Bust). (3) **iPhone Air "red flags" + "subtract the emotions and it's the worst
one"** + the **"texts from friends / compress to one sentence"** explainer method + the MacBook-Air
first-gen-category-bet analogy → tech-reviews/voice. (4) **Production-craft confession**: MKBHD shot
manual-focus on RED (weak AF) + "the tool should enable the creative idea" + "Porsche 911 of X"
framework for iteratively-perfected products (Dope Tech) → production-filmmaking/beliefs. (5) **EV**:
the "are we cooked?" Chinese-EV thesis + "normal parts, elite integration" + "competition rising
raises the ceiling for all EVs" + "multiple personalities is the superpower of electric cars"
(Xiaomi SU7) → ev-cars. (6) **Industry read**: silicon-carbon "bimodal battery distribution"
(7,000-8,000 mAh haves vs Apple/Samsung 5,000-5,500 have-nots), 2025 as the battery-leap year.
Debt now 6 batches since synthesis pass 1 (checkpoint at 10). Next iteration: 1 P1 left on @mkbhd
(Retro Tech Wearables, retry the errored fetch); if it treats the main-channel P1 era as complete,
move to @WaveformClips P1 (×2) or @AutoFocus/@Waveform P2, else Stage S at the 10-batch checkpoint.

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — origin era: first video + earliest 2009 uploads

Stage B (P1-first) on @mkbhd, batch size 8. The driver's selection (priority asc, oldest-first)
pulled the 1 open P1 + the oldest P2 tail — i.e. the **origin era**: Marques's earliest transcribed
uploads (Jan 2009, age 15). Outcome: **4 ingested L2, 3 no-captions (auto-marked L1), 1 fetch-error
(left open)**. No rate-limiting (1 isolated yt-dlp error, not the 3-consecutive threshold; 0 HTTP 429s).

Ingested (→ `wiki/sources/`): 2009-01-01 **HP Pavilion dv7t Media Center Remote Overview** (opens
"welcome to my first video") · 2009-01-30 **HQ Tutorial: Firefox Preloader** · 2009-01-30 **HQ
Tutorial: Download Skype** · 2009-01-30 **MY Internet Speed!** (86 Mbps brag). All solo, fully
Marques-attributed (persona/voice data); no quarantine needed.

No-captions → L1 (no page): 2008-09-16 High fps LG Voyager footage · 2009-01-01 Fraps HD Test in
1080p · 2009-01-29 15 Year old Golf Swing Analysis. Fetch-error → left open: **Retro Tech: Wearables**
(`yt-k_vD2S49INE`, views=0, undated — possibly unavailable/private; noted for manual inspection).

**Attribution:** all 4 pages are solo MKBHD-fronted, no guests → clean persona/voice data.

**⚠️ Driver bug surfaced (not fixed this batch):** the landmark P1 **"The Worst Product I've Ever
Reviewed… For Now"** (Humane AI Pin, `yt-TitZV6k8zfA`, 2024-04-14) is silently excluded from every
batch — `ingest_batch.py`'s `FLAG_RE = re.compile(r"429|…")` matches the substring "429" inside its
notes field `views=9429879`, so a genuine landmark review is treated as rate-limited. It is the real
reason "@mkbhd P1" reads as ~drained. Fix: word-boundary the 429 pattern (`(?<!\d)429(?!\d)`) or
strip raw view counts from `notes`. Left for the user / next iteration to unstick.

Synthesis notes: **Origin/biography material (genuinely new).** (1) Self-described **"my first video"**
= the HP Pavilion dv7t Media Center remote overview (2009-01-01) — earliest *transcribed* upload (an
earlier 2008-09-16 LG Voyager clip exists but is no-captions), and the **review format + "leave
comments and subscribe" CTA are already present in video #1** → persona/biography.md + voice.md origin
section. (2) Earliest gear on record: **HP Pavilion dv7t laptop (3 GB RAM, ExpressCard slot)**, screen-
recorded with the **CamStudio lossless codec**, **RocketDock** launcher, **Windows Vista**, and an
owned-but-untested **Mac Pro** (2009-01-30) → production-filmmaking origin context. (3) Early instincts
visible young: a **head-to-head comparison** (Firefox-preloaded vs Safari) and **scope-splitting**
(download-tutorial now, how-to-use later). Flag `yt-9gk_rl3y_SU` as ★ L3-candidate for the next
synthesis (biography/voice). Also flagged above: the Humane AI Pin P1 is stuck behind a driver false-
positive and should be ingested once unstuck. Debt now 7 batches since synthesis pass 1 (checkpoint
at 10). Next iteration: continue @mkbhd P2 oldest-first (or @AutoFocus/@Waveform P2); unstick + ingest
the Humane AI Pin P1; Stage S when the 10-batch checkpoint or a channel/era boundary hits.

## [2026-07-19] ingest | yt batch (@mkbhd, 8) — Humane AI Pin P1 (unstuck) + Galaxy Fold + 2009 origin tutorials

Stage B (P1-first) on @mkbhd, batch size 8 — the first batch after **fixing the `FLAG_RE` driver bug**
flagged in the previous entry (view-count digits like `views=9429879` falsely matched the bare "429"
token). With the pattern word-boundaried (`(?<!\d)429(?!\d)`, commit `accc8f4`), the previously-hidden
landmark P1 became selectable. Driver selection (priority asc, oldest-first) pulled the **2 open P1 +
the oldest 6 P2**. Outcome: **8 ingested L2, 0 no-captions, 0 rate-limits, 0 errors** (all 8 captions
fetched cleanly — no yt-dlp failures, 0 HTTP 429s).

Ingested (→ `wiki/sources/`):
- **P1** 2024-04-14 **The Worst Product I've Ever Reviewed… For Now** (`yt-TitZV6k8zfA`, Humane AI Pin —
  the row that was stuck behind the FLAG_RE bug) ★
- **P1** 2019-04-16 **Samsung Galaxy Fold Unboxing: Magnets!** (`yt-x4yF3a3Zn4Y`) — retail unboxing,
  companion to the already-ingested 2019-04-18 "Broken Galaxy Folds: Explained!"
- **P2 origin cluster (2009-01-30, age 15):** HQ Tutorial: Windows 7 Calculator · HQ Tutorial: Safari
  for Windows · Quick Note on Speedfan · HQ Tutorial: Rocket Dock Application · Camstudio Clarity ·
  Tutorial: Camstudio HQ.

**Attribution:** all 8 pages are solo MKBHD-fronted — no guests, no interview/collab episodes in this
batch → clean persona/voice data, no per-line quarantine needed.

Synthesis notes: **Genuinely new.** (1) **Landmark review doctrine (Humane AI Pin, 2024-04-14)** — a
canonical statement of several recurring MKBHD frameworks worth promoting at the next synthesis:
**"smartphones are OP"** (any new personal-computing form factor is judged against what a phone already
does better/faster/easier); **"never buy a product based on the future promise of updates"**;
**"victim of its future ambition"** (deliberately refusing phone-pairing hamstrings the present
product — same critique he applies to Vision Pro); and his **respect-the-attempt** stance toward
first-gen hardware even when panning it. Note the exact, frequently-misquoted verdict: "the new worst
product I think I've ever reviewed, **in its current state**" (qualified, not absolute). → tech-reviews
+ tech-industry-commentary topics, persona/beliefs.md. (2) **Foldables first-gen risk** — the Galaxy
Fold unboxing ($1,980 "luxury device," Galaxy Buds bundled to commit to wireless, the magnet demo)
pairs with the existing Broken-Folds page to document the 2019 first-gen foldable launch. (3) **More
production-origin breadcrumbs (2009-01-30)** — the CamStudio pages document Marques's earliest
video-production toolchain (CamStudio + DivX 6.8.7, 30 fps, 720 HD @ 3,000 kbps, 640×360; "Windows
Movie Maker is not good") and an early quality-obsession; the Win7-calc page adds a dated biography
breadcrumb ("I use trigonometry, I'm in school right now"). Flag `yt-TitZV6k8zfA` as ★ L3-candidate.
Debt now **8 batches** since synthesis pass 1 (checkpoint at 10). Next iteration: continue @mkbhd P2
oldest-first (or @AutoFocus/@Waveform P2); **Stage S synthesis due after ~2 more batches** or at the
next channel/era boundary.

## [2026-07-19] ingest | yt batch (@AutoFocus, 8) — first @AutoFocus batch: 2026 EV reviews (Mercedes CLA, Subaru Uncharted, Chevy Bolt, Ferrari Luce, Nissan Leaf, Slate Truck, Porsche Macan) + April Fools Cozy Coupe

Stage B (P2). First ingest from the **@AutoFocus** car channel — pivoted here after the @mkbhd
main-channel P1 drained; @AutoFocus is Marques-fronted, so attribution is cleanest of the
non-@mkbhd channels. 8 videos, all L2, captions clean (0 no-captions, 0 429s). New `## @AutoFocus`
section added to youtube-index.md. Batch drained oldest-first from 2026-04-01 → 2026-07-13.

Videos: Little Tikes Cozy Coupe (yt-Gs5r8iGPjSg, April Fools comedy — voice only); Mercedes CLA 350
EV (yt-9s69aThM7rA); Subaru Uncharted (yt-4-eB-n5NYRs); Chevy Bolt (yt-bYw5GAzP2Ds, Chemical Guys
sponsor read); Ferrari Luce world-exclusive walkaround (yt-6Reu1WS3BhM); Nissan Leaf facelift
(yt-clsbuM6uf1A); Slate Truck first drive (yt-d0t7wpkFc6U); Porsche Macan Turbo EV (yt-FefIWhfl5Lg).

Attribution: 7 of 8 are Marques-solo (clean persona/voice data). **Porsche Macan (yt-FefIWhfl5Lg)
hands the entire driving section to co-host "Miles"** — quarantined on the page (`attribution:
co-host`); only Marques's static-review lines are persona data. "Miles" is an Auto Focus contributor
not yet in wiki/entities/ (flagged for synthesis: confirm name/spelling + consider a context page).
The Little Tikes video is an April Fools joke (kept for voice; no factual car claims). The
2026-06-26 @Waveform "Steam Machine" episode also mentions the Slate Truck but is not a duplicate of
the AutoFocus first-drive.

Synthesis notes: **Genuinely new (ev-cars is a newly-populated domain — first substantial EV-review
corpus).** (1) ★ **EV design thesis** (Nissan Leaf 2026-06-01 + Ferrari Luce 2026-05-25) — "EVs look
like blobs" because current battery energy density forces an obsessive low-drag/teardrop shape; when
battery tech improves "we can have design again." He extends it into a **critical position on the
Ferrari Luce**: a Ferrari shouldn't chase aero efficiency — "it should look like a Ferrari... now it
just looks like a Nissan Leaf." High-confidence, repeated → ev-cars topic + persona/beliefs.md.
(2) ★ **One-pedal-driving demand** — a recurring, near-universal review criterion: he dings Mercedes,
Nissan (the "e-Step" that isn't true one-pedal), and Porsche ("please, please give us the option")
for lacking/poor one-pedal driving. (3) ★ **"Affordable EV that doesn't suck" through-line** — Chevy
Bolt ("is it possible in 2026 to make an EV under 30 grand that doesn't suck? ... the answer is yes"),
Slate Truck modular "pay only for the bells and whistles you want" ("legitimately a brand new idea"),
Leaf "glow-up" — he's openly rooting for cheap EVs done right, vs. skepticism of the premium-badge
"tax" (Macan "worth 3 Model Ys?"). (4) **Rebadge/hybrid-company critique** — "Toyota doesn't like
making EVs; they love hybrids," applied to the Subaru Uncharted = rebadged Toyota bZ. (5) **Car-review
method** — consistent rubric (exterior → frunk/trunk → interior materials → screens/CarPlay → backseat
vs. his "6'3 driving position" → drive: suspension/quietness/range/charging/regen), the recurring
"real physical buttons / next-track on the wheel" demand, the "New Jersey potholes" soft-suspension
frame, and Auto Focus's shot-on-phone/Osmo production gimmick. (6) ★ **UI taste applied to cars**
(Ferrari Luce) — "everything you touch is metal, aluminum, glass, or leather," physical vent bezels +
cutout displays over real gauges = his "physical + digital done right" lens. Debt now **9 batches**
since synthesis pass 1 (checkpoint at 10). **Stage S synthesis is due next iteration** (10th batch, and
this is a natural channel-boundary start for @AutoFocus/ev-cars).

## [2026-07-19] lint | synthesis pass 2 — @mkbhd 2021→2025 P1 completion + origin-2009 + Humane AI Pin + @AutoFocus 2026 EV (batches 11–19, 59 new L2)

**Second Stage S / second synthesis pass.** Trigger: the @mkbhd main-channel P1 era completed and the
first @AutoFocus (ev-cars) batch landed — a channel/era boundary (the batch-19 log entry itself flagged
"Stage S synthesis is due next iteration"). Drained all **9 accumulated `Synthesis notes:` lines**
(batches 11–19). Done in one agent context, one file at a time (no sub-agents, per the run constraint).

**Topic hubs extended (7/7):**
- tech-reviews — the golden rule (never buy for a promised update), "The Great Separation," "smartphones
  are OP," "victim of its future ambition" + qualified "in its current state" verdict, "series zero"/
  "compared to what?", the "two buckets" Apple lens, "Porsche 911 of ___" iterative-refinement praise,
  the "was it worth it?" long-term format, diminishing-returns and utility-vs-aesthetics; a Humane AI Pin
  landmark box.
- smartphones — Smartphone Awards **2020–2025** slate added to the winner table; MVP-as-"story of the
  year" doctrine, the 2024→2025 iPhone-camera-streak-broken arc, high-refresh/incremental-craft, skin-tone
  criterion, "they need each other," bimodal battery distribution, canonical iPhone-line verdicts
  (with the iOS-7/4S misstatement flagged ⚠️ and NOT promoted).
- ev-cars — new "@AutoFocus era" section: EV-design-is-battery-constrained ("blobs"), one-pedal demand,
  affordable-EV-that-doesn't-suck, rebadge/hybrid critique, "multiple personalities," UI-taste-applied-to-
  cars, the @AutoFocus review rubric; plus Cybertruck "impressions ≠ review."
- production-filmmaking — three-levels-of-production, "the tool should enable the creative idea," and the
  documented **2009 origin toolchain** (CamStudio/DivX on an HP dv7t).
- creator-business — self-sponsorship ($40k iPhone), Barbara-Corcoran loss-leader credit, and the
  2021-03-17 Auto Focus pre-announcement node.
- tech-industry-commentary — "this will be copied" (Dynamic Island), "form over function," "two-in-one is
  always worse at one thing," and the solo-hardened AI-hardware-vs-phone judgment.
- consumer-tech-culture — Retro Tech S2 tech-optimist frame, "straight line" withered-tech-to-today, and
  the VR motion-sickness teaching explainer.

**Persona refreshed + recompiled to v2:**
- `beliefs.md` — 10 new frameworks + 4 values + 4 opinions + updated predictions; two @Waveform
  attribution-to-confirm items (paperware, AI-hardware) marked **solo-hardened** by main-channel sources.
- `voice.md` — new catchphrases ("glass is glass," "in its current state," "are we cooked?", "Porsche 911
  of ___," "compared to what?"), car-review cadence, and 6 new verbatim quotes (exact wording verified
  against source pages).
- `biography.md` — new "origin-2009 + 2021–2026" anchors section (first video, school breadcrumb, Auto
  Focus pre-announcement, Humane, Tim Cook, first @AutoFocus corpus, 6'3").
- `appearance.md` — seeded with the one caption-supplied fact (~6'3" build); rest still needs watched video.
- `system-prompt.md` — recompiled **v1 → v2**, `compiled_from_sources` 74 → 133; coverage now 2009→2025
  main channel + 2026 @AutoFocus; changelog inline.

**Attribution discipline:** interview/co-host material stayed quarantined and OUT of persona — Tim Cook
(interview), Doctor Mike (Dyson Zone medical expert), @AutoFocus co-host "Miles" (Macan driving section),
and Retro Tech guest historians. Only Marques-attributed framing/voice was promoted. "Miles" flagged as a
candidate `wiki/entities/` context page (name/spelling unconfirmed).

**Bookkeeping:** advanced the high-water mark to batches 1–19 (133 L2) and moved the checkpoint to Done
(tagged v2) in `pipeline/synthesis-state.md`. No new topic pages created (hubs extended in place), so
`index.md` unchanged. No ledger changes (synthesis promotes content, doesn't move L2→L3 rows). No rate
limits, no yt-dlp calls, no fabrication.

Synthesis notes: none — debt fully drained (9/9 → 0). Next ingest batch starts a fresh counter; resume
Stage B next iteration (@AutoFocus P2 remainder, or @mkbhd P2 long tail / @Waveform).

## [2026-07-20] ingest | yt batch (@AutoFocus, 7) — 2026 Q1 P2 EV/performance reviews: Ioniq 5 XRT / Rivian R2 / EV-in-winter / Corvette ZR1 / Lamborghini Temerario / Polestar 4 / Audi RS e-tron GT
Stage B, P2, @AutoFocus (cleanest-attribution Marques-fronted channel; continued the first @AutoFocus
batch backward into 2026 Q1). Prepared 8 oldest-first P2 rows; captions fetched cleanly for all 8 (0×429,
0 no-captions). Ingested **7 to L2**, **skipped 1**.

**Ingested (L2):**
- 2026-01-29 Hyundai Ioniq 5 XRT — solo Marques. "Specialty EVs" framing; NACS-at-Supercharger slower than
  expected (~50–60 kW).
- 2026-02-10 Rivian R2 first drive — solo Marques. Half-price R1S via "simplify by fewer parts"; ~5 mi/kWh;
  haptic dials; "their Model Y."
- 2026-02-13 "Electric Cars Suck in the Winter" explainer — solo Marques. Prefers EV in winter; one downside
  (road trips), several upsides; home charging neutralizes daily range hit.
- 2026-02-19 Corvette C8 ZR1 ("Model S Plaid Walked…") — **co-host**: Marques intro/interior/Plaid tech-angle
  comparison; **Miles driving segment quarantined**.
- 2026-02-24 Lamborghini Temerario — **co-host**: Marques aesthetics/interior/hybrid-tech + close;
  **Miles dynamics segment quarantined**.
- 2026-03-03 Polestar 4 — solo Marques. "What's stopping me from recommending it?" → no rear window +
  sub-200mi winter range; "best software that's not CarPlay."
- 2026-03-09 Audi RS e-tron GT — **co-host**: Marques intro/tech/interior + depreciation logic;
  **Miles early interjection + driving segment quarantined**.

**Skipped:**
- 2026-03-27 Porsche Cayenne Electric Turbo (yt-We-lvUeRGb0) — **co-host-only: Miles solo hosts, Marques
  absent** ("while he's doing that, I thought it'd be good to take another look…"). No subject-attributable
  content → marked `skipped` per SUBJECT.md ensemble rules; no source page.

**Attribution discipline:** only Marques-attributed lines fed the pages; all co-host "Miles" driving
segments quarantined in a dedicated section on each co-host page (`attribution: co-host`), following the
Porsche Macan precedent. Miles now solo-hosts at least one full @AutoFocus upload (Cayenne) — reinforces the
open candidate for a `wiki/entities/miles` context page (name/spelling still unconfirmed).

**Bookkeeping:** 7 ledger rows → L2, 1 → skipped; 7 rows inserted into `wiki/sources/youtube-index.md`
@AutoFocus section (date order, ahead of 2026-04-01); footer 133 → 140; `index.md` count 133 → 140. Deleted
staging none (driver-managed). No rate limits, no fabrication, all English.

Synthesis notes: fresh debt counter starts (1 batch). Genuinely-new, worth promoting at next checkpoint —
(1) the **"specialty EVs" market-maturation** observation (2026); (2) **NACS isn't always faster** real-world
finding; (3) the **winter-EV ownership framework** (road-trip downside vs. preheat-anywhere / superior
traction / no-warm-up upsides; home charging neutralizes daily loss) — strong `wiki/topics/ev-cars` +
`persona/beliefs.md` candidate; (4) the **"performance bargain / democratized daily-usable 1,000-hp"** lens
(Model S Plaid ↔ Corvette ZR1); (5) the signature **"what's stopping me from recommending it?"** review
framework and the running **"best software that's not CarPlay"** ranking (Tesla/Rivian/Polestar);
(6) **depreciation-aware buying logic** on expensive performance EVs (buy the better platform-twin / used).

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: CCleaner / HD-upload workflow / Aerosnap / first hardware unboxing (NZXT Cryo LX) / Firefox New-Tab / PowerPoint avatar / Vista logon / Microsoft Mouse 6000
**Stage B, P2 — cleanest-attribution channel (@mkbhd, Marques-solo, no co-hosts to quarantine).**
Ingested 8 origin-era @mkbhd videos (2009-01-30 → 2009-02-01), all solo screencasts/reviews by a
15-year-old Marques → `attribution: solo`, all content is persona/voice data (no per-line quarantine).
Videos: CCleaner software walkthrough (`oP41yum-wFg`); **How to Upload HD Youtube Videos** (`4vwd_pQHUBE`,
★); Aerosnap-for-Vista tutorial (`reI8CsNd88Y`); **Unboxed: NZXT Cryo LX** — self-declared *first hardware
unboxing* (`SWSqBFGT50A`, ★); Firefox New-Tab-button tutorial (`J_RVM09Lefg`); PowerPoint YouTube-avatar
tutorial (`zArasubfsPI`); Vista logon-screen tutorial (`DMpoZNJmdpE`); **HD Review: Microsoft Wireless 6000
Mouse** (`RTxrS1lLwjY`, ★, ~304K views).

**Bookkeeping:** 8 ledger rows → L2; 8 rows inserted into `wiki/sources/youtube-index.md` @mkbhd section
(date order, after 2009-01-30 block, ahead of 2013-10-12); footer 140 → 148; `index.md` count 140 → 148.
No staging to delete. **Rate limits: 0 (8 ok, 0 retry/error — no 429s).** No fabrication, all English.

Synthesis notes: debt counter now 2 batches (checkpoint at 10). Genuinely-new origin material worth
promoting at next checkpoint — (1) **"How to Upload HD Youtube Videos" is the earliest explicit statement
of the HD/production-quality obsession that names the channel** (CamStudio→Movie Maker→720p pipeline) —
strong `production-filmmaking`/`creator-business` biography anchor; (2) the **NZXT Cryo LX = self-declared
first hardware unboxing** and **Microsoft Mouse 6000 = early two-part hardware+software review structure**
— origin markers for the unboxing and review-methodology formats (`tech-reviews`); (3) **branding/bio
breadcrumbs**: the **"MKB" initials** (Marques Keith Brownlee) placed on his first PowerPoint avatar, and
the self-reported detail that his prior avatar was "a picture of me playing golf"; (4) recurring early
tells already present at age 15 — side-by-side comparison instinct, lived-with testing, and "download
drivers from the manufacturer's website" practical-tip habit. All L2-only here; not inlined.

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: CPU-Intensive demo / Opera 10 Alpha first-look / Extended Task Manager / Firefox add-ons (redo) / Fraps / Firefox theme / Thunderbird add-ons / Justhearit

Stage B (P2) on @mkbhd — @mkbhd P1 fully drained, so the driver selected the oldest open
P2 rows: the next block of **2009-02-01/02 origin-era freeware/how-to screencasts** (age-15
Marques, all **solo**). Batch size 8. All 8 had English captions; 0 no-captions, 0 skipped,
0 duplicates. **Rate limits: 0 (8 ok, 0 retry/error — no 429s).**

Videos (→ `wiki/sources/`): 2009-02-01 HD Example: CPU Intensive (yt-ZZnVdFjig88) ·
HD first look: Opera 10 Alpha (yt-r8b7qMeUHsg) · HD Tutorial: Extended Task Manager
(yt-s9lU1eAXVn4) · HD Tutorial: Firefox Addons / redo (yt-NuxUMQ5CrX0) · HD Tutorial: Fraps
(yt-XCuIjLI2VMg) · Tutorial: Firefox Addons / theme (yt-TVMu1S8jY2A) · HD Tutorial:
Thunderbird Addons (yt-QYRvQh043GQ) · 2009-02-02 HD Tutorial: Justhearit! (yt-Ec7_yCwXmWY).

**Attribution:** all 8 are solo MKBHD-fronted screencasts — no co-hosts/guests, no
quarantine needed (this is the cleanest-attribution corpus, hence preferred over the
co-hosted side channels @Waveform/@TheStudio and the dedup-tier @WaveformClips this round).

**Bookkeeping:** 8 ledger rows → L2; 8 rows inserted into `wiki/sources/youtube-index.md`
@mkbhd section (date order, after the 2009-02-01 Mouse-6000 row, ahead of 2013-10-12);
footer 148 → 156; `index.md` count 148 → 156. No staging to delete. No fabrication, all English.

Synthesis notes: debt counter now 3 batches (checkpoint at 10). Genuinely-new, all L2-only
(not inlined): (1) **early explicit review intent** — in the Extended Task Manager video he
says "I'll start reviewing freeware," one of the earliest on-record statements of the
reviewing instinct (`tech-reviews`/`creator-business` origin marker); (2) **reshoot /
do-it-until-it's-right perfectionism** on record — the Firefox add-ons "redo" opens by
scrapping a bad take; (3) **audience-request content loop** at age 15 — invites email/PM
tutorial requests and promises HD tutorials back; (4) **early 1080p experimentation** (Fraps
video references a prior "1080p test" upload — extends the HD-obsession thread from the
"How to Upload HD Youtube Videos" origin video); (5) ⚠️ **candid software-piracy admission**
(torrenting the full Fraps) — historical/context only, note verbatim, do not over-weight;
(6) **hardware/gaming background** breadcrumbs — Nvidia GeForce 9200M (512 MB) laptop GPU,
Fraps game-capture use; (7) confirms the "Marques" Windows user account ("Marcus downloads")
seen in the Thunderbird video. Marginal-value tutorials (Firefox theme, Thunderbird add-ons)
carry little persona signal.

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: browser-tuning cluster (Firefox/IE/Safari-WebKit) + wallpapers / DreamScene / webcam-mic boost / Start-menu shutdown / screencast-zoom

Stage B (P2, @mkbhd solo — cleanest attribution; main P1 drained). Eight 2009-02-02→04
origin-era **HD Tutorial** screencasts, all solo Marques (no co-hosts/guests). All 8 had
captions; 0 yt-dlp failures / 0 429s. Wrote 8 `wiki/sources/` L2 pages.

Videos: wallpapers via Firefox set-as-background (`ySgD6j5yj3w`); Make IE7 Faster —
regedit/CCleaner (`wuYhGKkTTx8`); Make Firefox Faster — about:config pipelining
(`V3MQgxfv0h0`); Non-Ultimate DreamScene on Vista (`q90rFEbiLI8`); Boost built-in webcam
mic +10 dB (`sTt-9R6FQ6E`); Start-menu Shutdown button (`PssBv2rusgw`); Screencasting
zoom/magnify (`8OUGVgQLxNU`); Safari & WebKit plugins on Windows (`7g2q___Kiag`).

**Attribution:** all solo (`attribution: solo`) — MKBHD-fronted personal screencasts, all
quotes are persona/voice data. No co-hosted material this round (the ensemble channels
@Waveform/@TheStudio and dedup-tier @WaveformClips were not touched).

**Bookkeeping:** 8 ledger rows → L2; 8 rows inserted into `wiki/sources/youtube-index.md`
@mkbhd section (date order, after the 2009-02-02 Justhearit row); footer 156 → 164;
`index.md` count 156 → 164. No staging to delete. No fabrication, all English.

Synthesis notes: debt counter now 4 batches (checkpoint at 10). Genuinely-new, all L2-only
(not inlined): (1) ★ **gear-origin evidence** — states on record he has **no external mic**
and records with the **built-in webcam mic** (+10 dB boost); strongest primary source yet
for the `production-filmmaking` "started with nothing" origin narrative; (2) ★ **early
screencasting-craft** — deliberately zooms/magnifies so viewers can follow his clicks,
early evidence of viewer-legibility thinking; (3) ⚠️ **dated 2009 browser preference** —
was "using Safari primarily" and "slowly moving to Firefox" (Feb 2009); do not present as
current; part of a three-browser Feb-2009 cluster (IE/Firefox/Safari+WebKit); (4) **early
comparative-review instinct** — closes the IE tutorial by conceding IE "is not the fastest
web browser" and demoing Safari faster (proto tech-review); (5) **audience-engagement tell
repeats** — again invites viewers to send tutorial requests. Both ★ items flagged as
L3-candidates for the next synthesis pass; do not inline-promote.

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: Vista tweak cluster (UAC / virtual-memory / menu-delay / boot-speed / ViStart / volume-mixer) + Safari 4 WebKit Acid3 benchmark

Stage B (P2, @mkbhd solo — cleanest attribution; main P1 drained). Eight 2009-02-04→05
origin-era **HD Tutorial** screencasts, all solo Marques (no co-hosts/guests). Seven had
captions and were ingested; **1 no-captions** (`gU9kqC8rEcM` "HD Benchmark: Safari Webkit",
auto-marked L1 `notes: no-captions` by the driver — never Whispered). 0 yt-dlp failures /
**0 429s**. Wrote 7 `wiki/sources/` L2 pages.

Videos: Disable UAC — advanced-users-only caveat (`1g1aQTEocX0`); Virtual Memory — 1.5×
RAM rule, his 2009 rig = 4 GB RAM + 7200 RPM HDD (`q0aKUO9xmds`); Eliminate Menu Show
Delay — regedit MenuShowDelay (`khEaSeMShk8`); Boot Faster — msconfig, keeps GUI boot over
faster No-GUI boot (`OBNkCLRGx2k`); Safari 4 WebKit — Acid3 75 vs 100 benchmark argument
(`NrOWLTqRLc8`); ViStart — Vista Start menu on XP freeware (`ADK6fdkWiBY`); per-app Volume
Mixer, recorded while multitasking uploads (`SkXXq2cOAso`).

**Attribution:** all solo (`attribution: solo`) — MKBHD-fronted personal screencasts, all
quotes are persona/voice data. No co-hosted material this round (ensemble channels
@Waveform/@TheStudio and dedup-tier @WaveformClips were not touched; the 2 open @WaveformClips
P1 rows were deliberately left for an attribution-gated pass, not this solo batch).

**Bookkeeping:** 7 ledger rows → L2 (+1 → L1 no-captions); 7 rows inserted into
`wiki/sources/youtube-index.md` @mkbhd section (date order, after the 2009-02-04 Safari
Addons row); footer 164 → 171; `index.md` count 164 → 171. No staging to delete. No
fabrication, all English.

Synthesis notes: debt counter now 5 batches (checkpoint at 10). Genuinely-new, all L2-only
(not inlined): (1) ★ **early benchmark-driven review instinct** — the Safari 4 WebKit video
leans on the standardized **Acid3 test (75/100 stock vs 100/100 WebKit nightly)** to make a
comparative claim; strongest 2009 precursor yet to his later spec/benchmark-led review
methodology (`tech-reviews`); (2) ★ **aesthetics-over-raw-numbers value tell** — in the
boot-speed video he keeps the slower GUI boot because he "actually like[s] the GUI boot,"
choosing experience/polish over the faster No-GUI number; early experience-vs-spec value;
(3) **measured-advice pattern** — recurring "set it low but not to zero" caution and an
explicit "advanced users only" caveat on the UAC tweak, prefiguring his duty-of-care tone;
(4) **creator/audience-relationship origins repeat** — "the features that i use in my
videos" (ViStart) + "send me a message and i'll make it" (Volume Mixer) confirm the early
audience-request loop; (5) **gear-origin datapoint** — 2009 rig on record: 4 GB RAM, 7200
RPM HDD. Both ★ items flagged as L3-candidates for the next synthesis pass; do not
inline-promote.

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: Camtasia/CamStudio production-tooling cluster (Sidebar Gadgets / RocketDock icons / CamStudio hotkeys / Thunderbird RSS / Camtasia PowerPoint / first HD Test / OS X cursors request / command-prompt customize)

Stage B P2 on @mkbhd (Marques-solo, cleanest attribution). 8 videos ingested → L2, all
`attribution: solo` (single-speaker origin screencasts, age 15; no co-hosts/guests — no
quarantine needed). Domains: consumer-tech-culture across all; production-filmmaking on
the three Camtasia/CamStudio tooling videos. 8 ok, 0 no-captions, 0 skipped, 0 dup, 0 429.

Synthesis notes: two ★ L3-candidates worth the next pass — (1) **first-HD-test milestone**
(`fa1Lr-W2aBU`, "HD Test 1"): earliest documented pursuit of upload/production quality —
"i'll upload it and see if i get that watching hd link that we all dream of" — a genuine
origin-of-the-craft moment for production-filmmaking/persona; (2) **earliest red-on-black
aesthetic** (`E63fdjyck2k`, command-prompt): sets CMD + WebKit to red text on black for
"very sharp contrast" — a *candidate* (not asserted) seed of the later crimson-red brand;
flag the connection, do not claim causation. Minor recurring threads (not new): the
audience-request content loop repeats (CamStudio-hotkeys editing-efficiency rationale;
OS X cursors is a direct viewer-fix follow-up; "PM me for a tutorial" across the batch),
and a self-description datapoint — Marques frames his early output as "i do a lot of
software reviews" (Thunderbird RSS). Both ★ items flagged as L3-candidates for the next
synthesis pass; do not inline-promote.

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: macOS-in-Windows cluster (RocketDock OS X theme / Firefox Mac theme / OS X cursors) + offline Gmail (Google Gears) / Vista Explorer Alt-menus / Vista Start-menu customization / Firefox 'Superbar' / speedtest.net
8 videos ingested L2 (@mkbhd solo, 2009-02-08/09), all clean single-speaker attribution, 0 rate-limits, 0 no-captions. Stage B, P2, oldest-first — continues the 2009 origin-era software-tutorial drain.
Synthesis notes: one coherent NEW thread worth the next pass — a **2009 macOS-aesthetic-in-Windows cluster**: within days, 15-year-old Marques imports the Mac OS X look onto his Windows Vista machine three ways — a RocketDock OS X "Leopard" dock skin (`uGL9arjQRl0`), a Firefox Mac OS X theme (`MqudmZQVWyo`), and OS X mouse cursors he adopts "as my default from now on" (`1VRajWZr-PE`). Read together this is early, documented Apple-aesthetic affinity years before the reviewer career — flag as a *candidate* character/aesthetic datapoint for persona (do NOT assert it caused anything; no crimson-red link here — that's the separate `E63fdjyck2k` red-on-black thread). Second ★ signal: earliest explicit **"review"** framing — in the Firefox Superbar video (`S1ThX4gDPrQ`) he announces "Google Chrome which I'll be doing a review on shortly," an origin datapoint for the review format. Minor recurring (not new): audience-request loop again ("PM me for a tutorial"; OS X cursors is a viewer request); on-camera test-don't-assert habit (Alt-key trick fails in Word 2007, he shows it live); early benchmark instinct (speedtest ~86/2.3 Mbps personal best). ⚠️ Possible near-duplicate to reconcile in synthesis: this batch's `1VRajWZr-PE` "Get OS X Cursors in Windows" vs. the already-ingested `DmqmZ_ORPbc` "Get OS X Cursors in Windows (Request)" — distinct video IDs, likely a re-upload/companion; verify and dedup at synthesis. All ★/ threads flagged as L3-candidates; do not inline-promote.

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: Aero Shake (Vista/XP) / SRWare Iron first-look / Vista screenshots (Snipping Tool) / CamStudio zoom / Tweak Safari for speed / classic Vista Start menu / Compatibility Mode / Sage offline dictionary-thesaurus

8 L2 pages written, all @mkbhd solo (age-15 Marques screencasts), attribution: solo — no co-hosts/guests. Batch 8/10 since last synthesis (checkpoint at 10). yt-dlp: 8/8 captions OK, 0×429.

Synthesis notes: SRWare Iron first-look (yt-oNMFjL1M1rA) is a ★L3-candidate — clearest early evidence of MKBHD **review methodology**: side-by-side **benchmarking** (Acid3) + **resource/RAM comparison** in Task Manager across browsers, a hedged verdict, and an explicit **audience-request→review** loop (video made because a commenter asked). Two more minor ★ signals reinforce a nascent tiered-review instinct: CamStudio-zoom (yt-lX9NdNvq78Y, production-tooling to optimize his own screencasts) and the Sage dictionary (yt-tu6vXjxtfR8) where he calls it a "limited software review" and promises a "much more in-depth software review" later. Self-referential series-building continues (Tweak-Safari cites his own CCleaner + Develop-menu videos). No new bio facts, no contradictions.

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: CamStudio review / iTunes 8 Plus / free YouTube layouts / Battery Saver #1 (defrag) / Safari autofill / internet-speed benchmark / Google Earth 5.0

7 L2 pages written (8 selected; yt-3Cuaj8FKWfQ "HD & Zoom/Pan Test - Camtasia Studio 6" had no captions → auto-marked L1, skipped). All @mkbhd solo (age-15 Marques screencasts + one webcam video), attribution: solo — no co-hosts/guests. Batch 9/10 since last synthesis (checkpoint at 10 → Stage S next iteration). yt-dlp: 7/7 captions OK, 0×429.

Synthesis notes: two ★L3-candidate signals worth promoting at the next synthesis. (1) **CamStudio review** (yt-PkRXVGJ0ods) is a primary-source record of MKBHD's **actual origin-era production stack** — CamStudio + DivX 6.8.5 at a 720p profile / quality 100, recording 640×360 with auto-pan — plus an explicit self-referential "review of the tool I'm using right now" transparency instinct; feeds production-filmmaking. (2) **Internet-speed benchmark** (yt-4FlLW_BA__M) shows the early **measure-it / benchmarking reflex** that prefigures his review methodology, and the NJ ISP + NJ (Fortress ITX) test server **corroborate the New Jersey base** (consistent with the Maplewood, NJ biography). Minor: **Battery Saver #1** (yt-5TSxRdgVnVs) is among the earliest **on-camera (webcam, not screencast) appearances** and an early numbered-series-format instinct — but its defrag-saves-battery advice is dated 2009 guidance, not durable belief (flag as historical). **Free YouTube layouts** (yt-jxSkySN3kks) is the earliest evidence of MKBHD branding/customizing his own channel (creator-business seed). No new bio facts beyond NJ corroboration; no contradictions.

## [2026-07-20] lint | synthesis pass 3 — @mkbhd Feb-2009 origin/production-methodology + @AutoFocus 2026 Q1 EV (batches 20–28, 69 new L2)

Stage S (3rd synthesis checkpoint). Drained the **9 accumulated `Synthesis notes:` lines** since pass 2
(debt counter 9/10 — judged the origin-2009 + @AutoFocus-Q1 debt a coherent, ripe synthesis unit rather
than wait one more batch; persona v2 was compiled from 133 while L2 had reached 202). One writer, one file
at a time; every promotion dated + cited to its `wiki/sources/` page; candidate/causal claims flagged, pure
repeats dropped. Only Marques-attributed material fed persona (co-host "Miles" @AutoFocus driving segments
stayed quarantined at source).

**Topic hubs promoted (L3):**
- **production-filmmaking** — origin toolchain deepened: the CamStudio + DivX 6.8.5 720p/quality-100 640×360
  stack (`PkRXVGJ0ods`), the first "HD Test" milestone (`fa1Lr-W2aBU`) + the HD-upload origin (`4vwd_pQHUBE`),
  the "started with nothing" gear origin (built-in webcam mic, no external mic; `sTt-9R6FQ6E`), and
  viewer-legibility zoom/magnify screencast craft (`8OUGVgQLxNU`).
- **tech-reviews** — new "Origin of the review methodology (Feb 2009)" section: SRWare Iron Acid3 + Task-Manager
  RAM comparison + hedged verdict + request→review loop (`oNMFjL1M1rA`), Safari-4 WebKit Acid3 75-vs-100
  (`NrOWLTqRLc8`), earliest explicit "review" framings (`s9lU1eAXVn4`, `S1ThX4gDPrQ`), first hardware unboxing
  (NZXT Cryo LX, `SWSqBFGT50A`), Microsoft Mouse 6000 two-part review (`RTxrS1lLwjY`), experience-over-benchmark
  GUI-boot choice (`OBNkCLRGx2k`).
- **creator-business** — origin nodes: first channel branding (`jxSkySN3kks`), "MKB"-initials avatar + prior
  golf avatar (`zArasubfsPI`), day-one audience-request content loop.
- **consumer-tech-culture** — candidate aesthetic seeds (flagged, NOT asserted causal): red-on-black "very sharp
  contrast" (`E63fdjyck2k`) and the macOS-in-Windows Apple-aesthetic cluster (`uGL9arjQRl0`/`MqudmZQVWyo`/`1VRajWZr-PE`).
- **ev-cars** — 2026 Q1 @AutoFocus positions: "what's stopping me from recommending it?" + "best software that's
  not CarPlay" (`i4eCZ6dLVrg`), winter-EV ownership framework (`cAmEAgNc0eY`), "specialty EVs" maturation +
  "NACS isn't always faster" (`46tvrNZFxjQ`), democratized-performance / "performance bargain" (`1q-hpaepgk0`),
  "simplify by fewer parts" (`EfReqcUJfBU`), depreciation-aware buying (`fOwC95ZXh08`).

**Persona:** `beliefs.md` (+origin values: experience-over-benchmark, native benchmark-led method, reshoot
perfectionism, duty-of-care advice; +EV frameworks), `voice.md` (+origin & EV catchphrases and verbatim:
"watching-HD link we all dream of", "I'll start reviewing freeware", "what's stopping me from recommending it?"),
`biography.md` (origin-2009 deepening + 2026 Q1 anchors), `appearance.md` (candidate brand-aesthetic origins).
Recompiled **`persona/system-prompt.md` v2 → v3** (compiled_from_sources 133 → 202).

**Bookkeeping:** advanced the high-water mark in `pipeline/synthesis-state.md` (through batches 1–28 / L2=202)
and logged the pass-3 Done checkpoint; refreshed `index.md` (persona lines + system-prompt v3 + pass-3 note).
No new pages created (all promotions extended existing hubs/persona). No rate limits, no fabrication, all English.
Debt counter resets to 0 (next checkpoint at the next channel/era boundary or ~10 more batches).

Synthesis notes: none — debt fully drained (9/9 → 0). Resume Stage B next iteration (@mkbhd 2009→2010 origin
P2 long tail, or @AutoFocus P2 remainder / @Waveform attribution-gated).

## [2026-07-20] ingest | yt batch (@mkbhd, 8) — 2009 origin P2: Windows-7 first-look/$50-upgrade opinion + WMP-11-in-XP / Vista AutoPlay / battery-saver #2-#3 (Aero, external-devices) / Animoto YouTube-intro pipeline / eliminate-background-tasks

Stage B (P2) on @mkbhd — cleanest-attribution channel (Marques solo, age 15, Feb 2009; no co-hosts in
this era, so no quarantine needed). Batch of 8 selected oldest-first from the 2009 origin era.
7 → L2, 1 skipped. 0 no-captions, 0 duplicates, no yt-dlp rate-limiting (0×429).

L2 pages (→ `wiki/sources/`): 2009-02-13 Could Windows 7 Be a $50 Upgrade? (first Windows 7 video —
opinion, CNET-sourced rumor) · 2009-02-13 WMP 11 in Windows XP · 2009-02-13 Customizing Vista AutoPlay ·
2009-02-13 Battery Saver #2 Disable Aero · 2009-02-13 Battery Saver #3 External Devices · 2009-02-15
Create A YouTube Intro Video (Animoto→Movie Maker) · 2009-02-15 Eliminate Background Tasks.
Skipped: 2009-02-14 "My new Official Intro Video" (yt-f4B3FMSFqpE) — music-only intro animation, no
spoken content; its creation is documented in the 2009-02-15 Animoto intro tutorial.

Attribution: all 7 L2 pages `attribution: solo` — MKBHD-fronted, every quote is persona/voice data.
Battery-saver #2/#3 join the series (part #1 = 2009-02-12 Defragmenting).

Synthesis notes: (1) ★ First "is it worth it?" value judgment in the corpus — the Windows 7 video weighs
price vs. worth ("wasn't worth as much money as you may have spent") and cites CNET for a rumor rather
than asserting it: origin seed of the review/"worth it" instinct + source-citing discipline. (2) ★ Documented
origin-era production pipeline: Animoto slideshow → export to YouTube → re-download → trim Animoto end-card
in Windows Movie Maker → prepend as HD intro; plus early copyright caution (used royalty-free music
deliberately) and request-driven content model. (3) Self-flagged in-video contradiction in Battery Saver #3
(future USB-cooler rec) — reconcile when that video is ingested. (4) Bio/rig datapoints: owned an LG Voyager
(VX10000); origin rig = 17" laptop, Nvidia GeForce, 512MB dedicated VRAM. (5) Caption garble noted: Animoto
title-card "Marquez Brownley" = misspelling of Marques Brownlee, not an alt spelling. Promote at next
synthesis checkpoint (creator-business + tech-reviews origin history).
