# Synthesis state

_Tracks the synthesis **high-water mark** so the synthesis loop never misses material and never
re-does work. Companion to the ingest ledger (`ledger.csv`). The detailed debt lives in `log.md`
as `Synthesis notes:` lines (every ingest batch appends one). See `tools/SYNTHESIS.md` for the loop
and `tools/synthesis_batch.py` for the driver._

## High-water mark
Synthesized through: **nine real ingest batches since pass 9 (643 L2 sources)** — passes 1–8 through
L2=500, pass 9 through L2=571 (full 2012 origin year), PLUS **pass 10's nine @mkbhd batches (2026-07-23)
covering the late-2012 Nexus season + the full 2013 origin year Nov 2012→Aug 2013 (L2 571→643)**.
Covers every `wiki/sources/` page that was L2 as of 2026-07-23 at the 643-source mark.

## Pending checkpoints
_(oldest first; the synthesis loop drains these top-down)_

_None currently — **synthesis pass 10 (2026-07-23)** drained the nine-batch debt accumulated since pass 9
(571→643 L2), covering Nov 2012 → Aug 2013 (the late-2012 Nexus season + the full 2013 origin year).
Promotions: `persona/beliefs.md` (a "2013 origin-era doctrines" subsection — geeks-vs-consumers,
value-via-software, optics-over-megapixels canonical, Beats-EQ consumer-education, price-must-match-value,
copying-goes-both-ways, one-critical-flaw verdict, buy-by-your-values, upgradeability-sharpened,
rolling-release, anti-entitlement, Halo-product, 4K viewing-distance quantified, perspective-disclosure,
Oppo long-arc origin; + a 2013 predictions ledger — Chromebook-Android-apps ✅, 1080p-iPhone ✅, GS4-1080p
✅, 4K-diffusion ≈, dream-Chromebook resolved), `persona/biography.md` (a "Nov 2012–Aug 2013" section —
the Five-Facts self-disclosure incl. NJ Hammerheads/6'3"/house-music/anti-desktop origin, first CES 2013,
the definitive early-2013 workstation + desk, the Canon 5D Mark III, sophomore→junior, the no-daily-driver
two-phone-line reviewer setup, 4th birth-year corroboration), `persona/voice.md` (2013 register —
"Stormtrooper", "Legos for adults", "stay geeky", "Magic Mouse — just no", "OCD like me"),
`persona/appearance.md` (the "inverted Stormtrooper" earliest matched black-and-white studio aesthetic),
`wiki/topics/tech-reviews` (the 2013 verdict-frameworks + hands-on-evidence section), and
`wiki/topics/tech-industry-commentary` (the incentive lens sharpens across 2013 — geeks-vs-consumers,
value-via-software, rolling-release, segmentation/cannibalization, anti-entitlement, consumer-education,
even-handedness, Oppo hardened). `persona/system-prompt.md` recompiled **v9→v10** (571→643 sources). Next
checkpoint at ~10 more ingest batches or an era completion._

_**Driver quirk (still unfixed, worked around):** `synthesis_batch.py status/prepare` reads `- [ ]`
checklist bullets and prints "caught up" while a debt is due; passes 7–9 trusted the manual tally + the
`Synthesis notes:` lines in `log.md`. Worth fixing the driver or switching this section to real checklist
syntax._

## Ingest infra notes (archived — PO-token gate history, not synthesis debt)
_Kept for operational continuity across ingest iterations; this is about caption-fetch
infrastructure, not pending synthesis work. See `log.md` for the full blow-by-blow._

