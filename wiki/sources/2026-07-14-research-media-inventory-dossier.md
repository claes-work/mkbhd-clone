---
type: web-research
source_date: 2026-07-14
ingested: 2026-07-14
tags: [media-inventory, pipeline, enumeration, channels, podcast, socials, apps, guest-appearances]
---

# Media inventory dossier — Marques Brownlee / MKBHD (as of 2026-07-14)

Phase-2 consolidation of the full media surface of the SUBJECT (Marques Brownlee,
"MKBHD"). YouTube channel IDs and rough video/shorts counts come from yt-dlp
enumeration on 2026-07-14 (authoritative for IDs; counts are the `/videos` and
`/shorts` tab item counts, which exclude live/members-only and can lag the true
total by a handful). Everything else was verified or extended via web research on
2026-07-14. Every number carries its as-of date and source. Follower/subscriber
counts are platform-self-reported (via yt-dlp `channel_follower_count` or the live
profile) unless noted; nothing here is registry-verified.

## YouTube channels (yt-dlp enumeration, 2026-07-14 — authoritative for IDs)

| Channel | Channel ID | Subs | Content (videos + shorts) | Role | Status |
|---|---|---|---|---|---|
| [@mkbhd](https://www.youtube.com/@mkbhd) | `UCBJycsmduvYEL83R_U4JriQ` | 21,100,000 | ~1,708 long-form + ~119 shorts | Main tech-review corpus. Marques is sole on-camera host. Founded 2008 (as "MKBHD" / "Marques Brownlee Reviews"); flagship channel. | **TARGET** |
| [@Waveform](https://www.youtube.com/@Waveform) | `UCEcrRXW3oEYfUctetZTAWLw` | 520,000 | ~299 long-form + ~89 shorts | "WVFRM Podcast" — the video feed of *Waveform: The MKBHD Podcast* (Marques + Andrew Manganelli + David Imel). Video ≈ audio of the podcast → dedup (see below). | **TARGET** |
| [@WaveformClips](https://www.youtube.com/@WaveformClips) | `UCc_ycus0q7DSd85ZkmEY5ig` | 537,000 | ~628 long-form clips + ~31 shorts | "Waveform Clips" — official clips channel; every item is a segment cut from a full Waveform episode. Almost 100% derivative. | **TARGET** (catalog/dedup tier) |
| [@AutoFocus](https://www.youtube.com/@AutoFocus) | `UC2J-0g_nxlwcD9JBK1eTleQ` | 1,260,000 | ~120 long-form + ~20 shorts | "Auto Focus" — MKBHD team's car/EV channel. Marques hosts many but NOT all episodes (team members present cars too). Speaker attribution required. | **TARGET** |
| [@TheStudio](https://www.youtube.com/@TheStudio) | `UCG7J20LhUeLl6y_Emi7OJrA` | 1,120,000 | ~104 long-form + ~103 shorts | "The Studio" — secondary channel (launched Jul 2021) for behind-the-scenes, vlogs, challenges, mini-reviews. Frequently ensemble content (whole MKBHD team on camera), not Marques-solo. | **TARGET** (attribution-gated) |

**Host-attribution notes (critical for fidelity rule 6):**
- **@mkbhd** — effectively 100% Marques on camera and in voice; the cleanest persona
  training corpus. Even here, scripts are co-written with writer/researcher David Imel
  and the team, so the *voice* is Marques but the *research framing* is collaborative.
- **@Waveform / @WaveformClips** — three-host conversation (Marques, Andrew Manganelli,
  David Imel; earlier eras had different co-hosts). **Attribute every statement to a
  speaker before it flows into `persona/voice.md` or `beliefs.md`.** Only
  Marques-attributed lines train the persona; Andrew and David get `wiki/entities/`
  context pages.
- **@AutoFocus** and **@TheStudio** — mixed hosting. Titles/thumbnails often feature
  team members (Andrew, David, Vinh Dang, Brandon Havard, etc.). Treat as
  attribution-gated: an item trains the persona only when Marques is the speaker.

### Excluded channels

| Channel | Channel ID | Reason for exclusion |
|---|---|---|
| [@WVFRMclips](https://www.youtube.com/@WVFRMclips) | `UC9fK_9n0MTZ0zGDKHNWp1oA` | "WVFRM Clips" — abandoned/legacy clips channel. **1 subscriber**, ~30 old videos, superseded by @WaveformClips. Negligible reach; not maintained. EXCLUDED. |
| Fan re-upload / compilation channels ("MKBHD Clips", "Best of MKBHD", etc.) | — | Not operated by Marques or his team; re-hosted copyrighted content. EXCLUDED (not official). |
| Topic auto-channels ("Marques Brownlee - Topic") | — | YouTube-generated auto-channels, not human-curated. EXCLUDED. |

No separate "MKBHD Shorts", "MKBHD Gaming", or personal-vlog channel exists as of
2026-07-14 (yt-dlp handle checks + web research). Shorts live inside each channel's
`/shorts` tab, not a dedicated channel.

## Podcast — *Waveform: The MKBHD Podcast*

- **RSS feed**: `https://feeds.megaphone.fm/STU4418364045` — hosted on **Megaphone**;
  part of the **Vox Media Podcast Network** (moved to Megaphone/Vox Sep 2021; was
  self-hosted before that). Feed/directory data verified via
  [podnews.net/podcast/il00](https://podnews.net/podcast/il00), 2026-07-14.
- **Directory IDs**: Apple `id1474429475`
  ([podcasts.apple.com](https://podcasts.apple.com/us/podcast/waveform-the-mkbhd-podcast/id1474429475)) ·
  Spotify show `6o81QuW22s5m2nfcXWjucc`
  ([open.spotify.com](https://open.spotify.com/show/6o81QuW22s5m2nfcXWjucc)) ·
  Podcast Index `947138` · GUID `dbaa1d5f-2d6d-5852-a6de-6cd11c25f732`.
- **Hosts**: Marques Brownlee, Andrew Manganelli, David Imel (current core trio).
  Earlier co-hosts rotated through the MKBHD team.
- **First episode**: 2019-07-31 (teaser); first full episode 2019-08-09
  ([Wikipedia](https://en.wikipedia.org/wiki/Waveform_(podcast)), 2026-07-14). Weekly
  cadence since. 300+ episodes as of 2026-07-14 (approx.; the @Waveform video feed
  shows ~299 long-form items, and audio-only episodes/mailbags add a few more).
- **Dedup rule (binding for the ledger)**: the full podcast is published as video on
  **@Waveform** AND as audio on the Megaphone RSS feed. **YouTube @Waveform is the
  primary ingestion source** for full episodes (captions + video). Podcast feed items
  enter the ledger only when no matching @Waveform video exists (match on title +
  publish week); matched audio items stay L1 with `dup-of:<youtube-id>`.
- **Clips dedup**: every **@WaveformClips** item is a cut of a full episode → stays L1
  `dup-of:<waveform-episode-id>` unless a clip is the *only* surviving copy of a
  segment. Do not L2-ingest clips by default.

## Apps / products

| Product | Status | Details | Source |
|---|---|---|---|
| **Panels** (wallpaper app; [panels.art](https://panels.art)) | **SHUTTING DOWN end of 2025** | Curated artist-wallpaper app, iOS + Android, launched 2024-09-24. Marques was co-founder/front-man. Subscription ($11.99/mo or ~$49.99/yr) drew heavy criticism at launch. Announced shutdown Dec 2025 after the dev team's makeup changed and no "right fit" collaborators were found. | [TechCrunch 2025-12-01](https://techcrunch.com/2025/12/01/mkbhds-wallpaper-app-panels-is-shutting-down/), [MacRumors](https://www.macrumors.com/2025/12/01/mkbhd-wallpaper-app-shutdown/), [TechCrunch launch 2024-09-24](https://techcrunch.com/2024/09/24/tech-youtuber-mkbhds-panels-app-is-a-bit-underwhelming/) |
| **MKBHD Merch store** ([shop.mkbhd.com](https://shop.mkbhd.com) / [mkbhd.com](https://mkbhd.com)) | Active | Apparel/accessories. Flagship lines: "The Core Four" tees ($29 ea — Production, Shutter Speed, Reverb, Deconstructed), Chevron Hoodie ($65), wristbands, clearance. Design ethos: "balance between familiar and fashionable." mkbhd.com resolves to the shop. | [mkbhd.com](https://mkbhd.com), fetched 2026-07-14 |

No book and no paid course/newsletter product is established for Marques as of
2026-07-14 (unlike many creators, his revenue is ads/sponsorship/merch/apps, not
info-products). If a newsletter exists it was not confirmable — treat as not-present
until verified.

## Websites

| Site | Role | Notes |
|---|---|---|
| [mkbhd.com](https://mkbhd.com) | Hub → merch store | Front page is the shop; also links out to all video properties (main, The Studio, Waveform, AutoFocus), socials (YouTube, Instagram, Twitter/X, Discord community), recent uploads. Fetched 2026-07-14. |
| [shop.mkbhd.com](https://shop.mkbhd.com) | Merch commerce | Same store surface as mkbhd.com. |
| [panels.art](https://panels.art) | Panels app site | Winding down (see Apps). |

## Socials

| Platform | Handle | Count | As of | Source | Confidence |
|---|---|---|---|---|---|
| YouTube (main) | [@mkbhd](https://www.youtube.com/@mkbhd) | 21,100,000 | 2026-07-14 | yt-dlp `channel_follower_count` | High |
| X / Twitter | [@MKBHD](https://x.com/MKBHD) | ~6,100,000 | 2026 (web search snippet) | web search, 2026-07-14 | Medium (X blocks scraping; snippet figure) |
| Instagram | [@mkbhd](https://www.instagram.com/mkbhd/) | ~5,190,000 | 2026-06 | web search (HypeAuditor/SocialBlade snippet) | Medium |
| TikTok | [@mkbhd](https://www.tiktok.com/@mkbhd) | ~2,300,000 | 2026 | web search snippet | Medium |
| Threads | [@mkbhd](https://www.threads.com/@mkbhd) | ~1,700,000 | 2026 | web search snippet | Medium |
| Bluesky | [mkbhd.com](https://bsky.app/profile/mkbhd.com) | count not established | 2026-07-14 | profile confirmed via web search; count not fetched | Low — existence confirmed, count unknown |
| Facebook | [facebook.com/MKBHD](https://facebook.com/MKBHD) | count not established | 2026-07-14 | linked from @mkbhd channel description | Low — exists, low activity |
| Discord | linked from mkbhd.com | community server | 2026-07-14 | mkbhd.com | Existence confirmed |

Reach hierarchy for growth curves: YouTube (21.1M) ≫ X (6.1M) > Instagram (5.2M) >
TikTok (2.3M) > Threads (1.7M). YouTube is by far the dominant persona surface;
socials are promotional/repost layers.

## Enumeration universe — what feeds pipeline/ledger.csv

Ledger population order and dedup precedence (all counts as of 2026-07-14):

1. **@mkbhd YouTube** — ~1,708 long-form + ~119 shorts = **~1,827 items** (yt-dlp).
   Primary corpus, cleanest attribution. Shorts dedup against long-form
   (`dup-of:<id>`).
2. **@Waveform** — ~299 long-form + ~89 shorts = **~388 items**. Podcast video feed;
   multi-host → attribution-gated. Primary source for podcast episodes (audio feed
   dedups against these).
3. **@AutoFocus** — ~120 + ~20 = **~140 items**. Car/EV; attribution-gated.
4. **@TheStudio** — ~104 + ~103 = **~207 items**. BTS/vlogs; ensemble → attribution-gated.
5. **@WaveformClips** — ~628 + ~31 = **~659 items**, almost all `dup-of:` a full
   Waveform episode → stay L1; do not L2 by default.
6. **Waveform podcast RSS** (Megaphone `STU4418364045`) — 300+ episodes; only items
   with NO matching @Waveform video get their own ledger row; the rest L1 `dup-of:`.
7. **Products** — Panels (winding down) and merch → context/entity rows, not corpus.
8. **External guest appearances** — Marques is a frequent podcast/keynote guest
   (Stratechery/Ben Thompson interview 2024, Colbert, many tech podcasts, plus marquee
   sit-downs — see landmark markers below). Enumerate opportunistically; each carries
   high biographical yield.

Rough total enumeration universe: **~2,560 primary YouTube items** (~1,827 main +
~735 satellite channels) + **~659 clips (mostly dup)** + podcast-only stragglers +
opportunistic guest appearances.

## Proposed domain taxonomy (for SUBJECT.md — user to confirm)

1. **tech-reviews/** — gadget review methodology, scoring, "is it worth it", reviews of
   phones/laptops/wearables/audio/tablets; the review philosophy itself.
2. **smartphones/** — flagship smartphone deep-dives, camera shootouts, the annual
   **Blind Smartphone Camera Test** and **Smartphone Awards**, iPhone vs Android.
3. **production-filmmaking/** — cinematography, cameras (RED, Sony), lighting, color
   grading, editing, how MKBHD videos are made, the studio build-out.
4. **creator-business/** — YouTube as a business, team/hiring, sponsorship ethics and
   disclosure, monetization, running the Studio, apps (Panels), merch.
5. **ev-cars/** — electric vehicles, Tesla/Rivian/Lucid, autonomy, car-tech reviews,
   Auto Focus.
6. **tech-industry-commentary/** — reactions to Apple/Google/Samsung launch events, AI
   hardware (Humane, Rabbit), industry opinions, the "most influential reviewer /
   power to make or break a product" discourse.
7. **consumer-tech-culture/** — Retro Tech, Dope Tech, accessibility of tech, everyday
   carry, desk/tech setups, "the state of" explainers.

## Proposed merge_staging markers (for the ingest/synthesis loops)

**P1_EXTRA — landmark regexes** (auto-flag as priority-1 / L3 candidates):
```
(?i)\bretro tech\b
(?i)\bdope tech\b
(?i)\bsmartphone awards\b
(?i)\bblind (smartphone|camera) (test|comparison)\b
(?i)\b(interview|sat down|talking) (with|w/)? ?(obama|barack|bill gates|gates|elon|musk|tim cook|sundar|pichai|jensen|zuckerberg)\b
(?i)\bfirst video\b|\bchannel (origin|anniversary|10 years|15 years)\b
(?i)\bstate of (smartphones|the smartphone|reviews|youtube)\b
```

**P3_EXTRA — guest / Q&A / conversational formats** (long-tail, attribution-gated):
```
(?i)\bwaveform\b
(?i)\bq&a\b|\bq and a\b
(?i)\bask (marques|mkbhd)\b|\bmailbag\b
(?i)\bpodcast\b
```

## Persona command slug

Suggested: **`/mkbhd`** (alias of `/persona`).
