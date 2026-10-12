# MP3 metadata branding standard

Approved 2026-10-10. Apply to every future branded song and downloadable MP3.

- Use ID3v2.3 tags. Artist and album artist remain **RUACH**; channel identity is **RUACH Music**.
- Set the clean song title, actual album or collection, release year, appropriate genre, and track number when known. Do not invent production facts. Public titles omit take/version/speed labels unless requested; retain take identity in filenames and metadata records.
- Add a RUACH Music brand comment and full written lyrics, matching the selected recording. Unsynchronized lyrics are not timing cues.
- Embed the user-approved RUACH Music album cover v002 as front cover (APIC type 3, image/png). Exact source: `channel/ruach-music/album-cover-v002/ruach-music-album-cover-v002.png`. Approved 2026-10-12 by explicit image selection; this supersedes the previous Anthem avatar artwork requirement.
- Preserve encoder provenance and original recordings. Create versioned branded derivatives; avoid re-encoding MP3 audio for tag changes.
- Verify the compressed audio-stream SHA-256 before and after tagging, reread the tags and embedded artwork, and record source/output/artwork hashes and exact asset paths in the song metadata.
- Metadata branding is not an audible watermark, cryptographic signature, or proof of ownership. No audible watermark is added unless explicitly requested.
- Video rendering converts the MP3 audio to the export codec; cover art and lyrics in MP3 tags do not automatically become video overlays. Apply video branding separately.
- Record local updates separately from hosted download updates. Preserve old release records and never claim the public download changed without verifying the hosted asset.

## Signed audio is the production and download master

Standing user instruction, 2026-10-12: sign the selected recording before creating its video. Here signing means the ID3 branding above, including the approved cover, not an audible or cryptographic signature.

Use that signed MP3 as the video renderer audio input and as the public GitHub Release MP3 linked in the YouTube description. Never render from an unsigned original or publish an older unsigned/differently tagged copy after signing. Renaming a byte-identical release copy is allowed; verify its complete-file SHA-256 equals the signed master. Record the renderer input path/hash, signed-file hash, compressed-audio hash and artwork hash outside assets. Check embedded artwork and tags after signing, then verify the hosted download digest against the same signed master. Video audio is encoded to the delivery codec, so verify content/alignment rather than requiring the MP4 audio bytes to match the MP3.

After verified approved publication, retain that signed release MP3 as the sole file under the song assets folder, following the cleanup standard. The shared cover stays under channel/. Existing published releases remain historical unless an explicit update is requested.