_Historical record (20 consecutive blocked confirmations, 2026-07-21→22, before resolution): the
ingest→captions path (yt-dlp PO-token gate) was blocked environment-wide, confirmed on
**all 5 of 5 TARGET channels** — @mkbhd, @AutoFocus, @TheStudio, @Waveform, @WaveformClips — a
fully settled infra blocker, not a per-channel caption gap. pip/pip3/node/npm were absent from
PATH throughout, `python3 -m ensurepip` reported no `ensurepip` module either (no user-level pip
bootstrap path), and yt-dlp stayed pinned at `stable@2026.07.04` across all twenty checks. The 15th
confirmation (2026-07-22) departed from the cheap-check-only
pattern and ran a real `ingest_batch.py prepare --channel @mkbhd --n 8` as a live re-test (not
just the PATH/version check) — same PO-token gate, 8/8 no-captions. That run also caught and
fixed a ledger-hygiene issue: the driver auto-marks PO-token-blocked rows `L1 no-captions`, which
is a misclassification (blocked ≠ confirmed absent); the 8 rows were reverted to `L0-discovered`
with an accurate `caption-fetch blocked ... retry once resolved` note (same treatment the
2026-07-21 `@AutoFocus` batch established). The 16th confirmation (2026-07-22) resumed the
cheap-check-only pattern per the standing recommendation — PATH/version/sudo unchanged from the
15th confirmation's live re-test, so no new caption probe was run. The 17th confirmation
(2026-07-22, this iteration) ran another live re-test — `ingest_batch.py prepare --channel @mkbhd
--n 8 --no-mark` (the `--no-mark` flag avoids ledger mutation so no revert was needed this time)
— identical result, 8/8 no-captions, plus a manual verbose `yt-dlp -v` probe on one id
(`m89I065ngos`) confirming the exact same `[pot] PO Token Providers: none` / "PO Token was not
provided" gate. Also tried `python3 -m ensurepip` this iteration as a new avenue (no root needed
for a user-local pip bootstrap) — not available in this Python 3.12.3 install, ruling out that
workaround too. The 16 `@mkbhd` rows marked plain `no-captions` by the two batches immediately
BEFORE the gate was first diagnosed (2009 origin P2 "Nov 10 → Dec 2" and 2010 origin P2
"Feb 23 → Apr 25") remain **not** corrected — flagged as a P1 curatorial follow-up since
2026-07-21, still open, still out of scope for a single iteration. The 18th confirmation
(2026-07-22) resumed the cheap-check-only pattern (as the 16th did) since the 17th confirmation
had just run a full live re-test one iteration prior — PATH/version/sudo/ensurepip all unchanged,
no new caption probe run. The 19th confirmation (2026-07-22) escalated back to a live re-test
per the alternating pattern (cheap-only two iterations back-to-back at 16/18 flanking live tests
at 15/17) — cheap check (PATH/version/sudo/ensurepip) unchanged, then `prepare --channel @mkbhd
--n 8 --no-mark` (same 8 oldest-P2 ids as prior probes) came back 8/8 no-captions, plus a manual
`yt-dlp -v` probe on `m89I065ngos` reconfirming the identical `[pot] PO Token Providers: none` /
"PO Token was not provided" gate. `--no-mark` again avoided ledger churn. The 20th confirmation
(2026-07-22) resumed the cheap-check-only pattern (as 16/18 did) since the 19th confirmation had
just run a full live re-test one iteration prior — `which pip pip3 node npm` (still empty),
`yt-dlp --version` (still `2026.07.04`), `sudo -n true` (still needs a password), and
`python3 -m ensurepip` (still no module) all unchanged, so no new caption probe was run this
iteration (would only reconfirm the same gate at the cost of a wasted `--no-mark` prepare call).
Future iterations should keep doing ONE cheap environment check per wakeup (pip/node on PATH?
yt-dlp version changed?) and only re-run a full caption probe if that check shows something
changed — but should also periodically (every few iterations, not every one) run a live
`prepare --no-mark` re-test regardless of the cheap check (prefer `--no-mark` over plain
`prepare` to avoid ledger churn/reverts on an already-known-blocked batch), since a server-side
gate lifting wouldn't show up in PATH/version alone. Stage C (shorts dedup) also depends on
caption fetch, so no caption-dependent stage is currently workable. Escalate as its own
workstream (infra: install a PO-token provider or await a yt-dlp release) rather than repeatedly
re-diagnosing._

