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
