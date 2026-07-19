# SUBJECT — who this repo clones

STATUS: INITIALIZED (2026-07-14)

## Identity (user-confirmed 2026-07-14)
- **Name**: Marques Brownlee (Marques Keith Brownlee; online as **MKBHD**)
- **Born**: December 3, 1993; raised in **Maplewood, New Jersey**. See
  [[wiki/sources/2026-07-14-research-biography-dossier]].
  > ⚠️ Common "Maspeth/NYC" or "Merrimac" birthplace claims are unsupported — every
  > reliable source says Maplewood, NJ.
- **Known for**: The most influential consumer-**tech reviewer** on YouTube. Started
  the MKBHD channel as a high-schooler (account created 2008-03-21; first uploads Jan
  2009) and grew it to ~21M subscribers. B.S. Business & Information Technology, Stevens
  Institute of Technology (2015; honorary DBA + commencement speaker 2024). Runs a
  ~7,000 sq ft studio in Kearny, NJ (business trademark "MKBHD" Reg. 5080445, owned by
  **JMMS, LLC** [registry-verified]). Founded the **Waveform** podcast (2019), the
  **Retro Tech** series (Dec 2019), the **Auto Focus** car channel (Aug 2022), and
  co-founded the **Panels** wallpaper app (Sep 2024 → shut down Dec 31, 2025).
  Marquee interviews: Elon Musk (2018), Bill Gates (2019), Barack Obama (2020),
  Tim Cook (2024). Also a genuine semi-pro **ultimate frisbee** athlete (UFA champion).
  Signature topics: smartphone reviews, camera/production craft, EVs, the creator
  business, and level-headed tech-industry commentary.
- **Disambiguation**: no notable same-name confusion; distinguishers: MKBHD, @mkbhd
  everywhere, the crimson-red studio aesthetic, Waveform, Auto Focus.
- **Persona command**: /mkbhd  (alias of /persona, created at bootstrap)

## Content universe (feeds pipeline/ledger.csv)
### YouTube channels (TARGET = enumerated into the ledger)
1. @mkbhd `UCBJycsmduvYEL83R_U4JriQ` — ~1,708 long-form + ~119 shorts (21.1M subs,
   2026-07-14), main tech-review channel, Marques-fronted primary corpus — TARGET
2. @Waveform `UCEcrRXW3oEYfUctetZTAWLw` — ~299 videos + ~89 shorts (520K subs), the
   Waveform podcast video feed, **ensemble/multi-host** — TARGET (attribution-gated)
3. @WaveformClips `UCc_ycus0q7DSd85ZkmEY5ig` — ~628 videos + ~31 shorts (537K subs),
   podcast clips — TARGET (dedup tier; dedupe against @Waveform, attribution-gated)
4. @AutoFocus `UC2J-0g_nxlwcD9JBK1eTleQ` — ~120 videos + ~20 shorts (1.26M subs), cars/EV
   channel, Marques-fronted — TARGET
5. @TheStudio `UCG7J20LhUeLl6y_Emi7OJrA` — ~104 videos + ~103 shorts (1.12M subs),
   behind-the-scenes / vlogs, **ensemble** — TARGET (attribution-gated)
- Excluded: **@WVFRMclips** `UC9fK_9n0MTZ0zGDKHNWp1oA` (abandoned legacy clips channel,
  1 subscriber, superseded by @WaveformClips); fan re-upload/compilation channels;
  YouTube "- Topic" auto-channels. No dedicated shorts/gaming/personal-vlog channel exists.

### Other platforms (Phase 4)
- Podcast: **"Waveform: The MKBHD Podcast"** — RSS `https://feeds.megaphone.fm/STU4418364045`
  (Vox Media Podcast Network), Apple `id1474429475`, Spotify `6o81QuW22s5m2nfcXWjucc`.
  First ep 2019-07-31, weekly, 300+ eps. **Dedup: @Waveform YouTube is canonical; audio
  feed items only entered when there is no video match.**
- App: **Panels** (panels.art) — co-founded, launched 2024-09-24, shut down end of 2025.
- Websites: mkbhd.com (hub + store) · shop.mkbhd.com. No book, no course.
- Socials: X @MKBHD ~6.1M · Instagram @mkbhd ~5.19M · TikTok @mkbhd ~2.3M ·
  Threads @mkbhd ~1.7M · Bluesky mkbhd.com · Facebook /MKBHD · Discord.

## Domain taxonomy (user-confirmed 2026-07-14; folders under wiki/topics/)
- tech-reviews/ — review methodology, scoring, "is it worth it", the review as a format
- smartphones/ — flagships, camera shootouts, the Blind Smartphone Test, Smartphone Awards
- production-filmmaking/ — cameras, color, editing, how MKBHD videos are made, the studio build
- creator-business/ — YouTube-as-a-business, team, sponsorship ethics, merch, the Panels app
- ev-cars/ — EVs, Tesla/Rivian, autonomy, the Auto Focus channel
- tech-industry-commentary/ — launch-event reactions, AI hardware, the "most influential reviewer" discourse
- consumer-tech-culture/ — Retro Tech, Dope Tech, accessibility, setups, "state of" explainers

## Subject-specific rules (grown during ingest; loops must re-read this section)
- **Speaker attribution is critical on the ensemble channels** (@Waveform, @WaveformClips,
  @TheStudio): co-hosts/team **Andrew Manganelli, David Imel, Adam Molina** appear heavily.
  Only Marques-attributed material trains the persona; co-hosts get wiki/entities/ context
  pages. Uncertain attribution is flagged, never silently included.
- @WaveformClips is clipped from @Waveform → dedupe against the full episodes first;
  duplicates stay L1 with `dup-of:<id>`.
- Waveform podcast episodes are republished on YouTube → the YouTube upload is the
  canonical ledger item; the audio feed is not enumerated separately.
- Shorts across all channels are largely clipped from long-form → dedupe first.
- Corporate form: the "MKBHD" trademark is held by **JMMS, LLC** (Kearny, NJ)
  [registry-verified]; a directory-listed "MKBHD, Inc." is unverified — mark as such.
- Marques keeps his personal/family life private → treat family facts as not-public;
  do not infer or fabricate.
- Sponsorship-ethics and "worst car I've ever reviewed" (Fisker) are frequently
  misquoted → use verbatim wording and cite.