**NEW blocker, distinct from the PO-token gate above (2026-07-22, post-pass-7).** The PO-token
gate stayed resolved through pass 7's 10th consecutive clean `@mkbhd` batch (`[pot] PO Token
Providers: bgutil:http-1.3.1, bgutil:script-node-1.3.1, bgutil:script-deno-1.3.1` — correctly
configured, not the old "none" state). The very next real ingest attempt (this iteration, 8
oldest-first `@mkbhd` P2 rows, 2011-09-12→2011-10-05) hit a **different** failure: every video
returns `android_vr`/`web_safari` player response `LOGIN_REQUIRED` and yt-dlp errors `Sign in to
confirm you're not a bot. Use --cookies-from-browser or --cookies ...`, despite
`/home/roster/.config/yt-dlp/config` already passing `--cookies /home/roster/roster-run/cookies.txt`
(file present, 43KB). Cross-checked on a second channel (`@Waveform`'s `yt-NofmSGPCDr4`, today's
fresh upload) — identical failure, confirming this is environment-wide (cookie/bot-check), not a
per-video or per-channel issue, and not a caption-availability question at all (it fails before
reaching the subtitle-fetch stage). `tools/ingest_batch.py`'s classifier has no pattern for this
either (falls into the generic `error`/`retry` bucket, correctly left open/unmarked — no ledger
corruption risk here, unlike the old no-captions misclassification). **Likely cause:** the cookies
file has gone stale (YouTube session cookies expire/rotate) and needs re-exporting from a
signed-in browser session; can't rule out a broader YouTube bot-check escalation independent of
cookie freshness without an external check. **Next iteration:** cheap check first — cookie file
mtime vs. last-known-good, one single-video live re-probe — before committing to a full batch.
If unresolved, this blocks ALL caption-dependent stages (B and C) across every channel; escalate
as its own infra workstream (refresh/rotate the cookies file) rather than repeatedly re-diagnosing
with full 8-video batches.

**2nd confirmation (2026-07-22, ~2h later).** Followed the standing recommendation: cookie file
mtime checked (12:10 UTC, ~2h stale relative to this run — not obviously expired on its own),
then a cheap single-video live probe (`yt-dlp -v --skip-download --write-auto-sub`, no full
batch) against the exact P1 target (`@Waveform`'s `yt-NofmSGPCDr4`, the same fresh-upload video
this workflow would otherwise have ingested first). Identical failure signature: `android_vr`/
`web_safari` both `LOGIN_REQUIRED`, same `Sign in to confirm you're not a bot...` error, PO Token
Providers still correctly listed (not a recurrence of the old "none" gate). Confirms the block is
still live ~2 hours on, unchanged, and is not resolved by mere time passing. Still unresolved;
still needs a cookie refresh from a signed-in browser session (or external confirmation of a
broader YouTube-side bot-check escalation) before any caption-dependent stage (B or C) can run
on any of the 5 TARGET channels.

