---
type: youtube-video
source_date: 2019-10-11
url: https://www.youtube.com/watch?v=JR4KHfqw-oE
channel: "@mkbhd"
ingested: 2026-07-19
tier: L2
domains: [production-filmmaking, consumer-tech-culture]
tags: [youtube-compression, video-codec, generational-loss, block-motion-estimation, re-encoding, bitrate, audio-drift, 720p, talking-head, experiment, transcoding, image-quality]
attribution: solo
---

# This Is What Happens When You Re-Upload a YouTube Video 1000 Times! (@mkbhd, 2019-10-11)

## Summary
Marques runs an experiment to measure how aggressively YouTube compresses uploaded video by re-uploading and re-downloading the same clip 1,000 times, watching quality degrade generation by generation. He starts from a pristine 8K talking-head clip against a white background, then repeatedly uploads it, lets YouTube process it, downloads it via YouTube's native downloader (which returns 720p, locking the test to 720p from generation two onward), and re-uploads — accumulating compression damage each cycle. He narrates the visible artifacts as they emerge: softening, then blocky pixel groups from block motion estimation, then color shifts (his skin drifts from brown toward magenta/pink), then magenta smear trails, and finally near-total loss of facial structure into "Minecraft"-level pink blocks by the 1,000th upload. He also flags audio behavior: YouTube shifts the audio ~2 frames earlier per cycle, so it drifts progressively out of sync and slides entirely off the end — the audio is effectively gone by roughly the 800th upload, with no audio at all in the 1,000th. The background, being static frame-to-frame, survives almost intact throughout, which he uses to explain how motion-based compression preserves unchanging regions. He references a 2010 predecessor experiment by a channel called Ontologist (a webcam/audio experiment) and concludes YouTube's 2019 processing holds up notably better than the decade-old version, especially on audio quality, leaving him with more respect for YouTube's compression.

## Key claims
- [2019-10-11] The video file Marques uploads looks significantly better in QuickTime on his computer than the version YouTube serves back, because YouTube must compress uploads.
- [2019-10-11] YouTube's compression is heavy enough that heavy noise or high-ISO grain gets softened/cleaned by processing anyway, making a denoiser less necessary — described as a running joke.
- [2019-10-11] YouTube processes each upload into multiple renditions (4K, 1440p, 1080p, 720p, 480p) and dynamically switches between them, requiring aggressive file-size reduction.
- [2019-10-11] A ~5 GB final rendered file is not what YouTube streams back; it compresses down to a few megabytes and still looks "pretty much just as good," because viewers' internet couldn't stream the large file anyway.
- [2019-10-11] The experiment method: upload → let process → download → re-upload, repeated 1,000 times, until original characteristics of voice and image are destroyed.
- [2019-10-11] YouTube's native video-manager downloader returns a 720p file, so the test runs at 720p from generation two on; a third-party downloader might have given 1080p but those are less consistent.
- [2019-10-11] Video compression divides frames into blocks/groups of pixels and, via block motion estimation, keeps pixels that don't change across frames to save space — so static regions (background) hold up while moving regions (his face, arms) break down.
- [2019-10-11] When Marques pauses and holds still for consecutive frames, those frames sharpen/reset because duplicated pixels are preserved; motion returns it to "chaos."
- [2019-10-11] YouTube shifts/cuts the audio by about two frames per download-and-upload cycle, accumulating into seconds of drift over many generations.
- [2019-10-11] By ~generation 20, larger held-together pixel blocks are visible; he analogizes it to repeatedly rounding a precise number (15,555) until it collapses to 20,000.
- [2019-10-11] Skin tone shifts from brown toward magenta/pink and waving arms leave faint magenta trails on his shirt and the wall over successive generations.
- [2019-10-11] The 800th video is about the last generation where his speech is still audible; audio is completely gone (empty) by the 1,000th upload.
- [2019-10-11] The re-uploaded file still triggers YouTube's HD badge because it is technically still a 720p file, even when the image is heavily degraded.
- [2019-10-11] Conclusion: YouTube's 2019 processing looks much better than the 2010 Ontologist version; audio held up well aside from the shifting/sync drift, leaving him with more respect for YouTube's compression.

## Notable verbatim quotes (Marques — voice data)
> "the actual video file that i'm uploading to youtube looks significantly better on my computer than on youtube"
> "youtube processing will just clean up all that noise for you it'll just soften it up anyway"
> "they can compress it all the way down to just a few megabytes and it'll look pretty much just as good"
> "this whole process is called block motion estimation it's very common with video compression"
> "the parts of the video that do move like me will start to break down a little bit"
> "youtube sort of shifts the audio or cuts back the audio by about two frames with every download and upload"
> "it kind of just looks like now like a struggling graphics card like like someone turned rtx off"
> "you might end up with that sort of level of minecraft quality"
> "the 800th video is about the last time you can hear me say anything"
> "i think i have more respect for youtube's processing and all their compression than i did before"

## Notes
- Attribution note: solo. Entire video is Marques narrating his own experiment; no second speaker to quarantine.
- Caption garbles corrected (listed): "mr b style" refers to the "Mr Beast style" of doing something at extreme scale — left as-is verbatim in quotes but noted here; "backed by a channel" (line 84) is a caption slip for "by a channel"; "his 1000th video" (2010 predecessor) refers to the 1000th generation, not literal video count. No codec/bitrate/resolution figures were mis-transcribed. "rtx" and "minecraft" are correct as spoken.
