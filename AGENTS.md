# Repository instructions

## Scope and organization

- Use this repository for all music created for the user. Each song belongs in its own `songs/YYYY-MM-DD-song-slug/` folder.
- Read the root README, `docs/STANDARDS.md`, `docs/LYRIC-VIDEO-STANDARD.md`, and the song README before editing a song.
- Start new songs from `templates/song/`. Keep lyrics, prompts, links, generation metadata, audio, stems, artwork, video, project files, and evidence within the song folder.
- Update the root catalog, song README, and song changelog whenever status or deliverables change.
- Preserve previous generated takes and released files. Version revisions instead of overwriting approved material. Do not modify unrelated work.

## Kingdom perspective

- For biblical topics, use a Kingdom perspective: God's Kingdom is a heavenly government and Jesus is the King with absolute authority.
- Emphasize sovereignty, government, dominion, allegiance, citizenship, authority, purpose, and the King's will. Follow each song's specific brief for obedience, love, and intimacy with the Holy Spirit.
- Avoid religious, denominational, institutional-Christian, and traditional church framing or imagery.
- Do not present original lyrics as Scripture quotations. Identify exact quotations and their translation when used.
- Apply the same creative direction to cover art and video. Flag automatically generated imagery that conflicts with it; do not treat platform-generated artwork as approved branding.

## Lyric videos and thumbnails

- For every new video, lyric video, visualizer, and matching thumbnail, use the approved RUACH Anthem **Breath into Song** identity in `channel/ruach-anthem/identity-approved-v001/` and its `platform-kit-v001/` exports. This is the standing brand standard confirmed by the user on 2026-10-10. Use the distinct musical-note/breath emblem and RUACH ANTHEM wordmark, not the parent RUACH two-ribbon logo. Preserve existing approved releases.
- Latest video direction (2026-10-10): use the main RUACH white lockup for lyric-video overlays, superseding the Anthem-overlay requirement above. Choose accents to suit the song rather than requiring red; add subtle environmental shapes that belong to the song and scene (such as wind wisps and drifting seeds in country landscapes), avoiding detached geometric overlays. Channel identity and MP3 standards remain separate.
- Follow the approved [lyric-video standard](docs/LYRIC-VIDEO-STANDARD.md): 1920x1080 only, never 4K delivery under this standard.
- Keep RUACH branding, title position, lyric placement, and subtle next-line preview consistent with the approved reference layout. Use plain lyrics; no word highlighting or karaoke color changes.
- Make mobile readability a required check: current lyrics target 100 px (minimum 96 px) and preview target 56 px (minimum 52 px) at 1080p; split long phrases instead of shrinking them. Verify and save 390-pixel-wide and 640-pixel-wide preview frames under the lyric-video standard.
- Create a distinct motion background for each song, specifically expressing its vibe, lyrics, and message. Subscribers should recognize different songs at preview size; minor variations of the same generic background are insufficient.
- After the user approves a lyric video, create its matching static YouTube thumbnail as the next deliverable. No teaser video is implied. Save all assets in the song folder and track video and thumbnail approvals separately.
- Follow the current requested scope: a documentation-only update records this workflow and pending deliverables; it does not itself create or publish media.

## YouTube releases

- Follow `docs/MP3-BRANDING-STANDARD.md` for every future branded song: ID3v2.3 RUACH artist/album artist, accurate song metadata, brand comment, full lyrics, and approved RUACH Anthem front-cover artwork. Preserve originals, version derivatives, and verify unchanged compressed audio hashes. No audible watermark or cryptographic signature is implied.
- The approved channel identity is [RUACH Anthem — Breath into Song](channel/ruach-anthem/identity-approved-v001/README.md), approved 2026-10-10. Use its distinct musical-note/breath emblem for new channel identity work; do not substitute the parent RUACH two-ribbon logo. Preserve historical releases.

- Follow `docs/YOUTUBE-RELEASE-STANDARD.md`. The destination is RUACH Anthem, `@RuachAnthem`, channel ID `UCrEm70zv0iTkSro5cl_pdAg`.
- The user has given standing authorization to upload approved songs to this channel. Once the song and its release video are approved, carry the release workflow through upload; do not ask again for generic upload permission. Respect any later hold or limited approval scope.
- Use the exact title format `[SONG TITLE] by RUACH`, with no literal brackets, take numbers, version labels, or speed labels unless specifically requested.
- Include the full lyrics matching the approved recording in every video description. Save the exact title, description, thumbnail, upload settings, approval evidence, and resulting YouTube URL in the song folder.
- Publish approved releases as Public and select Not made for kids, as directed by the user. Respect any later song-specific hold or schedule. Distinguish upload completion, processing, and verified public availability.
- For every approved release, host a clean RUACH-branded MP3 on a versioned GitHub Release in this repository and add the verified direct download link near the top of the video description. This is standing user authorization; the download is public, not subscriber-gated. Preserve originals and avoid unrelated commits or uploads.
- Include the matching static thumbnail, full lyrics, channel link, and accurate production credits. Use Music category, the actual song language, and truthful AI/paid-promotion disclosures. Future lyric-video delivery remains 1080p.

## Tools and authorization

- Prioritize the in-app browser for browser tasks and reuse the user's signed-in session when authorized.
- Verify current music-service controls and account availability. Record actual model/settings used, not settings merely requested in a prompt.
- A request to create music authorizes the ordinary creation workflow, but does not imply buying a plan, distributing elsewhere, or messaging others. Approved-song YouTube uploads have the standing authorization described above.
- Do not commit, push, publish, or delete unrelated files unless the user asks. Never store passwords, cookies, access tokens, or payment details.

## Evidence and completion

- Distinguish a submitted prompt, generated track, locally downloaded file, listening review, approved master, and published release.
- Record reference-audio access honestly. A title, transcript, or screenshot does not prove the audio was heard.
- Capture generation links, dates, model, displayed duration, lyrics revision, prompt revision, and known limitations.
- Preserve original downloads. Use versioned derivatives for edits and exports. Document tools and export settings when applicable.
- Before finishing, check Git status and changes, required package files, catalog links, and whether every claimed local asset exists. Report outstanding review or missing assets explicitly.

## Post-publication cleanup and push

Latest standing user instruction, 2026-10-12 (Asia/Singapore): once a song is approved and successfully uploaded to YouTube, clean its `songs/.../assets/` folder and keep **only the exact released audio file**, under `assets/audio/releases/`. Verify its hash against the published release before deleting anything.

Remove every other file under that song's assets folder, including uploaded MP4s, motion backgrounds, song-local branding, thumbnails, original/alternate audio, duplicate exports, project sources, previews and evidence. This supersedes the earlier instruction to preserve reusable backgrounds, branding and other release assets inside the song's assets folder. Shared channel branding outside the song folder is outside this cleanup scope. Do not relocate unwanted assets elsewhere as a substitute for deletion.

Keep lyrics, prompts, release URLs, approvals, hashes and cleanup manifests outside assets. Inventory exact paths and byte totals before deletion; verify the resolved targets stay inside the intended song's assets folder. After deletion, verify that the only remaining file is the released audio and its hash is unchanged. Update active documentation links and identify historical paths as intentionally removed. Do not delete hosted YouTube videos or GitHub Release downloads.

Update the root catalog, song README, changelog and release records, then commit and push approved scoped changes to the configured remote. Exclude unrelated work. Do not rewrite history or force-push. If deletion is blocked, record it as blocked with zero deletions and report the limitation; never claim cleanup completed.