**3rd confirmation (2026-07-22, later same day) — rules out "stale cookies" as the cause.**
Two infra-side changes had landed since the 2nd confirmation: `/etc/yt-dlp.conf` gained a
`--sleep-requests`/`--sleep-interval` throttle block (commented "added 2026-07-22 to reduce
datacenter-IP bot-checks"), and `/home/roster/roster-run/cookies.txt` was rewritten essentially
during this very check (mtime 15:30:55 UTC vs. the probe's 15:31 UTC) with genuine authenticated
Google-session cookies (`SID`, `SSID`, `HSID`, `APISID`, `SAPISID`, `__Secure-1PSID`,
`__Secure-3PSID`, etc. — not just consent/analytics cookies). A live probe against the exact P1
target (`@Waveform`'s `yt-NofmSGPCDr4`) with both changes in effect still returned the byte-for-
byte identical `LOGIN_REQUIRED` / "Sign in to confirm you're not a bot" failure on both
`android_vr` and `web_safari` player clients. **This is the key new finding: a same-minute-fresh,
genuinely-authenticated cookie file does not fix it**, so this is not simple credential staleness.
Recommend trying yt-dlp's other player clients explicitly (`--extractor-args
"youtube:player_client=tv,web"` or similar) or checking whether the signed-in account itself is
challenge-gated (CAPTCHA/phone verification) independent of yt-dlp, before further re-probing with
the same command. Safety rail invoked at 3 consecutive confirmations; this iteration stopped
without spending a full batch.

## Done checkpoints
- [x] **Era: @mkbhd 2010 origin long tail + Aug–Sep 2011 (68 new L2, batches 54–63,
  386→454)** — seventh synthesis pass. Drained the ten-batch debt (the driver's own pending-
  checkpoints parser under-reports because this file recorded the debt as prose, not `- [ ]`
  checklist items — see the driver note under "High-water mark"; trusted the manual tally +
  the pass-6 iteration's explicit "run Stage S next" instruction in `log.md` instead).
  **Topic hubs (L3):** `tech-reviews` — the origin scoring ladder's **first two perfect 10/10
  scores** (iKey Audio M808-V2 monitors, paired with a rare self-aware red-and-black bias
  disclaimer; Asus UL30A-X5, self-consciously counted as "the second ever"), and a "fat
  laptops" weight-threshold category-naming review; `tech-industry-commentary` — that same
  review visibly **prompting a manufacturer response** (Razer Blade, three days later) — the
  earliest documented instance of his content shaping industry output, a precursor to "this
  will be copied"; `production-filmmaking` — the **channel-name-origin story** told directly
  (started under his own name, switched to MKBHD for memorability) + his literal **first
  hardware video** (webcam on a box) + CamStudio named, a three-tier microphone framework +
  free-light-first lighting principle (collab w/ Austin Evans), and a second independent GIMP
  citation resolving an earlier caption garble; `creator-business` — a **10,000-subscriber
  milestone** (2010-08-22) with a self-funded-vs-PR-seeded giveaway distinction, cross-linked
  to the channel-name story; `consumer-tech-culture` — the red-and-black preference's
  strongest evidence yet (the self-aware bias disclaimer). **Persona:** `beliefs.md` (+1
  value: separate aesthetic preference from the verdict, and say so), `voice.md` (+6 verbatim
  quotes: the channel-name-origin line, the bias-disclaimer line, two "Stop It!" lines, the
  persistence-commitment line; +1 cadence/humor entry: the "Stop It!" rapid-fire delivery
  sample, with its "stop comparing... to the MacBook Air" pet peeve flagged — not asserted —
  as a candidate early precursor to "compared to what?"), `biography.md` (+4 dated anchors:
  10,000 subs, the channel-name/first-hardware-video story, the MKBHD Update 6.0 hiatus +
  persistence commitment, a self-reported Motorola-Droid personal-device anchor),
  `appearance.md` (+1: the bias-disclaimer as evidence the red/black preference is
  self-recognized, not just asserted by the wiki). Recompiled `persona/system-prompt.md`
  **v6 → v7** (compiled_from_sources 386 → 454). No new topic pages created (all promotions
  extended existing hubs/persona). No contradictions flagged. No fabrication, all English.
  Done 2026-07-22 (synthesis pass 7).
- [x] **Era: @mkbhd Jul–Nov 2009 origin P2 long tail (37 new L2, batches 49–53) + the debt-counter
  padding from two zero-yield no-captions batches and three PO-token-block diagnostics** — sixth
  synthesis pass. Debt hit the 10-batch checkpoint largely via administrative/zero-yield entries (a
  systemic yt-dlp PO-token caption-fetch block, six-times confirmed as of this pass) rather than raw
  volume — synthesizing now was the productive move while ingest is network-blocked. Drained the five
  real batches' worth of `Synthesis notes:`. **Topic hubs (L3):** `tech-reviews` — the origin scoring
  ladder's new high (Wrapsol 9.5/10, "the highest rating I have ever given," + its side-by-side
  comparative method, an early "compared to what?" ancestor), the widest unbox→review turnaround yet
  (DS Intl keyboard, ~9 weeks) + a hardware-review filmed in Camtasia Studio 6, HQ-by-default put to a
  vote + an on-camera self-correction, scoring explicitly named a hardware-only convention (Desktube),
  and an early price-to-value video-response judgment (MacBook Pro vs. Alienware M17x, "not paying
  $1,000 for a casing"); `creator-business` — the subscriber timeline to 2,300 + the first explicit
  upload-cadence policy, MKBHD Update 4.0's four threads (the two-week wrongful suspension, the
  YouTube Partnership threshold raised ~2,000→~10,000 as an evolving position, the mega-widescreen
  format vote, the varsity-sport+AP-classes time-constraint disclosure), a second named PR-outreach
  relationship (iSkin), dedicated review-outreach email tooling, and giveaways starting to
  cross-promote a second platform (Twitter); `consumer-tech-culture` — the red-and-black customization
  statement upgraded from preference to deliberate choice (iFrogz Fallouts), and a genuine "Dope Tech"
  precursor a decade early (gScreen Spacebook, specs-only/no-unit novelty coverage). **Persona:**
  `beliefs.md` (+2 origin values: do-the-math-yourself-transparently, corrects-his-own-mistakes-on-camera),
  `voice.md` (+5 verbatim quotes: red-and-black-customization, the cadence policy, the "highest rating"
  superlative, the suspension disclosure, the "$1,000 casing" judgment), `biography.md` (subscriber
  timeline to 2,300, the two-week suspension, the varsity-sport/AP-classes constraint, a note that the
  2009 origin era is now closed to the extent captions exist). Recompiled `persona/system-prompt.md`
  **v5 → v6** (compiled_from_sources 349 → 386). No new topic pages created (all promotions extended
  existing hubs/persona). No contradictions flagged (the Partnership-threshold change is an evolving
  position, explicitly noted as such, not a contradiction). No fabrication, all English. Done
  2026-07-21 (synthesis pass 6).
- [x] **Era: @WaveformClips first dedup batch + @mkbhd Apr–Jul 2009 origin P2 long tail (75 new L2,
  batches 39–48)** — fifth synthesis pass. Drained the ten accumulated `Synthesis notes:` lines since
  pass 4 (all @mkbhd solo except 4 @WaveformClips L2's, ensemble-gated — 0 confident-Marques quotes
  promoted from those). **Topic hubs (L3):** `tech-reviews` — review-business origin (emailing companies
  for units), the sent-for-review/PO-box workflow, "first hardware unboxing" + the unbox→review split
  named outright, "an unboxing needs a reason to exist" (Wrapsol, + corrects the manufacturer's own spec),
  the unbox/review firewall stated as an explicit rule (Sena), the origin scoring ladder (9/10 → 8.5/10 →
  8/10 → 8/10, with a flagged no-score contrast the same week), con-vs-con-for-me + the lived-with-it
  standard, first in-review comparison to his own prior review, the two-methods-with-a-tradeoff verdict
  (ancestor of "compared to what?"), hardware/software alternation stated as policy; `creator-business` —
  the dated subscriber/catalog timeline to 1,570 subs/230 videos/202K views, the YouTube Partnership
  rejection arc (3 denials disclosed), pre-Partner constraint economics (FLV delivery-encode workaround),
  "Use that Search Box!" audience-management system, the first PR-agency-seeded review unit
  (Fleishman-Hillard), the reciprocal-subscription TCOTW growth engine + explicit growth thesis, analytics-
  as-sponsor-pitch framing, attribution-ethics origin (credit the music), channel-layout branding step;
  `production-filmmaking` — the encoding standard extended to camera footage (MPEG Streamclip), the
  audio-pipeline unbox→review two-step applied to his own gear, a live unretakeable demo (honesty over
  polish), a second "redo when the platform changes" instance (metadata update vs. reshoot), an audio-tool
  preference; `consumer-tech-culture` — red-and-black hardens from candidate seed to a first-person
  "favorite colors" statement, the earliest pro-restraint branding judgment (Griffin Elevator). **Persona:**
  `beliefs.md` (+7 origin values: unbox-needs-a-reason, unbox/review firewall, hardware/software
  alternation, price-tier grading, lived-with-it standard, growth thesis), `voice.md` (+6 verbatim quotes:
  "generous nine out of ten," "favorite colors," alternation rule, the firewall rule, the Griffin
  restraint quote), `biography.md` (subscriber/catalog timeline, Partnership rejection arc, PR-agency
  milestone; the "outside freelance writing" lead flagged to `wiki/gaps.md`, not asserted), `appearance.md`
  (red-and-black as a stated personal colour preference, causation still open). Recompiled
  `persona/system-prompt.md` **v4 → v5** (compiled_from_sources 274 → 349). No new topic pages created
  (all promotions extended existing hubs/persona). `wiki/gaps.md` opened with 2 entries (an unconfirmed
  biography lead + 2 ensemble ★ findings gated on solo-source confirmation). No rate limits, no
  fabrication, all English. Done 2026-07-21 (synthesis pass 5).
- [x] **Era: @mkbhd Feb–Apr 2009 origin P2 long tail (72 new L2, batches 29–38)** — fourth synthesis
  pass. Drained the ten accumulated `Synthesis notes:` lines since pass 3 (all @mkbhd solo, age 15,
  cleanest attribution — no quarantine). Promoted the genuinely-new material only; long-tail repeats of
  the pass-3 origin thread dropped (stay L2). **Topic hubs (L3):** `production-filmmaking` — origin
  encoding STANDARDS + the "redo it better" ethos (the "What does YouTube Want?" 720p/h.264/two-mic/
  test-before-publish spec `ZPv25BKcQtU`; the Camtasia-6 720p export preset `8imsZ-ADhMM`; Update-1.1
  Camtasia-6 upgrade + re-record plan `SsgBuvCKJE4`; the zoom/tilt push-in origin `1E_1KfMIexQ`; the
  dual-production method + no-tripod `WaqNXARd3Fo`; the Audacity+Camtasia audio-post pipeline
  `CwapC2jZ_JI`); `creator-business` — the dated first-months subscriber timeline (74→95→260→450 subs),
  the "New Ideas" commentary-format + Update/Inbox format origins, the GIMP-built MKBHD wordmark
  `oix079jUkVU`, Chris-Pirillo influence + YouTube-Partner ambition, deliberate playlist/series curation;
  `smartphones` — the iPhone-software origin (non-iPhone/Verizon-LG-Voyager owner critiquing iPhone OS 3.0,
  push≠multitasking spec-literacy); `tech-reviews` — the "is-it-worth-it?" + cite-CNET origin
  `or8t_Zi7S38` and the earliest structured buying-guide `yDie-JzVlKM`; `tech-industry-commentary` — the
  "New Ideas" commentary-format seed. **Persona:** `beliefs.md` (+worth-it/cite-your-source + correct-the-
  spec origin values), `voice.md` (+4 origin verbatim quotes: dual-method, MKBHD-logo, initials, worth-it),
  `biography.md` (new pass-4 anchors: subscriber timeline, GIMP logo, non-iPhone/LG-Voyager, origin gear),
  `appearance.md` (red-on-black now concretely dated to the GIMP wordmark build). Recompiled
  `persona/system-prompt.md` **v3 → v4** (compiled_from_sources 202 → 274). No new pages created (all
  promotions extended existing hubs/persona). No rate limits, no fabrication, all English. Branding
  causation to the later crimson studio brand left explicitly open. Done 2026-07-20 (synthesis pass 4).
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
